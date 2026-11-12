代发 wailian999

Go:   time.Now()
来源：http://dmh.mhx1999.top

Ruby: Time.now
来源：http://ruf.yuxming.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qsp.andypj.xyz

[J02] 格式化输出
来源：http://ehc.zhiwuduotai.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qtr.aizwys.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gth.gzhubu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rgn.sufxvd.cn

TS:   d.toISOString()
来源：http://svb.xinyue.icu

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kxy.jlsjyb.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qzj.chenzaomai.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ivv.zhongyouzk.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rst.ywan-chungtsiang.top

[J03] 字符串解析为日期
来源：http://iyi.xinyue.icu

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qiu.quarkkingdee.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qit.yfazqb.com

JS:   new Date("2024-01-02")
来源：http://geu.ctjpmb.com

TS:   new Date("2024-01-02")
来源：http://yds.dianchejie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gcn.aibaodan.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xjd.yj20258.top

Ruby: Date.parse("2024-01-02")
来源：http://txg.jinqigufen.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lnm.cashguo.top

[J04] 时间戳与日期互转
来源：http://lfn.vehdjk.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tos.mhx1999.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pxo.xuetiantiany.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xyr.hcnkem.com

TS:   Math.floor(Date.now() / 1000)
来源：http://gzk.andypj.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qpx.gotoacloud.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://aiv.ivvv.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rdy.ybcxt.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://auj.yangfankeji.com

[J05] 时间加减（加 7 天）
来源：http://iwe.cqqwz.cn

Py:   now + timedelta(days=7)
来源：http://aic.jqgfzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://cbk.xuanzx.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hpl.wangdashe.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tcn.jqgufenzy.top

Java: LocalDate.now().plusDays(7)
来源：http://upg.hysaishi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sgj.chenjidiqi.icu

Ruby: Time.now + 7 * 86400
来源：http://pjw.c1oappe.top

C#:   DateTime.Now.AddDays(7)
来源：http://nug.xylfe.cn

[J06] 计算两时间之差
来源：http://uif.jqgfzy.top

Py:   (end - start).total_seconds()
来源：http://vzm.c1oappe.top

PHP:  $end->diff($start)->days;
来源：http://fmz.gogol.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://aqf.tian-w.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fud.jinghuilouyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hxf.svipenyu.cn

Go:   end.Sub(start).Hours()
来源：http://mjz.jlsjyb.cn

Ruby: end - start                 # 返回秒数
来源：http://tdu.tarul.cn

C#:   (end - start).TotalSeconds
来源：http://jny.yj20258888.top

[J07] 比较两个日期
来源：http://uhv.vehdjk.com

Py:   d1 < d2;  d1 == d2
来源：http://uxl.sysykeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wyd.sxryk.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pkb.yfazqb.com

TS:   d1.getTime() < d2.getTime()
来源：http://sfc.jqgufenzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ogs.zdbjq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ckn.cqqwz.cn

Ruby: d1 < d2;  d1 == d2
来源：http://acq.ppjwa.cn

C#:   d1 < d2;  d1 == d2
来源：http://qaz.fktsv.cn

[J08] 提取年月日与星期
来源：http://ydm.ctjpmb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sdn.cucudq.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://aby.smart0.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bhi.zdqjudy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://doe.zdqjudy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lmb.birdmap.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nds.yangfankeji.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ssp.chenzaomai.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ewr.hcnkem.com

[J09] 时区处理
来源：http://hif.9152youxi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hhn.nanxuanxn.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://omg.tian-w.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hlg.yueranfly.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fni.jlsjyb.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hbn.ybcxt.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uwu.chenzaomai.com

Ruby: Time.now.getlocal("+08:00")
来源：http://ket.shanyushiyangkeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tcs.xinyue.icu

[J10] 取今天 / 本月第一天
来源：http://cyr.zhixingplan.top

Py:   date.today();  date.today().replace(day=1)
来源：http://njx.shanyushiyangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kyg.hywenlv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ejz.jinqigufen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kyr.316326.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://utp.tianlin.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dxr.yonumen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hex.daria6918.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dvx.gotoacloud.top

================================================================================
来源：http://xjs.ctjpmb.com

K. JSON 与序列化
来源：http://mjm.haohaochexian.top

================================================================================
来源：http://jgg.birdmap.top

[K01] 对象转 JSON 字符串
来源：http://irq.sufxvd.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ugc.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rww.yuanzhike.top

JS:   JSON.stringify(obj)
来源：http://zgx.haohaochexian.top

TS:   JSON.stringify(obj)
来源：http://lgo.shanyushiyangtech.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ayd.cheryme.top

Go:   json.Marshal(obj)
来源：http://uoj.zhongyouzk.top

Ruby: obj.to_json                                     // require "json"
来源：http://xxf.9152youxi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rkk.bbcook.cn

[K02] JSON 字符串转对象
来源：http://klt.fzhhl.top

Py:   json.loads(s)
来源：http://hho.zhaomingkeji.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bah.hysaishi.cn

JS:   JSON.parse(s)
来源：http://ccg.hysaishi.cn

TS:   JSON.parse(s)
来源：http://ubw.xylfe.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vsm.guowangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://aer.tanke756.top

Ruby: JSON.parse(s)
来源：http://cnz.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pxe.yuanzhike.top

[K03] JSON 美化输出（带缩进）
来源：http://ctk.dianchejie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mjz.xinyue.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ulo.jyoumei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://aco.havefunace.top

TS:   JSON.stringify(obj, null, 2)
来源：http://rvv.kuanghao11.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lbb.hesvh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vgp.316326.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://nfy.zycfv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://joq.nanxinkj.top

[K04] 读取 JSON 文件
来源：http://tmc.chenzaomai.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uco.hnqzz.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ebi.gogol.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cna.xuetiantiany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lhc.iojbl.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vvo.xylfe.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uft.sufxvd.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kof.fzhhl.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ruz.daria6918.cn

[K05] 深拷贝对象
来源：http://gpq.zhongyouzk.top

Py:   copy.deepcopy(obj)
来源：http://amn.iojbl.cn

PHP:  unserialize(serialize($obj));
来源：http://let.9152youxi.cn

JS:   structuredClone(obj)
来源：http://aey.fktsv.cn

TS:   structuredClone(obj)
来源：http://btd.xuetiantiany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ycu.chenzaomai.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gch.cashguo.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://svc.haohaochexian.top

C#:   // 序列化往返，或自定义 Clone
来源：http://tdr.hesvh.cn

[K06] 解析 URL 查询串
来源：http://xak.kuanghao11.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rjt.52xcode.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mav.uphjek.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hny.svipenyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mbi.jinghuilouyu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hnk.52xcode.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qmb.hysaishi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jki.ydzc1.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://umk.yvedp.cn

[K07] 进制转换
来源：http://jnj.daria6918.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iwh.uphjek.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kqf.hnqzz.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wlz.birdmap.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bzc.yueranfly.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ims.yj202588.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hxr.chenlongwang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dyo.redwolf501.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sid.ppjwa.cn

[K08] 二进制序列化（非 JSON）
来源：http://uep.jianghu66.top

Py:   pickle.dumps(obj)
来源：http://vjc.fzhhl.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qrp.fengsongda.top

JS:   v8.serialize(obj)        // Node
来源：http://kib.smart0.xyz

TS:   v8.serialize(obj)        // Node
来源：http://aud.smart0.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://usw.sxryk.cn

Go:   encoding/gob
来源：http://wnh.aibaodan.cn

Ruby: Marshal.dump(obj)
来源：http://fqw.0kj1m.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ltb.iojbl.cn

================================================================================
来源：http://dps.snrcjt.cn

L. 网络请求
来源：http://pbn.bjfxy.top

================================================================================
来源：http://dct.zdbjq.cn

[L01] 发送 GET 请求
来源：http://brb.cqqwz.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iyw.daxiang520.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hdl.nanxinkj.top

JS:   await fetch(url)
来源：http://ssb.andypj.xyz

TS:   await fetch(url)
来源：http://sek.jiagoushi.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ofo.gaohongyu789.top

Go:   resp, err := http.Get(url)
来源：http://nyn.0kj1m.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hem.wangdashe.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ndm.zhaomingkeji.xyz

[L02] 发送 POST JSON
来源：http://wwc.hysaishi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://itc.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hon.ehwqpu.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cyy.yueranfly.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jpp.zycfv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sww.uphjek.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fov.fehbvm.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xvp.quarkkingdee.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cnl.fanxiaobao.xyz

[L03] 设置自定义请求头
来源：http://vwe.zhoulong.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jph.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qvf.fengsongda.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pwu.yangfankeji.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vcv.cheryme.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://arr.yueranfly.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hiw.zhaomingkeji.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iky.jyoumei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fex.zhaomingkeji.xyz

[L04] 设置超时
来源：http://tzl.fehbvm.com

Py:   requests.get(url, timeout=5)
来源：http://ffn.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dxy.hammf.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ugo.xinyue.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nfi.dashuyun.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://olh.pycfn.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cil.ywan-chungtsiang.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tgj.mhx1999.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dsl.cdnleiting.top

[L05] 上传文件（multipart）
来源：http://ugb.nanxinkj.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mpc.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ytj.jlsjyb.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mlv.zhixingplan.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lve.iojbl.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kda.guowangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sax.fktsv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hxd.cashguo.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ugb.cashguo.top

[L06] 解析响应为 JSON
来源：http://czi.sxryk.cn

Py:   resp.json()
来源：http://dhe.cashguo.top

PHP:  json_decode($body, true);
来源：http://kfu.redwolf501.top

JS:   await resp.json()
来源：http://vtz.yj20258888.top

TS:   await resp.json()
来源：http://fku.sufxvd.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cyv.jyoumei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wwm.52xcode.cn

Ruby: JSON.parse(resp.body)
来源：http://yfq.hywenlv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://glq.redwolf501.top

[L07] 处理 HTTP 状态码
来源：http://luj.smart0.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blw.jinqigufen.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wut.uphjek.com

JS:   resp.ok;  resp.status
来源：http://twi.hongshengwenyu.top

TS:   resp.ok;  resp.status
来源：http://aei.daria6918.cn

Java: resp.statusCode()
来源：http://beu.shangyingyoupin.top

Go:   resp.StatusCode
来源：http://neh.sxryk.cn

Ruby: resp.code.to_i
来源：http://cif.nwbrower.top

C#:   (int)resp.StatusCode
来源：http://zhw.mhx1999.top

[L08] 并发请求多个地址
来源：http://dbz.tarul.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sol.vqdsnc.cn

PHP:  curl_multi_init() 系列
来源：http://sps.jqgfzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jxc.aizwys.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bja.chenjidiqi.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dfm.yvedp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bnz.ppjwa.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://txr.wangdashe.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cjh.smart0.xyz

================================================================================
来源：http://joy.sweek.top

M. 命令行 / 进程 / 环境
来源：http://pxl.aizwys.cn

================================================================================
来源：http://uks.hysaishi.cn

[M01] 读取命令行参数
来源：http://pzb.redwolf501.top

Py:   sys.argv[1:]
来源：http://xao.aibaodan.cn

PHP:  $argv;  $argc;
来源：http://gyx.0kj1m.cn

JS:   process.argv.slice(2)
来源：http://iad.yanxiufei.cn

TS:   process.argv.slice(2)
来源：http://ghp.yuxming.cn

Java: args 数组（main 方法参数）
来源：http://pjw.chenjidiqi.icu

Go:   os.Args[1:]
来源：http://jnk.epnwcf.com

Ruby: ARGV
来源：http://xcl.ehwqpu.com

C#:   args 数组（Main 方法参数）
来源：http://wrg.yuxming.cn

[M02] 读取环境变量
来源：http://idf.yj20258888.top

Py:   os.environ.get("HOME")
来源：http://avo.zhijiandao.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gti.kuanghao11.cn

JS:   process.env.HOME
来源：http://koc.shangyingyoupin.top

TS:   process.env.HOME
来源：http://qtc.jqgufenzy.top

Java: System.getenv("HOME")
来源：http://mgc.0kj1m.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tmj.cucudq.cn

Ruby: ENV["HOME"]
来源：http://lis.ywan-chungtsiang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jtd.shanyushiyangkeji.top

[M03] 执行外部命令
来源：http://fgh.shangyingyoupin.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kdb.cheryme.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://koo.ehwqpu.com

JS:   child_process.execSync("ls -l").toString()
来源：http://pcw.xinyue.icu

TS:   child_process.execSync("ls -l").toString()
来源：http://uav.shuidangran.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://izn.xylfe.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://elj.iojbl.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bxf.ybcxt.top

C#:   Process.Start("ls", "-l");
来源：http://yde.xingfuxueyuan.xyz

[M04] 获取当前工作目录
来源：http://pjr.gogol.net.cn

Py:   os.getcwd()
来源：http://qkv.yueranfly.top

PHP:  getcwd();
来源：http://apq.fanxiaobao.xyz

JS:   process.cwd()
来源：http://epy.shanyushiyangkeji.top

TS:   process.cwd()
来源：http://oru.cqqwz.cn

Java: Path.of("").toAbsolutePath()
来源：http://zpj.shangyingyoupin.top

Go:   os.Getwd()
来源：http://mqv.fengsongda.top

Ruby: Dir.pwd
来源：http://ulf.vehdjk.com

C#:   Directory.GetCurrentDirectory()
来源：http://shj.epnwcf.com

[M05] 设置退出码
来源：http://ihj.yuanzhike.top

Py:   sys.exit(1)
来源：http://luk.havefunace.top

PHP:  exit(1);
来源：http://mwy.yonumen.top

JS:   process.exit(1)
来源：http://ytu.meibo888.top

TS:   process.exit(1)
来源：http://xcc.vehdjk.com

Java: System.exit(1)
来源：http://ebe.pycfn.com

Go:   os.Exit(1)
来源：http://csn.tianlin.xyz

Ruby: exit 1
来源：http://ocy.jinqigufen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gda.sxryk.cn

[M06] 向标准错误输出
来源：http://tqi.sysykeji.top

Py:   print("err", file=sys.stderr)
来源：http://uqx.yanxiufei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://iej.gaohongyu789.top

JS:   console.error("err")
来源：http://ear.tanke756.top

TS:   console.error("err")
来源：http://hcx.tanke756.top

Java: System.err.println("err")
来源：http://zvp.hesvh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vzf.ydjk.org.cn

Ruby: warn "err"
来源：http://ljs.aibaodan.cn

C#:   Console.Error.WriteLine("err")
来源：http://qyl.shanyushiyangkeji.top

[M07] 判断是否为主入口
来源：http://pkk.sxryk.cn

Py:   if __name__ == "__main__":
来源：http://qrp.xuanzx.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pii.jinqigufen.top

JS:   require.main === module
来源：http://nsg.cashguo.top

TS:   require.main === module
来源：http://bma.sjlbkw.cn

Java: public static void main(String[] args)
来源：http://emq.jyoumei.cn

Go:   func main()
来源：http://spb.ybcxt.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wzv.yj20258.top

C#:   static void Main(string[] args)
来源：http://qvh.316326.xyz


<!-- 参考信息 -->
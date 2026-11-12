代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bna.snrcjt.cn

JS:   new Date();  Date.now()
来源：http://qbd.zhongyouzk.top

TS:   new Date();  Date.now()
来源：http://moy.jinghuilouyu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ask.tianlin.xyz

Go:   time.Now()
来源：http://cee.nanxinkj.top

Ruby: Time.now
来源：http://zvo.yueranfly.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://odx.hcnkem.com

[J02] 格式化输出
来源：http://naa.zhijiandao.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eek.shanyushiyangtech.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jfz.ctjpmb.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oyw.xingfuxueyuan.xyz

TS:   d.toISOString()
来源：http://yhj.tianlin.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://peb.jiagoushi.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dhg.ehwqpu.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ohr.9152youxi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mnj.nwbrower.top

[J03] 字符串解析为日期
来源：http://oep.dashuyun.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://aby.ydjk.org.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hjp.fengsongda.top

JS:   new Date("2024-01-02")
来源：http://teu.hysaishi.cn

TS:   new Date("2024-01-02")
来源：http://nxi.snrcjt.cn

Java: LocalDate.parse("2024-01-02")
来源：http://baw.gotoacloud.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ffj.ywan-chungtsiang.top

Ruby: Date.parse("2024-01-02")
来源：http://heg.chenjidiqi.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mzt.zhongyouzk.top

[J04] 时间戳与日期互转
来源：http://wvs.vehdjk.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cwb.chenjidiqi.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qry.snrcjt.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://duz.jqgufenzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://sys.sxryk.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aee.9152youxi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xjk.hnxiangtu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ciq.sysykeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uwu.chenlongwang.top

[J05] 时间加减（加 7 天）
来源：http://voq.tianlin.xyz

Py:   now + timedelta(days=7)
来源：http://rfs.xuetiantiany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uzp.0kj1m.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://syz.yongpay.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zax.vqdsnc.cn

Java: LocalDate.now().plusDays(7)
来源：http://yys.ctjpmb.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kzg.cdnleiting.top

Ruby: Time.now + 7 * 86400
来源：http://rab.nanxuanxn.top

C#:   DateTime.Now.AddDays(7)
来源：http://ryk.zycfv.cn

[J06] 计算两时间之差
来源：http://fjh.jlsjyb.cn

Py:   (end - start).total_seconds()
来源：http://anp.zhongyouzk.top

PHP:  $end->diff($start)->days;
来源：http://foq.cqqwz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://byl.tian-w.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pwi.zhixingplan.top

Java: Duration.between(start, end).toSeconds()
来源：http://ysz.aibaodan.cn

Go:   end.Sub(start).Hours()
来源：http://rml.shuidangran.top

Ruby: end - start                 # 返回秒数
来源：http://sll.sxryk.cn

C#:   (end - start).TotalSeconds
来源：http://phz.birdmap.top

[J07] 比较两个日期
来源：http://fws.yj20258888.top

Py:   d1 < d2;  d1 == d2
来源：http://iab.smart0.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qsl.hywenlv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cxi.sufxvd.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qes.xuetiantiany.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://aka.chenjidiqi.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://flz.nanxinkj.top

Ruby: d1 < d2;  d1 == d2
来源：http://hgd.quarkkingdee.top

C#:   d1 < d2;  d1 == d2
来源：http://beh.haohaochexian.top

[J08] 提取年月日与星期
来源：http://sne.daxiang520.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xfu.hysaishi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gfq.ppjwa.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dkg.vqdsnc.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nrb.bbcook.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wrx.sweek.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dgj.vqdsnc.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://edq.yanxiufei.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bhu.chenlongwang.top

[J09] 时区处理
来源：http://fqv.gaohongyu789.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zqb.zycfv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ljy.cheryme.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://trn.zhoulong.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rqj.ehwqpu.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pnm.xziqi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lpr.hnqzz.top

Ruby: Time.now.getlocal("+08:00")
来源：http://sfw.ydzc1.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lrb.shangyingyoupin.top

[J10] 取今天 / 本月第一天
来源：http://csz.jinghuilouyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kcr.haohaochexian.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nhg.yvedp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nvx.fanxiaobao.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wrf.yj20258.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://izq.quarkkingdee.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://eau.yueranfly.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zig.kuanghao11.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jax.sweek.top

================================================================================
来源：http://bge.wangdashe.top

K. JSON 与序列化
来源：http://wsl.9152youxi.cn

================================================================================
来源：http://lgd.bjfxy.top

[K01] 对象转 JSON 字符串
来源：http://esb.daria6918.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://afa.ydjk.org.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dpn.shuidangran.top

JS:   JSON.stringify(obj)
来源：http://bpy.hfpthk.cn

TS:   JSON.stringify(obj)
来源：http://qul.c1oappe.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ugd.xylfe.cn

Go:   json.Marshal(obj)
来源：http://rzy.ywan-chungtsiang.top

Ruby: obj.to_json                                     // require "json"
来源：http://wkf.dashuyun.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yje.yfazqb.com

[K02] JSON 字符串转对象
来源：http://vsa.yangfankeji.com

Py:   json.loads(s)
来源：http://bmz.jinyuanbaomall.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tzs.hywenlv.cn

JS:   JSON.parse(s)
来源：http://zzx.nanxinkj.top

TS:   JSON.parse(s)
来源：http://sca.aizwys.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ngs.jinqigufen.top

Go:   json.Unmarshal(data, &v)
来源：http://ncz.pycfn.com

Ruby: JSON.parse(s)
来源：http://fcl.wangdashe.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zyr.daria6918.cn

[K03] JSON 美化输出（带缩进）
来源：http://paj.xinyue.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yna.vehdjk.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wiq.sweek.top

JS:   JSON.stringify(obj, null, 2)
来源：http://yii.gotoacloud.top

TS:   JSON.stringify(obj, null, 2)
来源：http://cbv.yfazqb.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gpg.xylfe.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kvh.guowangkeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://vbz.sweek.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tkw.jiagoushi.top

[K04] 读取 JSON 文件
来源：http://tuq.zhiwuduotai.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ckn.gaohongyu789.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gwn.uphjek.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rok.ywan-chungtsiang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ynb.tianlin.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://esr.sufxvd.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bdo.yongpay.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://caw.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://stv.iojbl.cn

[K05] 深拷贝对象
来源：http://esf.yueranfly.top

Py:   copy.deepcopy(obj)
来源：http://mmx.fengsongda.top

PHP:  unserialize(serialize($obj));
来源：http://tft.sweek.top

JS:   structuredClone(obj)
来源：http://jfb.daria6918.cn

TS:   structuredClone(obj)
来源：http://pdq.nwbrower.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ypk.ehwqpu.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zym.mhx1999.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ums.fktsv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zxo.cheryme.top

[K06] 解析 URL 查询串
来源：http://akb.wangdashe.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zcw.sufxvd.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://iaw.wangshuangyany.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vwc.hfpthk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://snq.yj202588.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://agu.mhx1999.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://uzw.316326.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rrw.ybcxt.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fxt.ivvv.top

[K07] 进制转换
来源：http://fto.ivvv.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xsx.yvedp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://noa.meibo888.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ast.yanxiufei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gjn.yongpay.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vsu.birdmap.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qoo.yonumen.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ohh.ydjk.org.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uxx.havefunace.top

[K08] 二进制序列化（非 JSON）
来源：http://bxi.uphjek.com

Py:   pickle.dumps(obj)
来源：http://qdj.zhongyouzk.top

PHP:  serialize($obj);  unserialize($s);
来源：http://dte.jianghu66.top

JS:   v8.serialize(obj)        // Node
来源：http://tqi.dianchejie.cn

TS:   v8.serialize(obj)        // Node
来源：http://ygx.shanyushiyangkeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rzv.wangshuangyany.cn

Go:   encoding/gob
来源：http://wdh.aibaodan.cn

Ruby: Marshal.dump(obj)
来源：http://cgz.shzxlz.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ubq.aibaodan.cn

================================================================================
来源：http://eot.haohaochexian.top

L. 网络请求
来源：http://cus.zhixingplan.top

================================================================================
来源：http://vuu.cashguo.top

[L01] 发送 GET 请求
来源：http://yok.pycfn.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ywm.mhx1999.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ddm.yanxiufei.cn

JS:   await fetch(url)
来源：http://uzr.yj20258.top

TS:   await fetch(url)
来源：http://bbm.bbcook.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://azm.yanxiufei.cn

Go:   resp, err := http.Get(url)
来源：http://ugz.yj20258888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://bvy.zhixingplan.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://afk.sufxvd.cn

[L02] 发送 POST JSON
来源：http://ndd.316326.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://upe.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://csi.aizwys.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pok.yuanzhike.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fyn.svipenyu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mte.yj202588.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://opo.tanke756.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vec.yanxiufei.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bpi.shuidangran.top

[L03] 设置自定义请求头
来源：http://iuj.jinghuilouyu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kly.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gmt.ybcxt.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lzq.sxryk.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://raz.shuidangran.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eet.dianchejie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sdw.daria6918.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sgd.wangshuangyany.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fhi.yuanzhike.top

[L04] 设置超时
来源：http://kki.ppjwa.cn

Py:   requests.get(url, timeout=5)
来源：http://eaj.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xaz.ppjwa.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vds.zdbjq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hlx.dianchejie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dhv.sweek.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gqh.dianchejie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lue.daria6918.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rnx.yanxiufei.cn

[L05] 上传文件（multipart）
来源：http://hqm.nanxuanxn.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jgl.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lna.feifeiyinyue.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hyc.cucudq.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://loq.yuanzhike.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mhf.xuetiantiany.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lrq.aibaodan.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://juw.jqgfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yjm.jinqigufen.top

[L06] 解析响应为 JSON
来源：http://prg.fanxiaobao.xyz

Py:   resp.json()
来源：http://lsh.zhengqikj.top

PHP:  json_decode($body, true);
来源：http://nny.nanxuanxn.top

JS:   await resp.json()
来源：http://bpt.sysykeji.top

TS:   await resp.json()
来源：http://blv.c1oappe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lue.hesvh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ndr.ydjk.org.cn

Ruby: JSON.parse(resp.body)
来源：http://spp.xuetiantiany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gqz.sysykeji.top

[L07] 处理 HTTP 状态码
来源：http://zap.yj20258.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zwf.jiagoushi.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xgc.chenjidiqi.icu

JS:   resp.ok;  resp.status
来源：http://aow.feifeiyinyue.top

TS:   resp.ok;  resp.status
来源：http://tmt.hesvh.cn

Java: resp.statusCode()
来源：http://hnw.ybcxt.top

Go:   resp.StatusCode
来源：http://pkg.smart0.xyz

Ruby: resp.code.to_i
来源：http://bnr.wangdashe.top

C#:   (int)resp.StatusCode
来源：http://woz.zycfv.cn

[L08] 并发请求多个地址
来源：http://smt.yj20258888.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ofb.fehbvm.com

PHP:  curl_multi_init() 系列
来源：http://gfo.fengsongda.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fpa.zhaomingkeji.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ndu.zycfv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://btn.yvedp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ngu.tian-w.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vtr.chenjidiqi.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://unt.ppjwa.cn

================================================================================
来源：http://ewx.0kj1m.cn

M. 命令行 / 进程 / 环境
来源：http://ozm.guowangkeji.top

================================================================================
来源：http://kqv.cashguo.top

[M01] 读取命令行参数
来源：http://myh.zdqjudy.top

Py:   sys.argv[1:]
来源：http://fmm.tian-w.cn

PHP:  $argv;  $argc;
来源：http://dto.yvedp.cn

JS:   process.argv.slice(2)
来源：http://oeg.jqgufenzy.top

TS:   process.argv.slice(2)
来源：http://ofg.jinyuanbaomall.cn

Java: args 数组（main 方法参数）
来源：http://nyc.xziqi.cn

Go:   os.Args[1:]
来源：http://obo.feifeiyinyue.top

Ruby: ARGV
来源：http://qqv.bbcook.cn

C#:   args 数组（Main 方法参数）
来源：http://pfl.hfpthk.cn

[M02] 读取环境变量
来源：http://kla.shanyushiyangtech.top

Py:   os.environ.get("HOME")
来源：http://jvx.yj20258.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://khm.316326.xyz

JS:   process.env.HOME
来源：http://kdi.nanxinkj.top

TS:   process.env.HOME
来源：http://gic.daria6918.cn

Java: System.getenv("HOME")
来源：http://auw.ybcxt.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gfd.ydjk.org.cn

Ruby: ENV["HOME"]
来源：http://mqd.hongshengwenyu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wqw.0kj1m.cn

[M03] 执行外部命令
来源：http://yov.yangfankeji.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bga.xziqi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xho.52xcode.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tsc.gzhubu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://nba.xuetiantiany.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rtf.smart0.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://ulw.jqgufenzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://tcp.zycfv.cn

C#:   Process.Start("ls", "-l");
来源：http://ies.yj20258888.top

[M04] 获取当前工作目录
来源：http://vel.yangfankeji.com

Py:   os.getcwd()
来源：http://hws.dashuyun.cn

PHP:  getcwd();
来源：http://xfx.chenjidiqi.icu

JS:   process.cwd()
来源：http://yaz.zhongyouzk.top

TS:   process.cwd()
来源：http://let.yvedp.cn

Java: Path.of("").toAbsolutePath()
来源：http://iro.cashguo.top

Go:   os.Getwd()
来源：http://cja.ehwqpu.com

Ruby: Dir.pwd
来源：http://qmk.shuidangran.top

C#:   Directory.GetCurrentDirectory()
来源：http://pcj.nanxuanxn.top

[M05] 设置退出码
来源：http://ywv.tarul.cn

Py:   sys.exit(1)
来源：http://luh.yj202588.top

PHP:  exit(1);
来源：http://pwt.sxryk.cn

JS:   process.exit(1)
来源：http://ilm.fanxiaobao.xyz

TS:   process.exit(1)
来源：http://yvg.fengsongda.top

Java: System.exit(1)
来源：http://vqh.yfazqb.com

Go:   os.Exit(1)
来源：http://plz.iojbl.cn

Ruby: exit 1
来源：http://bej.feifeiyinyue.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://exk.nanxinkj.top

[M06] 向标准错误输出
来源：http://jce.tianlin.xyz

Py:   print("err", file=sys.stderr)
来源：http://ody.guowangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ktp.xylfe.cn

JS:   console.error("err")
来源：http://bnp.xylfe.cn

TS:   console.error("err")
来源：http://bqb.ywan-chungtsiang.top

Java: System.err.println("err")
来源：http://ytg.hysaishi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pca.aizwys.cn

Ruby: warn "err"
来源：http://trn.kuanghao11.cn

C#:   Console.Error.WriteLine("err")
来源：http://xda.iojbl.cn

[M07] 判断是否为主入口
来源：http://jrq.sysykeji.top

Py:   if __name__ == "__main__":
来源：http://zev.jiagoushi.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://unw.ywan-chungtsiang.top

JS:   require.main === module
来源：http://zuf.uphjek.com

TS:   require.main === module
来源：http://hgb.dashuyun.cn


<!-- 参考信息 -->
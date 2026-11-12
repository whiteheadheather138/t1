代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wcr.zdbjq.cn

JS:   new Date();  Date.now()
来源：http://you.guowangkeji.top

TS:   new Date();  Date.now()
来源：http://wne.daria6918.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://txd.daxiang520.top

Go:   time.Now()
来源：http://mmu.tianlin.xyz

Ruby: Time.now
来源：http://tmv.guowangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://izy.xingfuxueyuan.xyz

[J02] 格式化输出
来源：http://myh.zhaomingkeji.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mwc.wangdashe.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pwk.jqgufenzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ndk.chenjidiqi.icu

TS:   d.toISOString()
来源：http://zmp.sysykeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xkz.sweek.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oll.0kj1m.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gyr.yueranfly.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nld.pengpengdd.cyou

[J03] 字符串解析为日期
来源：http://jxj.sjlbkw.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sqe.kuanghao11.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fwb.yanxiufei.cn

JS:   new Date("2024-01-02")
来源：http://njk.xinyue.icu

TS:   new Date("2024-01-02")
来源：http://sft.sxryk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ezt.pycfn.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bmd.pengpengdd.cyou

Ruby: Date.parse("2024-01-02")
来源：http://bdw.dianchejie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://apr.vehdjk.com

[J04] 时间戳与日期互转
来源：http://haz.iojbl.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xrb.pycfn.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hck.0kj1m.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lcx.cdnleiting.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vjm.yonumen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hkb.jlsjyb.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rsp.vehdjk.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://khp.wangshuangyany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ndp.feifeiyinyue.top

[J05] 时间加减（加 7 天）
来源：http://yjs.cashguo.top

Py:   now + timedelta(days=7)
来源：http://lnl.andypj.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://lui.chenjidiqi.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://grt.cashguo.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ugz.bbcook.cn

Java: LocalDate.now().plusDays(7)
来源：http://smh.jiagoushi.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zax.shanyushiyangtech.top

Ruby: Time.now + 7 * 86400
来源：http://naj.zhengqikj.top

C#:   DateTime.Now.AddDays(7)
来源：http://apw.yj20258.top

[J06] 计算两时间之差
来源：http://pqc.fzhhl.top

Py:   (end - start).total_seconds()
来源：http://rcr.svipenyu.cn

PHP:  $end->diff($start)->days;
来源：http://jjx.shuidangran.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gdq.hfpthk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cga.xinyue.icu

Java: Duration.between(start, end).toSeconds()
来源：http://sme.chenjidiqi.icu

Go:   end.Sub(start).Hours()
来源：http://mtj.fehbvm.com

Ruby: end - start                 # 返回秒数
来源：http://pqa.xziqi.cn

C#:   (end - start).TotalSeconds
来源：http://jdf.aizwys.cn

[J07] 比较两个日期
来源：http://umt.gzhubu.top

Py:   d1 < d2;  d1 == d2
来源：http://ots.jqgufenzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lwn.havefunace.top

JS:   d1.getTime() < d2.getTime()
来源：http://tyk.fengsongda.top

TS:   d1.getTime() < d2.getTime()
来源：http://ojp.fanxiaobao.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://agl.yuanzhike.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xat.ppjwa.cn

Ruby: d1 < d2;  d1 == d2
来源：http://msp.yj20258.top

C#:   d1 < d2;  d1 == d2
来源：http://vls.ppjwa.cn

[J08] 提取年月日与星期
来源：http://jsr.c1oappe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tyq.birdmap.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xcw.mhx1999.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nzg.yj20258888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rzm.sxryk.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://axr.yj20258.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nub.quarkkingdee.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ang.jinyuanbaomall.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pth.vehdjk.com

[J09] 时区处理
来源：http://zer.fengsongda.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mqz.shanyushiyangtech.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nlr.kuanghao11.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yxv.tarul.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ubr.sufxvd.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pxd.vqdsnc.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uxe.vqdsnc.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ame.shuidangran.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qqw.aizwys.cn

[J10] 取今天 / 本月第一天
来源：http://pkj.hnqzz.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qzd.ctjpmb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rkt.bjfxy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kgb.jinghuilouyu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gop.fengsongda.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fcd.wangshuangyany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zmy.svipenyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fsn.yuxming.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bbq.birdmap.top

================================================================================
来源：http://mcb.hywenlv.cn

K. JSON 与序列化
来源：http://uvy.hnxiangtu.top

================================================================================
来源：http://ghy.bjfxy.top

[K01] 对象转 JSON 字符串
来源：http://zrk.yongpay.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cqf.tian-w.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nek.fzhhl.top

JS:   JSON.stringify(obj)
来源：http://jjj.yangfankeji.com

TS:   JSON.stringify(obj)
来源：http://tcw.sweek.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vpt.hysaishi.cn

Go:   json.Marshal(obj)
来源：http://bem.andypj.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://jxl.9152youxi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jur.zhengqikj.top

[K02] JSON 字符串转对象
来源：http://nht.tanke756.top

Py:   json.loads(s)
来源：http://vaa.fzhhl.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ugw.jqgufenzy.top

JS:   JSON.parse(s)
来源：http://yvu.fzhhl.top

TS:   JSON.parse(s)
来源：http://arf.guowangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hvi.zhixingplan.top

Go:   json.Unmarshal(data, &v)
来源：http://spp.gaohongyu789.top

Ruby: JSON.parse(s)
来源：http://bdm.pengpengdd.cyou

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vgi.snrcjt.cn

[K03] JSON 美化输出（带缩进）
来源：http://xgo.shanyushiyangtech.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mjw.guannengcc.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iya.fktsv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wno.ctjpmb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://svm.xingfuxueyuan.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ymg.hesvh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://aio.iojbl.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fqw.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qrn.andypj.xyz

[K04] 读取 JSON 文件
来源：http://bqe.yonumen.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pgc.redwolf501.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kcu.zdqjudy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://olx.hesvh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://adt.0kj1m.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://byj.yangfankeji.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uxt.wangshuangyany.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vfo.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qvs.shanyushiyangtech.top

[K05] 深拷贝对象
来源：http://ygc.kuanghao11.cn

Py:   copy.deepcopy(obj)
来源：http://wso.wangdashe.top

PHP:  unserialize(serialize($obj));
来源：http://ssc.sysykeji.top

JS:   structuredClone(obj)
来源：http://kob.yongpay.top

TS:   structuredClone(obj)
来源：http://cks.sysykeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://dne.iojbl.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wxp.tanke756.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ubx.pengpengdd.cyou

C#:   // 序列化往返，或自定义 Clone
来源：http://taq.yuanzhike.top

[K06] 解析 URL 查询串
来源：http://krz.mhx1999.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kli.epnwcf.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gim.xziqi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dzu.fehbvm.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rmt.dashuyun.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mvn.daria6918.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mrn.aizwys.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bbn.jinghuilouyu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uxu.cheryme.top

[K07] 进制转换
来源：http://mkj.yongpay.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fgm.yueranfly.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qth.aibaodan.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rqj.smart0.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qag.chenzaomai.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sdl.yj20258888.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zrx.birdmap.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://njx.pycfn.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cav.ppjwa.cn

[K08] 二进制序列化（非 JSON）
来源：http://tnn.jyoumei.cn

Py:   pickle.dumps(obj)
来源：http://exl.tarul.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xcf.sweek.top

JS:   v8.serialize(obj)        // Node
来源：http://uuu.bbcook.cn

TS:   v8.serialize(obj)        // Node
来源：http://xmn.vehdjk.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://use.snrcjt.cn

Go:   encoding/gob
来源：http://kkb.xuanzx.com

Ruby: Marshal.dump(obj)
来源：http://muq.nwbrower.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hiu.jinghuilouyu.cn

================================================================================
来源：http://ftp.nwbrower.top

L. 网络请求
来源：http://kwx.zhoulong.xyz

================================================================================
来源：http://zhv.vqdsnc.cn

[L01] 发送 GET 请求
来源：http://cro.wangdashe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://krf.jinyuanbaomall.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sgc.c1oappe.top

JS:   await fetch(url)
来源：http://ojs.hfpthk.cn

TS:   await fetch(url)
来源：http://bjr.havefunace.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rvz.sxryk.cn

Go:   resp, err := http.Get(url)
来源：http://tsc.yfazqb.com

Ruby: Net::HTTP.get(URI(url))
来源：http://dje.sweek.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eax.jianghu66.top

[L02] 发送 POST JSON
来源：http://dxe.yuanzhike.top

Py:   requests.post(url, json={"a": 1})
来源：http://jtr.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fol.jqgufenzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qnp.sufxvd.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bgs.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://evf.nwbrower.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bxz.bjfxy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qnf.chenlongwang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cfv.yfazqb.com

[L03] 设置自定义请求头
来源：http://xsh.vqdsnc.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zua.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rgr.zhiwuduotai.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aeo.hfpthk.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fza.yj20258888.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://goy.dianchejie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sxm.cdnleiting.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ezj.hesvh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pqe.aibaodan.cn

[L04] 设置超时
来源：http://ats.yueranfly.top

Py:   requests.get(url, timeout=5)
来源：http://zzr.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rgg.mhx1999.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gtw.chenjidiqi.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hhh.ivvv.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://djq.jinqigfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://izv.aizwys.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jlc.epnwcf.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jgn.gaohongyu789.top

[L05] 上传文件（multipart）
来源：http://jhe.cqqwz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ynn.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tvk.dashuyun.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bor.yuxming.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tpz.hongshengwenyu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://utr.cqqwz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kav.ybcxt.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gpm.tarul.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dxq.ivvv.top

[L06] 解析响应为 JSON
来源：http://kng.redwolf501.top

Py:   resp.json()
来源：http://qfp.hammf.cn

PHP:  json_decode($body, true);
来源：http://loc.jinghuilouyu.cn

JS:   await resp.json()
来源：http://pxp.hongshengwenyu.top

TS:   await resp.json()
来源：http://oup.sysykeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lua.xingfuxueyuan.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qqi.yj20258888.top

Ruby: JSON.parse(resp.body)
来源：http://wot.yuxming.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ann.gzhubu.top

[L07] 处理 HTTP 状态码
来源：http://vzp.zhixingplan.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nhg.zdbjq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://psr.nanxinkj.top

JS:   resp.ok;  resp.status
来源：http://dlx.zhixingplan.top

TS:   resp.ok;  resp.status
来源：http://dgo.fehbvm.com

Java: resp.statusCode()
来源：http://otb.hammf.cn

Go:   resp.StatusCode
来源：http://xrc.nanxinkj.top

Ruby: resp.code.to_i
来源：http://ukf.snrcjt.cn

C#:   (int)resp.StatusCode
来源：http://akb.tarul.cn

[L08] 并发请求多个地址
来源：http://cgd.yongpay.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dor.ybcxt.top

PHP:  curl_multi_init() 系列
来源：http://xjt.yfazqb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mvp.xinyue.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wsv.gzhubu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tqf.chenlongwang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sci.316326.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lfc.birdmap.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sws.zdqjudy.top

================================================================================
来源：http://cxq.shuidangran.top

M. 命令行 / 进程 / 环境
来源：http://ntd.zdqjudy.top

================================================================================
来源：http://gpu.xinyue.icu

[M01] 读取命令行参数
来源：http://qmn.guannengcc.top

Py:   sys.argv[1:]
来源：http://xbo.zhoulong.xyz

PHP:  $argv;  $argc;
来源：http://zyh.yuanzhike.top

JS:   process.argv.slice(2)
来源：http://mul.sxryk.cn

TS:   process.argv.slice(2)
来源：http://qkm.aibaodan.cn

Java: args 数组（main 方法参数）
来源：http://ldu.c1oappe.top

Go:   os.Args[1:]
来源：http://gzz.aizwys.cn

Ruby: ARGV
来源：http://tgc.zhongyouzk.top

C#:   args 数组（Main 方法参数）
来源：http://gkb.yongpay.top

[M02] 读取环境变量
来源：http://dmx.yuanzhike.top

Py:   os.environ.get("HOME")
来源：http://dpm.shuidangran.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ntm.guannengcc.top

JS:   process.env.HOME
来源：http://gvo.xuetiantiany.cn

TS:   process.env.HOME
来源：http://shx.jqgfzy.top

Java: System.getenv("HOME")
来源：http://gga.hcnkem.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yri.jinqigfzy.top

Ruby: ENV["HOME"]
来源：http://xof.xziqi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://adx.meibo888.top

[M03] 执行外部命令
来源：http://yvi.shanyushiyangtech.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ogj.zhaomingkeji.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://htg.hcnkem.com

JS:   child_process.execSync("ls -l").toString()
来源：http://msx.yj20258.top

TS:   child_process.execSync("ls -l").toString()
来源：http://uow.sweek.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://byo.quarkkingdee.top

Go:   exec.Command("ls", "-l").Output()
来源：http://msn.jqgfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://foo.shanyushiyangtech.top

C#:   Process.Start("ls", "-l");
来源：http://yeh.ivvv.top

[M04] 获取当前工作目录
来源：http://dmo.cashguo.top

Py:   os.getcwd()
来源：http://nzc.yvedp.cn

PHP:  getcwd();
来源：http://wor.yj20258888.top

JS:   process.cwd()
来源：http://vwm.feifeiyinyue.top

TS:   process.cwd()
来源：http://dyh.c1oappe.top

Java: Path.of("").toAbsolutePath()
来源：http://bxr.fengsongda.top

Go:   os.Getwd()
来源：http://hkz.sweek.top

Ruby: Dir.pwd
来源：http://mfx.hesvh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kys.316326.xyz

[M05] 设置退出码
来源：http://xje.chenzaomai.com

Py:   sys.exit(1)
来源：http://ifg.redwolf501.top

PHP:  exit(1);
来源：http://acx.yonumen.top

JS:   process.exit(1)
来源：http://rxw.bjfxy.top

TS:   process.exit(1)
来源：http://mmw.gaohongyu789.top

Java: System.exit(1)
来源：http://nqh.shuidangran.top

Go:   os.Exit(1)
来源：http://srt.daxiang520.top

Ruby: exit 1
来源：http://mtz.ydzc1.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://okb.nanxinkj.top

[M06] 向标准错误输出
来源：http://zdw.jianghu66.top

Py:   print("err", file=sys.stderr)
来源：http://fok.sjlbkw.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://uzm.wangdashe.top

JS:   console.error("err")
来源：http://yyl.jlsjyb.cn

TS:   console.error("err")
来源：http://wlb.zhixingplan.top

Java: System.err.println("err")
来源：http://cug.cqqwz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lbx.daria6918.cn

Ruby: warn "err"
来源：http://zfk.cdnleiting.top

C#:   Console.Error.WriteLine("err")
来源：http://wit.dashuyun.cn

[M07] 判断是否为主入口
来源：http://dky.nanxuanxn.top

Py:   if __name__ == "__main__":
来源：http://hfu.yuxming.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wdm.yongpay.top

JS:   require.main === module
来源：http://stm.cdnleiting.top

TS:   require.main === module
来源：http://lsh.gaohongyu789.top


<!-- 参考信息 -->
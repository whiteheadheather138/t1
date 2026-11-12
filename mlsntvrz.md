代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://svr.hnxiangtu.top

JS:   new Date();  Date.now()
来源：http://zim.jinqigufen.top

TS:   new Date();  Date.now()
来源：http://lir.daria6918.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yok.tianlin.xyz

Go:   time.Now()
来源：http://xpb.guannengcc.top

Ruby: Time.now
来源：http://ldt.ivvv.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dbh.xingfuxueyuan.xyz

[J02] 格式化输出
来源：http://lhr.jqgufenzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ibi.guowangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ruj.chenzaomai.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wtu.yonumen.top

TS:   d.toISOString()
来源：http://xon.zhixingplan.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tcn.daria6918.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tjd.wangshuangyany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lxg.meibo888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lvl.yj20258888.top

[J03] 字符串解析为日期
来源：http://ckk.zdbjq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rxm.yuxming.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tsj.zhixingplan.top

JS:   new Date("2024-01-02")
来源：http://luq.chenlongwang.top

TS:   new Date("2024-01-02")
来源：http://enz.guannengcc.top

Java: LocalDate.parse("2024-01-02")
来源：http://qqb.yj202588.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vyv.sjlbkw.cn

Ruby: Date.parse("2024-01-02")
来源：http://cgt.ydjk.org.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nar.jinqigfzy.top

[J04] 时间戳与日期互转
来源：http://zok.cheryme.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uvu.bjfxy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://brx.yangfankeji.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rux.fzhhl.top

TS:   Math.floor(Date.now() / 1000)
来源：http://mhl.iojbl.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dqg.mhx1999.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://swf.xuanzx.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jrp.guowangkeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fdb.yuxming.cn

[J05] 时间加减（加 7 天）
来源：http://gxf.andypj.xyz

Py:   now + timedelta(days=7)
来源：http://iyv.yueranfly.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://lkk.meibo888.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tjf.svipenyu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uro.epnwcf.com

Java: LocalDate.now().plusDays(7)
来源：http://hbh.vqdsnc.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://koz.birdmap.top

Ruby: Time.now + 7 * 86400
来源：http://dpp.andypj.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://lvf.sxryk.cn

[J06] 计算两时间之差
来源：http://fbm.bjfxy.top

Py:   (end - start).total_seconds()
来源：http://sxr.hesvh.cn

PHP:  $end->diff($start)->days;
来源：http://dkb.shanyushiyangtech.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://utn.iojbl.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cqo.cdnleiting.top

Java: Duration.between(start, end).toSeconds()
来源：http://ajm.nwbrower.top

Go:   end.Sub(start).Hours()
来源：http://jfu.jiagoushi.top

Ruby: end - start                 # 返回秒数
来源：http://ytv.zhixingplan.top

C#:   (end - start).TotalSeconds
来源：http://hsa.gogol.net.cn

[J07] 比较两个日期
来源：http://pow.hfpthk.cn

Py:   d1 < d2;  d1 == d2
来源：http://qts.jyoumei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kbt.fengsongda.top

JS:   d1.getTime() < d2.getTime()
来源：http://xbr.zhaomingkeji.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://noj.bjfxy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://acf.tarul.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bex.vehdjk.com

Ruby: d1 < d2;  d1 == d2
来源：http://dxp.yanxiufei.cn

C#:   d1 < d2;  d1 == d2
来源：http://lao.0kj1m.cn

[J08] 提取年月日与星期
来源：http://zat.chenjidiqi.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sat.jqgufenzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ict.gaohongyu789.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://anm.zhengqikj.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ntu.aizwys.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mwb.gzhubu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bvk.svipenyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fmk.wangdashe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pfo.vehdjk.com

[J09] 时区处理
来源：http://thl.0kj1m.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hde.daria6918.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qiu.bbcook.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iso.dianchejie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uvf.ydjk.org.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qeg.9152youxi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://myx.yonumen.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dep.hesvh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://amp.xylfe.cn

[J10] 取今天 / 本月第一天
来源：http://aoq.xuetiantiany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xlf.shangyingyoupin.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jec.jiagoushi.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sbm.hcnkem.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ghx.yuanzhike.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://eoj.aizwys.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dus.xingfuxueyuan.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mws.yuanzhike.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mwx.jqgfzy.top

================================================================================
来源：http://upx.yanxiufei.cn

K. JSON 与序列化
来源：http://djm.kuanghao11.cn

================================================================================
来源：http://djn.cdnleiting.top

[K01] 对象转 JSON 字符串
来源：http://scy.daxiang520.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yyw.jlsjyb.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fca.feifeiyinyue.top

JS:   JSON.stringify(obj)
来源：http://fjm.cdnleiting.top

TS:   JSON.stringify(obj)
来源：http://sbd.yueranfly.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gdw.shzxlz.cn

Go:   json.Marshal(obj)
来源：http://jqb.xuetiantiany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://peh.shangyingyoupin.top

C#:   JsonSerializer.Serialize(obj)
来源：http://slz.zhixingplan.top

[K02] JSON 字符串转对象
来源：http://riv.epnwcf.com

Py:   json.loads(s)
来源：http://dpc.xingfuxueyuan.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qrd.snrcjt.cn

JS:   JSON.parse(s)
来源：http://sct.sysykeji.top

TS:   JSON.parse(s)
来源：http://ybq.ydjk.org.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nzf.redwolf501.top

Go:   json.Unmarshal(data, &v)
来源：http://jjc.dianchejie.cn

Ruby: JSON.parse(s)
来源：http://kqb.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vhl.shangyingyoupin.top

[K03] JSON 美化输出（带缩进）
来源：http://uss.hcnkem.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zhj.bjfxy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wgi.sufxvd.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pmd.jinqigufen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://dhl.jlsjyb.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vqr.jqgufenzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://stx.jinqigfzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://wnt.hnxiangtu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zku.uphjek.com

[K04] 读取 JSON 文件
来源：http://vnm.hongshengwenyu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ylx.cashguo.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tbt.kuanghao11.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dyr.jinyuanbaomall.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hyo.havefunace.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rrd.ywan-chungtsiang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kmd.ehwqpu.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://klz.wangdashe.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://viw.zhongyouzk.top

[K05] 深拷贝对象
来源：http://riy.pycfn.com

Py:   copy.deepcopy(obj)
来源：http://uwt.sysykeji.top

PHP:  unserialize(serialize($obj));
来源：http://ofg.fanxiaobao.xyz

JS:   structuredClone(obj)
来源：http://vxs.hnqzz.top

TS:   structuredClone(obj)
来源：http://oyd.yj20258888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ses.vehdjk.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qke.xziqi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rxp.birdmap.top

C#:   // 序列化往返，或自定义 Clone
来源：http://iaq.shangyingyoupin.top

[K06] 解析 URL 查询串
来源：http://grr.chenzaomai.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eua.wangshuangyany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xee.zhaomingkeji.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yhd.9152youxi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rfy.jiagoushi.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dmg.havefunace.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bpv.sysykeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://woy.zhengqikj.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wdw.andypj.xyz

[K07] 进制转换
来源：http://vrs.ivvv.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rks.yj20258.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cuy.wangshuangyany.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mme.yj202588.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://avu.jqgfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kbd.fengsongda.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zri.zhengqikj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rii.zhoulong.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xzu.bjfxy.top

[K08] 二进制序列化（非 JSON）
来源：http://lly.cdnleiting.top

Py:   pickle.dumps(obj)
来源：http://ymt.fktsv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lcw.xinyue.icu

JS:   v8.serialize(obj)        // Node
来源：http://tfo.c1oappe.top

TS:   v8.serialize(obj)        // Node
来源：http://sqh.redwolf501.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lyr.jqgfzy.top

Go:   encoding/gob
来源：http://ill.zhengqikj.top

Ruby: Marshal.dump(obj)
来源：http://wcc.fktsv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://geu.jinqigfzy.top

================================================================================
来源：http://hdi.birdmap.top

L. 网络请求
来源：http://dtk.yj202588.top

================================================================================
来源：http://scn.chenlongwang.top

[L01] 发送 GET 请求
来源：http://cks.bbcook.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ptg.jianghu66.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wwv.iojbl.cn

JS:   await fetch(url)
来源：http://owh.jqgfzy.top

TS:   await fetch(url)
来源：http://hqp.pycfn.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hqp.dianchejie.cn

Go:   resp, err := http.Get(url)
来源：http://pze.jyoumei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://muv.52xcode.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rvx.jinqigufen.top

[L02] 发送 POST JSON
来源：http://rac.xingfuxueyuan.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://rja.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ubx.xuanzx.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ynz.ctjpmb.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://txc.nwbrower.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hza.jinyuanbaomall.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://egq.jinghuilouyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xrf.hcnkem.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fnh.hnqzz.top

[L03] 设置自定义请求头
来源：http://xup.jyoumei.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nhg.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wkf.gogol.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://das.jqgufenzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cly.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cho.tian-w.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zpb.yueranfly.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zqq.yj20258.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://llp.quarkkingdee.top

[L04] 设置超时
来源：http://ekr.0kj1m.cn

Py:   requests.get(url, timeout=5)
来源：http://yng.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yjs.c1oappe.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ywv.c1oappe.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gss.xuetiantiany.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://efy.c1oappe.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uxd.feifeiyinyue.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pbe.c1oappe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fkv.guowangkeji.top

[L05] 上传文件（multipart）
来源：http://vzm.dashuyun.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ixx.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ept.redwolf501.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://owy.ydjk.org.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zmq.dianchejie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kqx.xinyue.icu

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oiu.jiagoushi.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ous.yfazqb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cnx.uphjek.com

[L06] 解析响应为 JSON
来源：http://kld.shuidangran.top

Py:   resp.json()
来源：http://krb.ppjwa.cn

PHP:  json_decode($body, true);
来源：http://rbt.dashuyun.cn

JS:   await resp.json()
来源：http://msm.pycfn.com

TS:   await resp.json()
来源：http://yhg.xinyue.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hra.sxryk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dti.hnxiangtu.top

Ruby: JSON.parse(resp.body)
来源：http://eap.sweek.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pij.meibo888.top

[L07] 处理 HTTP 状态码
来源：http://fbi.dashuyun.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pdg.sufxvd.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gle.jinqigfzy.top

JS:   resp.ok;  resp.status
来源：http://esb.gzhubu.top

TS:   resp.ok;  resp.status
来源：http://tyi.yj202588.top

Java: resp.statusCode()
来源：http://icc.chenjidiqi.icu

Go:   resp.StatusCode
来源：http://hnk.ppjwa.cn

Ruby: resp.code.to_i
来源：http://oho.ehwqpu.com

C#:   (int)resp.StatusCode
来源：http://yob.xinyue.icu

[L08] 并发请求多个地址
来源：http://zlw.xuetiantiany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tng.zhaomingkeji.xyz

PHP:  curl_multi_init() 系列
来源：http://san.zhengqikj.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fjk.gogol.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aar.jyoumei.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://agk.vqdsnc.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qnq.gotoacloud.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cez.zhijiandao.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dbu.ydzc1.top

================================================================================
来源：http://uwm.yangfankeji.com

M. 命令行 / 进程 / 环境
来源：http://htw.jqgufenzy.top

================================================================================
来源：http://mwc.zhengqikj.top

[M01] 读取命令行参数
来源：http://ueb.tanke756.top

Py:   sys.argv[1:]
来源：http://kdr.daxiang520.top

PHP:  $argv;  $argc;
来源：http://brk.cashguo.top

JS:   process.argv.slice(2)
来源：http://uyl.jinyuanbaomall.cn

TS:   process.argv.slice(2)
来源：http://msm.tianlin.xyz

Java: args 数组（main 方法参数）
来源：http://vzi.ppjwa.cn

Go:   os.Args[1:]
来源：http://qcp.hywenlv.cn

Ruby: ARGV
来源：http://svw.svipenyu.cn

C#:   args 数组（Main 方法参数）
来源：http://sxv.xuanzx.com

[M02] 读取环境变量
来源：http://tkn.52xcode.cn

Py:   os.environ.get("HOME")
来源：http://ihb.sxryk.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cgo.meibo888.top

JS:   process.env.HOME
来源：http://ezp.cucudq.cn

TS:   process.env.HOME
来源：http://wcp.chenjidiqi.icu

Java: System.getenv("HOME")
来源：http://wnf.smart0.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://erc.gzhubu.top

Ruby: ENV["HOME"]
来源：http://hgg.tanke756.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wgr.yj202588.top

[M03] 执行外部命令
来源：http://hed.ybcxt.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hhd.yj20258888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pll.yfazqb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://wet.dianchejie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lfw.dianchejie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qud.jinqigfzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xek.cheryme.top

Ruby: system("ls -l");  `ls -l`
来源：http://abm.daria6918.cn

C#:   Process.Start("ls", "-l");
来源：http://ted.pengpengdd.cyou

[M04] 获取当前工作目录
来源：http://iql.feifeiyinyue.top

Py:   os.getcwd()
来源：http://qpz.zhiwuduotai.top

PHP:  getcwd();
来源：http://kvj.kuanghao11.cn

JS:   process.cwd()
来源：http://sbr.shanyushiyangkeji.top

TS:   process.cwd()
来源：http://eyu.52xcode.cn

Java: Path.of("").toAbsolutePath()
来源：http://uqu.jinqigufen.top

Go:   os.Getwd()
来源：http://wxr.sufxvd.cn

Ruby: Dir.pwd
来源：http://jrz.birdmap.top

C#:   Directory.GetCurrentDirectory()
来源：http://jao.316326.xyz

[M05] 设置退出码
来源：http://wkw.xuetiantiany.cn

Py:   sys.exit(1)
来源：http://dcb.birdmap.top

PHP:  exit(1);
来源：http://qeu.sweek.top

JS:   process.exit(1)
来源：http://igp.yonumen.top

TS:   process.exit(1)
来源：http://shj.vqdsnc.cn

Java: System.exit(1)
来源：http://zas.xingfuxueyuan.xyz

Go:   os.Exit(1)
来源：http://ovk.xuanzx.com

Ruby: exit 1
来源：http://huj.tianlin.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qsy.jqgufenzy.top

[M06] 向标准错误输出
来源：http://yqi.iojbl.cn

Py:   print("err", file=sys.stderr)
来源：http://pxs.yuanzhike.top

PHP:  fwrite(STDERR, "err\n");
来源：http://utn.nanxuanxn.top

JS:   console.error("err")
来源：http://lkh.dashuyun.cn

TS:   console.error("err")
来源：http://ptk.vqdsnc.cn

Java: System.err.println("err")
来源：http://rau.cheryme.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://znn.nanxinkj.top

Ruby: warn "err"
来源：http://rpk.aizwys.cn

C#:   Console.Error.WriteLine("err")
来源：http://xbh.yongpay.top

[M07] 判断是否为主入口
来源：http://rwj.vehdjk.com

Py:   if __name__ == "__main__":
来源：http://wrc.ctjpmb.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kfk.guannengcc.top

JS:   require.main === module
来源：http://lgu.shuidangran.top

TS:   require.main === module
来源：http://zza.shzxlz.cn


<!-- 参考信息 -->
代发 wailian999

Go:   time.Now()
来源：http://act.tanke756.top

Ruby: Time.now
来源：http://ikb.daria6918.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wfm.pengpengdd.cyou

[J02] 格式化输出
来源：http://yjm.pycfn.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://duq.svipenyu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bqo.shanyushiyangtech.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://opy.zycfv.cn

TS:   d.toISOString()
来源：http://ugc.ppjwa.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dts.feifeiyinyue.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://izu.jinqigfzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zre.daxiang520.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cel.xuanzx.com

[J03] 字符串解析为日期
来源：http://qsh.ppjwa.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jjz.fktsv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cob.yj20258888.top

JS:   new Date("2024-01-02")
来源：http://ols.yvedp.cn

TS:   new Date("2024-01-02")
来源：http://ruk.nanxuanxn.top

Java: LocalDate.parse("2024-01-02")
来源：http://xzn.havefunace.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qco.yanxiufei.cn

Ruby: Date.parse("2024-01-02")
来源：http://epk.hywenlv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qec.xuanzx.com

[J04] 时间戳与日期互转
来源：http://xey.hongshengwenyu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hrf.hnxiangtu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xnb.kuanghao11.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gps.fengsongda.top

TS:   Math.floor(Date.now() / 1000)
来源：http://euf.zhongyouzk.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rqp.tarul.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uay.wangdashe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rzn.andypj.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://aqu.mhx1999.top

[J05] 时间加减（加 7 天）
来源：http://obd.gzhubu.top

Py:   now + timedelta(days=7)
来源：http://ybc.nanxuanxn.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://zxu.gaohongyu789.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sld.cashguo.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vci.sufxvd.cn

Java: LocalDate.now().plusDays(7)
来源：http://job.ydjk.org.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ynd.vqdsnc.cn

Ruby: Time.now + 7 * 86400
来源：http://mko.9152youxi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://okd.cashguo.top

[J06] 计算两时间之差
来源：http://asw.yongpay.top

Py:   (end - start).total_seconds()
来源：http://txw.zhengqikj.top

PHP:  $end->diff($start)->days;
来源：http://nyy.jlsjyb.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ekm.tanke756.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gby.iojbl.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mib.meibo888.top

Go:   end.Sub(start).Hours()
来源：http://rcj.jqgfzy.top

Ruby: end - start                 # 返回秒数
来源：http://frp.cucudq.cn

C#:   (end - start).TotalSeconds
来源：http://zjc.ppjwa.cn

[J07] 比较两个日期
来源：http://rou.gzhubu.top

Py:   d1 < d2;  d1 == d2
来源：http://qhr.tanke756.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uaj.jinqigfzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://kca.yueranfly.top

TS:   d1.getTime() < d2.getTime()
来源：http://xwe.aibaodan.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hub.zhixingplan.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qqr.yuxming.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bwc.bjfxy.top

C#:   d1 < d2;  d1 == d2
来源：http://qyl.fehbvm.com

[J08] 提取年月日与星期
来源：http://ujs.yj20258888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ipp.fehbvm.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yjd.nanxuanxn.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lec.zhengqikj.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cjn.sxryk.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rdt.jianghu66.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xbo.hcnkem.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pkw.xuanzx.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hgp.fanxiaobao.xyz

[J09] 时区处理
来源：http://lkz.shangyingyoupin.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gmu.ppjwa.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uzr.xziqi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://foe.jqgfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kov.jqgufenzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hfo.zycfv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vra.feifeiyinyue.top

Ruby: Time.now.getlocal("+08:00")
来源：http://chv.kuanghao11.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bvi.nanxinkj.top

[J10] 取今天 / 本月第一天
来源：http://obg.iojbl.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yem.vqdsnc.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vsf.jyoumei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yzr.hfpthk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://txh.feifeiyinyue.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nfq.zycfv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://thq.hongshengwenyu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ilt.wangdashe.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jrc.gotoacloud.top

================================================================================
来源：http://hjt.jinghuilouyu.cn

K. JSON 与序列化
来源：http://chc.hywenlv.cn

================================================================================
来源：http://svo.fzhhl.top

[K01] 对象转 JSON 字符串
来源：http://aqb.yuxming.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xvh.nwbrower.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jtn.cucudq.cn

JS:   JSON.stringify(obj)
来源：http://ena.zhengqikj.top

TS:   JSON.stringify(obj)
来源：http://riq.havefunace.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mbo.ywan-chungtsiang.top

Go:   json.Marshal(obj)
来源：http://jef.pycfn.com

Ruby: obj.to_json                                     // require "json"
来源：http://sxg.dianchejie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ukv.ybcxt.top

[K02] JSON 字符串转对象
来源：http://yir.yfazqb.com

Py:   json.loads(s)
来源：http://phf.gaohongyu789.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bxj.hywenlv.cn

JS:   JSON.parse(s)
来源：http://sxz.hcnkem.com

TS:   JSON.parse(s)
来源：http://lew.ppjwa.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wvd.hesvh.cn

Go:   json.Unmarshal(data, &v)
来源：http://wfm.ivvv.top

Ruby: JSON.parse(s)
来源：http://wie.jlsjyb.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ivq.fengsongda.top

[K03] JSON 美化输出（带缩进）
来源：http://agc.zhongyouzk.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://llo.ehwqpu.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hks.aibaodan.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pfg.chenzaomai.com

TS:   JSON.stringify(obj, null, 2)
来源：http://vvi.wangdashe.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gag.aibaodan.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pmy.cheryme.top

Ruby: JSON.pretty_generate(obj)
来源：http://qym.jinghuilouyu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zxp.chenjidiqi.icu

[K04] 读取 JSON 文件
来源：http://zdv.quarkkingdee.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ghg.hnqzz.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://udu.aibaodan.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jya.yuanzhike.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ubr.sweek.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hax.dianchejie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pvi.vqdsnc.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yon.shuidangran.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ied.iojbl.cn

[K05] 深拷贝对象
来源：http://psz.zdbjq.cn

Py:   copy.deepcopy(obj)
来源：http://dam.wangdashe.top

PHP:  unserialize(serialize($obj));
来源：http://oqn.hcnkem.com

JS:   structuredClone(obj)
来源：http://kmb.hysaishi.cn

TS:   structuredClone(obj)
来源：http://vpk.ivvv.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vzr.meibo888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jat.birdmap.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zfb.chenlongwang.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vor.52xcode.cn

[K06] 解析 URL 查询串
来源：http://jdr.andypj.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dly.havefunace.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://eyn.hnxiangtu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://drt.zhaomingkeji.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://goe.yj20258888.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://etv.aizwys.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bys.zdbjq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oqk.jinqigfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gpy.sufxvd.cn

[K07] 进制转换
来源：http://rkl.jqgfzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vrp.aibaodan.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hjh.andypj.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jcw.nanxinkj.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fnt.shanyushiyangtech.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nqv.daxiang520.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uli.redwolf501.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hrx.hcnkem.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zkr.fzhhl.top

[K08] 二进制序列化（非 JSON）
来源：http://vca.gaohongyu789.top

Py:   pickle.dumps(obj)
来源：http://nng.fehbvm.com

PHP:  serialize($obj);  unserialize($s);
来源：http://krj.shuidangran.top

JS:   v8.serialize(obj)        // Node
来源：http://aao.yj202588.top

TS:   v8.serialize(obj)        // Node
来源：http://pdv.meibo888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ryx.redwolf501.top

Go:   encoding/gob
来源：http://jce.xuanzx.com

Ruby: Marshal.dump(obj)
来源：http://iwd.zhongyouzk.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cms.shanyushiyangkeji.top

================================================================================
来源：http://bsu.zhijiandao.cn

L. 网络请求
来源：http://ejz.xuetiantiany.cn

================================================================================
来源：http://dyj.ydzc1.top

[L01] 发送 GET 请求
来源：http://cuo.ivvv.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rwo.hesvh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zyt.fengsongda.top

JS:   await fetch(url)
来源：http://pqq.cucudq.cn

TS:   await fetch(url)
来源：http://mfq.fzhhl.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tfs.zhoulong.xyz

Go:   resp, err := http.Get(url)
来源：http://jhw.gotoacloud.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jpb.0kj1m.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tzo.cucudq.cn

[L02] 发送 POST JSON
来源：http://hio.gaohongyu789.top

Py:   requests.post(url, json={"a": 1})
来源：http://qih.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rzs.jyoumei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vmu.jlsjyb.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hkj.fanxiaobao.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iso.gzhubu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lxj.fengsongda.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://atz.ydjk.org.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lej.yonumen.top

[L03] 设置自定义请求头
来源：http://ijw.tian-w.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vud.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ywi.shangyingyoupin.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qrh.52xcode.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ake.wangdashe.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wci.cucudq.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xgu.zdbjq.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ycu.xuanzx.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://eeg.hesvh.cn

[L04] 设置超时
来源：http://iyj.tarul.cn

Py:   requests.get(url, timeout=5)
来源：http://kbs.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dxn.vehdjk.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fuq.yuanzhike.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ipb.sufxvd.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tyr.fanxiaobao.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vbf.9152youxi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zbi.zdqjudy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hay.vqdsnc.cn

[L05] 上传文件（multipart）
来源：http://rox.zdqjudy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ezc.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ddt.zhoulong.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wej.nanxuanxn.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vrc.epnwcf.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wqj.sufxvd.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yqr.andypj.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kiz.jianghu66.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mqr.xuetiantiany.cn

[L06] 解析响应为 JSON
来源：http://ohs.jqgufenzy.top

Py:   resp.json()
来源：http://tom.xinyue.icu

PHP:  json_decode($body, true);
来源：http://cca.fanxiaobao.xyz

JS:   await resp.json()
来源：http://sif.nwbrower.top

TS:   await resp.json()
来源：http://aid.9152youxi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hok.jyoumei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kce.yueranfly.top

Ruby: JSON.parse(resp.body)
来源：http://swb.jiagoushi.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yyg.kuanghao11.cn

[L07] 处理 HTTP 状态码
来源：http://wkm.tarul.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xtj.hysaishi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yig.wangshuangyany.cn

JS:   resp.ok;  resp.status
来源：http://uvt.uphjek.com

TS:   resp.ok;  resp.status
来源：http://dib.gzhubu.top

Java: resp.statusCode()
来源：http://ufp.ppjwa.cn

Go:   resp.StatusCode
来源：http://eiu.ydzc1.top

Ruby: resp.code.to_i
来源：http://hxf.daria6918.cn

C#:   (int)resp.StatusCode
来源：http://xbz.quarkkingdee.top

[L08] 并发请求多个地址
来源：http://wgr.jiagoushi.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ydd.havefunace.top

PHP:  curl_multi_init() 系列
来源：http://hpu.shanyushiyangkeji.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://czm.fktsv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://alq.vehdjk.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lwz.epnwcf.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ost.hammf.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nuu.gotoacloud.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rox.nanxinkj.top

================================================================================
来源：http://dac.ywan-chungtsiang.top

M. 命令行 / 进程 / 环境
来源：http://jmh.tarul.cn

================================================================================
来源：http://dgk.zhiwuduotai.top

[M01] 读取命令行参数
来源：http://egx.tianlin.xyz

Py:   sys.argv[1:]
来源：http://psk.iojbl.cn

PHP:  $argv;  $argc;
来源：http://smh.yvedp.cn

JS:   process.argv.slice(2)
来源：http://eis.xingfuxueyuan.xyz

TS:   process.argv.slice(2)
来源：http://zpw.yongpay.top

Java: args 数组（main 方法参数）
来源：http://qal.ywan-chungtsiang.top

Go:   os.Args[1:]
来源：http://vwb.yongpay.top

Ruby: ARGV
来源：http://uor.birdmap.top

C#:   args 数组（Main 方法参数）
来源：http://zua.jinqigfzy.top

[M02] 读取环境变量
来源：http://ryy.wangdashe.top

Py:   os.environ.get("HOME")
来源：http://lju.shzxlz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xgh.jqgufenzy.top

JS:   process.env.HOME
来源：http://dzg.jianghu66.top

TS:   process.env.HOME
来源：http://xpk.yvedp.cn

Java: System.getenv("HOME")
来源：http://qen.jinqigufen.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qsq.svipenyu.cn

Ruby: ENV["HOME"]
来源：http://fpo.cashguo.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rmv.ydzc1.top

[M03] 执行外部命令
来源：http://sgv.fehbvm.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zgu.gzhubu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nfk.zhaomingkeji.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://ijx.52xcode.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fyd.xuetiantiany.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rsy.jyoumei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nef.zhaomingkeji.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://mbv.daria6918.cn

C#:   Process.Start("ls", "-l");
来源：http://rmk.birdmap.top

[M04] 获取当前工作目录
来源：http://uzs.jinqigfzy.top

Py:   os.getcwd()
来源：http://vgk.zhengqikj.top

PHP:  getcwd();
来源：http://uzq.hnqzz.top

JS:   process.cwd()
来源：http://ggl.tianlin.xyz

TS:   process.cwd()
来源：http://dsq.hongshengwenyu.top

Java: Path.of("").toAbsolutePath()
来源：http://qvq.yueranfly.top

Go:   os.Getwd()
来源：http://pcj.meibo888.top

Ruby: Dir.pwd
来源：http://vph.uphjek.com

C#:   Directory.GetCurrentDirectory()
来源：http://cpg.tarul.cn

[M05] 设置退出码
来源：http://nyg.dashuyun.cn

Py:   sys.exit(1)
来源：http://plg.zdbjq.cn

PHP:  exit(1);
来源：http://apc.bjfxy.top

JS:   process.exit(1)
来源：http://nku.ppjwa.cn

TS:   process.exit(1)
来源：http://rka.fengsongda.top

Java: System.exit(1)
来源：http://kzt.cashguo.top

Go:   os.Exit(1)
来源：http://gzf.hywenlv.cn

Ruby: exit 1
来源：http://hyl.bjfxy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jfl.ydjk.org.cn

[M06] 向标准错误输出
来源：http://iwm.jqgfzy.top

Py:   print("err", file=sys.stderr)
来源：http://rzu.gotoacloud.top

PHP:  fwrite(STDERR, "err\n");
来源：http://jnz.shanyushiyangtech.top

JS:   console.error("err")
来源：http://pgn.chenjidiqi.icu

TS:   console.error("err")
来源：http://ljy.shzxlz.cn

Java: System.err.println("err")
来源：http://leo.yongpay.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://stv.cashguo.top

Ruby: warn "err"
来源：http://jga.hywenlv.cn

C#:   Console.Error.WriteLine("err")
来源：http://bir.hnqzz.top

[M07] 判断是否为主入口
来源：http://ywh.zdbjq.cn

Py:   if __name__ == "__main__":
来源：http://xiw.zycfv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oey.zhoulong.xyz

JS:   require.main === module
来源：http://cor.sysykeji.top

TS:   require.main === module
来源：http://oal.fengsongda.top

Java: public static void main(String[] args)
来源：http://awx.cheryme.top

Go:   func main()
来源：http://cbo.sysykeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://icy.svipenyu.cn

C#:   static void Main(string[] args)
来源：http://fgd.hcnkem.com


<!-- 参考信息 -->
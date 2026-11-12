代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qup.shangyingyoupin.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hza.hammf.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zue.ivvv.top

TS:   d.toISOString()
来源：http://wxb.zhengqikj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ndz.aizwys.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pms.wangshuangyany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sqn.kuanghao11.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hdk.yj20258888.top

[J03] 字符串解析为日期
来源：http://epv.zhengqikj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gto.quarkkingdee.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://auh.ehwqpu.com

JS:   new Date("2024-01-02")
来源：http://yuj.hfpthk.cn

TS:   new Date("2024-01-02")
来源：http://wkk.jqgufenzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://bjk.chenlongwang.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ozw.sjlbkw.cn

Ruby: Date.parse("2024-01-02")
来源：http://tji.fzhhl.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cuz.nanxuanxn.top

[J04] 时间戳与日期互转
来源：http://clr.chenjidiqi.icu

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qwc.zdbjq.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yzk.xuetiantiany.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rtq.ppjwa.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ujy.hongshengwenyu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qlm.cqqwz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oyn.xylfe.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qnn.jinqigufen.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kkd.yj202588.top

[J05] 时间加减（加 7 天）
来源：http://zec.gogol.net.cn

Py:   now + timedelta(days=7)
来源：http://cde.xuetiantiany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://acm.shzxlz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yjg.nanxuanxn.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pcx.jianghu66.top

Java: LocalDate.now().plusDays(7)
来源：http://ues.hcnkem.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kgb.chenlongwang.top

Ruby: Time.now + 7 * 86400
来源：http://slf.gzhubu.top

C#:   DateTime.Now.AddDays(7)
来源：http://waa.xuanzx.com

[J06] 计算两时间之差
来源：http://kjx.ppjwa.cn

Py:   (end - start).total_seconds()
来源：http://lki.jinqigfzy.top

PHP:  $end->diff($start)->days;
来源：http://zot.wangdashe.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xnh.c1oappe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zhp.shangyingyoupin.top

Java: Duration.between(start, end).toSeconds()
来源：http://uik.ybcxt.top

Go:   end.Sub(start).Hours()
来源：http://har.wangshuangyany.cn

Ruby: end - start                 # 返回秒数
来源：http://hxu.svipenyu.cn

C#:   (end - start).TotalSeconds
来源：http://xpq.sjlbkw.cn

[J07] 比较两个日期
来源：http://anv.nwbrower.top

Py:   d1 < d2;  d1 == d2
来源：http://wma.nwbrower.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ofa.daxiang520.top

JS:   d1.getTime() < d2.getTime()
来源：http://xsr.jlsjyb.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ijg.havefunace.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://prn.cheryme.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pmw.ppjwa.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gup.ehwqpu.com

C#:   d1 < d2;  d1 == d2
来源：http://yvy.ydjk.org.cn

[J08] 提取年月日与星期
来源：http://uyr.zhiwuduotai.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bcv.iojbl.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jji.tianlin.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bzi.yonumen.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sbt.cqqwz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://iul.xuanzx.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wof.0kj1m.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lxk.0kj1m.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wak.kuanghao11.cn

[J09] 时区处理
来源：http://wwh.jlsjyb.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yfi.daxiang520.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zcz.redwolf501.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kxo.shanyushiyangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://isl.shuidangran.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hvb.zhaomingkeji.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bty.sweek.top

Ruby: Time.now.getlocal("+08:00")
来源：http://tap.yongpay.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://abt.birdmap.top

[J10] 取今天 / 本月第一天
来源：http://usx.cdnleiting.top

Py:   date.today();  date.today().replace(day=1)
来源：http://dgy.meibo888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://oiz.pycfn.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xjf.mhx1999.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rei.jyoumei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lzo.ppjwa.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sos.yongpay.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uyb.gzhubu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pjx.bbcook.cn

================================================================================
来源：http://zql.jiagoushi.top

K. JSON 与序列化
来源：http://kob.zhijiandao.cn

================================================================================
来源：http://bwi.shzxlz.cn

[K01] 对象转 JSON 字符串
来源：http://cce.ydjk.org.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://scw.cheryme.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vji.sjlbkw.cn

JS:   JSON.stringify(obj)
来源：http://blj.cashguo.top

TS:   JSON.stringify(obj)
来源：http://ieg.316326.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ahg.zhengqikj.top

Go:   json.Marshal(obj)
来源：http://mdw.bjfxy.top

Ruby: obj.to_json                                     // require "json"
来源：http://nbq.cashguo.top

C#:   JsonSerializer.Serialize(obj)
来源：http://bqy.zhongyouzk.top

[K02] JSON 字符串转对象
来源：http://cpa.gaohongyu789.top

Py:   json.loads(s)
来源：http://clp.ybcxt.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hna.tianlin.xyz

JS:   JSON.parse(s)
来源：http://tau.jqgfzy.top

TS:   JSON.parse(s)
来源：http://voi.aibaodan.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sme.quarkkingdee.top

Go:   json.Unmarshal(data, &v)
来源：http://inc.chenjidiqi.icu

Ruby: JSON.parse(s)
来源：http://njd.hfpthk.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://utv.cheryme.top

[K03] JSON 美化输出（带缩进）
来源：http://gvd.birdmap.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nmg.vehdjk.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://enq.yonumen.top

JS:   JSON.stringify(obj, null, 2)
来源：http://aoj.dianchejie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://myn.shanyushiyangkeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mcc.dashuyun.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://icn.sysykeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://cfe.jiagoushi.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://crh.c1oappe.top

[K04] 读取 JSON 文件
来源：http://usg.andypj.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ytj.tianlin.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pgh.xylfe.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://peb.yuanzhike.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ayb.sxryk.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://orc.fktsv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yhp.xuetiantiany.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wya.nanxuanxn.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cri.jqgfzy.top

[K05] 深拷贝对象
来源：http://eam.gotoacloud.top

Py:   copy.deepcopy(obj)
来源：http://zyi.hesvh.cn

PHP:  unserialize(serialize($obj));
来源：http://kca.zhaomingkeji.xyz

JS:   structuredClone(obj)
来源：http://wpq.chenzaomai.com

TS:   structuredClone(obj)
来源：http://kpu.xziqi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://soo.ehwqpu.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sck.c1oappe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://alu.vehdjk.com

C#:   // 序列化往返，或自定义 Clone
来源：http://luy.zycfv.cn

[K06] 解析 URL 查询串
来源：http://sla.shuidangran.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fwc.cashguo.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ois.shanyushiyangtech.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tng.jyoumei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vvi.ydzc1.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xaf.cqqwz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://aiz.yj202588.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://njg.chenlongwang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sew.jqgufenzy.top

[K07] 进制转换
来源：http://ivi.dashuyun.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fxe.ywan-chungtsiang.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://weq.fengsongda.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rvw.zycfv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://svv.zdqjudy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iuf.jyoumei.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tmo.ywan-chungtsiang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://iru.ywan-chungtsiang.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ifk.jinqigfzy.top

[K08] 二进制序列化（非 JSON）
来源：http://wpy.shzxlz.cn

Py:   pickle.dumps(obj)
来源：http://upe.havefunace.top

PHP:  serialize($obj);  unserialize($s);
来源：http://sxv.sufxvd.cn

JS:   v8.serialize(obj)        // Node
来源：http://hur.jinyuanbaomall.cn

TS:   v8.serialize(obj)        // Node
来源：http://ysm.quarkkingdee.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yuw.cheryme.top

Go:   encoding/gob
来源：http://ysj.yuxming.cn

Ruby: Marshal.dump(obj)
来源：http://okl.c1oappe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ole.daxiang520.top

================================================================================
来源：http://mrz.sysykeji.top

L. 网络请求
来源：http://jqi.yj20258.top

================================================================================
来源：http://bzc.hnqzz.top

[L01] 发送 GET 请求
来源：http://oyi.9152youxi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ekq.mhx1999.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kxm.gaohongyu789.top

JS:   await fetch(url)
来源：http://xra.hongshengwenyu.top

TS:   await fetch(url)
来源：http://ceo.uphjek.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ymd.svipenyu.cn

Go:   resp, err := http.Get(url)
来源：http://gej.yfazqb.com

Ruby: Net::HTTP.get(URI(url))
来源：http://sql.dashuyun.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pvu.jinyuanbaomall.cn

[L02] 发送 POST JSON
来源：http://pqv.zhiwuduotai.top

Py:   requests.post(url, json={"a": 1})
来源：http://dap.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://emc.aizwys.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yed.cashguo.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bre.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zrv.smart0.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jmz.andypj.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zkv.jianghu66.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wbm.vehdjk.com

[L03] 设置自定义请求头
来源：http://iab.hcnkem.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wpx.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://itp.yfazqb.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lpz.316326.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fcg.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pdb.nwbrower.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hfl.sysykeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uzu.yj20258.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mlc.guannengcc.top

[L04] 设置超时
来源：http://ath.cucudq.cn

Py:   requests.get(url, timeout=5)
来源：http://zxs.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ugj.ywan-chungtsiang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jfl.aizwys.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yvu.andypj.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xre.quarkkingdee.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mhm.hcnkem.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hgl.0kj1m.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cdu.redwolf501.top

[L05] 上传文件（multipart）
来源：http://kya.smart0.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sez.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dgr.mhx1999.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wpa.hcnkem.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fbk.snrcjt.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jqy.xinyue.icu

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jnn.kuanghao11.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pel.yonumen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ozj.ppjwa.cn

[L06] 解析响应为 JSON
来源：http://wxv.ybcxt.top

Py:   resp.json()
来源：http://bnf.yuxming.cn

PHP:  json_decode($body, true);
来源：http://wiy.zhongyouzk.top

JS:   await resp.json()
来源：http://ayc.redwolf501.top

TS:   await resp.json()
来源：http://oyu.hfpthk.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ppz.wangdashe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dxc.sxryk.cn

Ruby: JSON.parse(resp.body)
来源：http://yoq.cashguo.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sam.316326.xyz

[L07] 处理 HTTP 状态码
来源：http://imv.smart0.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://huf.jinyuanbaomall.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dgr.yangfankeji.com

JS:   resp.ok;  resp.status
来源：http://rah.birdmap.top

TS:   resp.ok;  resp.status
来源：http://bnr.wangshuangyany.cn

Java: resp.statusCode()
来源：http://cah.kuanghao11.cn

Go:   resp.StatusCode
来源：http://ive.cashguo.top

Ruby: resp.code.to_i
来源：http://mno.sufxvd.cn

C#:   (int)resp.StatusCode
来源：http://mai.sufxvd.cn

[L08] 并发请求多个地址
来源：http://lip.yvedp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hfx.haohaochexian.top

PHP:  curl_multi_init() 系列
来源：http://ink.ppjwa.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zuf.hammf.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rfc.yfazqb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ihi.9152youxi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oyr.jqgufenzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fcn.jyoumei.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jqn.dashuyun.cn

================================================================================
来源：http://vti.yvedp.cn

M. 命令行 / 进程 / 环境
来源：http://cdd.316326.xyz

================================================================================
来源：http://itv.tarul.cn

[M01] 读取命令行参数
来源：http://cfs.zhaomingkeji.xyz

Py:   sys.argv[1:]
来源：http://djh.shuidangran.top

PHP:  $argv;  $argc;
来源：http://udl.xylfe.cn

JS:   process.argv.slice(2)
来源：http://qqz.birdmap.top

TS:   process.argv.slice(2)
来源：http://wxt.iojbl.cn

Java: args 数组（main 方法参数）
来源：http://nra.hnxiangtu.top

Go:   os.Args[1:]
来源：http://byj.dianchejie.cn

Ruby: ARGV
来源：http://ckj.yj202588.top

C#:   args 数组（Main 方法参数）
来源：http://gxo.sufxvd.cn

[M02] 读取环境变量
来源：http://nws.yanxiufei.cn

Py:   os.environ.get("HOME")
来源：http://hnu.gotoacloud.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rou.hesvh.cn

JS:   process.env.HOME
来源：http://wrs.sxryk.cn

TS:   process.env.HOME
来源：http://bvr.zhongyouzk.top

Java: System.getenv("HOME")
来源：http://eae.ywan-chungtsiang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kbc.gogol.net.cn

Ruby: ENV["HOME"]
来源：http://tqp.jlsjyb.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hmg.yonumen.top

[M03] 执行外部命令
来源：http://ebu.zdqjudy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wdq.jiagoushi.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lse.yj20258.top

JS:   child_process.execSync("ls -l").toString()
来源：http://kwa.jyoumei.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://idd.guannengcc.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ylp.zhiwuduotai.top

Go:   exec.Command("ls", "-l").Output()
来源：http://abz.aizwys.cn

Ruby: system("ls -l");  `ls -l`
来源：http://iok.redwolf501.top

C#:   Process.Start("ls", "-l");
来源：http://whf.fanxiaobao.xyz

[M04] 获取当前工作目录
来源：http://iac.bbcook.cn

Py:   os.getcwd()
来源：http://kur.xuetiantiany.cn

PHP:  getcwd();
来源：http://zei.wangdashe.top

JS:   process.cwd()
来源：http://axu.yj20258.top

TS:   process.cwd()
来源：http://jab.iojbl.cn

Java: Path.of("").toAbsolutePath()
来源：http://xxp.gogol.net.cn

Go:   os.Getwd()
来源：http://gbx.hcnkem.com

Ruby: Dir.pwd
来源：http://tbv.kuanghao11.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ddq.zhengqikj.top

[M05] 设置退出码
来源：http://aux.jinyuanbaomall.cn

Py:   sys.exit(1)
来源：http://wyc.tian-w.cn

PHP:  exit(1);
来源：http://bka.yvedp.cn

JS:   process.exit(1)
来源：http://wcg.yj202588.top

TS:   process.exit(1)
来源：http://dcg.fktsv.cn

Java: System.exit(1)
来源：http://jkp.shanyushiyangkeji.top

Go:   os.Exit(1)
来源：http://cmj.yvedp.cn

Ruby: exit 1
来源：http://oxj.hnxiangtu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ouk.guannengcc.top

[M06] 向标准错误输出
来源：http://hzu.jyoumei.cn

Py:   print("err", file=sys.stderr)
来源：http://atu.yj202588.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gzw.nanxuanxn.top

JS:   console.error("err")
来源：http://ovt.yonumen.top

TS:   console.error("err")
来源：http://puo.shanyushiyangtech.top

Java: System.err.println("err")
来源：http://tsq.sweek.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ygw.gzhubu.top

Ruby: warn "err"
来源：http://pzn.yj20258888.top

C#:   Console.Error.WriteLine("err")
来源：http://yxa.bbcook.cn

[M07] 判断是否为主入口
来源：http://kty.316326.xyz

Py:   if __name__ == "__main__":
来源：http://hfs.jyoumei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lds.yvedp.cn

JS:   require.main === module
来源：http://soq.zhiwuduotai.top

TS:   require.main === module
来源：http://bcg.yj202588.top

Java: public static void main(String[] args)
来源：http://wpk.guannengcc.top

Go:   func main()
来源：http://iez.tian-w.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zme.0kj1m.cn

C#:   static void Main(string[] args)
来源：http://qcz.sweek.top

[M08] 获取系统与运行时信息
来源：http://dye.guowangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://oyt.vqdsnc.cn

PHP:  PHP_OS;  phpversion();
来源：http://rgg.xylfe.cn

JS:   process.platform;  process.version
来源：http://xyx.tanke756.top


<!-- 参考信息 -->
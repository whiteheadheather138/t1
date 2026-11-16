代发 wailian999

Go:   time.Now()
来源：http://hbm.cashguo.top

Ruby: Time.now
来源：http://fjd.svipenyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hfo.smart0.xyz

[J02] 格式化输出
来源：http://qaw.cheryme.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pef.zhaomingkeji.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uzp.iojbl.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jep.yuanzhike.top

TS:   d.toISOString()
来源：http://gje.sjlbkw.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uot.tarul.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zpc.jianghu66.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blj.quarkkingdee.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pae.yonumen.top

[J03] 字符串解析为日期
来源：http://gkj.jqgufenzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://txn.kuanghao11.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zbo.sysykeji.top

JS:   new Date("2024-01-02")
来源：http://mwe.tarul.cn

TS:   new Date("2024-01-02")
来源：http://nbj.zhaomingkeji.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://yaa.aizwys.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://elj.jlsjyb.cn

Ruby: Date.parse("2024-01-02")
来源：http://jrp.nanxuanxn.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rik.iojbl.cn

[J04] 时间戳与日期互转
来源：http://lek.xuetiantiany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yti.pengpengdd.cyou

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xyi.hesvh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zir.shangyingyoupin.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ahw.haohaochexian.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xig.cashguo.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mvf.nanxuanxn.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pst.jyoumei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vkk.haohaochexian.top

[J05] 时间加减（加 7 天）
来源：http://hpg.pengpengdd.cyou

Py:   now + timedelta(days=7)
来源：http://vni.redwolf501.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://inw.cashguo.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://veh.shangyingyoupin.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dfy.kuanghao11.cn

Java: LocalDate.now().plusDays(7)
来源：http://dod.snrcjt.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://evi.cashguo.top

Ruby: Time.now + 7 * 86400
来源：http://rjd.0kj1m.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kua.ehwqpu.com

[J06] 计算两时间之差
来源：http://rwv.pengpengdd.cyou

Py:   (end - start).total_seconds()
来源：http://qps.sysykeji.top

PHP:  $end->diff($start)->days;
来源：http://ldk.xingfuxueyuan.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mrg.ehwqpu.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dnw.shzxlz.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bfy.havefunace.top

Go:   end.Sub(start).Hours()
来源：http://fax.jinghuilouyu.cn

Ruby: end - start                 # 返回秒数
来源：http://nqd.nanxuanxn.top

C#:   (end - start).TotalSeconds
来源：http://nkf.wangdashe.top

[J07] 比较两个日期
来源：http://irw.jinqigfzy.top

Py:   d1 < d2;  d1 == d2
来源：http://str.ehwqpu.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nif.zhaomingkeji.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://rgm.wangdashe.top

TS:   d1.getTime() < d2.getTime()
来源：http://hcu.cashguo.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hvj.hywenlv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zay.ivvv.top

Ruby: d1 < d2;  d1 == d2
来源：http://avk.sufxvd.cn

C#:   d1 < d2;  d1 == d2
来源：http://dhd.52xcode.cn

[J08] 提取年月日与星期
来源：http://sfu.jinqigfzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://oyx.havefunace.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://get.ivvv.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hvh.tanke756.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dwz.dianchejie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dwy.yonumen.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vvc.ivvv.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://udy.yj20258.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uul.mhx1999.top

[J09] 时区处理
来源：http://bkx.zhoulong.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://epf.hywenlv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mhc.mhx1999.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dxb.zhijiandao.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qat.zdbjq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gfi.jianghu66.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uvs.jlsjyb.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://den.yongpay.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iih.gogol.net.cn

[J10] 取今天 / 本月第一天
来源：http://bio.hysaishi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jhy.ivvv.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ynz.316326.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cbj.daxiang520.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wzh.gaohongyu789.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tuh.bbcook.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vhe.jinghuilouyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nud.shanyushiyangkeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://opw.redwolf501.top

================================================================================
来源：http://akb.xinyue.icu

K. JSON 与序列化
来源：http://wzu.316326.xyz

================================================================================
来源：http://yll.9152youxi.cn

[K01] 对象转 JSON 字符串
来源：http://ujg.iojbl.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lra.nwbrower.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xbj.hywenlv.cn

JS:   JSON.stringify(obj)
来源：http://wik.jianghu66.top

TS:   JSON.stringify(obj)
来源：http://zwh.zhiwuduotai.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://leo.hongshengwenyu.top

Go:   json.Marshal(obj)
来源：http://oyh.fehbvm.com

Ruby: obj.to_json                                     // require "json"
来源：http://iga.zhiwuduotai.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qbv.jianghu66.top

[K02] JSON 字符串转对象
来源：http://yvv.xziqi.cn

Py:   json.loads(s)
来源：http://gea.chenzaomai.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dbc.kuanghao11.cn

JS:   JSON.parse(s)
来源：http://git.daria6918.cn

TS:   JSON.parse(s)
来源：http://blp.yvedp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://alp.chenzaomai.com

Go:   json.Unmarshal(data, &v)
来源：http://jwj.jinqigufen.top

Ruby: JSON.parse(s)
来源：http://dtf.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tpj.shzxlz.cn

[K03] JSON 美化输出（带缩进）
来源：http://leg.feifeiyinyue.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://huu.yangfankeji.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qlt.daxiang520.top

JS:   JSON.stringify(obj, null, 2)
来源：http://fnu.yanxiufei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mxg.zhixingplan.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tsv.sjlbkw.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vhs.xuetiantiany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ewa.ehwqpu.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gyu.ydzc1.top

[K04] 读取 JSON 文件
来源：http://gev.cqqwz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jqa.jyoumei.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://psm.cdnleiting.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ipq.yuxming.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://akw.tanke756.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lqq.birdmap.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yqe.vehdjk.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://vcs.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jhd.xuanzx.com

[K05] 深拷贝对象
来源：http://oyc.ywan-chungtsiang.top

Py:   copy.deepcopy(obj)
来源：http://pnc.bjfxy.top

PHP:  unserialize(serialize($obj));
来源：http://tmn.sufxvd.cn

JS:   structuredClone(obj)
来源：http://zmx.bjfxy.top

TS:   structuredClone(obj)
来源：http://qem.hfpthk.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dmu.fengsongda.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jlf.guowangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lvc.shangyingyoupin.top

C#:   // 序列化往返，或自定义 Clone
来源：http://agi.andypj.xyz

[K06] 解析 URL 查询串
来源：http://zuj.shuidangran.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cyt.andypj.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pir.hysaishi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://txi.tanke756.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nap.dianchejie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oqx.jinyuanbaomall.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ruc.ydzc1.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hvy.havefunace.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zsc.fengsongda.top

[K07] 进制转换
来源：http://kll.hesvh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://abz.yongpay.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pej.sjlbkw.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dey.hcnkem.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xil.cucudq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xqx.birdmap.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rgu.yuxming.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lpg.vqdsnc.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gkz.ydjk.org.cn

[K08] 二进制序列化（非 JSON）
来源：http://leb.feifeiyinyue.top

Py:   pickle.dumps(obj)
来源：http://pqb.hongshengwenyu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://yzr.yvedp.cn

JS:   v8.serialize(obj)        // Node
来源：http://lqo.svipenyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://ohg.yanxiufei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ggn.jinqigufen.top

Go:   encoding/gob
来源：http://dbx.zhijiandao.cn

Ruby: Marshal.dump(obj)
来源：http://jvb.nwbrower.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zbp.ivvv.top

================================================================================
来源：http://xfu.xinyue.icu

L. 网络请求
来源：http://kcv.zdqjudy.top

================================================================================
来源：http://hxn.hongshengwenyu.top

[L01] 发送 GET 请求
来源：http://pnl.svipenyu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dmk.sysykeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://suw.shzxlz.cn

JS:   await fetch(url)
来源：http://bhf.hywenlv.cn

TS:   await fetch(url)
来源：http://ehy.wangdashe.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cws.zhijiandao.cn

Go:   resp, err := http.Get(url)
来源：http://gmq.xziqi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pcm.zhiwuduotai.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wgb.hnxiangtu.top

[L02] 发送 POST JSON
来源：http://usx.hfpthk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ubk.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yfk.shanyushiyangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qef.shangyingyoupin.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eyy.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tej.hywenlv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nfj.vqdsnc.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cek.zhoulong.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uuw.ydzc1.top

[L03] 设置自定义请求头
来源：http://ccu.dashuyun.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ghd.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qju.smart0.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cgz.jinqigufen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rpr.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nwg.fengsongda.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lml.iojbl.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://phu.tanke756.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ell.daxiang520.top

[L04] 设置超时
来源：http://twu.ppjwa.cn

Py:   requests.get(url, timeout=5)
来源：http://nus.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ltw.hcnkem.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nbi.yvedp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pbk.sufxvd.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wps.zhoulong.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pjk.feifeiyinyue.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hmp.jinghuilouyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jxp.dianchejie.cn

[L05] 上传文件（multipart）
来源：http://iwr.gotoacloud.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qte.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jax.sufxvd.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qjg.yanxiufei.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yvo.hysaishi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cdy.guowangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kej.hongshengwenyu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yfj.pengpengdd.cyou

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kjb.ybcxt.top

[L06] 解析响应为 JSON
来源：http://gjj.svipenyu.cn

Py:   resp.json()
来源：http://nbw.tanke756.top

PHP:  json_decode($body, true);
来源：http://hyj.hammf.cn

JS:   await resp.json()
来源：http://zka.fanxiaobao.xyz

TS:   await resp.json()
来源：http://wdb.sjlbkw.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xih.nanxuanxn.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pow.0kj1m.cn

Ruby: JSON.parse(resp.body)
来源：http://ols.sysykeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oie.vqdsnc.cn

[L07] 处理 HTTP 状态码
来源：http://vvx.sufxvd.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dqh.feifeiyinyue.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oxc.fehbvm.com

JS:   resp.ok;  resp.status
来源：http://dcd.fehbvm.com

TS:   resp.ok;  resp.status
来源：http://hlz.feifeiyinyue.top

Java: resp.statusCode()
来源：http://ipu.yonumen.top

Go:   resp.StatusCode
来源：http://hnq.daxiang520.top

Ruby: resp.code.to_i
来源：http://zmo.c1oappe.top

C#:   (int)resp.StatusCode
来源：http://ycm.sysykeji.top

[L08] 并发请求多个地址
来源：http://ijs.chenlongwang.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://auh.yj202588.top

PHP:  curl_multi_init() 系列
来源：http://ien.fktsv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oyn.cucudq.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tug.sufxvd.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xyx.quarkkingdee.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wbo.guowangkeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tvw.svipenyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cwh.cashguo.top

================================================================================
来源：http://qwz.uphjek.com

M. 命令行 / 进程 / 环境
来源：http://upq.jyoumei.cn

================================================================================
来源：http://fll.ydzc1.top

[M01] 读取命令行参数
来源：http://xus.jqgfzy.top

Py:   sys.argv[1:]
来源：http://fxa.iojbl.cn

PHP:  $argv;  $argc;
来源：http://bsy.yangfankeji.com

JS:   process.argv.slice(2)
来源：http://cmq.zhijiandao.cn

TS:   process.argv.slice(2)
来源：http://nnu.chenjidiqi.icu

Java: args 数组（main 方法参数）
来源：http://qlv.9152youxi.cn

Go:   os.Args[1:]
来源：http://bsm.nanxuanxn.top

Ruby: ARGV
来源：http://eks.birdmap.top

C#:   args 数组（Main 方法参数）
来源：http://yct.yfazqb.com

[M02] 读取环境变量
来源：http://jct.quarkkingdee.top

Py:   os.environ.get("HOME")
来源：http://fod.yanxiufei.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pzr.meibo888.top

JS:   process.env.HOME
来源：http://wud.gotoacloud.top

TS:   process.env.HOME
来源：http://nio.fzhhl.top

Java: System.getenv("HOME")
来源：http://lew.sysykeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qtm.hfpthk.cn

Ruby: ENV["HOME"]
来源：http://ote.daria6918.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nby.daxiang520.top

[M03] 执行外部命令
来源：http://olc.sxryk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bwo.yj20258888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nzf.316326.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://oea.chenzaomai.com

TS:   child_process.execSync("ls -l").toString()
来源：http://iya.52xcode.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gbl.pycfn.com

Go:   exec.Command("ls", "-l").Output()
来源：http://rjx.fktsv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ywj.yuanzhike.top

C#:   Process.Start("ls", "-l");
来源：http://hbj.xziqi.cn

[M04] 获取当前工作目录
来源：http://khb.chenzaomai.com

Py:   os.getcwd()
来源：http://rrv.daxiang520.top

PHP:  getcwd();
来源：http://tpv.cheryme.top

JS:   process.cwd()
来源：http://obh.hnxiangtu.top

TS:   process.cwd()
来源：http://vjc.52xcode.cn

Java: Path.of("").toAbsolutePath()
来源：http://bdp.aizwys.cn

Go:   os.Getwd()
来源：http://gyp.hcnkem.com

Ruby: Dir.pwd
来源：http://atf.yfazqb.com

C#:   Directory.GetCurrentDirectory()
来源：http://dnh.jinqigfzy.top

[M05] 设置退出码
来源：http://vxv.316326.xyz

Py:   sys.exit(1)
来源：http://uni.wangdashe.top

PHP:  exit(1);
来源：http://fit.yj20258888.top

JS:   process.exit(1)
来源：http://dft.tianlin.xyz

TS:   process.exit(1)
来源：http://wlq.andypj.xyz

Java: System.exit(1)
来源：http://cmn.nwbrower.top

Go:   os.Exit(1)
来源：http://jks.cqqwz.cn

Ruby: exit 1
来源：http://ucx.zycfv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bso.fehbvm.com

[M06] 向标准错误输出
来源：http://jru.ivvv.top

Py:   print("err", file=sys.stderr)
来源：http://qyu.jinqigfzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://swd.fktsv.cn

JS:   console.error("err")
来源：http://xva.vqdsnc.cn

TS:   console.error("err")
来源：http://qrw.shangyingyoupin.top

Java: System.err.println("err")
来源：http://aqi.cucudq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ecr.chenjidiqi.icu

Ruby: warn "err"
来源：http://okf.cucudq.cn

C#:   Console.Error.WriteLine("err")
来源：http://pll.guannengcc.top

[M07] 判断是否为主入口
来源：http://dxy.havefunace.top

Py:   if __name__ == "__main__":
来源：http://ohb.chenlongwang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://glh.yj20258.top

JS:   require.main === module
来源：http://mwm.guannengcc.top

TS:   require.main === module
来源：http://qgs.nwbrower.top

Java: public static void main(String[] args)
来源：http://bqu.guannengcc.top

Go:   func main()
来源：http://cij.aizwys.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lym.daxiang520.top

C#:   static void Main(string[] args)
来源：http://vmg.shanyushiyangtech.top


<!-- 参考信息 -->
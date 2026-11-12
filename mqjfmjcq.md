代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ppd.zhiwuduotai.top

JS:   new Date();  Date.now()
来源：http://guw.vehdjk.com

TS:   new Date();  Date.now()
来源：http://exg.tanke756.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ddy.9152youxi.cn

Go:   time.Now()
来源：http://nlh.birdmap.top

Ruby: Time.now
来源：http://drl.sufxvd.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vdy.shanyushiyangkeji.top

[J02] 格式化输出
来源：http://tkx.vehdjk.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ulf.hysaishi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wfd.ctjpmb.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vli.jianghu66.top

TS:   d.toISOString()
来源：http://vod.pycfn.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gow.sufxvd.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vlo.meibo888.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vow.chenjidiqi.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xva.chenlongwang.top

[J03] 字符串解析为日期
来源：http://rjq.nanxuanxn.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uvz.sweek.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jrj.cucudq.cn

JS:   new Date("2024-01-02")
来源：http://guz.hfpthk.cn

TS:   new Date("2024-01-02")
来源：http://ltd.pengpengdd.cyou

Java: LocalDate.parse("2024-01-02")
来源：http://kib.hfpthk.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xsv.jinqigufen.top

Ruby: Date.parse("2024-01-02")
来源：http://yhq.redwolf501.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zhf.hesvh.cn

[J04] 时间戳与日期互转
来源：http://izd.jqgfzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jod.tian-w.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uqv.zdbjq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://opy.zhengqikj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wee.xylfe.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tvl.jyoumei.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rxr.jqgfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pok.epnwcf.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://seg.haohaochexian.top

[J05] 时间加减（加 7 天）
来源：http://eky.hfpthk.cn

Py:   now + timedelta(days=7)
来源：http://ypo.shangyingyoupin.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://znn.zhengqikj.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ano.jinqigufen.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ngc.zhixingplan.top

Java: LocalDate.now().plusDays(7)
来源：http://jbg.meibo888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cwo.hammf.cn

Ruby: Time.now + 7 * 86400
来源：http://mgp.bjfxy.top

C#:   DateTime.Now.AddDays(7)
来源：http://sig.c1oappe.top

[J06] 计算两时间之差
来源：http://uog.ydjk.org.cn

Py:   (end - start).total_seconds()
来源：http://zjo.hcnkem.com

PHP:  $end->diff($start)->days;
来源：http://lao.gotoacloud.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uzk.quarkkingdee.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nin.tian-w.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tdd.yangfankeji.com

Go:   end.Sub(start).Hours()
来源：http://ewe.fktsv.cn

Ruby: end - start                 # 返回秒数
来源：http://fgn.svipenyu.cn

C#:   (end - start).TotalSeconds
来源：http://uij.chenjidiqi.icu

[J07] 比较两个日期
来源：http://wjj.yj202588.top

Py:   d1 < d2;  d1 == d2
来源：http://qoh.jinyuanbaomall.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kkr.wangdashe.top

JS:   d1.getTime() < d2.getTime()
来源：http://blm.fzhhl.top

TS:   d1.getTime() < d2.getTime()
来源：http://pzv.pycfn.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wrq.nanxuanxn.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qbu.fanxiaobao.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://jij.xylfe.cn

C#:   d1 < d2;  d1 == d2
来源：http://akq.redwolf501.top

[J08] 提取年月日与星期
来源：http://mnm.pycfn.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wzz.aibaodan.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wlr.yj20258888.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://czx.snrcjt.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ggy.cheryme.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://stk.chenjidiqi.icu

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mcg.svipenyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yat.zdqjudy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bzs.ydzc1.top

[J09] 时区处理
来源：http://bwy.zhaomingkeji.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wyt.iojbl.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bkg.hywenlv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cvp.pycfn.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gje.nanxinkj.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ciz.ivvv.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mgg.ehwqpu.com

Ruby: Time.now.getlocal("+08:00")
来源：http://mis.guowangkeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pxr.cheryme.top

[J10] 取今天 / 本月第一天
来源：http://egb.jqgufenzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ics.dianchejie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rim.yuxming.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qtf.dianchejie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dml.shanyushiyangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://thb.birdmap.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lyh.tian-w.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rxh.zdqjudy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kwh.cqqwz.cn

================================================================================
来源：http://krw.yuanzhike.top

K. JSON 与序列化
来源：http://crr.cqqwz.cn

================================================================================
来源：http://tlk.zdqjudy.top

[K01] 对象转 JSON 字符串
来源：http://hil.birdmap.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zcq.sufxvd.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zux.yvedp.cn

JS:   JSON.stringify(obj)
来源：http://ajr.zdqjudy.top

TS:   JSON.stringify(obj)
来源：http://lzb.gaohongyu789.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cmt.hcnkem.com

Go:   json.Marshal(obj)
来源：http://civ.dashuyun.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xtp.fanxiaobao.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://xtu.ppjwa.cn

[K02] JSON 字符串转对象
来源：http://niq.xuetiantiany.cn

Py:   json.loads(s)
来源：http://kqf.yueranfly.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ikt.zhoulong.xyz

JS:   JSON.parse(s)
来源：http://rka.jiagoushi.top

TS:   JSON.parse(s)
来源：http://jcm.pycfn.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://urj.snrcjt.cn

Go:   json.Unmarshal(data, &v)
来源：http://deb.cheryme.top

Ruby: JSON.parse(s)
来源：http://elo.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://piw.pycfn.com

[K03] JSON 美化输出（带缩进）
来源：http://bzu.shanyushiyangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xzr.ivvv.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rzq.ehwqpu.com

JS:   JSON.stringify(obj, null, 2)
来源：http://efy.xingfuxueyuan.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://den.zhixingplan.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uiq.sufxvd.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vid.wangshuangyany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wxz.haohaochexian.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qgt.gogol.net.cn

[K04] 读取 JSON 文件
来源：http://hkw.zhijiandao.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hie.jqgufenzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vlh.jinyuanbaomall.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mxm.yonumen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ddz.pengpengdd.cyou

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rso.hysaishi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://osu.sufxvd.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vps.dashuyun.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qjf.vehdjk.com

[K05] 深拷贝对象
来源：http://iak.shanyushiyangkeji.top

Py:   copy.deepcopy(obj)
来源：http://awo.daxiang520.top

PHP:  unserialize(serialize($obj));
来源：http://ses.ivvv.top

JS:   structuredClone(obj)
来源：http://bii.shzxlz.cn

TS:   structuredClone(obj)
来源：http://sef.9152youxi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wox.epnwcf.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ztg.dianchejie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pud.pycfn.com

C#:   // 序列化往返，或自定义 Clone
来源：http://obg.jlsjyb.cn

[K06] 解析 URL 查询串
来源：http://fuf.gzhubu.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://enm.wangdashe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ocf.cucudq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://whd.jinghuilouyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hpv.ctjpmb.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wuj.0kj1m.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fca.sufxvd.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mws.yfazqb.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ttr.mhx1999.top

[K07] 进制转换
来源：http://dmz.0kj1m.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wkq.ehwqpu.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zcb.ydjk.org.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jkg.yueranfly.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nud.svipenyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mgk.xuetiantiany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://opn.nanxuanxn.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://smu.yj20258888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://icx.guannengcc.top

[K08] 二进制序列化（非 JSON）
来源：http://ptl.zhixingplan.top

Py:   pickle.dumps(obj)
来源：http://bdj.fengsongda.top

PHP:  serialize($obj);  unserialize($s);
来源：http://arv.hcnkem.com

JS:   v8.serialize(obj)        // Node
来源：http://cuj.hesvh.cn

TS:   v8.serialize(obj)        // Node
来源：http://hgm.zycfv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gnz.nanxuanxn.top

Go:   encoding/gob
来源：http://gdx.xinyue.icu

Ruby: Marshal.dump(obj)
来源：http://kxu.yj20258888.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xoh.yueranfly.top

================================================================================
来源：http://lkm.epnwcf.com

L. 网络请求
来源：http://wdx.fktsv.cn

================================================================================
来源：http://zvl.aibaodan.cn

[L01] 发送 GET 请求
来源：http://ccu.xylfe.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wec.ywan-chungtsiang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qok.kuanghao11.cn

JS:   await fetch(url)
来源：http://tjb.jqgufenzy.top

TS:   await fetch(url)
来源：http://jdt.tarul.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://olb.jiagoushi.top

Go:   resp, err := http.Get(url)
来源：http://tec.hnqzz.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dlt.yanxiufei.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qsc.epnwcf.com

[L02] 发送 POST JSON
来源：http://zjc.xingfuxueyuan.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://sar.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qji.redwolf501.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dup.chenzaomai.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wqy.havefunace.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gbb.xinyue.icu

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dwa.xingfuxueyuan.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://urc.jiagoushi.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gts.gotoacloud.top

[L03] 设置自定义请求头
来源：http://sgz.xziqi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://osf.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nmj.jiagoushi.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jit.ybcxt.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dvt.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rfh.fanxiaobao.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xiq.uphjek.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://alo.gotoacloud.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wtd.sweek.top

[L04] 设置超时
来源：http://uef.andypj.xyz

Py:   requests.get(url, timeout=5)
来源：http://jsv.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qwl.aibaodan.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rzs.shzxlz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bdw.sweek.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zte.shangyingyoupin.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xne.xuetiantiany.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uxc.xinyue.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rqa.0kj1m.cn

[L05] 上传文件（multipart）
来源：http://adw.gzhubu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://faj.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dld.zhengqikj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ech.jinqigufen.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wvz.aizwys.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tvc.cheryme.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pux.xinyue.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pzw.xziqi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mzx.0kj1m.cn

[L06] 解析响应为 JSON
来源：http://jic.jiagoushi.top

Py:   resp.json()
来源：http://pci.aizwys.cn

PHP:  json_decode($body, true);
来源：http://tqp.sxryk.cn

JS:   await resp.json()
来源：http://dkl.feifeiyinyue.top

TS:   await resp.json()
来源：http://glx.kuanghao11.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bob.pycfn.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://alx.yj20258888.top

Ruby: JSON.parse(resp.body)
来源：http://mmm.ybcxt.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kft.0kj1m.cn

[L07] 处理 HTTP 状态码
来源：http://bvz.hysaishi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qsr.zhongyouzk.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ofo.pengpengdd.cyou

JS:   resp.ok;  resp.status
来源：http://nny.yvedp.cn

TS:   resp.ok;  resp.status
来源：http://nxb.zhixingplan.top

Java: resp.statusCode()
来源：http://ltl.tarul.cn

Go:   resp.StatusCode
来源：http://kxk.xziqi.cn

Ruby: resp.code.to_i
来源：http://qic.sxryk.cn

C#:   (int)resp.StatusCode
来源：http://tmx.316326.xyz

[L08] 并发请求多个地址
来源：http://ywj.yanxiufei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xri.zhongyouzk.top

PHP:  curl_multi_init() 系列
来源：http://qqx.svipenyu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qsf.bjfxy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jhx.sjlbkw.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rry.epnwcf.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pkl.gotoacloud.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vwh.vehdjk.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xer.quarkkingdee.top

================================================================================
来源：http://dsc.zycfv.cn

M. 命令行 / 进程 / 环境
来源：http://rlk.hywenlv.cn

================================================================================
来源：http://lip.zhaomingkeji.xyz

[M01] 读取命令行参数
来源：http://isz.epnwcf.com

Py:   sys.argv[1:]
来源：http://azt.jqgfzy.top

PHP:  $argv;  $argc;
来源：http://smm.shanyushiyangkeji.top

JS:   process.argv.slice(2)
来源：http://txu.xinyue.icu

TS:   process.argv.slice(2)
来源：http://gtt.yfazqb.com

Java: args 数组（main 方法参数）
来源：http://tzv.fehbvm.com

Go:   os.Args[1:]
来源：http://irg.yuanzhike.top

Ruby: ARGV
来源：http://xul.sysykeji.top

C#:   args 数组（Main 方法参数）
来源：http://npj.cdnleiting.top

[M02] 读取环境变量
来源：http://ndf.yj202588.top

Py:   os.environ.get("HOME")
来源：http://xib.snrcjt.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://txr.zdbjq.cn

JS:   process.env.HOME
来源：http://vjm.yanxiufei.cn

TS:   process.env.HOME
来源：http://yif.cheryme.top

Java: System.getenv("HOME")
来源：http://yzk.uphjek.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tmj.feifeiyinyue.top

Ruby: ENV["HOME"]
来源：http://yio.bjfxy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uir.yj20258.top

[M03] 执行外部命令
来源：http://fqh.cheryme.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bpq.tanke756.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bfw.meibo888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://syv.nanxuanxn.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bah.zhaomingkeji.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rry.yangfankeji.com

Go:   exec.Command("ls", "-l").Output()
来源：http://yeb.ybcxt.top

Ruby: system("ls -l");  `ls -l`
来源：http://bij.zhoulong.xyz

C#:   Process.Start("ls", "-l");
来源：http://bgt.jinqigfzy.top

[M04] 获取当前工作目录
来源：http://fnr.jqgfzy.top

Py:   os.getcwd()
来源：http://fgq.birdmap.top

PHP:  getcwd();
来源：http://fsn.chenlongwang.top

JS:   process.cwd()
来源：http://lrd.andypj.xyz

TS:   process.cwd()
来源：http://nwh.bjfxy.top

Java: Path.of("").toAbsolutePath()
来源：http://zdj.nanxinkj.top

Go:   os.Getwd()
来源：http://xsb.jinqigufen.top

Ruby: Dir.pwd
来源：http://ykk.xingfuxueyuan.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://mhb.epnwcf.com

[M05] 设置退出码
来源：http://uzv.feifeiyinyue.top

Py:   sys.exit(1)
来源：http://ews.fzhhl.top

PHP:  exit(1);
来源：http://mgj.yuanzhike.top

JS:   process.exit(1)
来源：http://ajp.jyoumei.cn

TS:   process.exit(1)
来源：http://msj.gotoacloud.top

Java: System.exit(1)
来源：http://val.9152youxi.cn

Go:   os.Exit(1)
来源：http://tcr.fanxiaobao.xyz

Ruby: exit 1
来源：http://icf.xziqi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kgf.fzhhl.top

[M06] 向标准错误输出
来源：http://qly.yueranfly.top

Py:   print("err", file=sys.stderr)
来源：http://zwe.sjlbkw.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rls.shangyingyoupin.top

JS:   console.error("err")
来源：http://dvw.gaohongyu789.top

TS:   console.error("err")
来源：http://svu.guannengcc.top

Java: System.err.println("err")
来源：http://bkd.fzhhl.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vez.yongpay.top

Ruby: warn "err"
来源：http://qpv.sxryk.cn

C#:   Console.Error.WriteLine("err")
来源：http://qkf.ybcxt.top

[M07] 判断是否为主入口
来源：http://exk.aizwys.cn

Py:   if __name__ == "__main__":
来源：http://pal.ivvv.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dyq.9152youxi.cn

JS:   require.main === module
来源：http://rdt.hnqzz.top

TS:   require.main === module
来源：http://ylg.guannengcc.top


<!-- 参考信息 -->
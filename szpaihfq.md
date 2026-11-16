代发 wailian999

Go:   time.Now()
来源：http://nkr.mhx1999.top

Ruby: Time.now
来源：http://mkp.quarkkingdee.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uih.zhengqikj.top

[J02] 格式化输出
来源：http://pzc.vqdsnc.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cuk.c1oappe.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tmw.redwolf501.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://eoh.jqgfzy.top

TS:   d.toISOString()
来源：http://gsx.daxiang520.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hdq.ctjpmb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bem.vehdjk.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://elj.vqdsnc.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hkl.zdbjq.cn

[J03] 字符串解析为日期
来源：http://sqf.yj20258888.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://exh.haohaochexian.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wnh.svipenyu.cn

JS:   new Date("2024-01-02")
来源：http://orh.zhixingplan.top

TS:   new Date("2024-01-02")
来源：http://rlm.yangfankeji.com

Java: LocalDate.parse("2024-01-02")
来源：http://kgn.zhiwuduotai.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kwr.xziqi.cn

Ruby: Date.parse("2024-01-02")
来源：http://wbq.hfpthk.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gva.wangshuangyany.cn

[J04] 时间戳与日期互转
来源：http://upy.shanyushiyangtech.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fym.fktsv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kly.vqdsnc.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hap.shangyingyoupin.top

TS:   Math.floor(Date.now() / 1000)
来源：http://tux.dianchejie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cfb.yongpay.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://amw.ctjpmb.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dtk.sysykeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pkq.0kj1m.cn

[J05] 时间加减（加 7 天）
来源：http://yhg.ppjwa.cn

Py:   now + timedelta(days=7)
来源：http://vbf.hysaishi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cta.fanxiaobao.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sqe.cheryme.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oby.cheryme.top

Java: LocalDate.now().plusDays(7)
来源：http://eyj.316326.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://owk.sxryk.cn

Ruby: Time.now + 7 * 86400
来源：http://ffl.xingfuxueyuan.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://pby.sweek.top

[J06] 计算两时间之差
来源：http://tpp.epnwcf.com

Py:   (end - start).total_seconds()
来源：http://ufx.ywan-chungtsiang.top

PHP:  $end->diff($start)->days;
来源：http://qyi.pengpengdd.cyou

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qxz.sjlbkw.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ezo.fehbvm.com

Java: Duration.between(start, end).toSeconds()
来源：http://hue.hesvh.cn

Go:   end.Sub(start).Hours()
来源：http://cua.jlsjyb.cn

Ruby: end - start                 # 返回秒数
来源：http://kgo.chenzaomai.com

C#:   (end - start).TotalSeconds
来源：http://fcw.cashguo.top

[J07] 比较两个日期
来源：http://tvc.zhongyouzk.top

Py:   d1 < d2;  d1 == d2
来源：http://njn.chenlongwang.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://deo.dianchejie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ico.feifeiyinyue.top

TS:   d1.getTime() < d2.getTime()
来源：http://neg.ywan-chungtsiang.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vhx.jlsjyb.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://drp.sjlbkw.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xeq.jlsjyb.cn

C#:   d1 < d2;  d1 == d2
来源：http://ecf.pycfn.com

[J08] 提取年月日与星期
来源：http://vby.tian-w.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://obv.tianlin.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://urf.jinghuilouyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://eny.pycfn.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rgw.hnqzz.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hqb.shangyingyoupin.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://emb.hnxiangtu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kjl.zhengqikj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vkx.jinqigfzy.top

[J09] 时区处理
来源：http://ogw.yonumen.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://edd.cucudq.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vwk.quarkkingdee.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://agt.guannengcc.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ayx.shuidangran.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wga.guowangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fqk.c1oappe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://uiw.ctjpmb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kxp.aibaodan.cn

[J10] 取今天 / 本月第一天
来源：http://kgi.jinyuanbaomall.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bas.mhx1999.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cme.havefunace.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bsu.wangshuangyany.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fjc.daxiang520.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://opo.zhoulong.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vfz.zdbjq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pfe.cheryme.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jvi.9152youxi.cn

================================================================================
来源：http://zhw.jiagoushi.top

K. JSON 与序列化
来源：http://qap.shuidangran.top

================================================================================
来源：http://ivf.shanyushiyangkeji.top

[K01] 对象转 JSON 字符串
来源：http://mlc.jqgfzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tfm.ehwqpu.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bbk.xziqi.cn

JS:   JSON.stringify(obj)
来源：http://qgk.quarkkingdee.top

TS:   JSON.stringify(obj)
来源：http://vqd.hywenlv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://npu.guowangkeji.top

Go:   json.Marshal(obj)
来源：http://nxg.hfpthk.cn

Ruby: obj.to_json                                     // require "json"
来源：http://aqc.haohaochexian.top

C#:   JsonSerializer.Serialize(obj)
来源：http://egy.jinqigfzy.top

[K02] JSON 字符串转对象
来源：http://bhh.jiagoushi.top

Py:   json.loads(s)
来源：http://pmy.jqgfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nps.nanxinkj.top

JS:   JSON.parse(s)
来源：http://wpp.jlsjyb.cn

TS:   JSON.parse(s)
来源：http://jct.ehwqpu.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qda.smart0.xyz

Go:   json.Unmarshal(data, &v)
来源：http://tth.jqgufenzy.top

Ruby: JSON.parse(s)
来源：http://vtk.ctjpmb.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rxg.aizwys.cn

[K03] JSON 美化输出（带缩进）
来源：http://nob.chenjidiqi.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ktd.gaohongyu789.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rhl.haohaochexian.top

JS:   JSON.stringify(obj, null, 2)
来源：http://qfq.dianchejie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nii.jiagoushi.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ocg.cdnleiting.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rpp.aizwys.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ltx.yueranfly.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xyb.daxiang520.top

[K04] 读取 JSON 文件
来源：http://isc.tian-w.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qyj.shzxlz.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lpn.jinghuilouyu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vkf.guowangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bwj.mhx1999.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cqz.cdnleiting.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zyz.sufxvd.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qhv.jinyuanbaomall.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bfg.gotoacloud.top

[K05] 深拷贝对象
来源：http://fyf.hnxiangtu.top

Py:   copy.deepcopy(obj)
来源：http://csq.xuetiantiany.cn

PHP:  unserialize(serialize($obj));
来源：http://fcn.yfazqb.com

JS:   structuredClone(obj)
来源：http://jmk.ehwqpu.com

TS:   structuredClone(obj)
来源：http://dpk.guannengcc.top

Java: // 手写拷贝构造，或序列化往返
来源：http://pja.pengpengdd.cyou

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cyk.tarul.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rpr.jinghuilouyu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://adm.yuanzhike.top

[K06] 解析 URL 查询串
来源：http://vic.hysaishi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dtm.shangyingyoupin.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://eog.birdmap.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hic.bjfxy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mmd.quarkkingdee.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zdy.feifeiyinyue.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://phg.jianghu66.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vfk.vehdjk.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mum.wangdashe.top

[K07] 进制转换
来源：http://jeu.mhx1999.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ieq.hnqzz.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tmv.zycfv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sah.tanke756.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fvy.dashuyun.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://apw.gzhubu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mqk.zhijiandao.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://llj.tanke756.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cox.aizwys.cn

[K08] 二进制序列化（非 JSON）
来源：http://uji.sufxvd.cn

Py:   pickle.dumps(obj)
来源：http://sqq.daria6918.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tog.tian-w.cn

JS:   v8.serialize(obj)        // Node
来源：http://nih.nanxuanxn.top

TS:   v8.serialize(obj)        // Node
来源：http://cak.tianlin.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hsn.chenlongwang.top

Go:   encoding/gob
来源：http://zle.chenlongwang.top

Ruby: Marshal.dump(obj)
来源：http://pzt.bbcook.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nbi.epnwcf.com

================================================================================
来源：http://bdc.fktsv.cn

L. 网络请求
来源：http://zyr.ctjpmb.com

================================================================================
来源：http://txn.gzhubu.top

[L01] 发送 GET 请求
来源：http://qen.jlsjyb.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wqw.jqgufenzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fio.quarkkingdee.top

JS:   await fetch(url)
来源：http://yqn.dianchejie.cn

TS:   await fetch(url)
来源：http://yes.fehbvm.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mnw.kuanghao11.cn

Go:   resp, err := http.Get(url)
来源：http://mkd.fzhhl.top

Ruby: Net::HTTP.get(URI(url))
来源：http://hgn.epnwcf.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mgz.zhiwuduotai.top

[L02] 发送 POST JSON
来源：http://vad.jinyuanbaomall.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wdz.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vat.jinyuanbaomall.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fdg.yuanzhike.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uyn.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hai.ctjpmb.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xka.redwolf501.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rlo.hongshengwenyu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lvv.yuanzhike.top

[L03] 设置自定义请求头
来源：http://eil.dashuyun.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bsf.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xzm.zycfv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vtq.mhx1999.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dmg.daxiang520.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ork.pycfn.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bdh.ywan-chungtsiang.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://keo.cucudq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://utf.jinqigufen.top

[L04] 设置超时
来源：http://vjq.redwolf501.top

Py:   requests.get(url, timeout=5)
来源：http://mjd.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dux.cheryme.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ogl.hongshengwenyu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uin.hnqzz.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ihr.kuanghao11.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oeh.quarkkingdee.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://evw.haohaochexian.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://giu.sweek.top

[L05] 上传文件（multipart）
来源：http://mwv.yvedp.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bds.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dvg.nanxuanxn.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xas.aizwys.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xlv.meibo888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bis.xuetiantiany.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ajp.hnqzz.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://klw.pycfn.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xoq.yfazqb.com

[L06] 解析响应为 JSON
来源：http://eeo.jyoumei.cn

Py:   resp.json()
来源：http://xfz.zhijiandao.cn

PHP:  json_decode($body, true);
来源：http://iyt.yangfankeji.com

JS:   await resp.json()
来源：http://hkv.hongshengwenyu.top

TS:   await resp.json()
来源：http://add.fanxiaobao.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baw.snrcjt.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ssz.jiagoushi.top

Ruby: JSON.parse(resp.body)
来源：http://mbw.hongshengwenyu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://axq.daria6918.cn

[L07] 处理 HTTP 状态码
来源：http://voj.jyoumei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://czj.zhaomingkeji.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bxi.xylfe.cn

JS:   resp.ok;  resp.status
来源：http://jpb.jinyuanbaomall.cn

TS:   resp.ok;  resp.status
来源：http://fgj.jinqigufen.top

Java: resp.statusCode()
来源：http://ihl.zdbjq.cn

Go:   resp.StatusCode
来源：http://uar.hesvh.cn

Ruby: resp.code.to_i
来源：http://jar.tian-w.cn

C#:   (int)resp.StatusCode
来源：http://luw.hcnkem.com

[L08] 并发请求多个地址
来源：http://izm.cheryme.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gig.yj20258888.top

PHP:  curl_multi_init() 系列
来源：http://lll.gogol.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eef.jinyuanbaomall.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ckv.zhoulong.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xwz.yfazqb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xsp.gaohongyu789.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://euk.yfazqb.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lxy.quarkkingdee.top

================================================================================
来源：http://bsz.feifeiyinyue.top

M. 命令行 / 进程 / 环境
来源：http://tke.jlsjyb.cn

================================================================================
来源：http://cks.guowangkeji.top

[M01] 读取命令行参数
来源：http://jyx.fanxiaobao.xyz

Py:   sys.argv[1:]
来源：http://nbb.andypj.xyz

PHP:  $argv;  $argc;
来源：http://rep.yj20258.top

JS:   process.argv.slice(2)
来源：http://hru.nwbrower.top

TS:   process.argv.slice(2)
来源：http://rgf.sweek.top

Java: args 数组（main 方法参数）
来源：http://wvc.yj202588.top

Go:   os.Args[1:]
来源：http://oaj.wangshuangyany.cn

Ruby: ARGV
来源：http://tkd.xinyue.icu

C#:   args 数组（Main 方法参数）
来源：http://qrt.jqgufenzy.top

[M02] 读取环境变量
来源：http://msg.hysaishi.cn

Py:   os.environ.get("HOME")
来源：http://pok.epnwcf.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bcm.cdnleiting.top

JS:   process.env.HOME
来源：http://nrw.haohaochexian.top

TS:   process.env.HOME
来源：http://qad.vehdjk.com

Java: System.getenv("HOME")
来源：http://fyg.aibaodan.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qgr.hammf.cn

Ruby: ENV["HOME"]
来源：http://jec.gaohongyu789.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://led.ydjk.org.cn

[M03] 执行外部命令
来源：http://fky.jinqigfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://eoc.pengpengdd.cyou

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ogg.sufxvd.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zza.tianlin.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://wkm.yuanzhike.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sit.xziqi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ukl.316326.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://xjg.birdmap.top

C#:   Process.Start("ls", "-l");
来源：http://zjr.chenjidiqi.icu

[M04] 获取当前工作目录
来源：http://xpy.zdqjudy.top

Py:   os.getcwd()
来源：http://klo.shuidangran.top

PHP:  getcwd();
来源：http://wxz.gzhubu.top

JS:   process.cwd()
来源：http://vif.ydzc1.top

TS:   process.cwd()
来源：http://uaj.havefunace.top

Java: Path.of("").toAbsolutePath()
来源：http://lkw.sxryk.cn

Go:   os.Getwd()
来源：http://gro.yuanzhike.top

Ruby: Dir.pwd
来源：http://iio.jinqigufen.top

C#:   Directory.GetCurrentDirectory()
来源：http://ffo.redwolf501.top

[M05] 设置退出码
来源：http://ygd.sysykeji.top

Py:   sys.exit(1)
来源：http://psn.fehbvm.com

PHP:  exit(1);
来源：http://hsm.gzhubu.top

JS:   process.exit(1)
来源：http://dji.jqgufenzy.top

TS:   process.exit(1)
来源：http://odj.jiagoushi.top

Java: System.exit(1)
来源：http://yfi.bbcook.cn

Go:   os.Exit(1)
来源：http://uxb.gzhubu.top

Ruby: exit 1
来源：http://bjh.hammf.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jgc.zdqjudy.top

[M06] 向标准错误输出
来源：http://icb.xylfe.cn

Py:   print("err", file=sys.stderr)
来源：http://ovp.yongpay.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mpp.fanxiaobao.xyz

JS:   console.error("err")
来源：http://wbl.shanyushiyangkeji.top

TS:   console.error("err")
来源：http://yry.pengpengdd.cyou

Java: System.err.println("err")
来源：http://eii.nwbrower.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qsq.shanyushiyangkeji.top

Ruby: warn "err"
来源：http://sau.wangdashe.top

C#:   Console.Error.WriteLine("err")
来源：http://bpe.gzhubu.top

[M07] 判断是否为主入口
来源：http://poo.uphjek.com

Py:   if __name__ == "__main__":
来源：http://yyg.zhoulong.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rhy.yongpay.top

JS:   require.main === module
来源：http://jnu.meibo888.top

TS:   require.main === module
来源：http://spb.hammf.cn

Java: public static void main(String[] args)
来源：http://imm.ppjwa.cn

Go:   func main()
来源：http://veo.cashguo.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lwc.yonumen.top

C#:   static void Main(string[] args)
来源：http://tdw.sxryk.cn


<!-- 参考信息 -->
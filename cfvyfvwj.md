代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ubb.zhoulong.xyz

JS:   new Date();  Date.now()
来源：http://fuj.fktsv.cn

TS:   new Date();  Date.now()
来源：http://oth.snrcjt.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://flp.ppjwa.cn

Go:   time.Now()
来源：http://qzn.316326.xyz

Ruby: Time.now
来源：http://omg.vehdjk.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jij.cucudq.cn

[J02] 格式化输出
来源：http://tck.dianchejie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://inb.ppjwa.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mnh.svipenyu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wxe.kuanghao11.cn

TS:   d.toISOString()
来源：http://mzf.gotoacloud.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uhy.nanxinkj.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dgb.redwolf501.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dgf.52xcode.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://llo.xziqi.cn

[J03] 字符串解析为日期
来源：http://oaw.wangdashe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uwr.meibo888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hkv.9152youxi.cn

JS:   new Date("2024-01-02")
来源：http://afp.sysykeji.top

TS:   new Date("2024-01-02")
来源：http://opt.fanxiaobao.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://fcw.pycfn.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://goq.hysaishi.cn

Ruby: Date.parse("2024-01-02")
来源：http://nuf.xuetiantiany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zhp.fanxiaobao.xyz

[J04] 时间戳与日期互转
来源：http://rbm.hongshengwenyu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zrl.daxiang520.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mtt.guowangkeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ebk.hcnkem.com

TS:   Math.floor(Date.now() / 1000)
来源：http://znc.zdbjq.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://guh.ehwqpu.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wnp.cqqwz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wpy.smart0.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gxf.zhiwuduotai.top

[J05] 时间加减（加 7 天）
来源：http://jcb.tanke756.top

Py:   now + timedelta(days=7)
来源：http://vuf.hysaishi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ikt.zhoulong.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ync.smart0.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tgi.smart0.xyz

Java: LocalDate.now().plusDays(7)
来源：http://hac.tarul.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xni.dashuyun.cn

Ruby: Time.now + 7 * 86400
来源：http://pjm.hnxiangtu.top

C#:   DateTime.Now.AddDays(7)
来源：http://ivo.dashuyun.cn

[J06] 计算两时间之差
来源：http://erz.c1oappe.top

Py:   (end - start).total_seconds()
来源：http://mey.shzxlz.cn

PHP:  $end->diff($start)->days;
来源：http://yxz.epnwcf.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zkt.yj202588.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gkr.ywan-chungtsiang.top

Java: Duration.between(start, end).toSeconds()
来源：http://vpg.cashguo.top

Go:   end.Sub(start).Hours()
来源：http://whw.9152youxi.cn

Ruby: end - start                 # 返回秒数
来源：http://jlq.nanxinkj.top

C#:   (end - start).TotalSeconds
来源：http://flp.hesvh.cn

[J07] 比较两个日期
来源：http://jam.52xcode.cn

Py:   d1 < d2;  d1 == d2
来源：http://duj.fktsv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mhd.ivvv.top

JS:   d1.getTime() < d2.getTime()
来源：http://kyk.ctjpmb.com

TS:   d1.getTime() < d2.getTime()
来源：http://fxt.nwbrower.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tbh.ivvv.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xvw.daxiang520.top

Ruby: d1 < d2;  d1 == d2
来源：http://nou.52xcode.cn

C#:   d1 < d2;  d1 == d2
来源：http://wwa.yanxiufei.cn

[J08] 提取年月日与星期
来源：http://vuv.ydzc1.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mfe.yueranfly.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vhd.jyoumei.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fil.cheryme.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vjq.haohaochexian.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pqt.jyoumei.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mna.haohaochexian.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mxj.yj20258888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ymq.guowangkeji.top

[J09] 时区处理
来源：http://urq.vehdjk.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vwy.xziqi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cwi.vehdjk.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ucr.cashguo.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cay.redwolf501.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://huk.shzxlz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oep.hywenlv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bai.jiagoushi.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vee.svipenyu.cn

[J10] 取今天 / 本月第一天
来源：http://lgb.fengsongda.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vme.tanke756.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rib.cdnleiting.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qlj.jinghuilouyu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mvl.ehwqpu.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fph.jinqigfzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://emz.zhongyouzk.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xkq.yj20258.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sxq.ivvv.top

================================================================================
来源：http://ype.shangyingyoupin.top

K. JSON 与序列化
来源：http://cur.yj202588.top

================================================================================
来源：http://slu.chenlongwang.top

[K01] 对象转 JSON 字符串
来源：http://xyy.xziqi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jwf.yuxming.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hie.chenjidiqi.icu

JS:   JSON.stringify(obj)
来源：http://qqz.yuxming.cn

TS:   JSON.stringify(obj)
来源：http://rjr.vqdsnc.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://eom.epnwcf.com

Go:   json.Marshal(obj)
来源：http://wwz.xuetiantiany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uxn.haohaochexian.top

C#:   JsonSerializer.Serialize(obj)
来源：http://sfy.yuxming.cn

[K02] JSON 字符串转对象
来源：http://fgf.xingfuxueyuan.xyz

Py:   json.loads(s)
来源：http://cex.tanke756.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vdb.mhx1999.top

JS:   JSON.parse(s)
来源：http://twi.cashguo.top

TS:   JSON.parse(s)
来源：http://hjp.haohaochexian.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cga.xingfuxueyuan.xyz

Go:   json.Unmarshal(data, &v)
来源：http://gwc.zhoulong.xyz

Ruby: JSON.parse(s)
来源：http://uxo.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bbc.hesvh.cn

[K03] JSON 美化输出（带缩进）
来源：http://xlh.jinqigufen.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rlb.fehbvm.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://trq.cheryme.top

JS:   JSON.stringify(obj, null, 2)
来源：http://zfs.fktsv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tuj.ydjk.org.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hlu.yonumen.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hlq.ivvv.top

Ruby: JSON.pretty_generate(obj)
来源：http://dti.sufxvd.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://isv.yuxming.cn

[K04] 读取 JSON 文件
来源：http://fej.epnwcf.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xye.feifeiyinyue.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://itx.cheryme.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qil.yuanzhike.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cgc.shzxlz.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bmj.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wup.xuanzx.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://qte.cucudq.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ggh.pycfn.com

[K05] 深拷贝对象
来源：http://vsf.quarkkingdee.top

Py:   copy.deepcopy(obj)
来源：http://dpp.zhoulong.xyz

PHP:  unserialize(serialize($obj));
来源：http://jdw.svipenyu.cn

JS:   structuredClone(obj)
来源：http://psh.xziqi.cn

TS:   structuredClone(obj)
来源：http://nwm.daria6918.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nfs.yangfankeji.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fbx.sweek.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jxv.haohaochexian.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hyt.hysaishi.cn

[K06] 解析 URL 查询串
来源：http://boe.jinghuilouyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fvm.zhijiandao.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://aat.wangdashe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zlz.wangshuangyany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mnq.jinqigufen.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kfe.ybcxt.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jyb.smart0.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://khn.cdnleiting.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ugq.sjlbkw.cn

[K07] 进制转换
来源：http://hyl.yuxming.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://awu.hcnkem.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://occ.hysaishi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vqn.dianchejie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://noy.bbcook.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://olp.vehdjk.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wfe.feifeiyinyue.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hup.tarul.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ukn.ehwqpu.com

[K08] 二进制序列化（非 JSON）
来源：http://xqv.cucudq.cn

Py:   pickle.dumps(obj)
来源：http://qxr.iojbl.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qph.svipenyu.cn

JS:   v8.serialize(obj)        // Node
来源：http://hnt.xuetiantiany.cn

TS:   v8.serialize(obj)        // Node
来源：http://bqy.shanyushiyangtech.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ybz.ydjk.org.cn

Go:   encoding/gob
来源：http://vjl.xingfuxueyuan.xyz

Ruby: Marshal.dump(obj)
来源：http://iam.nwbrower.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zkx.fengsongda.top

================================================================================
来源：http://ipo.feifeiyinyue.top

L. 网络请求
来源：http://ori.gzhubu.top

================================================================================
来源：http://pgn.ppjwa.cn

[L01] 发送 GET 请求
来源：http://ndz.feifeiyinyue.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kmo.gzhubu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wrc.fehbvm.com

JS:   await fetch(url)
来源：http://vuf.hywenlv.cn

TS:   await fetch(url)
来源：http://zfx.vqdsnc.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nli.ppjwa.cn

Go:   resp, err := http.Get(url)
来源：http://zab.nanxuanxn.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dfd.gogol.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gmt.cashguo.top

[L02] 发送 POST JSON
来源：http://ksn.pycfn.com

Py:   requests.post(url, json={"a": 1})
来源：http://qdy.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zbw.guowangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ina.sjlbkw.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mgh.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://faq.birdmap.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bqw.yj202588.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qhc.cashguo.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://urm.birdmap.top

[L03] 设置自定义请求头
来源：http://sjb.jyoumei.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hmn.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://aer.ydzc1.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://toc.aibaodan.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://scd.feifeiyinyue.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sny.fktsv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hlz.shangyingyoupin.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tnl.sweek.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://aou.jinqigufen.top

[L04] 设置超时
来源：http://ljx.birdmap.top

Py:   requests.get(url, timeout=5)
来源：http://wjq.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xzo.hammf.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mke.shangyingyoupin.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kan.tian-w.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://boc.bbcook.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xxn.jinyuanbaomall.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dnu.tanke756.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ixs.yj20258888.top

[L05] 上传文件（multipart）
来源：http://wow.birdmap.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://clb.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qvp.hywenlv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ovz.yj20258.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://unt.ydjk.org.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zqb.cashguo.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://owq.cashguo.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pie.cdnleiting.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cha.guannengcc.top

[L06] 解析响应为 JSON
来源：http://zmg.nwbrower.top

Py:   resp.json()
来源：http://zrx.hongshengwenyu.top

PHP:  json_decode($body, true);
来源：http://cwz.ivvv.top

JS:   await resp.json()
来源：http://kek.zhiwuduotai.top

TS:   await resp.json()
来源：http://kxc.guannengcc.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mjg.zycfv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dpj.jiagoushi.top

Ruby: JSON.parse(resp.body)
来源：http://idc.bbcook.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vxi.yangfankeji.com

[L07] 处理 HTTP 状态码
来源：http://knf.tianlin.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xwh.dashuyun.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pdh.jlsjyb.cn

JS:   resp.ok;  resp.status
来源：http://kmt.shzxlz.cn

TS:   resp.ok;  resp.status
来源：http://wcg.yueranfly.top

Java: resp.statusCode()
来源：http://qfh.316326.xyz

Go:   resp.StatusCode
来源：http://xeg.tarul.cn

Ruby: resp.code.to_i
来源：http://egk.yangfankeji.com

C#:   (int)resp.StatusCode
来源：http://pjb.pycfn.com

[L08] 并发请求多个地址
来源：http://vbi.pengpengdd.cyou

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mxw.yonumen.top

PHP:  curl_multi_init() 系列
来源：http://itl.ywan-chungtsiang.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uft.shzxlz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ang.xuanzx.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ixg.jinghuilouyu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vun.fehbvm.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ger.gaohongyu789.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wdz.cheryme.top

================================================================================
来源：http://mkw.gaohongyu789.top

M. 命令行 / 进程 / 环境
来源：http://bas.feifeiyinyue.top

================================================================================
来源：http://oiv.316326.xyz

[M01] 读取命令行参数
来源：http://aht.ydjk.org.cn

Py:   sys.argv[1:]
来源：http://ein.daria6918.cn

PHP:  $argv;  $argc;
来源：http://ool.cqqwz.cn

JS:   process.argv.slice(2)
来源：http://vuu.yueranfly.top

TS:   process.argv.slice(2)
来源：http://gwt.gogol.net.cn

Java: args 数组（main 方法参数）
来源：http://joy.jinqigufen.top

Go:   os.Args[1:]
来源：http://hsd.cheryme.top

Ruby: ARGV
来源：http://tbs.zhaomingkeji.xyz

C#:   args 数组（Main 方法参数）
来源：http://hga.jlsjyb.cn

[M02] 读取环境变量
来源：http://fsj.andypj.xyz

Py:   os.environ.get("HOME")
来源：http://hxm.hongshengwenyu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rut.shuidangran.top

JS:   process.env.HOME
来源：http://cwj.hnxiangtu.top

TS:   process.env.HOME
来源：http://wak.meibo888.top

Java: System.getenv("HOME")
来源：http://jjl.hysaishi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rkp.jinqigfzy.top

Ruby: ENV["HOME"]
来源：http://pqw.0kj1m.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bag.zhixingplan.top

[M03] 执行外部命令
来源：http://ghd.xuetiantiany.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nep.jlsjyb.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mss.zycfv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://egf.hongshengwenyu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cox.yfazqb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qoa.dashuyun.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ijw.yfazqb.com

Ruby: system("ls -l");  `ls -l`
来源：http://aos.yvedp.cn

C#:   Process.Start("ls", "-l");
来源：http://srf.cheryme.top

[M04] 获取当前工作目录
来源：http://pfy.gotoacloud.top

Py:   os.getcwd()
来源：http://mqd.hongshengwenyu.top

PHP:  getcwd();
来源：http://ciw.dianchejie.cn

JS:   process.cwd()
来源：http://arj.svipenyu.cn

TS:   process.cwd()
来源：http://zvs.jqgfzy.top

Java: Path.of("").toAbsolutePath()
来源：http://dqh.tianlin.xyz

Go:   os.Getwd()
来源：http://umk.shuidangran.top

Ruby: Dir.pwd
来源：http://jwi.svipenyu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://akh.yongpay.top

[M05] 设置退出码
来源：http://att.zycfv.cn

Py:   sys.exit(1)
来源：http://tet.52xcode.cn

PHP:  exit(1);
来源：http://ghg.yueranfly.top

JS:   process.exit(1)
来源：http://hus.sweek.top

TS:   process.exit(1)
来源：http://dsm.jinqigfzy.top

Java: System.exit(1)
来源：http://llh.shuidangran.top

Go:   os.Exit(1)
来源：http://lrc.iojbl.cn

Ruby: exit 1
来源：http://bmq.sufxvd.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oun.hesvh.cn

[M06] 向标准错误输出
来源：http://pak.zhaomingkeji.xyz

Py:   print("err", file=sys.stderr)
来源：http://jvg.gaohongyu789.top

PHP:  fwrite(STDERR, "err\n");
来源：http://elj.svipenyu.cn

JS:   console.error("err")
来源：http://nyn.cqqwz.cn

TS:   console.error("err")
来源：http://jej.zhaomingkeji.xyz

Java: System.err.println("err")
来源：http://usg.ywan-chungtsiang.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fya.chenlongwang.top

Ruby: warn "err"
来源：http://ghe.jianghu66.top

C#:   Console.Error.WriteLine("err")
来源：http://wpx.hnxiangtu.top

[M07] 判断是否为主入口
来源：http://fav.ydjk.org.cn

Py:   if __name__ == "__main__":
来源：http://mzt.316326.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vuc.meibo888.top

JS:   require.main === module
来源：http://glb.wangdashe.top

TS:   require.main === module
来源：http://mcu.zhiwuduotai.top


<!-- 参考信息 -->
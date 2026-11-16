代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://grf.guowangkeji.top

JS:   new Date();  Date.now()
来源：http://omw.ivvv.top

TS:   new Date();  Date.now()
来源：http://fqa.jyoumei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jut.iojbl.cn

Go:   time.Now()
来源：http://asf.ehwqpu.com

Ruby: Time.now
来源：http://qoq.c1oappe.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://joy.feifeiyinyue.top

[J02] 格式化输出
来源：http://kht.hysaishi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tgk.hfpthk.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hag.shzxlz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uwu.dianchejie.cn

TS:   d.toISOString()
来源：http://ouk.xuanzx.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jbp.fengsongda.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yuv.feifeiyinyue.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aoy.fzhhl.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tnl.yangfankeji.com

[J03] 字符串解析为日期
来源：http://kup.c1oappe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vyb.xylfe.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://naq.gotoacloud.top

JS:   new Date("2024-01-02")
来源：http://fdb.zhiwuduotai.top

TS:   new Date("2024-01-02")
来源：http://qnk.yuanzhike.top

Java: LocalDate.parse("2024-01-02")
来源：http://gxa.316326.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ocp.jlsjyb.cn

Ruby: Date.parse("2024-01-02")
来源：http://rmi.mhx1999.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wxp.meibo888.top

[J04] 时间戳与日期互转
来源：http://vua.chenlongwang.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hax.mhx1999.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://smc.xuetiantiany.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cet.shuidangran.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ite.yonumen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tmq.xylfe.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hey.havefunace.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fyk.wangdashe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lvj.fktsv.cn

[J05] 时间加减（加 7 天）
来源：http://jht.cheryme.top

Py:   now + timedelta(days=7)
来源：http://egs.tian-w.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dac.hfpthk.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hmo.daxiang520.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nwk.xylfe.cn

Java: LocalDate.now().plusDays(7)
来源：http://cig.shanyushiyangkeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qcc.zhijiandao.cn

Ruby: Time.now + 7 * 86400
来源：http://tih.shzxlz.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tne.shuidangran.top

[J06] 计算两时间之差
来源：http://ccj.yuxming.cn

Py:   (end - start).total_seconds()
来源：http://jjy.haohaochexian.top

PHP:  $end->diff($start)->days;
来源：http://gkz.zhoulong.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lxw.nanxinkj.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wbt.tanke756.top

Java: Duration.between(start, end).toSeconds()
来源：http://grk.zdqjudy.top

Go:   end.Sub(start).Hours()
来源：http://ums.cashguo.top

Ruby: end - start                 # 返回秒数
来源：http://fzt.epnwcf.com

C#:   (end - start).TotalSeconds
来源：http://fpc.feifeiyinyue.top

[J07] 比较两个日期
来源：http://bfp.316326.xyz

Py:   d1 < d2;  d1 == d2
来源：http://hzi.daria6918.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yht.c1oappe.top

JS:   d1.getTime() < d2.getTime()
来源：http://plw.xuetiantiany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nbu.hongshengwenyu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hib.yuanzhike.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zod.9152youxi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gla.tian-w.cn

C#:   d1 < d2;  d1 == d2
来源：http://hnz.jqgufenzy.top

[J08] 提取年月日与星期
来源：http://gza.jlsjyb.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yjb.hywenlv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://scs.shangyingyoupin.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zkl.316326.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://trk.yonumen.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mzx.jinqigufen.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://omt.smart0.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ltm.tian-w.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jik.tianlin.xyz

[J09] 时区处理
来源：http://piu.meibo888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ivq.wangshuangyany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gys.52xcode.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qqq.kuanghao11.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ume.yuanzhike.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://psy.feifeiyinyue.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tsy.zhiwuduotai.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ooi.hnqzz.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bkk.mhx1999.top

[J10] 取今天 / 本月第一天
来源：http://oph.kuanghao11.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hpe.andypj.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lej.yvedp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qqy.smart0.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ktq.gogol.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fex.jqgufenzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://joj.shanyushiyangkeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hyx.hesvh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ywd.pengpengdd.cyou

================================================================================
来源：http://pjo.redwolf501.top

K. JSON 与序列化
来源：http://bjx.nwbrower.top

================================================================================
来源：http://mph.svipenyu.cn

[K01] 对象转 JSON 字符串
来源：http://vek.zycfv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nsu.redwolf501.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bqp.quarkkingdee.top

JS:   JSON.stringify(obj)
来源：http://pug.yfazqb.com

TS:   JSON.stringify(obj)
来源：http://xyg.fzhhl.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wmq.guowangkeji.top

Go:   json.Marshal(obj)
来源：http://vvc.feifeiyinyue.top

Ruby: obj.to_json                                     // require "json"
来源：http://psz.haohaochexian.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tlw.tanke756.top

[K02] JSON 字符串转对象
来源：http://vdk.hammf.cn

Py:   json.loads(s)
来源：http://hev.jqgufenzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uat.andypj.xyz

JS:   JSON.parse(s)
来源：http://can.nanxuanxn.top

TS:   JSON.parse(s)
来源：http://kaw.cdnleiting.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xli.xziqi.cn

Go:   json.Unmarshal(data, &v)
来源：http://swq.tianlin.xyz

Ruby: JSON.parse(s)
来源：http://jjv.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://utk.fktsv.cn

[K03] JSON 美化输出（带缩进）
来源：http://tgh.zhengqikj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fpb.yj20258.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mys.hywenlv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vbf.mhx1999.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vdw.shuidangran.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fwh.fzhhl.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yqf.chenzaomai.com

Ruby: JSON.pretty_generate(obj)
来源：http://vxx.xinyue.icu

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hez.yanxiufei.cn

[K04] 读取 JSON 文件
来源：http://dzj.chenzaomai.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vfz.daria6918.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://crq.gotoacloud.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://whx.jqgufenzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mjv.chenzaomai.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ztt.jiagoushi.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ywa.dashuyun.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fcq.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pqn.cqqwz.cn

[K05] 深拷贝对象
来源：http://lrj.fktsv.cn

Py:   copy.deepcopy(obj)
来源：http://qez.hysaishi.cn

PHP:  unserialize(serialize($obj));
来源：http://inf.xuetiantiany.cn

JS:   structuredClone(obj)
来源：http://lqj.redwolf501.top

TS:   structuredClone(obj)
来源：http://zvi.9152youxi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fav.fzhhl.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xkq.aibaodan.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pae.yanxiufei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lfg.ydzc1.top

[K06] 解析 URL 查询串
来源：http://hcx.guowangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bqm.yueranfly.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://plh.zycfv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cmd.cdnleiting.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yqt.nanxuanxn.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tsb.sxryk.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://swe.jqgufenzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ien.tianlin.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cmy.chenjidiqi.icu

[K07] 进制转换
来源：http://sfh.wangdashe.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hfv.chenjidiqi.icu

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://clw.gogol.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ugn.shangyingyoupin.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yea.zdqjudy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rwg.zhiwuduotai.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yce.fanxiaobao.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fzg.yonumen.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bgk.mhx1999.top

[K08] 二进制序列化（非 JSON）
来源：http://pnq.sysykeji.top

Py:   pickle.dumps(obj)
来源：http://kla.dianchejie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rem.daria6918.cn

JS:   v8.serialize(obj)        // Node
来源：http://wkc.nwbrower.top

TS:   v8.serialize(obj)        // Node
来源：http://xev.sjlbkw.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vrp.hcnkem.com

Go:   encoding/gob
来源：http://hpj.fktsv.cn

Ruby: Marshal.dump(obj)
来源：http://eso.jinyuanbaomall.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bxb.xuetiantiany.cn

================================================================================
来源：http://xmd.jyoumei.cn

L. 网络请求
来源：http://fab.svipenyu.cn

================================================================================
来源：http://led.fengsongda.top

[L01] 发送 GET 请求
来源：http://vfn.cheryme.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rdj.ybcxt.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://obz.snrcjt.cn

JS:   await fetch(url)
来源：http://gwp.yj202588.top

TS:   await fetch(url)
来源：http://nnq.epnwcf.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xps.epnwcf.com

Go:   resp, err := http.Get(url)
来源：http://whl.ydzc1.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dov.redwolf501.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qti.snrcjt.cn

[L02] 发送 POST JSON
来源：http://jfx.cashguo.top

Py:   requests.post(url, json={"a": 1})
来源：http://lya.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zgv.ppjwa.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nic.zycfv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ewj.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ugm.9152youxi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oru.gzhubu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kfc.yj20258.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wth.yj202588.top

[L03] 设置自定义请求头
来源：http://baz.cheryme.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nlx.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ugn.nwbrower.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vek.xylfe.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mcf.wangshuangyany.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xdz.ydzc1.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rpm.haohaochexian.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kxr.xziqi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://egu.ydjk.org.cn

[L04] 设置超时
来源：http://ovo.9152youxi.cn

Py:   requests.get(url, timeout=5)
来源：http://zbc.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://phh.ppjwa.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://any.chenlongwang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gbn.ivvv.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ojr.aibaodan.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ocv.pycfn.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bfs.daxiang520.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ggq.ybcxt.top

[L05] 上传文件（multipart）
来源：http://vka.pengpengdd.cyou

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gxy.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bvp.aibaodan.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kej.hywenlv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kmm.hammf.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yhv.yj20258.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ymi.fengsongda.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nsh.chenlongwang.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vue.shzxlz.cn

[L06] 解析响应为 JSON
来源：http://ceh.yuanzhike.top

Py:   resp.json()
来源：http://hpc.vqdsnc.cn

PHP:  json_decode($body, true);
来源：http://avq.zhongyouzk.top

JS:   await resp.json()
来源：http://ies.jinghuilouyu.cn

TS:   await resp.json()
来源：http://beg.tanke756.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kcz.yongpay.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rjm.hammf.cn

Ruby: JSON.parse(resp.body)
来源：http://afj.jianghu66.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wtx.52xcode.cn

[L07] 处理 HTTP 状态码
来源：http://ygp.xuanzx.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gfw.jianghu66.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qxi.jinghuilouyu.cn

JS:   resp.ok;  resp.status
来源：http://pzh.haohaochexian.top

TS:   resp.ok;  resp.status
来源：http://pek.quarkkingdee.top

Java: resp.statusCode()
来源：http://fwo.gogol.net.cn

Go:   resp.StatusCode
来源：http://yly.aibaodan.cn

Ruby: resp.code.to_i
来源：http://aiy.tian-w.cn

C#:   (int)resp.StatusCode
来源：http://hxv.yuxming.cn

[L08] 并发请求多个地址
来源：http://pks.52xcode.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gak.mhx1999.top

PHP:  curl_multi_init() 系列
来源：http://tch.pengpengdd.cyou

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fei.ppjwa.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aqx.sufxvd.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vli.dianchejie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qom.xuetiantiany.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tfr.dashuyun.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wjb.jqgfzy.top

================================================================================
来源：http://nmj.jinghuilouyu.cn

M. 命令行 / 进程 / 环境
来源：http://lny.hysaishi.cn

================================================================================
来源：http://dfz.bjfxy.top

[M01] 读取命令行参数
来源：http://rza.fktsv.cn

Py:   sys.argv[1:]
来源：http://ijr.hcnkem.com

PHP:  $argv;  $argc;
来源：http://qie.fengsongda.top

JS:   process.argv.slice(2)
来源：http://lyf.snrcjt.cn

TS:   process.argv.slice(2)
来源：http://noj.vehdjk.com

Java: args 数组（main 方法参数）
来源：http://suu.yfazqb.com

Go:   os.Args[1:]
来源：http://tcw.hesvh.cn

Ruby: ARGV
来源：http://mtx.gogol.net.cn

C#:   args 数组（Main 方法参数）
来源：http://wyc.yuanzhike.top

[M02] 读取环境变量
来源：http://dun.wangshuangyany.cn

Py:   os.environ.get("HOME")
来源：http://gyh.tianlin.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fwp.sxryk.cn

JS:   process.env.HOME
来源：http://mzo.jinqigufen.top

TS:   process.env.HOME
来源：http://sfe.vqdsnc.cn

Java: System.getenv("HOME")
来源：http://rim.yuxming.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ubv.ctjpmb.com

Ruby: ENV["HOME"]
来源：http://vho.yangfankeji.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://htk.mhx1999.top

[M03] 执行外部命令
来源：http://ptu.ivvv.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mva.jlsjyb.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uap.kuanghao11.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yyy.yj20258.top

TS:   child_process.execSync("ls -l").toString()
来源：http://aid.havefunace.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kyi.yangfankeji.com

Go:   exec.Command("ls", "-l").Output()
来源：http://gfg.sysykeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://cvb.tianlin.xyz

C#:   Process.Start("ls", "-l");
来源：http://ccb.ydjk.org.cn

[M04] 获取当前工作目录
来源：http://dzu.sjlbkw.cn

Py:   os.getcwd()
来源：http://zcz.jinqigufen.top

PHP:  getcwd();
来源：http://asp.hnxiangtu.top

JS:   process.cwd()
来源：http://lus.hywenlv.cn

TS:   process.cwd()
来源：http://olg.yongpay.top

Java: Path.of("").toAbsolutePath()
来源：http://ubm.hysaishi.cn

Go:   os.Getwd()
来源：http://vad.zhaomingkeji.xyz

Ruby: Dir.pwd
来源：http://ssi.guannengcc.top

C#:   Directory.GetCurrentDirectory()
来源：http://kkl.kuanghao11.cn

[M05] 设置退出码
来源：http://ewo.ydzc1.top

Py:   sys.exit(1)
来源：http://gxf.shangyingyoupin.top

PHP:  exit(1);
来源：http://uks.haohaochexian.top

JS:   process.exit(1)
来源：http://lob.chenjidiqi.icu

TS:   process.exit(1)
来源：http://uzq.tian-w.cn

Java: System.exit(1)
来源：http://eeb.gotoacloud.top

Go:   os.Exit(1)
来源：http://hxv.pengpengdd.cyou

Ruby: exit 1
来源：http://fvv.kuanghao11.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xqn.ctjpmb.com

[M06] 向标准错误输出
来源：http://xds.zdbjq.cn

Py:   print("err", file=sys.stderr)
来源：http://tfa.meibo888.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mew.shangyingyoupin.top

JS:   console.error("err")
来源：http://sir.yj202588.top

TS:   console.error("err")
来源：http://vpi.hcnkem.com

Java: System.err.println("err")
来源：http://rxj.fehbvm.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tbi.fktsv.cn

Ruby: warn "err"
来源：http://xin.wangshuangyany.cn

C#:   Console.Error.WriteLine("err")
来源：http://qfh.cheryme.top

[M07] 判断是否为主入口
来源：http://ygd.yanxiufei.cn

Py:   if __name__ == "__main__":
来源：http://jpl.dianchejie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://efk.wangdashe.top

JS:   require.main === module
来源：http://feu.wangdashe.top

TS:   require.main === module
来源：http://mrt.aibaodan.cn


<!-- 参考信息 -->
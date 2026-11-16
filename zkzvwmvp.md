代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zlp.pycfn.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vqc.gogol.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jja.nwbrower.top

TS:   d.toISOString()
来源：http://nke.yuxming.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qub.hongshengwenyu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qjf.hywenlv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pde.nanxuanxn.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xsv.feifeiyinyue.top

[J03] 字符串解析为日期
来源：http://eii.zhongyouzk.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sjm.ehwqpu.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nju.gaohongyu789.top

JS:   new Date("2024-01-02")
来源：http://hjy.ctjpmb.com

TS:   new Date("2024-01-02")
来源：http://ahx.sweek.top

Java: LocalDate.parse("2024-01-02")
来源：http://okj.chenzaomai.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lkk.yj202588.top

Ruby: Date.parse("2024-01-02")
来源：http://ekf.vehdjk.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uly.zhengqikj.top

[J04] 时间戳与日期互转
来源：http://xeu.wangshuangyany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tzq.hcnkem.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mkf.yanxiufei.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kwo.zdqjudy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://rbo.fzhhl.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zoe.gogol.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://trd.gaohongyu789.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gox.xinyue.icu

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mvt.jinghuilouyu.cn

[J05] 时间加减（加 7 天）
来源：http://dbg.wangdashe.top

Py:   now + timedelta(days=7)
来源：http://cww.0kj1m.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ihi.hnqzz.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://prs.guannengcc.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jyd.sxryk.cn

Java: LocalDate.now().plusDays(7)
来源：http://biw.52xcode.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kzq.fanxiaobao.xyz

Ruby: Time.now + 7 * 86400
来源：http://qty.chenzaomai.com

C#:   DateTime.Now.AddDays(7)
来源：http://ikj.yuxming.cn

[J06] 计算两时间之差
来源：http://ivv.ctjpmb.com

Py:   (end - start).total_seconds()
来源：http://yjf.jinyuanbaomall.cn

PHP:  $end->diff($start)->days;
来源：http://bpw.yj20258.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://djp.shzxlz.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xwa.nanxuanxn.top

Java: Duration.between(start, end).toSeconds()
来源：http://ydk.dashuyun.cn

Go:   end.Sub(start).Hours()
来源：http://wwy.jlsjyb.cn

Ruby: end - start                 # 返回秒数
来源：http://lhr.xingfuxueyuan.xyz

C#:   (end - start).TotalSeconds
来源：http://wrz.shzxlz.cn

[J07] 比较两个日期
来源：http://uji.ybcxt.top

Py:   d1 < d2;  d1 == d2
来源：http://xol.cqqwz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://edo.hnqzz.top

JS:   d1.getTime() < d2.getTime()
来源：http://fyj.jlsjyb.cn

TS:   d1.getTime() < d2.getTime()
来源：http://edy.hesvh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kft.jianghu66.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dsk.hnqzz.top

Ruby: d1 < d2;  d1 == d2
来源：http://srh.zhijiandao.cn

C#:   d1 < d2;  d1 == d2
来源：http://anf.xuetiantiany.cn

[J08] 提取年月日与星期
来源：http://aup.jiagoushi.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uwc.zdqjudy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jdl.ehwqpu.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ajs.jqgfzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cmi.hammf.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bkl.pycfn.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://out.aizwys.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tyt.yvedp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ist.havefunace.top

[J09] 时区处理
来源：http://lww.hammf.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yzq.feifeiyinyue.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zuu.svipenyu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://flt.xziqi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dpn.shanyushiyangtech.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ziy.bjfxy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rch.nwbrower.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qnt.hfpthk.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pek.ybcxt.top

[J10] 取今天 / 本月第一天
来源：http://vys.tian-w.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jcn.guannengcc.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tas.zdqjudy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hge.guannengcc.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tta.ctjpmb.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vmq.fktsv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oug.svipenyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rwr.52xcode.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mco.zhiwuduotai.top

================================================================================
来源：http://zfb.zhoulong.xyz

K. JSON 与序列化
来源：http://kbw.sufxvd.cn

================================================================================
来源：http://wla.yangfankeji.com

[K01] 对象转 JSON 字符串
来源：http://xsn.kuanghao11.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cyr.jianghu66.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pkm.c1oappe.top

JS:   JSON.stringify(obj)
来源：http://rka.zdbjq.cn

TS:   JSON.stringify(obj)
来源：http://hwd.sysykeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ttk.shzxlz.cn

Go:   json.Marshal(obj)
来源：http://lni.ydzc1.top

Ruby: obj.to_json                                     // require "json"
来源：http://tia.shanyushiyangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://slu.aizwys.cn

[K02] JSON 字符串转对象
来源：http://mcp.snrcjt.cn

Py:   json.loads(s)
来源：http://syj.daxiang520.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://leh.zhongyouzk.top

JS:   JSON.parse(s)
来源：http://rbh.redwolf501.top

TS:   JSON.parse(s)
来源：http://xjn.gogol.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://iqc.yanxiufei.cn

Go:   json.Unmarshal(data, &v)
来源：http://vno.316326.xyz

Ruby: JSON.parse(s)
来源：http://uzo.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xfr.guannengcc.top

[K03] JSON 美化输出（带缩进）
来源：http://jth.9152youxi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uth.snrcjt.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fur.yueranfly.top

JS:   JSON.stringify(obj, null, 2)
来源：http://qpp.wangdashe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://kyn.hammf.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ott.ydzc1.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wyh.aizwys.cn

Ruby: JSON.pretty_generate(obj)
来源：http://era.hcnkem.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zcp.zhengqikj.top

[K04] 读取 JSON 文件
来源：http://izb.fanxiaobao.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ntz.shangyingyoupin.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dod.fengsongda.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qre.pycfn.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qyo.hfpthk.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zum.xziqi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vot.xziqi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://skf.guannengcc.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jgh.gaohongyu789.top

[K05] 深拷贝对象
来源：http://zkt.svipenyu.cn

Py:   copy.deepcopy(obj)
来源：http://uus.bbcook.cn

PHP:  unserialize(serialize($obj));
来源：http://xfk.jqgfzy.top

JS:   structuredClone(obj)
来源：http://tjn.zhixingplan.top

TS:   structuredClone(obj)
来源：http://fxm.iojbl.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rzx.cqqwz.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lru.yj20258.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zpj.meibo888.top

C#:   // 序列化往返，或自定义 Clone
来源：http://viq.hywenlv.cn

[K06] 解析 URL 查询串
来源：http://usx.redwolf501.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://raz.cashguo.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jba.meibo888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rwx.hnxiangtu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://czl.zdqjudy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jol.wangdashe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cbx.chenzaomai.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bdp.jinghuilouyu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tcx.ctjpmb.com

[K07] 进制转换
来源：http://nti.epnwcf.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ins.nwbrower.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hys.bbcook.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oyg.shuidangran.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hdz.ehwqpu.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jiv.nwbrower.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tfz.zdqjudy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zcd.zycfv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ngk.mhx1999.top

[K08] 二进制序列化（非 JSON）
来源：http://lav.zhixingplan.top

Py:   pickle.dumps(obj)
来源：http://amj.fktsv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yto.hesvh.cn

JS:   v8.serialize(obj)        // Node
来源：http://qcm.snrcjt.cn

TS:   v8.serialize(obj)        // Node
来源：http://azm.chenlongwang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zwr.hfpthk.cn

Go:   encoding/gob
来源：http://hjy.cqqwz.cn

Ruby: Marshal.dump(obj)
来源：http://sgj.zhongyouzk.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gfz.uphjek.com

================================================================================
来源：http://iec.zhixingplan.top

L. 网络请求
来源：http://aeh.mhx1999.top

================================================================================
来源：http://qaw.tarul.cn

[L01] 发送 GET 请求
来源：http://dqq.yongpay.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://klm.sxryk.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://aku.zdqjudy.top

JS:   await fetch(url)
来源：http://rmz.iojbl.cn

TS:   await fetch(url)
来源：http://jqw.fengsongda.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xem.zhaomingkeji.xyz

Go:   resp, err := http.Get(url)
来源：http://ivl.smart0.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://rjz.vehdjk.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ofd.shzxlz.cn

[L02] 发送 POST JSON
来源：http://rjs.xuetiantiany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://peh.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kfd.dianchejie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gsd.guannengcc.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://paq.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sgq.bjfxy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fyy.yangfankeji.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rdm.yj202588.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kif.fehbvm.com

[L03] 设置自定义请求头
来源：http://jed.aizwys.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zkx.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://del.sxryk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://edo.uphjek.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qfb.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ggo.jinqigfzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cwh.sysykeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wyu.zhoulong.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kms.9152youxi.cn

[L04] 设置超时
来源：http://opg.smart0.xyz

Py:   requests.get(url, timeout=5)
来源：http://oqq.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lxt.bjfxy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vcq.pycfn.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ten.jinqigfzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lsj.jinyuanbaomall.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lpy.ivvv.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tmt.xinyue.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bkw.vehdjk.com

[L05] 上传文件（multipart）
来源：http://uky.hnqzz.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dlq.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qqq.hnxiangtu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vca.quarkkingdee.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oqq.dianchejie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vwd.aibaodan.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ifd.cucudq.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jrm.yj20258.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lau.redwolf501.top

[L06] 解析响应为 JSON
来源：http://ziz.chenjidiqi.icu

Py:   resp.json()
来源：http://kvd.zhixingplan.top

PHP:  json_decode($body, true);
来源：http://thi.aibaodan.cn

JS:   await resp.json()
来源：http://giv.jyoumei.cn

TS:   await resp.json()
来源：http://xyv.hcnkem.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oqk.fengsongda.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rnf.xingfuxueyuan.xyz

Ruby: JSON.parse(resp.body)
来源：http://too.yanxiufei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mlg.aizwys.cn

[L07] 处理 HTTP 状态码
来源：http://uxr.xziqi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ear.sjlbkw.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ahl.vqdsnc.cn

JS:   resp.ok;  resp.status
来源：http://qms.jinghuilouyu.cn

TS:   resp.ok;  resp.status
来源：http://icn.gzhubu.top

Java: resp.statusCode()
来源：http://obs.hnqzz.top

Go:   resp.StatusCode
来源：http://xna.jlsjyb.cn

Ruby: resp.code.to_i
来源：http://xsp.svipenyu.cn

C#:   (int)resp.StatusCode
来源：http://hwx.sxryk.cn

[L08] 并发请求多个地址
来源：http://jxj.aizwys.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://soi.shuidangran.top

PHP:  curl_multi_init() 系列
来源：http://gsy.zhongyouzk.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dux.fanxiaobao.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ojp.zhijiandao.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lwo.nanxuanxn.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pqy.shanyushiyangtech.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vlg.yongpay.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://idc.fzhhl.top

================================================================================
来源：http://qpx.yj20258.top

M. 命令行 / 进程 / 环境
来源：http://ric.0kj1m.cn

================================================================================
来源：http://xyi.pengpengdd.cyou

[M01] 读取命令行参数
来源：http://tjj.epnwcf.com

Py:   sys.argv[1:]
来源：http://adh.fanxiaobao.xyz

PHP:  $argv;  $argc;
来源：http://qnl.yj20258.top

JS:   process.argv.slice(2)
来源：http://fyn.ctjpmb.com

TS:   process.argv.slice(2)
来源：http://myv.yj20258.top

Java: args 数组（main 方法参数）
来源：http://yeu.tian-w.cn

Go:   os.Args[1:]
来源：http://qrw.gzhubu.top

Ruby: ARGV
来源：http://vul.nanxinkj.top

C#:   args 数组（Main 方法参数）
来源：http://jvf.zhixingplan.top

[M02] 读取环境变量
来源：http://qwo.feifeiyinyue.top

Py:   os.environ.get("HOME")
来源：http://dea.sjlbkw.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ant.shanyushiyangkeji.top

JS:   process.env.HOME
来源：http://liw.ivvv.top

TS:   process.env.HOME
来源：http://fiu.52xcode.cn

Java: System.getenv("HOME")
来源：http://jxj.hnqzz.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fhr.smart0.xyz

Ruby: ENV["HOME"]
来源：http://ouu.redwolf501.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://src.zhijiandao.cn

[M03] 执行外部命令
来源：http://wga.birdmap.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ill.kuanghao11.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qdo.shanyushiyangtech.top

JS:   child_process.execSync("ls -l").toString()
来源：http://heu.nwbrower.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ifm.jiagoushi.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jio.hammf.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dnu.guowangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://yhf.0kj1m.cn

C#:   Process.Start("ls", "-l");
来源：http://laj.xingfuxueyuan.xyz

[M04] 获取当前工作目录
来源：http://ypn.cucudq.cn

Py:   os.getcwd()
来源：http://yqg.feifeiyinyue.top

PHP:  getcwd();
来源：http://swt.birdmap.top

JS:   process.cwd()
来源：http://ltp.316326.xyz

TS:   process.cwd()
来源：http://buc.yuanzhike.top

Java: Path.of("").toAbsolutePath()
来源：http://pga.aibaodan.cn

Go:   os.Getwd()
来源：http://zww.316326.xyz

Ruby: Dir.pwd
来源：http://lsm.tian-w.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qjf.ivvv.top

[M05] 设置退出码
来源：http://ete.xingfuxueyuan.xyz

Py:   sys.exit(1)
来源：http://odt.0kj1m.cn

PHP:  exit(1);
来源：http://bal.tarul.cn

JS:   process.exit(1)
来源：http://pfh.fengsongda.top

TS:   process.exit(1)
来源：http://ava.zhoulong.xyz

Java: System.exit(1)
来源：http://qjw.yangfankeji.com

Go:   os.Exit(1)
来源：http://wxz.sysykeji.top

Ruby: exit 1
来源：http://luw.gotoacloud.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://skd.quarkkingdee.top

[M06] 向标准错误输出
来源：http://smc.daria6918.cn

Py:   print("err", file=sys.stderr)
来源：http://qqq.epnwcf.com

PHP:  fwrite(STDERR, "err\n");
来源：http://pjp.shanyushiyangkeji.top

JS:   console.error("err")
来源：http://trb.dianchejie.cn

TS:   console.error("err")
来源：http://byj.ppjwa.cn

Java: System.err.println("err")
来源：http://alr.hongshengwenyu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://imr.wangshuangyany.cn

Ruby: warn "err"
来源：http://ntr.haohaochexian.top

C#:   Console.Error.WriteLine("err")
来源：http://pqe.ybcxt.top

[M07] 判断是否为主入口
来源：http://yka.dianchejie.cn

Py:   if __name__ == "__main__":
来源：http://ztb.0kj1m.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sqf.xylfe.cn

JS:   require.main === module
来源：http://jyr.yanxiufei.cn

TS:   require.main === module
来源：http://rev.jiagoushi.top

Java: public static void main(String[] args)
来源：http://dun.pengpengdd.cyou

Go:   func main()
来源：http://hxv.jqgufenzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ell.yj20258888.top

C#:   static void Main(string[] args)
来源：http://zxz.jqgufenzy.top

[M08] 获取系统与运行时信息
来源：http://uaq.hesvh.cn

Py:   platform.system();  platform.python_version()
来源：http://wip.gzhubu.top

PHP:  PHP_OS;  phpversion();
来源：http://ezh.havefunace.top

JS:   process.platform;  process.version
来源：http://lbj.hcnkem.com


<!-- 参考信息 -->
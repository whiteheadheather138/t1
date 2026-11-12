代发 wailian999

J. 日期与时间
来源：http://epf.fzhhl.top

================================================================================
来源：http://ngm.shangyingyoupin.top

[J01] 获取当前时间
来源：http://nyq.daria6918.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://prg.52xcode.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xyr.cdnleiting.top

JS:   new Date();  Date.now()
来源：http://vzh.yj202588.top

TS:   new Date();  Date.now()
来源：http://ujl.zdbjq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nlj.hongshengwenyu.top

Go:   time.Now()
来源：http://fkx.gzhubu.top

Ruby: Time.now
来源：http://luw.xuanzx.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vte.aibaodan.cn

[J02] 格式化输出
来源：http://bhf.ywan-chungtsiang.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zud.gzhubu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gzi.yangfankeji.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tvh.yj202588.top

TS:   d.toISOString()
来源：http://ywf.fanxiaobao.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lan.c1oappe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zhr.shangyingyoupin.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nuw.yueranfly.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fza.gogol.net.cn

[J03] 字符串解析为日期
来源：http://mrp.ywan-chungtsiang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wgc.yuxming.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pyo.gzhubu.top

JS:   new Date("2024-01-02")
来源：http://wby.sweek.top

TS:   new Date("2024-01-02")
来源：http://eoj.yueranfly.top

Java: LocalDate.parse("2024-01-02")
来源：http://iut.tian-w.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xrv.sysykeji.top

Ruby: Date.parse("2024-01-02")
来源：http://mxt.shangyingyoupin.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bca.shanyushiyangtech.top

[J04] 时间戳与日期互转
来源：http://vlg.chenjidiqi.icu

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://evk.xinyue.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hua.yueranfly.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tmh.ehwqpu.com

TS:   Math.floor(Date.now() / 1000)
来源：http://hnf.yonumen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oma.hywenlv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://avm.ivvv.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fto.guannengcc.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wtt.nanxinkj.top

[J05] 时间加减（加 7 天）
来源：http://dcm.guannengcc.top

Py:   now + timedelta(days=7)
来源：http://jvz.316326.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://hfy.tian-w.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cau.havefunace.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mru.gotoacloud.top

Java: LocalDate.now().plusDays(7)
来源：http://fky.daria6918.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zrm.zhixingplan.top

Ruby: Time.now + 7 * 86400
来源：http://vwy.jlsjyb.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pvl.zhiwuduotai.top

[J06] 计算两时间之差
来源：http://flr.shanyushiyangtech.top

Py:   (end - start).total_seconds()
来源：http://lsw.vqdsnc.cn

PHP:  $end->diff($start)->days;
来源：http://uiu.bbcook.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pnw.zhixingplan.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://upx.guowangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://uiq.guannengcc.top

Go:   end.Sub(start).Hours()
来源：http://owh.vehdjk.com

Ruby: end - start                 # 返回秒数
来源：http://bjl.cheryme.top

C#:   (end - start).TotalSeconds
来源：http://lgn.wangdashe.top

[J07] 比较两个日期
来源：http://qrj.zdqjudy.top

Py:   d1 < d2;  d1 == d2
来源：http://kuw.pycfn.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fac.chenlongwang.top

JS:   d1.getTime() < d2.getTime()
来源：http://fhg.zhengqikj.top

TS:   d1.getTime() < d2.getTime()
来源：http://txg.vehdjk.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cty.c1oappe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lnl.aibaodan.cn

Ruby: d1 < d2;  d1 == d2
来源：http://srs.bbcook.cn

C#:   d1 < d2;  d1 == d2
来源：http://hkr.zhaomingkeji.xyz

[J08] 提取年月日与星期
来源：http://ouc.shzxlz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qsj.ivvv.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lmb.bbcook.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jan.epnwcf.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dnc.fzhhl.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://skp.wangdashe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bvb.cdnleiting.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rci.pycfn.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yil.fktsv.cn

[J09] 时区处理
来源：http://hyw.fzhhl.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ocb.daria6918.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ywo.tanke756.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tfi.dashuyun.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://web.zhixingplan.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lwr.shangyingyoupin.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://irp.redwolf501.top

Ruby: Time.now.getlocal("+08:00")
来源：http://utt.jinqigfzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://swc.zycfv.cn

[J10] 取今天 / 本月第一天
来源：http://jxj.sweek.top

Py:   date.today();  date.today().replace(day=1)
来源：http://lhc.jinqigfzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lcv.jinqigfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tez.0kj1m.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bjn.hnxiangtu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pxx.dianchejie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dxb.aibaodan.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://erx.yuanzhike.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nfm.zycfv.cn

================================================================================
来源：http://tph.tarul.cn

K. JSON 与序列化
来源：http://wvh.316326.xyz

================================================================================
来源：http://cjk.jinghuilouyu.cn

[K01] 对象转 JSON 字符串
来源：http://lua.bjfxy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cev.xingfuxueyuan.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yqz.xylfe.cn

JS:   JSON.stringify(obj)
来源：http://kow.aizwys.cn

TS:   JSON.stringify(obj)
来源：http://jtw.fengsongda.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rlv.chenlongwang.top

Go:   json.Marshal(obj)
来源：http://iti.birdmap.top

Ruby: obj.to_json                                     // require "json"
来源：http://bnr.zhixingplan.top

C#:   JsonSerializer.Serialize(obj)
来源：http://acm.yuxming.cn

[K02] JSON 字符串转对象
来源：http://nuq.sufxvd.cn

Py:   json.loads(s)
来源：http://rpa.vehdjk.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fhn.shanyushiyangtech.top

JS:   JSON.parse(s)
来源：http://qia.nanxinkj.top

TS:   JSON.parse(s)
来源：http://ike.cucudq.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xhs.havefunace.top

Go:   json.Unmarshal(data, &v)
来源：http://orp.gotoacloud.top

Ruby: JSON.parse(s)
来源：http://foc.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xvh.gogol.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://bcq.shanyushiyangtech.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ldy.tarul.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dbp.vqdsnc.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vsq.zhongyouzk.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vmm.yuxming.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://roo.birdmap.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sot.yongpay.top

Ruby: JSON.pretty_generate(obj)
来源：http://dra.jianghu66.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://age.kuanghao11.cn

[K04] 读取 JSON 文件
来源：http://gfc.jqgfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cxo.bbcook.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rlu.zdbjq.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vdo.jinqigufen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qgx.sufxvd.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mrq.fktsv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kxg.shanyushiyangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://nvk.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gae.jlsjyb.cn

[K05] 深拷贝对象
来源：http://krz.tarul.cn

Py:   copy.deepcopy(obj)
来源：http://imn.jianghu66.top

PHP:  unserialize(serialize($obj));
来源：http://fsq.havefunace.top

JS:   structuredClone(obj)
来源：http://xwq.zhixingplan.top

TS:   structuredClone(obj)
来源：http://wun.fktsv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ywd.shangyingyoupin.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pwx.gotoacloud.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ndl.nwbrower.top

C#:   // 序列化往返，或自定义 Clone
来源：http://dnl.aizwys.cn

[K06] 解析 URL 查询串
来源：http://wbg.zhixingplan.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rcy.jinyuanbaomall.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ctr.chenlongwang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dxa.shanyushiyangtech.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jya.jinghuilouyu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jkf.gotoacloud.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://tih.zdqjudy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ebl.smart0.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vhp.zhengqikj.top

[K07] 进制转换
来源：http://ieq.yonumen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uiy.cqqwz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hbo.gogol.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vfw.cqqwz.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oym.tian-w.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rhr.xylfe.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jmi.feifeiyinyue.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hxl.316326.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lcc.fktsv.cn

[K08] 二进制序列化（非 JSON）
来源：http://mrr.nanxuanxn.top

Py:   pickle.dumps(obj)
来源：http://aqr.jinyuanbaomall.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cok.shanyushiyangtech.top

JS:   v8.serialize(obj)        // Node
来源：http://teh.gotoacloud.top

TS:   v8.serialize(obj)        // Node
来源：http://czz.cdnleiting.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qcz.jianghu66.top

Go:   encoding/gob
来源：http://irt.zhoulong.xyz

Ruby: Marshal.dump(obj)
来源：http://fru.zhoulong.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zhy.havefunace.top

================================================================================
来源：http://dhe.gaohongyu789.top

L. 网络请求
来源：http://inb.hongshengwenyu.top

================================================================================
来源：http://dnu.fanxiaobao.xyz

[L01] 发送 GET 请求
来源：http://hxz.ppjwa.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iib.gaohongyu789.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zri.iojbl.cn

JS:   await fetch(url)
来源：http://dry.smart0.xyz

TS:   await fetch(url)
来源：http://kuu.tanke756.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ocs.316326.xyz

Go:   resp, err := http.Get(url)
来源：http://mrj.nanxinkj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://pys.jianghu66.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://alx.hcnkem.com

[L02] 发送 POST JSON
来源：http://rhe.jianghu66.top

Py:   requests.post(url, json={"a": 1})
来源：http://dfa.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zli.hesvh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rwa.hysaishi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zzg.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ctv.shanyushiyangkeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hxx.dianchejie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qaz.fktsv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cde.hysaishi.cn

[L03] 设置自定义请求头
来源：http://vnl.zhaomingkeji.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dzd.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pmr.tian-w.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kuy.havefunace.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mht.feifeiyinyue.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://smn.tian-w.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ohv.jinyuanbaomall.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gyo.gzhubu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gia.zhengqikj.top

[L04] 设置超时
来源：http://gqa.gotoacloud.top

Py:   requests.get(url, timeout=5)
来源：http://suz.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ijm.tanke756.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ibu.zhongyouzk.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bil.jinghuilouyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jps.aizwys.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qvr.hammf.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ieq.hnxiangtu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iuz.yuxming.cn

[L05] 上传文件（multipart）
来源：http://sfk.tianlin.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tex.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wvp.nanxinkj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rsi.hammf.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pqc.jqgfzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zxm.ybcxt.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://azl.yj20258888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nqt.mhx1999.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vho.smart0.xyz

[L06] 解析响应为 JSON
来源：http://xcb.dianchejie.cn

Py:   resp.json()
来源：http://asr.9152youxi.cn

PHP:  json_decode($body, true);
来源：http://dyn.zhongyouzk.top

JS:   await resp.json()
来源：http://qqh.hongshengwenyu.top

TS:   await resp.json()
来源：http://cuy.tian-w.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cxo.kuanghao11.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vwm.fzhhl.top

Ruby: JSON.parse(resp.body)
来源：http://nbp.jqgufenzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ccv.vqdsnc.cn

[L07] 处理 HTTP 状态码
来源：http://qby.vqdsnc.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mce.sxryk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zzd.yueranfly.top

JS:   resp.ok;  resp.status
来源：http://fpp.yuanzhike.top

TS:   resp.ok;  resp.status
来源：http://sdi.andypj.xyz

Java: resp.statusCode()
来源：http://ldt.jyoumei.cn

Go:   resp.StatusCode
来源：http://cov.zdbjq.cn

Ruby: resp.code.to_i
来源：http://lgs.jiagoushi.top

C#:   (int)resp.StatusCode
来源：http://njz.shanyushiyangtech.top

[L08] 并发请求多个地址
来源：http://ecp.zdqjudy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rhk.jinqigufen.top

PHP:  curl_multi_init() 系列
来源：http://bqv.hongshengwenyu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zdm.cdnleiting.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zit.jiagoushi.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bfu.gaohongyu789.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wys.daria6918.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qob.ydjk.org.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ffb.shanyushiyangkeji.top

================================================================================
来源：http://wyk.yangfankeji.com

M. 命令行 / 进程 / 环境
来源：http://mcs.vehdjk.com

================================================================================
来源：http://urs.shangyingyoupin.top

[M01] 读取命令行参数
来源：http://zdk.jianghu66.top

Py:   sys.argv[1:]
来源：http://was.jinghuilouyu.cn

PHP:  $argv;  $argc;
来源：http://hop.sxryk.cn

JS:   process.argv.slice(2)
来源：http://mcb.tian-w.cn

TS:   process.argv.slice(2)
来源：http://gjb.xziqi.cn

Java: args 数组（main 方法参数）
来源：http://giu.ivvv.top

Go:   os.Args[1:]
来源：http://ihz.c1oappe.top

Ruby: ARGV
来源：http://kgy.aibaodan.cn

C#:   args 数组（Main 方法参数）
来源：http://iwb.yueranfly.top

[M02] 读取环境变量
来源：http://bhy.ppjwa.cn

Py:   os.environ.get("HOME")
来源：http://egs.yj20258888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rla.daxiang520.top

JS:   process.env.HOME
来源：http://qvy.gaohongyu789.top

TS:   process.env.HOME
来源：http://jli.hfpthk.cn

Java: System.getenv("HOME")
来源：http://xvk.ydjk.org.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lbt.bjfxy.top

Ruby: ENV["HOME"]
来源：http://jmw.shuidangran.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://aju.tanke756.top

[M03] 执行外部命令
来源：http://ysu.zhongyouzk.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lox.jiagoushi.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xvf.guowangkeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ivm.haohaochexian.top

TS:   child_process.execSync("ls -l").toString()
来源：http://dot.epnwcf.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kfl.zhijiandao.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jjv.xuanzx.com

Ruby: system("ls -l");  `ls -l`
来源：http://zey.hysaishi.cn

C#:   Process.Start("ls", "-l");
来源：http://zgz.zhijiandao.cn

[M04] 获取当前工作目录
来源：http://prv.jinqigufen.top

Py:   os.getcwd()
来源：http://kvu.hnxiangtu.top

PHP:  getcwd();
来源：http://qpt.c1oappe.top

JS:   process.cwd()
来源：http://ndq.shzxlz.cn

TS:   process.cwd()
来源：http://zwo.guowangkeji.top

Java: Path.of("").toAbsolutePath()
来源：http://bbu.pycfn.com

Go:   os.Getwd()
来源：http://hzj.yuanzhike.top

Ruby: Dir.pwd
来源：http://rra.316326.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://hee.316326.xyz

[M05] 设置退出码
来源：http://agh.wangshuangyany.cn

Py:   sys.exit(1)
来源：http://oco.fehbvm.com

PHP:  exit(1);
来源：http://nly.kuanghao11.cn

JS:   process.exit(1)
来源：http://ljf.sysykeji.top

TS:   process.exit(1)
来源：http://rnc.pycfn.com

Java: System.exit(1)
来源：http://ziy.guowangkeji.top

Go:   os.Exit(1)
来源：http://fnn.chenlongwang.top

Ruby: exit 1
来源：http://yim.wangshuangyany.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wxy.svipenyu.cn

[M06] 向标准错误输出
来源：http://kgn.pengpengdd.cyou

Py:   print("err", file=sys.stderr)
来源：http://spp.dianchejie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yls.hywenlv.cn

JS:   console.error("err")
来源：http://zai.zhaomingkeji.xyz

TS:   console.error("err")
来源：http://ctn.haohaochexian.top

Java: System.err.println("err")
来源：http://xaj.sxryk.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yyu.jianghu66.top

Ruby: warn "err"
来源：http://jyu.9152youxi.cn

C#:   Console.Error.WriteLine("err")
来源：http://fgx.316326.xyz

[M07] 判断是否为主入口
来源：http://nls.xingfuxueyuan.xyz


<!-- 参考信息 -->
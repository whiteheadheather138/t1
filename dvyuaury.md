代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kgc.yj20258.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rcs.xziqi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lro.meibo888.top

================================================================================
来源：http://uet.shangyingyoupin.top

J. 日期与时间
来源：http://uok.uphjek.com

================================================================================
来源：http://xib.shanyushiyangtech.top

[J01] 获取当前时间
来源：http://snr.nwbrower.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://nvs.fehbvm.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vop.gotoacloud.top

JS:   new Date();  Date.now()
来源：http://rpb.hongshengwenyu.top

TS:   new Date();  Date.now()
来源：http://jrx.aizwys.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jlt.hesvh.cn

Go:   time.Now()
来源：http://vgi.epnwcf.com

Ruby: Time.now
来源：http://grl.zycfv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kvc.zhoulong.xyz

[J02] 格式化输出
来源：http://gda.svipenyu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zww.snrcjt.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uue.yuanzhike.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tyk.aibaodan.cn

TS:   d.toISOString()
来源：http://eai.yvedp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jhm.fengsongda.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vmp.svipenyu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yjw.yueranfly.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ite.tanke756.top

[J03] 字符串解析为日期
来源：http://fww.nwbrower.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vki.zhixingplan.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sqn.wangshuangyany.cn

JS:   new Date("2024-01-02")
来源：http://kzz.tian-w.cn

TS:   new Date("2024-01-02")
来源：http://vdd.tian-w.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ipx.aizwys.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://twj.hammf.cn

Ruby: Date.parse("2024-01-02")
来源：http://xcj.tanke756.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lyd.zdbjq.cn

[J04] 时间戳与日期互转
来源：http://wwd.sufxvd.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://llg.daria6918.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hih.jqgufenzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iif.pycfn.com

TS:   Math.floor(Date.now() / 1000)
来源：http://wyg.quarkkingdee.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kyn.chenjidiqi.icu

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mya.zhaomingkeji.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uei.hammf.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ypu.nanxinkj.top

[J05] 时间加减（加 7 天）
来源：http://uue.xylfe.cn

Py:   now + timedelta(days=7)
来源：http://xuj.jiagoushi.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rme.shzxlz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://psm.yangfankeji.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dbt.havefunace.top

Java: LocalDate.now().plusDays(7)
来源：http://uur.aizwys.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rjy.nwbrower.top

Ruby: Time.now + 7 * 86400
来源：http://dmi.hnxiangtu.top

C#:   DateTime.Now.AddDays(7)
来源：http://bpx.hysaishi.cn

[J06] 计算两时间之差
来源：http://xhp.ydjk.org.cn

Py:   (end - start).total_seconds()
来源：http://lms.9152youxi.cn

PHP:  $end->diff($start)->days;
来源：http://hxi.cucudq.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baj.guowangkeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ucw.zhijiandao.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mhc.kuanghao11.cn

Go:   end.Sub(start).Hours()
来源：http://kks.fanxiaobao.xyz

Ruby: end - start                 # 返回秒数
来源：http://woo.hammf.cn

C#:   (end - start).TotalSeconds
来源：http://qnm.gaohongyu789.top

[J07] 比较两个日期
来源：http://nqo.316326.xyz

Py:   d1 < d2;  d1 == d2
来源：http://asr.fktsv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kze.zhijiandao.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jjq.shanyushiyangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://oas.yongpay.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gii.yj20258888.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kii.feifeiyinyue.top

Ruby: d1 < d2;  d1 == d2
来源：http://nmm.birdmap.top

C#:   d1 < d2;  d1 == d2
来源：http://anu.fengsongda.top

[J08] 提取年月日与星期
来源：http://thm.sufxvd.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mjb.yvedp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rsm.fehbvm.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lij.jqgufenzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://odq.yvedp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dts.xziqi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ixi.nwbrower.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cca.xylfe.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ahq.fktsv.cn

[J09] 时区处理
来源：http://djh.feifeiyinyue.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yjd.yongpay.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cix.chenjidiqi.icu

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rip.aizwys.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ftx.shangyingyoupin.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ofl.cucudq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bwy.yanxiufei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jfp.dashuyun.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://idz.yongpay.top

[J10] 取今天 / 本月第一天
来源：http://jng.zdqjudy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://wri.jqgufenzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cxm.hysaishi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vfh.wangdashe.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pbu.yuanzhike.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://prm.fktsv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pfa.vehdjk.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wac.hywenlv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hvf.yuanzhike.top

================================================================================
来源：http://ekb.9152youxi.cn

K. JSON 与序列化
来源：http://cww.hongshengwenyu.top

================================================================================
来源：http://anw.yangfankeji.com

[K01] 对象转 JSON 字符串
来源：http://bhs.hfpthk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xiv.chenlongwang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://efa.zhaomingkeji.xyz

JS:   JSON.stringify(obj)
来源：http://mei.jqgufenzy.top

TS:   JSON.stringify(obj)
来源：http://kgf.cqqwz.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rpw.zdbjq.cn

Go:   json.Marshal(obj)
来源：http://qtl.xuanzx.com

Ruby: obj.to_json                                     // require "json"
来源：http://vvb.hfpthk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lbu.ehwqpu.com

[K02] JSON 字符串转对象
来源：http://wub.hcnkem.com

Py:   json.loads(s)
来源：http://boo.cdnleiting.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vyb.yueranfly.top

JS:   JSON.parse(s)
来源：http://csv.jqgufenzy.top

TS:   JSON.parse(s)
来源：http://kvl.fanxiaobao.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nxu.jinyuanbaomall.cn

Go:   json.Unmarshal(data, &v)
来源：http://yzp.shuidangran.top

Ruby: JSON.parse(s)
来源：http://bjo.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nyb.ydzc1.top

[K03] JSON 美化输出（带缩进）
来源：http://lmd.jqgufenzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qva.havefunace.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pru.cheryme.top

JS:   JSON.stringify(obj, null, 2)
来源：http://pfr.zhiwuduotai.top

TS:   JSON.stringify(obj, null, 2)
来源：http://rkp.0kj1m.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dnm.guannengcc.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vdz.zhongyouzk.top

Ruby: JSON.pretty_generate(obj)
来源：http://jlk.redwolf501.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tdr.sufxvd.cn

[K04] 读取 JSON 文件
来源：http://iwg.hnxiangtu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zka.gotoacloud.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nlx.jlsjyb.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ohu.tanke756.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cnd.zhaomingkeji.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hqd.sysykeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lcv.zhongyouzk.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://waw.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mix.aizwys.cn

[K05] 深拷贝对象
来源：http://ebg.snrcjt.cn

Py:   copy.deepcopy(obj)
来源：http://ivo.bbcook.cn

PHP:  unserialize(serialize($obj));
来源：http://aab.xingfuxueyuan.xyz

JS:   structuredClone(obj)
来源：http://gnd.gogol.net.cn

TS:   structuredClone(obj)
来源：http://cff.cashguo.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jvs.iojbl.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://etm.epnwcf.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zem.guowangkeji.top

C#:   // 序列化往返，或自定义 Clone
来源：http://eij.iojbl.cn

[K06] 解析 URL 查询串
来源：http://ocd.chenjidiqi.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://svf.yonumen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dsg.meibo888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sch.cqqwz.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dmv.meibo888.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hvv.tanke756.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://zsz.yj202588.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kxz.gzhubu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gyn.9152youxi.cn

[K07] 进制转换
来源：http://xvs.hesvh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dzl.hfpthk.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zqp.chenlongwang.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uzy.gzhubu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jgr.pycfn.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://eer.chenlongwang.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://une.xingfuxueyuan.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vnn.gogol.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wtv.smart0.xyz

[K08] 二进制序列化（非 JSON）
来源：http://ucm.uphjek.com

Py:   pickle.dumps(obj)
来源：http://ekq.fanxiaobao.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://ztz.yj20258.top

JS:   v8.serialize(obj)        // Node
来源：http://nxe.feifeiyinyue.top

TS:   v8.serialize(obj)        // Node
来源：http://zzh.jqgfzy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ssq.tarul.cn

Go:   encoding/gob
来源：http://ndb.xylfe.cn

Ruby: Marshal.dump(obj)
来源：http://nje.gotoacloud.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vmi.nanxinkj.top

================================================================================
来源：http://qrs.c1oappe.top

L. 网络请求
来源：http://jvi.gzhubu.top

================================================================================
来源：http://ula.jinqigufen.top

[L01] 发送 GET 请求
来源：http://tee.tianlin.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rzo.epnwcf.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kqh.fengsongda.top

JS:   await fetch(url)
来源：http://ivt.hnxiangtu.top

TS:   await fetch(url)
来源：http://nee.ydjk.org.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tey.hfpthk.cn

Go:   resp, err := http.Get(url)
来源：http://vzu.shanyushiyangtech.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jgc.jyoumei.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mjx.birdmap.top

[L02] 发送 POST JSON
来源：http://qmv.uphjek.com

Py:   requests.post(url, json={"a": 1})
来源：http://mfq.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nfs.yvedp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hhu.tanke756.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://udy.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lft.52xcode.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mbu.hysaishi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jzx.fengsongda.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lyk.shanyushiyangkeji.top

[L03] 设置自定义请求头
来源：http://bep.dianchejie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lgu.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vys.yuanzhike.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aub.jiagoushi.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://agm.shanyushiyangkeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gjq.yvedp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rkl.zhongyouzk.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kvl.cucudq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qqt.bbcook.cn

[L04] 设置超时
来源：http://ekd.gotoacloud.top

Py:   requests.get(url, timeout=5)
来源：http://kfj.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yid.smart0.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nax.xziqi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fbk.fengsongda.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://itb.cqqwz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tsz.ybcxt.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xkp.hnxiangtu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jch.jyoumei.cn

[L05] 上传文件（multipart）
来源：http://hif.wangshuangyany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://auz.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mzm.daria6918.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kfn.hongshengwenyu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tzg.sjlbkw.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ili.hnqzz.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://izm.yangfankeji.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wdm.cqqwz.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kiw.yangfankeji.com

[L06] 解析响应为 JSON
来源：http://wqu.vqdsnc.cn

Py:   resp.json()
来源：http://jbr.hywenlv.cn

PHP:  json_decode($body, true);
来源：http://nje.shangyingyoupin.top

JS:   await resp.json()
来源：http://rbh.nanxinkj.top

TS:   await resp.json()
来源：http://nql.c1oappe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dxo.0kj1m.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ajh.fktsv.cn

Ruby: JSON.parse(resp.body)
来源：http://oeq.fehbvm.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zvf.zhixingplan.top

[L07] 处理 HTTP 状态码
来源：http://ktn.jiagoushi.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://trp.yvedp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vaw.zhiwuduotai.top

JS:   resp.ok;  resp.status
来源：http://kra.chenjidiqi.icu

TS:   resp.ok;  resp.status
来源：http://ltp.bbcook.cn

Java: resp.statusCode()
来源：http://jxi.yj20258888.top

Go:   resp.StatusCode
来源：http://ikx.sweek.top

Ruby: resp.code.to_i
来源：http://lsb.c1oappe.top

C#:   (int)resp.StatusCode
来源：http://ryf.vehdjk.com

[L08] 并发请求多个地址
来源：http://jyr.ydjk.org.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mld.ppjwa.cn

PHP:  curl_multi_init() 系列
来源：http://axn.hnqzz.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yrm.shanyushiyangtech.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uza.shangyingyoupin.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nht.ywan-chungtsiang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://klr.fktsv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://net.jinghuilouyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nxu.yj20258.top

================================================================================
来源：http://pwa.9152youxi.cn

M. 命令行 / 进程 / 环境
来源：http://awg.jlsjyb.cn

================================================================================
来源：http://fck.jinyuanbaomall.cn

[M01] 读取命令行参数
来源：http://muf.tianlin.xyz

Py:   sys.argv[1:]
来源：http://phd.smart0.xyz

PHP:  $argv;  $argc;
来源：http://aqn.daria6918.cn

JS:   process.argv.slice(2)
来源：http://aek.jianghu66.top

TS:   process.argv.slice(2)
来源：http://ust.ehwqpu.com

Java: args 数组（main 方法参数）
来源：http://rcs.ppjwa.cn

Go:   os.Args[1:]
来源：http://yrb.hysaishi.cn

Ruby: ARGV
来源：http://suz.zdbjq.cn

C#:   args 数组（Main 方法参数）
来源：http://drn.tanke756.top

[M02] 读取环境变量
来源：http://pwc.chenjidiqi.icu

Py:   os.environ.get("HOME")
来源：http://fwr.tanke756.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qzu.jianghu66.top

JS:   process.env.HOME
来源：http://anw.zhaomingkeji.xyz

TS:   process.env.HOME
来源：http://kyu.zhixingplan.top

Java: System.getenv("HOME")
来源：http://mbx.jinqigufen.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://iyf.fktsv.cn

Ruby: ENV["HOME"]
来源：http://xse.zdbjq.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://obs.xuanzx.com

[M03] 执行外部命令
来源：http://vya.gaohongyu789.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bog.ydjk.org.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tcz.chenlongwang.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zas.yanxiufei.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xqx.birdmap.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kvj.316326.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://ckv.aibaodan.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nsc.jinghuilouyu.cn

C#:   Process.Start("ls", "-l");
来源：http://ztv.sjlbkw.cn

[M04] 获取当前工作目录
来源：http://fvv.redwolf501.top

Py:   os.getcwd()
来源：http://iyb.hnqzz.top

PHP:  getcwd();
来源：http://lcj.jinghuilouyu.cn

JS:   process.cwd()
来源：http://zmt.hnxiangtu.top

TS:   process.cwd()
来源：http://szm.tanke756.top

Java: Path.of("").toAbsolutePath()
来源：http://cts.0kj1m.cn

Go:   os.Getwd()
来源：http://bbq.dashuyun.cn

Ruby: Dir.pwd
来源：http://zju.zhiwuduotai.top

C#:   Directory.GetCurrentDirectory()
来源：http://bzk.zhijiandao.cn

[M05] 设置退出码
来源：http://wrk.xuetiantiany.cn

Py:   sys.exit(1)
来源：http://ftn.yuxming.cn

PHP:  exit(1);
来源：http://nqh.yvedp.cn

JS:   process.exit(1)
来源：http://lke.jinqigfzy.top

TS:   process.exit(1)
来源：http://iec.52xcode.cn

Java: System.exit(1)
来源：http://pxq.yvedp.cn

Go:   os.Exit(1)
来源：http://wvg.yj20258.top

Ruby: exit 1
来源：http://nmm.gotoacloud.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nsu.hnqzz.top

[M06] 向标准错误输出
来源：http://efl.dashuyun.cn

Py:   print("err", file=sys.stderr)
来源：http://kiw.zhijiandao.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mgz.ivvv.top

JS:   console.error("err")
来源：http://zod.feifeiyinyue.top

TS:   console.error("err")
来源：http://aac.tanke756.top

Java: System.err.println("err")
来源：http://ung.fanxiaobao.xyz


<!-- 参考信息 -->
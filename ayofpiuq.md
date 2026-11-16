代发 wailian999

J. 日期与时间
来源：http://pfc.haohaochexian.top

================================================================================
来源：http://yaa.jinqigfzy.top

[J01] 获取当前时间
来源：http://nae.jinyuanbaomall.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wld.fengsongda.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nqo.c1oappe.top

JS:   new Date();  Date.now()
来源：http://ppd.daria6918.cn

TS:   new Date();  Date.now()
来源：http://vad.fehbvm.com

Java: LocalDateTime.now();  Instant.now()
来源：http://jfn.hysaishi.cn

Go:   time.Now()
来源：http://gjh.yj202588.top

Ruby: Time.now
来源：http://ibs.zycfv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ymc.hnxiangtu.top

[J02] 格式化输出
来源：http://zcc.hesvh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xyy.yfazqb.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yua.gogol.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dil.yongpay.top

TS:   d.toISOString()
来源：http://skm.jqgufenzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hnb.zycfv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://voh.havefunace.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gpc.shanyushiyangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kwg.mhx1999.top

[J03] 字符串解析为日期
来源：http://anr.ppjwa.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ebu.9152youxi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kcb.xziqi.cn

JS:   new Date("2024-01-02")
来源：http://xwg.sxryk.cn

TS:   new Date("2024-01-02")
来源：http://ykl.dianchejie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fsp.fzhhl.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://edn.shanyushiyangtech.top

Ruby: Date.parse("2024-01-02")
来源：http://igt.316326.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pys.shangyingyoupin.top

[J04] 时间戳与日期互转
来源：http://eet.chenlongwang.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://niz.shangyingyoupin.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rjt.redwolf501.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://eth.svipenyu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yfg.zhiwuduotai.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cjy.316326.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pmd.guannengcc.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://eva.jinyuanbaomall.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://icz.yj20258.top

[J05] 时间加减（加 7 天）
来源：http://wmv.hywenlv.cn

Py:   now + timedelta(days=7)
来源：http://bxy.aibaodan.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jlp.gogol.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jox.ybcxt.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vpb.hnxiangtu.top

Java: LocalDate.now().plusDays(7)
来源：http://sqg.daxiang520.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xsu.yvedp.cn

Ruby: Time.now + 7 * 86400
来源：http://wsv.redwolf501.top

C#:   DateTime.Now.AddDays(7)
来源：http://yhd.cheryme.top

[J06] 计算两时间之差
来源：http://xub.hysaishi.cn

Py:   (end - start).total_seconds()
来源：http://bsw.yfazqb.com

PHP:  $end->diff($start)->days;
来源：http://spy.hammf.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jcn.fehbvm.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yob.9152youxi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jdz.xinyue.icu

Go:   end.Sub(start).Hours()
来源：http://iwz.fehbvm.com

Ruby: end - start                 # 返回秒数
来源：http://mtd.xinyue.icu

C#:   (end - start).TotalSeconds
来源：http://bnc.hysaishi.cn

[J07] 比较两个日期
来源：http://qha.yj202588.top

Py:   d1 < d2;  d1 == d2
来源：http://cah.gotoacloud.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://seq.gogol.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://czr.ywan-chungtsiang.top

TS:   d1.getTime() < d2.getTime()
来源：http://wwv.meibo888.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sfn.jinyuanbaomall.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xgc.nanxinkj.top

Ruby: d1 < d2;  d1 == d2
来源：http://lcb.yueranfly.top

C#:   d1 < d2;  d1 == d2
来源：http://mjl.bjfxy.top

[J08] 提取年月日与星期
来源：http://gxa.cucudq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wpd.9152youxi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nwo.0kj1m.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wcy.jyoumei.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vms.ppjwa.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hfx.hongshengwenyu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gnd.yueranfly.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bpm.pycfn.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pjd.aizwys.cn

[J09] 时区处理
来源：http://gno.chenzaomai.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://slt.fktsv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ylo.aibaodan.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zga.uphjek.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yrx.shangyingyoupin.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hxi.nanxinkj.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tga.hongshengwenyu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://rgs.dashuyun.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hxg.shanyushiyangtech.top

[J10] 取今天 / 本月第一天
来源：http://was.xylfe.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gni.316326.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wqf.wangshuangyany.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bow.gogol.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jay.gogol.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jtv.sufxvd.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qzp.hnxiangtu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ott.ivvv.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://krs.fehbvm.com

================================================================================
来源：http://tyy.sjlbkw.cn

K. JSON 与序列化
来源：http://rwr.zycfv.cn

================================================================================
来源：http://yzd.iojbl.cn

[K01] 对象转 JSON 字符串
来源：http://pms.daria6918.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mez.hammf.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xxr.zdqjudy.top

JS:   JSON.stringify(obj)
来源：http://vuy.hnxiangtu.top

TS:   JSON.stringify(obj)
来源：http://riz.jianghu66.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ilw.redwolf501.top

Go:   json.Marshal(obj)
来源：http://fqv.gaohongyu789.top

Ruby: obj.to_json                                     // require "json"
来源：http://jei.shzxlz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://brg.hysaishi.cn

[K02] JSON 字符串转对象
来源：http://uhw.havefunace.top

Py:   json.loads(s)
来源：http://myw.vehdjk.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jki.9152youxi.cn

JS:   JSON.parse(s)
来源：http://lmw.aizwys.cn

TS:   JSON.parse(s)
来源：http://xzg.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uww.feifeiyinyue.top

Go:   json.Unmarshal(data, &v)
来源：http://yhp.aizwys.cn

Ruby: JSON.parse(s)
来源：http://csp.zhixingplan.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yjr.shanyushiyangkeji.top

[K03] JSON 美化输出（带缩进）
来源：http://gsw.jqgufenzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vdh.xylfe.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jdb.cqqwz.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qbp.meibo888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lbr.dashuyun.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kbl.jlsjyb.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tdz.gaohongyu789.top

Ruby: JSON.pretty_generate(obj)
来源：http://mrg.fehbvm.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yzb.sufxvd.cn

[K04] 读取 JSON 文件
来源：http://phn.ivvv.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hef.wangdashe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nea.wangdashe.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oeg.xuanzx.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cmk.hammf.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gkl.xuanzx.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://eyd.dashuyun.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wky.tian-w.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xdz.yj202588.top

[K05] 深拷贝对象
来源：http://cax.quarkkingdee.top

Py:   copy.deepcopy(obj)
来源：http://aio.meibo888.top

PHP:  unserialize(serialize($obj));
来源：http://tnw.guowangkeji.top

JS:   structuredClone(obj)
来源：http://jwf.snrcjt.cn

TS:   structuredClone(obj)
来源：http://qmk.shanyushiyangkeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vfl.xuanzx.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uju.aibaodan.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hve.jqgufenzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://aum.jinyuanbaomall.cn

[K06] 解析 URL 查询串
来源：http://izn.yj202588.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hoq.wangdashe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gnp.ywan-chungtsiang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ypl.gotoacloud.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nbf.gotoacloud.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ifk.yj20258888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://zjl.bbcook.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gxm.pengpengdd.cyou

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://epi.ppjwa.cn

[K07] 进制转换
来源：http://mkr.hammf.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zna.svipenyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wsp.zhijiandao.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tth.yongpay.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bgv.sxryk.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tfe.ywan-chungtsiang.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qkr.uphjek.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rjd.xylfe.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bkv.fktsv.cn

[K08] 二进制序列化（非 JSON）
来源：http://vao.shuidangran.top

Py:   pickle.dumps(obj)
来源：http://ocf.zhixingplan.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zna.chenjidiqi.icu

JS:   v8.serialize(obj)        // Node
来源：http://emu.kuanghao11.cn

TS:   v8.serialize(obj)        // Node
来源：http://bgd.cashguo.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jnl.nwbrower.top

Go:   encoding/gob
来源：http://yfu.yvedp.cn

Ruby: Marshal.dump(obj)
来源：http://vja.haohaochexian.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nmk.cashguo.top

================================================================================
来源：http://ysk.shanyushiyangtech.top

L. 网络请求
来源：http://owq.haohaochexian.top

================================================================================
来源：http://cec.cqqwz.cn

[L01] 发送 GET 请求
来源：http://jrb.jyoumei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mkz.yangfankeji.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://htz.hongshengwenyu.top

JS:   await fetch(url)
来源：http://vco.iojbl.cn

TS:   await fetch(url)
来源：http://obq.guowangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ybj.nanxuanxn.top

Go:   resp, err := http.Get(url)
来源：http://tkj.shanyushiyangtech.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wis.pycfn.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qlw.jqgfzy.top

[L02] 发送 POST JSON
来源：http://buz.ydzc1.top

Py:   requests.post(url, json={"a": 1})
来源：http://zjx.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oew.birdmap.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qhr.daxiang520.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ebu.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lov.svipenyu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xuf.ehwqpu.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zyn.shanyushiyangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ugh.cucudq.cn

[L03] 设置自定义请求头
来源：http://kax.daria6918.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ulv.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bvx.tianlin.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://htr.iojbl.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gue.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gvo.yfazqb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bkj.quarkkingdee.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dno.fengsongda.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fce.cucudq.cn

[L04] 设置超时
来源：http://fdo.aibaodan.cn

Py:   requests.get(url, timeout=5)
来源：http://muh.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://neq.gzhubu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cge.hysaishi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://clu.yj20258888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fxb.jqgufenzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://khs.birdmap.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mov.chenzaomai.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vza.chenlongwang.top

[L05] 上传文件（multipart）
来源：http://tfn.jinyuanbaomall.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nve.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sfj.kuanghao11.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rnr.xziqi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fiz.xingfuxueyuan.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://our.redwolf501.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kno.hesvh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fhb.yueranfly.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yqt.ydjk.org.cn

[L06] 解析响应为 JSON
来源：http://num.c1oappe.top

Py:   resp.json()
来源：http://imx.gzhubu.top

PHP:  json_decode($body, true);
来源：http://wrh.snrcjt.cn

JS:   await resp.json()
来源：http://xhx.xingfuxueyuan.xyz

TS:   await resp.json()
来源：http://igg.yuanzhike.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dgr.jqgfzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lhd.cucudq.cn

Ruby: JSON.parse(resp.body)
来源：http://iwx.nanxinkj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zst.kuanghao11.cn

[L07] 处理 HTTP 状态码
来源：http://xfa.zhaomingkeji.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yjv.yj202588.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gvo.shzxlz.cn

JS:   resp.ok;  resp.status
来源：http://bxv.yvedp.cn

TS:   resp.ok;  resp.status
来源：http://jju.mhx1999.top

Java: resp.statusCode()
来源：http://anr.haohaochexian.top

Go:   resp.StatusCode
来源：http://ssy.hongshengwenyu.top

Ruby: resp.code.to_i
来源：http://ihh.c1oappe.top

C#:   (int)resp.StatusCode
来源：http://pue.hnxiangtu.top

[L08] 并发请求多个地址
来源：http://enj.chenzaomai.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ogd.nanxuanxn.top

PHP:  curl_multi_init() 系列
来源：http://ocd.epnwcf.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aoq.hnxiangtu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yaf.dashuyun.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hpz.hywenlv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oig.chenlongwang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wxo.meibo888.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bzi.zdqjudy.top

================================================================================
来源：http://drv.kuanghao11.cn

M. 命令行 / 进程 / 环境
来源：http://qhq.gotoacloud.top

================================================================================
来源：http://gof.yj202588.top

[M01] 读取命令行参数
来源：http://wpq.wangshuangyany.cn

Py:   sys.argv[1:]
来源：http://qrw.ivvv.top

PHP:  $argv;  $argc;
来源：http://wub.shangyingyoupin.top

JS:   process.argv.slice(2)
来源：http://dqe.jlsjyb.cn

TS:   process.argv.slice(2)
来源：http://gmf.yuxming.cn

Java: args 数组（main 方法参数）
来源：http://smj.aibaodan.cn

Go:   os.Args[1:]
来源：http://bax.andypj.xyz

Ruby: ARGV
来源：http://tnu.jqgufenzy.top

C#:   args 数组（Main 方法参数）
来源：http://xoa.shangyingyoupin.top

[M02] 读取环境变量
来源：http://oza.snrcjt.cn

Py:   os.environ.get("HOME")
来源：http://jfl.zhaomingkeji.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hfn.fengsongda.top

JS:   process.env.HOME
来源：http://isq.snrcjt.cn

TS:   process.env.HOME
来源：http://jgu.cdnleiting.top

Java: System.getenv("HOME")
来源：http://udn.kuanghao11.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ucl.cqqwz.cn

Ruby: ENV["HOME"]
来源：http://vqh.52xcode.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mmj.dianchejie.cn

[M03] 执行外部命令
来源：http://lao.hcnkem.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fdg.chenjidiqi.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rmg.cdnleiting.top

JS:   child_process.execSync("ls -l").toString()
来源：http://deb.jinqigfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ndf.epnwcf.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vvi.jyoumei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hgn.9152youxi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nli.tian-w.cn

C#:   Process.Start("ls", "-l");
来源：http://npe.tarul.cn

[M04] 获取当前工作目录
来源：http://ioj.zhijiandao.cn

Py:   os.getcwd()
来源：http://wdj.cdnleiting.top

PHP:  getcwd();
来源：http://yiw.shangyingyoupin.top

JS:   process.cwd()
来源：http://jhw.smart0.xyz

TS:   process.cwd()
来源：http://xxf.epnwcf.com

Java: Path.of("").toAbsolutePath()
来源：http://swx.aizwys.cn

Go:   os.Getwd()
来源：http://hlc.snrcjt.cn

Ruby: Dir.pwd
来源：http://fxf.shuidangran.top

C#:   Directory.GetCurrentDirectory()
来源：http://rnp.ybcxt.top

[M05] 设置退出码
来源：http://cus.vehdjk.com

Py:   sys.exit(1)
来源：http://vpp.guowangkeji.top

PHP:  exit(1);
来源：http://nzi.hammf.cn

JS:   process.exit(1)
来源：http://oqb.sweek.top

TS:   process.exit(1)
来源：http://ozc.yfazqb.com

Java: System.exit(1)
来源：http://klj.c1oappe.top

Go:   os.Exit(1)
来源：http://iiv.snrcjt.cn

Ruby: exit 1
来源：http://bip.haohaochexian.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uum.wangshuangyany.cn

[M06] 向标准错误输出
来源：http://umu.jinqigfzy.top

Py:   print("err", file=sys.stderr)
来源：http://kqw.fengsongda.top

PHP:  fwrite(STDERR, "err\n");
来源：http://krh.cucudq.cn

JS:   console.error("err")
来源：http://vvp.shuidangran.top

TS:   console.error("err")
来源：http://hoz.hammf.cn

Java: System.err.println("err")
来源：http://lpf.gogol.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tjc.cqqwz.cn

Ruby: warn "err"
来源：http://ngp.9152youxi.cn

C#:   Console.Error.WriteLine("err")
来源：http://ygg.zdbjq.cn

[M07] 判断是否为主入口
来源：http://qkp.chenjidiqi.icu


<!-- 参考信息 -->
代发 wailian999

J. 日期与时间
来源：http://eww.52xcode.cn

================================================================================
来源：http://jji.mhx1999.top

[J01] 获取当前时间
来源：http://szm.xuetiantiany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qjs.xziqi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nnx.ivvv.top

JS:   new Date();  Date.now()
来源：http://jwy.zycfv.cn

TS:   new Date();  Date.now()
来源：http://snz.zhongyouzk.top

Java: LocalDateTime.now();  Instant.now()
来源：http://sin.tian-w.cn

Go:   time.Now()
来源：http://syq.jinqigufen.top

Ruby: Time.now
来源：http://tbb.ydzc1.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yrd.quarkkingdee.top

[J02] 格式化输出
来源：http://hqh.tarul.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tyx.chenlongwang.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uha.yanxiufei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://epp.yuxming.cn

TS:   d.toISOString()
来源：http://xoi.52xcode.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xlv.zycfv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lhc.tarul.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jvy.yuxming.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dnp.jlsjyb.cn

[J03] 字符串解析为日期
来源：http://yju.bjfxy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://oaq.havefunace.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ipw.andypj.xyz

JS:   new Date("2024-01-02")
来源：http://gxx.ydzc1.top

TS:   new Date("2024-01-02")
来源：http://yge.havefunace.top

Java: LocalDate.parse("2024-01-02")
来源：http://dme.sxryk.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mql.xuanzx.com

Ruby: Date.parse("2024-01-02")
来源：http://jwk.chenjidiqi.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mfk.birdmap.top

[J04] 时间戳与日期互转
来源：http://xze.chenjidiqi.icu

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pho.xingfuxueyuan.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hii.tianlin.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sjt.havefunace.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ksc.uphjek.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://imj.jinghuilouyu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://waz.gzhubu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qco.zhengqikj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yvw.0kj1m.cn

[J05] 时间加减（加 7 天）
来源：http://ymd.jinqigufen.top

Py:   now + timedelta(days=7)
来源：http://hdt.shzxlz.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://crh.sjlbkw.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bmc.redwolf501.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ocj.ehwqpu.com

Java: LocalDate.now().plusDays(7)
来源：http://xyf.andypj.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hck.zhiwuduotai.top

Ruby: Time.now + 7 * 86400
来源：http://jql.mhx1999.top

C#:   DateTime.Now.AddDays(7)
来源：http://unc.xingfuxueyuan.xyz

[J06] 计算两时间之差
来源：http://uda.shuidangran.top

Py:   (end - start).total_seconds()
来源：http://ldy.yj20258888.top

PHP:  $end->diff($start)->days;
来源：http://sma.zhongyouzk.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://guk.jqgufenzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lwt.nanxinkj.top

Java: Duration.between(start, end).toSeconds()
来源：http://nsa.yj202588.top

Go:   end.Sub(start).Hours()
来源：http://csx.hammf.cn

Ruby: end - start                 # 返回秒数
来源：http://yse.yj20258888.top

C#:   (end - start).TotalSeconds
来源：http://lig.hammf.cn

[J07] 比较两个日期
来源：http://jsb.epnwcf.com

Py:   d1 < d2;  d1 == d2
来源：http://ivs.cucudq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vkc.quarkkingdee.top

JS:   d1.getTime() < d2.getTime()
来源：http://tja.cheryme.top

TS:   d1.getTime() < d2.getTime()
来源：http://ira.yvedp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kxc.meibo888.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://njg.sjlbkw.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gjz.cqqwz.cn

C#:   d1 < d2;  d1 == d2
来源：http://yez.shangyingyoupin.top

[J08] 提取年月日与星期
来源：http://uno.chenlongwang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gqj.guannengcc.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://soi.jinqigfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vtj.hnxiangtu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uhs.shanyushiyangkeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rcc.ivvv.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rwc.vehdjk.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vmy.0kj1m.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wgy.c1oappe.top

[J09] 时区处理
来源：http://tku.shuidangran.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://azl.hongshengwenyu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cak.chenlongwang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lmb.ctjpmb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pzf.fehbvm.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kar.yj202588.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://him.quarkkingdee.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zrv.haohaochexian.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gnu.yuxming.cn

[J10] 取今天 / 本月第一天
来源：http://zep.haohaochexian.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ldv.zhaomingkeji.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bbf.ybcxt.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gby.jinqigufen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fhf.fzhhl.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pqw.wangshuangyany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xwn.ydzc1.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kmd.ppjwa.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jkx.sjlbkw.cn

================================================================================
来源：http://fec.jinyuanbaomall.cn

K. JSON 与序列化
来源：http://saf.pengpengdd.cyou

================================================================================
来源：http://vpz.52xcode.cn

[K01] 对象转 JSON 字符串
来源：http://xpd.316326.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iuc.fzhhl.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qed.nanxuanxn.top

JS:   JSON.stringify(obj)
来源：http://vac.yj202588.top

TS:   JSON.stringify(obj)
来源：http://qow.hysaishi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gwq.vehdjk.com

Go:   json.Marshal(obj)
来源：http://dki.jinqigfzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://ton.bjfxy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://cgf.daria6918.cn

[K02] JSON 字符串转对象
来源：http://bot.cashguo.top

Py:   json.loads(s)
来源：http://jhf.cucudq.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yaq.xuanzx.com

JS:   JSON.parse(s)
来源：http://qbg.nwbrower.top

TS:   JSON.parse(s)
来源：http://rhz.kuanghao11.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wcn.ybcxt.top

Go:   json.Unmarshal(data, &v)
来源：http://hhg.xingfuxueyuan.xyz

Ruby: JSON.parse(s)
来源：http://txa.jyoumei.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dil.jqgufenzy.top

[K03] JSON 美化输出（带缩进）
来源：http://rij.hesvh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kjp.zhixingplan.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://glf.birdmap.top

JS:   JSON.stringify(obj, null, 2)
来源：http://kcr.yuxming.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sxj.yanxiufei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://thh.jianghu66.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ami.ydjk.org.cn

Ruby: JSON.pretty_generate(obj)
来源：http://oqg.jqgufenzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kcz.hongshengwenyu.top

[K04] 读取 JSON 文件
来源：http://ezs.cheryme.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xza.hysaishi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cek.feifeiyinyue.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kkw.hnxiangtu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ghw.haohaochexian.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kbj.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yey.zycfv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://weh.zycfv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fis.pycfn.com

[K05] 深拷贝对象
来源：http://fmh.jqgufenzy.top

Py:   copy.deepcopy(obj)
来源：http://gzv.jianghu66.top

PHP:  unserialize(serialize($obj));
来源：http://xel.52xcode.cn

JS:   structuredClone(obj)
来源：http://oyo.chenjidiqi.icu

TS:   structuredClone(obj)
来源：http://dci.sysykeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://sur.cucudq.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fkf.jqgufenzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://acq.shanyushiyangkeji.top

C#:   // 序列化往返，或自定义 Clone
来源：http://dej.gotoacloud.top

[K06] 解析 URL 查询串
来源：http://gkn.ybcxt.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ezv.ydzc1.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ktt.ydzc1.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kbx.yuxming.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ale.jinghuilouyu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iuz.cucudq.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jrz.feifeiyinyue.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sjv.shuidangran.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kyj.smart0.xyz

[K07] 进制转换
来源：http://xti.316326.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qsj.iojbl.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://aim.ydjk.org.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sir.chenjidiqi.icu

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xuv.hongshengwenyu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vaq.ydjk.org.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wbr.xuetiantiany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://trl.iojbl.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://szn.nwbrower.top

[K08] 二进制序列化（非 JSON）
来源：http://lvn.daria6918.cn

Py:   pickle.dumps(obj)
来源：http://faz.yj20258888.top

PHP:  serialize($obj);  unserialize($s);
来源：http://iik.jyoumei.cn

JS:   v8.serialize(obj)        // Node
来源：http://iby.nanxuanxn.top

TS:   v8.serialize(obj)        // Node
来源：http://egf.zhongyouzk.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pop.yuanzhike.top

Go:   encoding/gob
来源：http://tks.ctjpmb.com

Ruby: Marshal.dump(obj)
来源：http://pgt.cheryme.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oeo.zdbjq.cn

================================================================================
来源：http://xom.dashuyun.cn

L. 网络请求
来源：http://wsi.hongshengwenyu.top

================================================================================
来源：http://yum.xingfuxueyuan.xyz

[L01] 发送 GET 请求
来源：http://rpr.wangshuangyany.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wdj.hysaishi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ame.9152youxi.cn

JS:   await fetch(url)
来源：http://lls.c1oappe.top

TS:   await fetch(url)
来源：http://zcx.jinqigufen.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gbz.jianghu66.top

Go:   resp, err := http.Get(url)
来源：http://ozc.cheryme.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ofj.ybcxt.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yjq.gogol.net.cn

[L02] 发送 POST JSON
来源：http://qbf.jinghuilouyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://oez.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://utx.cashguo.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bus.gzhubu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lnl.guowangkeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://psm.yvedp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://reu.wangdashe.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jap.sjlbkw.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gae.mhx1999.top

[L03] 设置自定义请求头
来源：http://nzk.ydjk.org.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pee.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jhf.feifeiyinyue.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://afv.xylfe.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ckv.ivvv.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ypg.yfazqb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xlu.yj20258888.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jez.9152youxi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rmj.jqgufenzy.top

[L04] 设置超时
来源：http://qje.xuanzx.com

Py:   requests.get(url, timeout=5)
来源：http://spo.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jdq.zhijiandao.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://quv.haohaochexian.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://njt.xingfuxueyuan.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hsm.fengsongda.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lnh.zhixingplan.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ugh.zhijiandao.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sxu.c1oappe.top

[L05] 上传文件（multipart）
来源：http://hoh.kuanghao11.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://idx.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zzc.sysykeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lzx.jiagoushi.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://srs.uphjek.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qea.zdbjq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bln.gotoacloud.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rfd.0kj1m.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://csc.zhixingplan.top

[L06] 解析响应为 JSON
来源：http://phw.xinyue.icu

Py:   resp.json()
来源：http://nis.kuanghao11.cn

PHP:  json_decode($body, true);
来源：http://npt.haohaochexian.top

JS:   await resp.json()
来源：http://lmd.zhaomingkeji.xyz

TS:   await resp.json()
来源：http://zrg.andypj.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://etq.aizwys.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fko.meibo888.top

Ruby: JSON.parse(resp.body)
来源：http://cfn.svipenyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dpr.cucudq.cn

[L07] 处理 HTTP 状态码
来源：http://kjv.cqqwz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bec.jinyuanbaomall.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cva.hammf.cn

JS:   resp.ok;  resp.status
来源：http://yoi.andypj.xyz

TS:   resp.ok;  resp.status
来源：http://voc.c1oappe.top

Java: resp.statusCode()
来源：http://obs.zdbjq.cn

Go:   resp.StatusCode
来源：http://hhv.ywan-chungtsiang.top

Ruby: resp.code.to_i
来源：http://gir.chenjidiqi.icu

C#:   (int)resp.StatusCode
来源：http://dyw.yuanzhike.top

[L08] 并发请求多个地址
来源：http://lbw.dashuyun.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://djl.hywenlv.cn

PHP:  curl_multi_init() 系列
来源：http://pyy.wangdashe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ccl.vehdjk.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dcp.yueranfly.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lii.xinyue.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lho.zhiwuduotai.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pzh.gzhubu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://juk.vqdsnc.cn

================================================================================
来源：http://mig.jianghu66.top

M. 命令行 / 进程 / 环境
来源：http://ryi.zhixingplan.top

================================================================================
来源：http://koi.jyoumei.cn

[M01] 读取命令行参数
来源：http://eak.quarkkingdee.top

Py:   sys.argv[1:]
来源：http://hox.shanyushiyangkeji.top

PHP:  $argv;  $argc;
来源：http://bth.jqgfzy.top

JS:   process.argv.slice(2)
来源：http://bsa.jyoumei.cn

TS:   process.argv.slice(2)
来源：http://afw.cqqwz.cn

Java: args 数组（main 方法参数）
来源：http://rrh.mhx1999.top

Go:   os.Args[1:]
来源：http://xwr.meibo888.top

Ruby: ARGV
来源：http://qfw.iojbl.cn

C#:   args 数组（Main 方法参数）
来源：http://llc.chenjidiqi.icu

[M02] 读取环境变量
来源：http://ust.jlsjyb.cn

Py:   os.environ.get("HOME")
来源：http://btt.zhoulong.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uru.ydjk.org.cn

JS:   process.env.HOME
来源：http://ini.zhongyouzk.top

TS:   process.env.HOME
来源：http://ikd.xinyue.icu

Java: System.getenv("HOME")
来源：http://czf.dianchejie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://suf.hysaishi.cn

Ruby: ENV["HOME"]
来源：http://rau.shanyushiyangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xvj.svipenyu.cn

[M03] 执行外部命令
来源：http://wij.shuidangran.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://eha.mhx1999.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xlg.haohaochexian.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xjz.jlsjyb.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xwu.zhixingplan.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://voo.iojbl.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://uwb.cashguo.top

Ruby: system("ls -l");  `ls -l`
来源：http://qsl.zhaomingkeji.xyz

C#:   Process.Start("ls", "-l");
来源：http://kdk.zdbjq.cn

[M04] 获取当前工作目录
来源：http://jpo.gogol.net.cn

Py:   os.getcwd()
来源：http://gpj.chenjidiqi.icu

PHP:  getcwd();
来源：http://zkf.zdbjq.cn

JS:   process.cwd()
来源：http://wzm.yvedp.cn

TS:   process.cwd()
来源：http://hmv.aibaodan.cn

Java: Path.of("").toAbsolutePath()
来源：http://qyh.hywenlv.cn

Go:   os.Getwd()
来源：http://mjf.sjlbkw.cn

Ruby: Dir.pwd
来源：http://akm.cqqwz.cn

C#:   Directory.GetCurrentDirectory()
来源：http://clo.316326.xyz

[M05] 设置退出码
来源：http://xkt.smart0.xyz

Py:   sys.exit(1)
来源：http://pas.ywan-chungtsiang.top

PHP:  exit(1);
来源：http://fhx.dashuyun.cn

JS:   process.exit(1)
来源：http://aaq.yonumen.top

TS:   process.exit(1)
来源：http://imy.hongshengwenyu.top

Java: System.exit(1)
来源：http://ngf.jlsjyb.cn

Go:   os.Exit(1)
来源：http://sbr.tarul.cn

Ruby: exit 1
来源：http://soy.hesvh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wjx.vehdjk.com

[M06] 向标准错误输出
来源：http://mhb.zhijiandao.cn

Py:   print("err", file=sys.stderr)
来源：http://baw.gogol.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://llv.jinghuilouyu.cn

JS:   console.error("err")
来源：http://svi.zdqjudy.top

TS:   console.error("err")
来源：http://wlr.jinyuanbaomall.cn

Java: System.err.println("err")
来源：http://mrn.ctjpmb.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oqa.zdbjq.cn

Ruby: warn "err"
来源：http://pgh.nanxinkj.top

C#:   Console.Error.WriteLine("err")
来源：http://znf.yj20258.top

[M07] 判断是否为主入口
来源：http://tek.zhiwuduotai.top


<!-- 参考信息 -->
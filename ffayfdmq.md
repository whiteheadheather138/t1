代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wyu.jiagoushi.top

JS:   new Date();  Date.now()
来源：http://mes.yj20258.top

TS:   new Date();  Date.now()
来源：http://cph.xinyue.icu

Java: LocalDateTime.now();  Instant.now()
来源：http://see.jlsjyb.cn

Go:   time.Now()
来源：http://pez.gzhubu.top

Ruby: Time.now
来源：http://dey.yueranfly.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fux.zhongyouzk.top

[J02] 格式化输出
来源：http://iaz.jinghuilouyu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://icm.yj202588.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iik.yangfankeji.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tna.xuetiantiany.cn

TS:   d.toISOString()
来源：http://grv.yonumen.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jrn.xingfuxueyuan.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bjc.c1oappe.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fgc.jinqigfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ppw.yongpay.top

[J03] 字符串解析为日期
来源：http://ony.quarkkingdee.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://chy.chenjidiqi.icu

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mlo.xylfe.cn

JS:   new Date("2024-01-02")
来源：http://ceq.tanke756.top

TS:   new Date("2024-01-02")
来源：http://ngx.wangshuangyany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://umj.wangdashe.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://axp.yongpay.top

Ruby: Date.parse("2024-01-02")
来源：http://wff.ppjwa.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pbj.ehwqpu.com

[J04] 时间戳与日期互转
来源：http://rfe.tanke756.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xxz.xziqi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ctf.wangdashe.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://buu.0kj1m.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pbj.xylfe.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aln.yuanzhike.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lzk.ywan-chungtsiang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dod.dianchejie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mmm.sufxvd.cn

[J05] 时间加减（加 7 天）
来源：http://cqr.aizwys.cn

Py:   now + timedelta(days=7)
来源：http://aqx.fktsv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fbj.shuidangran.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zvg.yueranfly.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uwy.daxiang520.top

Java: LocalDate.now().plusDays(7)
来源：http://pwu.birdmap.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yld.shanyushiyangtech.top

Ruby: Time.now + 7 * 86400
来源：http://lpz.nwbrower.top

C#:   DateTime.Now.AddDays(7)
来源：http://zdg.bbcook.cn

[J06] 计算两时间之差
来源：http://frm.sysykeji.top

Py:   (end - start).total_seconds()
来源：http://sgo.sufxvd.cn

PHP:  $end->diff($start)->days;
来源：http://myt.jqgfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://grz.snrcjt.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uyt.svipenyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gfo.daxiang520.top

Go:   end.Sub(start).Hours()
来源：http://mgk.meibo888.top

Ruby: end - start                 # 返回秒数
来源：http://lhc.hnxiangtu.top

C#:   (end - start).TotalSeconds
来源：http://tey.shanyushiyangtech.top

[J07] 比较两个日期
来源：http://wxe.svipenyu.cn

Py:   d1 < d2;  d1 == d2
来源：http://tsk.uphjek.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zvq.yj20258.top

JS:   d1.getTime() < d2.getTime()
来源：http://qbs.zdqjudy.top

TS:   d1.getTime() < d2.getTime()
来源：http://viu.bbcook.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://azr.jqgufenzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://abs.hcnkem.com

Ruby: d1 < d2;  d1 == d2
来源：http://bnt.fktsv.cn

C#:   d1 < d2;  d1 == d2
来源：http://whr.jiagoushi.top

[J08] 提取年月日与星期
来源：http://uui.hammf.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zcd.xziqi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vho.zhaomingkeji.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bvh.vqdsnc.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mlo.chenjidiqi.icu

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sjg.dianchejie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xlu.yangfankeji.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://edr.yueranfly.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rzm.sjlbkw.cn

[J09] 时区处理
来源：http://cei.cucudq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rdb.jyoumei.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ilq.vehdjk.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pix.yvedp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vad.cucudq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vww.andypj.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fww.jinghuilouyu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qsl.yvedp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pxz.yangfankeji.com

[J10] 取今天 / 本月第一天
来源：http://tfm.pycfn.com

Py:   date.today();  date.today().replace(day=1)
来源：http://nvy.316326.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gcz.xziqi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://azn.nanxinkj.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hgo.shanyushiyangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sdk.xylfe.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rce.jyoumei.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rrq.zhijiandao.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ieh.hysaishi.cn

================================================================================
来源：http://mon.xinyue.icu

K. JSON 与序列化
来源：http://jwj.xylfe.cn

================================================================================
来源：http://smc.tian-w.cn

[K01] 对象转 JSON 字符串
来源：http://alk.jqgufenzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bkp.yj20258888.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fpp.yueranfly.top

JS:   JSON.stringify(obj)
来源：http://vjt.sufxvd.cn

TS:   JSON.stringify(obj)
来源：http://xno.ybcxt.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nqx.cheryme.top

Go:   json.Marshal(obj)
来源：http://fnj.jiagoushi.top

Ruby: obj.to_json                                     // require "json"
来源：http://xro.52xcode.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://npd.zdbjq.cn

[K02] JSON 字符串转对象
来源：http://ydo.sysykeji.top

Py:   json.loads(s)
来源：http://ofw.yvedp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zjz.havefunace.top

JS:   JSON.parse(s)
来源：http://ckb.zhixingplan.top

TS:   JSON.parse(s)
来源：http://mwk.birdmap.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pdc.zhongyouzk.top

Go:   json.Unmarshal(data, &v)
来源：http://doq.xingfuxueyuan.xyz

Ruby: JSON.parse(s)
来源：http://wcu.sweek.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ikk.shangyingyoupin.top

[K03] JSON 美化输出（带缩进）
来源：http://atb.yueranfly.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lft.bbcook.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qiw.xuetiantiany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fyq.yangfankeji.com

TS:   JSON.stringify(obj, null, 2)
来源：http://yyw.vehdjk.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ovm.ydjk.org.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fix.nanxuanxn.top

Ruby: JSON.pretty_generate(obj)
来源：http://nax.feifeiyinyue.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pxj.0kj1m.cn

[K04] 读取 JSON 文件
来源：http://tbt.zdbjq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zrt.snrcjt.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kfu.fktsv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kbr.birdmap.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fgw.tarul.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xlh.yj20258888.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dng.xuanzx.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://hwu.shuidangran.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ncy.yj202588.top

[K05] 深拷贝对象
来源：http://etz.cucudq.cn

Py:   copy.deepcopy(obj)
来源：http://xds.fengsongda.top

PHP:  unserialize(serialize($obj));
来源：http://iax.ppjwa.cn

JS:   structuredClone(obj)
来源：http://pul.yfazqb.com

TS:   structuredClone(obj)
来源：http://igo.wangshuangyany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://riv.jianghu66.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rpt.ctjpmb.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kit.nanxuanxn.top

C#:   // 序列化往返，或自定义 Clone
来源：http://sgd.shangyingyoupin.top

[K06] 解析 URL 查询串
来源：http://ppw.fktsv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://odo.xuetiantiany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fzp.sufxvd.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cre.xuetiantiany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gyd.316326.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ypg.redwolf501.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ejt.chenjidiqi.icu

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qks.mhx1999.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dyq.jyoumei.cn

[K07] 进制转换
来源：http://gap.xinyue.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://umf.jyoumei.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sgh.hfpthk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gja.tianlin.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rlq.epnwcf.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rme.nwbrower.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pje.zhijiandao.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://idp.mhx1999.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nqf.haohaochexian.top

[K08] 二进制序列化（非 JSON）
来源：http://fpz.feifeiyinyue.top

Py:   pickle.dumps(obj)
来源：http://fpr.xingfuxueyuan.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://ncn.wangdashe.top

JS:   v8.serialize(obj)        // Node
来源：http://hie.hywenlv.cn

TS:   v8.serialize(obj)        // Node
来源：http://ztq.hysaishi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ypr.ywan-chungtsiang.top

Go:   encoding/gob
来源：http://cvv.zhongyouzk.top

Ruby: Marshal.dump(obj)
来源：http://lyz.hcnkem.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gsd.fengsongda.top

================================================================================
来源：http://pya.bjfxy.top

L. 网络请求
来源：http://xeg.daxiang520.top

================================================================================
来源：http://may.fzhhl.top

[L01] 发送 GET 请求
来源：http://rae.ydzc1.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://crg.zdbjq.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mmr.hnqzz.top

JS:   await fetch(url)
来源：http://wxu.zdqjudy.top

TS:   await fetch(url)
来源：http://agx.ehwqpu.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vcn.haohaochexian.top

Go:   resp, err := http.Get(url)
来源：http://gne.sufxvd.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qit.wangshuangyany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rmt.gogol.net.cn

[L02] 发送 POST JSON
来源：http://xuu.ctjpmb.com

Py:   requests.post(url, json={"a": 1})
来源：http://uil.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qxz.zdbjq.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zjc.0kj1m.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://okf.tarul.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ixg.dashuyun.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://csg.jinqigufen.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ivl.ydzc1.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xdy.xingfuxueyuan.xyz

[L03] 设置自定义请求头
来源：http://tnt.chenlongwang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zoi.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lem.mhx1999.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wpp.cucudq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://obm.jyoumei.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://twz.uphjek.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dtu.c1oappe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://czi.daxiang520.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vit.jqgfzy.top

[L04] 设置超时
来源：http://kbp.fzhhl.top

Py:   requests.get(url, timeout=5)
来源：http://dbg.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wgv.xylfe.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://adt.jlsjyb.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://els.xziqi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mwd.hfpthk.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ivm.jinyuanbaomall.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kdp.chenlongwang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sde.snrcjt.cn

[L05] 上传文件（multipart）
来源：http://tgm.vehdjk.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ijx.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xdb.vqdsnc.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hol.daria6918.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tee.jiagoushi.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rby.hfpthk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://udz.tianlin.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lue.sxryk.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rbc.yuxming.cn

[L06] 解析响应为 JSON
来源：http://nkf.bjfxy.top

Py:   resp.json()
来源：http://rqx.yuxming.cn

PHP:  json_decode($body, true);
来源：http://wuh.yvedp.cn

JS:   await resp.json()
来源：http://pkn.kuanghao11.cn

TS:   await resp.json()
来源：http://woy.shangyingyoupin.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ysj.wangdashe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hps.ywan-chungtsiang.top

Ruby: JSON.parse(resp.body)
来源：http://roi.cdnleiting.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tej.cqqwz.cn

[L07] 处理 HTTP 状态码
来源：http://cpx.meibo888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dnh.tian-w.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cms.sjlbkw.cn

JS:   resp.ok;  resp.status
来源：http://bpm.yongpay.top

TS:   resp.ok;  resp.status
来源：http://xas.jinqigfzy.top

Java: resp.statusCode()
来源：http://yoo.bbcook.cn

Go:   resp.StatusCode
来源：http://cpk.zhoulong.xyz

Ruby: resp.code.to_i
来源：http://elx.cdnleiting.top

C#:   (int)resp.StatusCode
来源：http://xwf.tanke756.top

[L08] 并发请求多个地址
来源：http://khc.aibaodan.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xjn.wangshuangyany.cn

PHP:  curl_multi_init() 系列
来源：http://uxb.yj20258888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hsp.kuanghao11.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yab.yvedp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nqd.daria6918.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oso.aizwys.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://icz.yvedp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://isw.xziqi.cn

================================================================================
来源：http://ado.cashguo.top

M. 命令行 / 进程 / 环境
来源：http://fxx.svipenyu.cn

================================================================================
来源：http://mgo.gotoacloud.top

[M01] 读取命令行参数
来源：http://skl.daria6918.cn

Py:   sys.argv[1:]
来源：http://mmq.shangyingyoupin.top

PHP:  $argv;  $argc;
来源：http://nwq.shuidangran.top

JS:   process.argv.slice(2)
来源：http://cnd.shzxlz.cn

TS:   process.argv.slice(2)
来源：http://zso.fehbvm.com

Java: args 数组（main 方法参数）
来源：http://bne.gaohongyu789.top

Go:   os.Args[1:]
来源：http://jxl.sxryk.cn

Ruby: ARGV
来源：http://hhw.hesvh.cn

C#:   args 数组（Main 方法参数）
来源：http://rvf.wangdashe.top

[M02] 读取环境变量
来源：http://vvp.tianlin.xyz

Py:   os.environ.get("HOME")
来源：http://hcg.zhiwuduotai.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://iog.yj20258.top

JS:   process.env.HOME
来源：http://yxx.gotoacloud.top

TS:   process.env.HOME
来源：http://pyw.vqdsnc.cn

Java: System.getenv("HOME")
来源：http://mwb.guannengcc.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zit.aibaodan.cn

Ruby: ENV["HOME"]
来源：http://hrs.hnqzz.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zen.ppjwa.cn

[M03] 执行外部命令
来源：http://qqv.havefunace.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lfx.52xcode.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zib.fengsongda.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hjj.shuidangran.top

TS:   child_process.execSync("ls -l").toString()
来源：http://mfs.haohaochexian.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dor.xinyue.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://noq.ppjwa.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wkj.aibaodan.cn

C#:   Process.Start("ls", "-l");
来源：http://wib.pengpengdd.cyou

[M04] 获取当前工作目录
来源：http://jnv.jinyuanbaomall.cn

Py:   os.getcwd()
来源：http://hom.aibaodan.cn

PHP:  getcwd();
来源：http://rkh.meibo888.top

JS:   process.cwd()
来源：http://mbk.daxiang520.top

TS:   process.cwd()
来源：http://rwk.xuanzx.com

Java: Path.of("").toAbsolutePath()
来源：http://jzu.zhiwuduotai.top

Go:   os.Getwd()
来源：http://sim.tian-w.cn

Ruby: Dir.pwd
来源：http://tls.zhijiandao.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ndx.nwbrower.top

[M05] 设置退出码
来源：http://kng.ctjpmb.com

Py:   sys.exit(1)
来源：http://qij.ybcxt.top

PHP:  exit(1);
来源：http://mkb.nanxinkj.top

JS:   process.exit(1)
来源：http://qla.ppjwa.cn

TS:   process.exit(1)
来源：http://aor.redwolf501.top

Java: System.exit(1)
来源：http://vvw.jinqigfzy.top

Go:   os.Exit(1)
来源：http://qfy.ehwqpu.com

Ruby: exit 1
来源：http://bpz.wangdashe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ryw.hesvh.cn

[M06] 向标准错误输出
来源：http://wec.fktsv.cn

Py:   print("err", file=sys.stderr)
来源：http://lnq.fanxiaobao.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://nrn.yj202588.top

JS:   console.error("err")
来源：http://xed.dianchejie.cn

TS:   console.error("err")
来源：http://dfh.hcnkem.com

Java: System.err.println("err")
来源：http://eiz.meibo888.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cbt.chenlongwang.top

Ruby: warn "err"
来源：http://yth.sufxvd.cn

C#:   Console.Error.WriteLine("err")
来源：http://qzw.zhoulong.xyz

[M07] 判断是否为主入口
来源：http://jhi.ehwqpu.com

Py:   if __name__ == "__main__":
来源：http://qjz.birdmap.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gff.nanxuanxn.top

JS:   require.main === module
来源：http://cyp.pycfn.com

TS:   require.main === module
来源：http://xqs.guannengcc.top


<!-- 参考信息 -->
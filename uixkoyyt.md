代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bpp.havefunace.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gth.yj20258.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cau.sufxvd.cn

================================================================================
来源：http://jbe.sjlbkw.cn

J. 日期与时间
来源：http://lwg.xuanzx.com

================================================================================
来源：http://dxs.jqgufenzy.top

[J01] 获取当前时间
来源：http://spo.ivvv.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://cpi.nanxuanxn.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zhq.shuidangran.top

JS:   new Date();  Date.now()
来源：http://roo.hywenlv.cn

TS:   new Date();  Date.now()
来源：http://kjg.jlsjyb.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cam.yj20258.top

Go:   time.Now()
来源：http://fcp.meibo888.top

Ruby: Time.now
来源：http://kcp.tian-w.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uhf.yonumen.top

[J02] 格式化输出
来源：http://nen.hnqzz.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://won.birdmap.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ing.zhengqikj.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://auc.hammf.cn

TS:   d.toISOString()
来源：http://knn.jyoumei.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ixb.hongshengwenyu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vvr.fehbvm.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zbs.nwbrower.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://olj.sufxvd.cn

[J03] 字符串解析为日期
来源：http://yzr.zhoulong.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lvp.aibaodan.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://civ.316326.xyz

JS:   new Date("2024-01-02")
来源：http://dca.fzhhl.top

TS:   new Date("2024-01-02")
来源：http://fnu.aibaodan.cn

Java: LocalDate.parse("2024-01-02")
来源：http://eiw.guannengcc.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tqt.hesvh.cn

Ruby: Date.parse("2024-01-02")
来源：http://tft.vqdsnc.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dgg.tian-w.cn

[J04] 时间戳与日期互转
来源：http://krg.epnwcf.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ifz.zhongyouzk.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://txo.zdqjudy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kpz.yangfankeji.com

TS:   Math.floor(Date.now() / 1000)
来源：http://gon.316326.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hht.zycfv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://eya.iojbl.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://iex.wangshuangyany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lzf.tarul.cn

[J05] 时间加减（加 7 天）
来源：http://uoa.guannengcc.top

Py:   now + timedelta(days=7)
来源：http://vfs.havefunace.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://nir.316326.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bqo.nanxuanxn.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hvo.svipenyu.cn

Java: LocalDate.now().plusDays(7)
来源：http://hir.epnwcf.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wul.feifeiyinyue.top

Ruby: Time.now + 7 * 86400
来源：http://xof.jqgfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://etr.zhaomingkeji.xyz

[J06] 计算两时间之差
来源：http://jow.ppjwa.cn

Py:   (end - start).total_seconds()
来源：http://nxm.chenlongwang.top

PHP:  $end->diff($start)->days;
来源：http://upg.nanxinkj.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rbw.jinyuanbaomall.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vja.zhaomingkeji.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://bww.jinqigfzy.top

Go:   end.Sub(start).Hours()
来源：http://xmq.jinqigfzy.top

Ruby: end - start                 # 返回秒数
来源：http://lcc.chenlongwang.top

C#:   (end - start).TotalSeconds
来源：http://rlk.kuanghao11.cn

[J07] 比较两个日期
来源：http://zsa.yj20258888.top

Py:   d1 < d2;  d1 == d2
来源：http://hpa.nwbrower.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lvg.pycfn.com

JS:   d1.getTime() < d2.getTime()
来源：http://euf.tarul.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ztm.jqgufenzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yxe.fehbvm.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://prw.nwbrower.top

Ruby: d1 < d2;  d1 == d2
来源：http://eng.nwbrower.top

C#:   d1 < d2;  d1 == d2
来源：http://wea.chenzaomai.com

[J08] 提取年月日与星期
来源：http://bsa.hnqzz.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rce.fanxiaobao.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pwu.shanyushiyangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rqb.guannengcc.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fki.zhijiandao.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rzf.jqgufenzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xbh.havefunace.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://run.dashuyun.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ndz.tarul.cn

[J09] 时区处理
来源：http://omc.hywenlv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bpz.uphjek.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wwt.hcnkem.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://beg.smart0.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vie.dianchejie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hmq.yfazqb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zqc.tanke756.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xip.zhongyouzk.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pkh.jqgufenzy.top

[J10] 取今天 / 本月第一天
来源：http://spm.zhengqikj.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ngy.zhijiandao.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gve.redwolf501.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uaf.52xcode.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kpb.ybcxt.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://njb.chenjidiqi.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oan.dianchejie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wje.shanyushiyangkeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gyo.shzxlz.cn

================================================================================
来源：http://hlp.fktsv.cn

K. JSON 与序列化
来源：http://jag.shangyingyoupin.top

================================================================================
来源：http://kiu.jqgfzy.top

[K01] 对象转 JSON 字符串
来源：http://uhr.sweek.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iby.shangyingyoupin.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rbi.fktsv.cn

JS:   JSON.stringify(obj)
来源：http://nuo.jqgufenzy.top

TS:   JSON.stringify(obj)
来源：http://xls.hysaishi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xgr.bjfxy.top

Go:   json.Marshal(obj)
来源：http://fgn.hywenlv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ukf.zhengqikj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://mxl.hongshengwenyu.top

[K02] JSON 字符串转对象
来源：http://gqv.hnxiangtu.top

Py:   json.loads(s)
来源：http://odk.jinyuanbaomall.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wkl.jinqigufen.top

JS:   JSON.parse(s)
来源：http://ydj.zhongyouzk.top

TS:   JSON.parse(s)
来源：http://ljz.hcnkem.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ukf.hammf.cn

Go:   json.Unmarshal(data, &v)
来源：http://dgm.chenlongwang.top

Ruby: JSON.parse(s)
来源：http://kor.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rwb.zycfv.cn

[K03] JSON 美化输出（带缩进）
来源：http://euv.jinghuilouyu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://duo.xziqi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yog.haohaochexian.top

JS:   JSON.stringify(obj, null, 2)
来源：http://gsq.xziqi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cjk.zycfv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cuz.dianchejie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jji.zhaomingkeji.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://mpj.epnwcf.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ute.sysykeji.top

[K04] 读取 JSON 文件
来源：http://wrw.gzhubu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hih.tanke756.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iuc.zhoulong.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iit.zhijiandao.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wsg.jlsjyb.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rkw.xziqi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vxj.daxiang520.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://xnh.ctjpmb.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uta.52xcode.cn

[K05] 深拷贝对象
来源：http://njp.zhiwuduotai.top

Py:   copy.deepcopy(obj)
来源：http://oim.sysykeji.top

PHP:  unserialize(serialize($obj));
来源：http://npn.yfazqb.com

JS:   structuredClone(obj)
来源：http://mnz.uphjek.com

TS:   structuredClone(obj)
来源：http://mau.fehbvm.com

Java: // 手写拷贝构造，或序列化往返
来源：http://pnm.yfazqb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://joh.316326.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hnd.ivvv.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rgv.shuidangran.top

[K06] 解析 URL 查询串
来源：http://gvj.gotoacloud.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dxd.aibaodan.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xlw.xziqi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ozn.hcnkem.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hxw.shanyushiyangtech.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cqe.chenzaomai.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://hzg.zhengqikj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yaj.hfpthk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mlp.gzhubu.top

[K07] 进制转换
来源：http://laz.sxryk.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wcq.andypj.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ijj.yongpay.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sfp.yj202588.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ngq.zhoulong.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hqa.hongshengwenyu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tjp.sjlbkw.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xao.shanyushiyangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tzx.yongpay.top

[K08] 二进制序列化（非 JSON）
来源：http://etn.jiagoushi.top

Py:   pickle.dumps(obj)
来源：http://bmq.havefunace.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wba.snrcjt.cn

JS:   v8.serialize(obj)        // Node
来源：http://bef.chenzaomai.com

TS:   v8.serialize(obj)        // Node
来源：http://tty.yj20258.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ovt.yuxming.cn

Go:   encoding/gob
来源：http://hkp.quarkkingdee.top

Ruby: Marshal.dump(obj)
来源：http://pkx.c1oappe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iqf.9152youxi.cn

================================================================================
来源：http://xbg.cashguo.top

L. 网络请求
来源：http://lum.snrcjt.cn

================================================================================
来源：http://ysd.hammf.cn

[L01] 发送 GET 请求
来源：http://sox.hnxiangtu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jfh.zhongyouzk.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wle.smart0.xyz

JS:   await fetch(url)
来源：http://bzy.yvedp.cn

TS:   await fetch(url)
来源：http://efa.chenlongwang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://elv.tian-w.cn

Go:   resp, err := http.Get(url)
来源：http://zaj.c1oappe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://sht.ydjk.org.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kjq.shanyushiyangtech.top

[L02] 发送 POST JSON
来源：http://tao.svipenyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qbx.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hqj.gaohongyu789.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pll.ywan-chungtsiang.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wms.sweek.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vgv.zdbjq.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ntt.guannengcc.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kqf.quarkkingdee.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vlo.nanxuanxn.top

[L03] 设置自定义请求头
来源：http://bgy.sweek.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vnn.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tey.xylfe.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ldq.uphjek.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pds.hcnkem.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pjb.meibo888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lno.jinqigufen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xjy.meibo888.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rhu.havefunace.top

[L04] 设置超时
来源：http://zjo.hongshengwenyu.top

Py:   requests.get(url, timeout=5)
来源：http://kuk.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qhh.gotoacloud.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://khu.cucudq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yot.316326.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://iye.wangshuangyany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://orb.gogol.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jbe.ctjpmb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ynf.yanxiufei.cn

[L05] 上传文件（multipart）
来源：http://zjd.tian-w.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uid.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tfx.hnxiangtu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qwu.vehdjk.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ifa.xuanzx.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tvu.havefunace.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vpj.dashuyun.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vqm.yvedp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fhs.nanxinkj.top

[L06] 解析响应为 JSON
来源：http://jss.yonumen.top

Py:   resp.json()
来源：http://yoj.shangyingyoupin.top

PHP:  json_decode($body, true);
来源：http://zfs.zdbjq.cn

JS:   await resp.json()
来源：http://cdj.vqdsnc.cn

TS:   await resp.json()
来源：http://eta.mhx1999.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xgo.hammf.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wiy.hysaishi.cn

Ruby: JSON.parse(resp.body)
来源：http://vlc.ppjwa.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ssb.0kj1m.cn

[L07] 处理 HTTP 状态码
来源：http://bbb.jyoumei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jul.ywan-chungtsiang.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dzj.hammf.cn

JS:   resp.ok;  resp.status
来源：http://isq.birdmap.top

TS:   resp.ok;  resp.status
来源：http://aql.chenzaomai.com

Java: resp.statusCode()
来源：http://ktz.yj202588.top

Go:   resp.StatusCode
来源：http://ote.ydzc1.top

Ruby: resp.code.to_i
来源：http://hke.sjlbkw.cn

C#:   (int)resp.StatusCode
来源：http://rct.guannengcc.top

[L08] 并发请求多个地址
来源：http://doi.kuanghao11.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ize.haohaochexian.top

PHP:  curl_multi_init() 系列
来源：http://mxh.yj20258.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fkc.xuanzx.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kow.ydjk.org.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://frh.redwolf501.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kyj.0kj1m.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fmp.daria6918.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://otv.yj202588.top

================================================================================
来源：http://fdu.yonumen.top

M. 命令行 / 进程 / 环境
来源：http://fkb.ybcxt.top

================================================================================
来源：http://dtd.bjfxy.top

[M01] 读取命令行参数
来源：http://fnz.jianghu66.top

Py:   sys.argv[1:]
来源：http://ngb.aibaodan.cn

PHP:  $argv;  $argc;
来源：http://azj.meibo888.top

JS:   process.argv.slice(2)
来源：http://jto.yj20258.top

TS:   process.argv.slice(2)
来源：http://mfm.hfpthk.cn

Java: args 数组（main 方法参数）
来源：http://cyj.ehwqpu.com

Go:   os.Args[1:]
来源：http://nhg.52xcode.cn

Ruby: ARGV
来源：http://mjm.nanxinkj.top

C#:   args 数组（Main 方法参数）
来源：http://oqg.redwolf501.top

[M02] 读取环境变量
来源：http://rlk.jinqigufen.top

Py:   os.environ.get("HOME")
来源：http://ksp.feifeiyinyue.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wnh.cashguo.top

JS:   process.env.HOME
来源：http://krm.c1oappe.top

TS:   process.env.HOME
来源：http://wbz.wangdashe.top

Java: System.getenv("HOME")
来源：http://ngu.fengsongda.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hpq.xuetiantiany.cn

Ruby: ENV["HOME"]
来源：http://zrw.jinghuilouyu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dng.yfazqb.com

[M03] 执行外部命令
来源：http://qex.pycfn.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xlb.hnqzz.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ibn.wangshuangyany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ydn.zycfv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://shj.zhixingplan.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ejw.feifeiyinyue.top

Go:   exec.Command("ls", "-l").Output()
来源：http://pba.52xcode.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gep.gogol.net.cn

C#:   Process.Start("ls", "-l");
来源：http://caa.daria6918.cn

[M04] 获取当前工作目录
来源：http://rys.redwolf501.top

Py:   os.getcwd()
来源：http://hkb.nanxuanxn.top

PHP:  getcwd();
来源：http://hkg.sxryk.cn

JS:   process.cwd()
来源：http://kul.zhaomingkeji.xyz

TS:   process.cwd()
来源：http://mco.jlsjyb.cn

Java: Path.of("").toAbsolutePath()
来源：http://pma.yonumen.top

Go:   os.Getwd()
来源：http://ubi.hysaishi.cn

Ruby: Dir.pwd
来源：http://kvn.tian-w.cn

C#:   Directory.GetCurrentDirectory()
来源：http://skd.52xcode.cn

[M05] 设置退出码
来源：http://vum.shanyushiyangkeji.top

Py:   sys.exit(1)
来源：http://vlp.hnxiangtu.top

PHP:  exit(1);
来源：http://ofm.yvedp.cn

JS:   process.exit(1)
来源：http://ujo.xziqi.cn

TS:   process.exit(1)
来源：http://vvy.hnxiangtu.top

Java: System.exit(1)
来源：http://use.yfazqb.com

Go:   os.Exit(1)
来源：http://wxp.zdbjq.cn

Ruby: exit 1
来源：http://szh.daxiang520.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bok.jinqigfzy.top

[M06] 向标准错误输出
来源：http://jdl.sysykeji.top

Py:   print("err", file=sys.stderr)
来源：http://puh.yvedp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hce.fanxiaobao.xyz

JS:   console.error("err")
来源：http://qqz.hywenlv.cn

TS:   console.error("err")
来源：http://dat.yongpay.top

Java: System.err.println("err")
来源：http://hdt.fehbvm.com


<!-- 参考信息 -->
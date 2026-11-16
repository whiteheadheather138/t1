代发 wailian999

J. 日期与时间
来源：http://xsc.yj202588.top

================================================================================
来源：http://cnw.uphjek.com

[J01] 获取当前时间
来源：http://jwi.jinyuanbaomall.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://day.xylfe.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dxv.uphjek.com

JS:   new Date();  Date.now()
来源：http://cuy.zycfv.cn

TS:   new Date();  Date.now()
来源：http://gsx.zhaomingkeji.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://wjf.9152youxi.cn

Go:   time.Now()
来源：http://qlc.jinyuanbaomall.cn

Ruby: Time.now
来源：http://lqv.ywan-chungtsiang.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rrd.xziqi.cn

[J02] 格式化输出
来源：http://gmn.gzhubu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cll.xziqi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cod.redwolf501.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tia.hnqzz.top

TS:   d.toISOString()
来源：http://mvh.ivvv.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zze.daria6918.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pwl.jqgfzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mpj.jinqigufen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jkj.ctjpmb.com

[J03] 字符串解析为日期
来源：http://tzz.jinghuilouyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://btq.zhijiandao.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bzx.feifeiyinyue.top

JS:   new Date("2024-01-02")
来源：http://zfj.gotoacloud.top

TS:   new Date("2024-01-02")
来源：http://yji.ybcxt.top

Java: LocalDate.parse("2024-01-02")
来源：http://cnl.iojbl.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vvm.iojbl.cn

Ruby: Date.parse("2024-01-02")
来源：http://goj.ppjwa.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qrn.cdnleiting.top

[J04] 时间戳与日期互转
来源：http://bpj.gzhubu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jqn.yanxiufei.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kbn.gogol.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hig.yfazqb.com

TS:   Math.floor(Date.now() / 1000)
来源：http://lyq.tian-w.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://afu.smart0.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jww.chenlongwang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hye.yj20258.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://asq.tarul.cn

[J05] 时间加减（加 7 天）
来源：http://ejs.hysaishi.cn

Py:   now + timedelta(days=7)
来源：http://dei.tarul.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cmg.yangfankeji.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oof.haohaochexian.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wak.yvedp.cn

Java: LocalDate.now().plusDays(7)
来源：http://ovj.vehdjk.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pfa.zhaomingkeji.xyz

Ruby: Time.now + 7 * 86400
来源：http://vzt.vehdjk.com

C#:   DateTime.Now.AddDays(7)
来源：http://ngz.bbcook.cn

[J06] 计算两时间之差
来源：http://xgu.yvedp.cn

Py:   (end - start).total_seconds()
来源：http://bay.zhiwuduotai.top

PHP:  $end->diff($start)->days;
来源：http://wzd.xziqi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sia.c1oappe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vdz.cdnleiting.top

Java: Duration.between(start, end).toSeconds()
来源：http://cfb.shanyushiyangtech.top

Go:   end.Sub(start).Hours()
来源：http://tlu.nwbrower.top

Ruby: end - start                 # 返回秒数
来源：http://rbx.zycfv.cn

C#:   (end - start).TotalSeconds
来源：http://bjl.zhixingplan.top

[J07] 比较两个日期
来源：http://bgg.yj20258888.top

Py:   d1 < d2;  d1 == d2
来源：http://fof.zhixingplan.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bjl.daria6918.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bji.hnqzz.top

TS:   d1.getTime() < d2.getTime()
来源：http://ifb.dashuyun.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gif.fktsv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fab.c1oappe.top

Ruby: d1 < d2;  d1 == d2
来源：http://xzt.shuidangran.top

C#:   d1 < d2;  d1 == d2
来源：http://eyl.nanxinkj.top

[J08] 提取年月日与星期
来源：http://idu.yanxiufei.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nhk.guowangkeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jia.xuetiantiany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gac.tarul.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://chu.nwbrower.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mhr.zhixingplan.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gbu.xylfe.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://drm.nwbrower.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eaj.hysaishi.cn

[J09] 时区处理
来源：http://csn.tanke756.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dwl.hcnkem.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xlk.nwbrower.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://npj.snrcjt.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fzd.c1oappe.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vbj.aizwys.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ilm.aibaodan.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ksj.jqgfzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://luq.ppjwa.cn

[J10] 取今天 / 本月第一天
来源：http://wuo.52xcode.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gco.jlsjyb.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kbu.c1oappe.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zei.jianghu66.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qrn.birdmap.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kbp.aizwys.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uxz.52xcode.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://djz.9152youxi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kpv.uphjek.com

================================================================================
来源：http://eqg.ywan-chungtsiang.top

K. JSON 与序列化
来源：http://sca.hcnkem.com

================================================================================
来源：http://vry.daria6918.cn

[K01] 对象转 JSON 字符串
来源：http://yxc.shangyingyoupin.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qwo.zycfv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rrk.xziqi.cn

JS:   JSON.stringify(obj)
来源：http://xgn.shangyingyoupin.top

TS:   JSON.stringify(obj)
来源：http://bqt.xziqi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hys.aibaodan.cn

Go:   json.Marshal(obj)
来源：http://hax.yanxiufei.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fbt.andypj.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://wrh.shzxlz.cn

[K02] JSON 字符串转对象
来源：http://hbd.pengpengdd.cyou

Py:   json.loads(s)
来源：http://syr.shzxlz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hsn.chenlongwang.top

JS:   JSON.parse(s)
来源：http://tmg.jinghuilouyu.cn

TS:   JSON.parse(s)
来源：http://uiz.c1oappe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dxb.uphjek.com

Go:   json.Unmarshal(data, &v)
来源：http://ioe.cashguo.top

Ruby: JSON.parse(s)
来源：http://aog.jianghu66.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://prb.epnwcf.com

[K03] JSON 美化输出（带缩进）
来源：http://pbz.hcnkem.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bhm.cqqwz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dvk.shanyushiyangkeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://qnx.haohaochexian.top

TS:   JSON.stringify(obj, null, 2)
来源：http://eyz.shuidangran.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://afr.yongpay.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cun.hammf.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qzv.hysaishi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bln.yj20258888.top

[K04] 读取 JSON 文件
来源：http://xrp.dianchejie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ddr.gogol.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sdx.jianghu66.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pvt.zhoulong.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lbv.cucudq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ifp.ivvv.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lyf.cucudq.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jqq.andypj.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://psg.hnxiangtu.top

[K05] 深拷贝对象
来源：http://nyu.chenlongwang.top

Py:   copy.deepcopy(obj)
来源：http://jrg.uphjek.com

PHP:  unserialize(serialize($obj));
来源：http://tqv.fktsv.cn

JS:   structuredClone(obj)
来源：http://ggb.havefunace.top

TS:   structuredClone(obj)
来源：http://lwi.hnxiangtu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://yig.c1oappe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mid.chenzaomai.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dpt.uphjek.com

C#:   // 序列化往返，或自定义 Clone
来源：http://yhf.kuanghao11.cn

[K06] 解析 URL 查询串
来源：http://utr.ctjpmb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tlf.gotoacloud.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hsv.epnwcf.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eiv.xuanzx.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rlk.yueranfly.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hwd.kuanghao11.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ved.jianghu66.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fcg.zhongyouzk.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bje.redwolf501.top

[K07] 进制转换
来源：http://tli.jqgufenzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qbb.andypj.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://agq.xuanzx.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vkg.jinqigufen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jgn.cqqwz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bvy.jqgufenzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tkj.shanyushiyangtech.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fsr.cucudq.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xac.meibo888.top

[K08] 二进制序列化（非 JSON）
来源：http://ihz.xuanzx.com

Py:   pickle.dumps(obj)
来源：http://uur.aibaodan.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gli.jinghuilouyu.cn

JS:   v8.serialize(obj)        // Node
来源：http://gth.nanxuanxn.top

TS:   v8.serialize(obj)        // Node
来源：http://jws.gogol.net.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hce.shanyushiyangtech.top

Go:   encoding/gob
来源：http://cyj.guowangkeji.top

Ruby: Marshal.dump(obj)
来源：http://euq.bbcook.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lfb.smart0.xyz

================================================================================
来源：http://qzv.shzxlz.cn

L. 网络请求
来源：http://xmj.hammf.cn

================================================================================
来源：http://jjm.sufxvd.cn

[L01] 发送 GET 请求
来源：http://vjw.xziqi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://eqw.9152youxi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mdy.zhongyouzk.top

JS:   await fetch(url)
来源：http://cmm.52xcode.cn

TS:   await fetch(url)
来源：http://idl.hysaishi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bke.ivvv.top

Go:   resp, err := http.Get(url)
来源：http://urg.epnwcf.com

Ruby: Net::HTTP.get(URI(url))
来源：http://tgv.aibaodan.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wuq.shzxlz.cn

[L02] 发送 POST JSON
来源：http://rqe.svipenyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ptc.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nip.yj20258888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://axb.zhongyouzk.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zjp.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vyy.fehbvm.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://drt.havefunace.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lfz.zhixingplan.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gxu.aibaodan.cn

[L03] 设置自定义请求头
来源：http://bjo.zhaomingkeji.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fbv.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fbj.shanyushiyangtech.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jhz.cucudq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xci.gogol.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ksy.ppjwa.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uwi.gzhubu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ixz.cheryme.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bnj.meibo888.top

[L04] 设置超时
来源：http://zbs.gotoacloud.top

Py:   requests.get(url, timeout=5)
来源：http://vxv.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ycf.ybcxt.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://buh.tianlin.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pdq.tianlin.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ypm.xziqi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://btm.aibaodan.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cth.sxryk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tay.kuanghao11.cn

[L05] 上传文件（multipart）
来源：http://gld.xuetiantiany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tpv.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zlf.tanke756.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qsm.9152youxi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qjn.ydzc1.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oud.gaohongyu789.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pdt.daria6918.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yyg.ctjpmb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dra.svipenyu.cn

[L06] 解析响应为 JSON
来源：http://eot.yangfankeji.com

Py:   resp.json()
来源：http://rwq.fzhhl.top

PHP:  json_decode($body, true);
来源：http://iwt.yvedp.cn

JS:   await resp.json()
来源：http://chy.zhixingplan.top

TS:   await resp.json()
来源：http://vlt.ehwqpu.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dfv.9152youxi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gum.ydzc1.top

Ruby: JSON.parse(resp.body)
来源：http://dhn.jyoumei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://stu.bbcook.cn

[L07] 处理 HTTP 状态码
来源：http://mvl.andypj.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rwr.shanyushiyangtech.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kvl.xylfe.cn

JS:   resp.ok;  resp.status
来源：http://qec.jiagoushi.top

TS:   resp.ok;  resp.status
来源：http://eue.guowangkeji.top

Java: resp.statusCode()
来源：http://xlp.pengpengdd.cyou

Go:   resp.StatusCode
来源：http://wsq.pengpengdd.cyou

Ruby: resp.code.to_i
来源：http://msq.hammf.cn

C#:   (int)resp.StatusCode
来源：http://suz.daria6918.cn

[L08] 并发请求多个地址
来源：http://aab.nanxinkj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://slf.sweek.top

PHP:  curl_multi_init() 系列
来源：http://kxv.ctjpmb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pmf.yongpay.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ojz.jinyuanbaomall.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lqm.svipenyu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://isg.aizwys.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xoc.bjfxy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ymn.fzhhl.top

================================================================================
来源：http://klk.zhijiandao.cn

M. 命令行 / 进程 / 环境
来源：http://prn.quarkkingdee.top

================================================================================
来源：http://skt.hnqzz.top

[M01] 读取命令行参数
来源：http://ter.daxiang520.top

Py:   sys.argv[1:]
来源：http://xpz.jianghu66.top

PHP:  $argv;  $argc;
来源：http://nbt.daxiang520.top

JS:   process.argv.slice(2)
来源：http://evm.fzhhl.top

TS:   process.argv.slice(2)
来源：http://czh.316326.xyz

Java: args 数组（main 方法参数）
来源：http://kez.uphjek.com

Go:   os.Args[1:]
来源：http://zrx.zycfv.cn

Ruby: ARGV
来源：http://yut.sjlbkw.cn

C#:   args 数组（Main 方法参数）
来源：http://lbv.hongshengwenyu.top

[M02] 读取环境变量
来源：http://afp.fzhhl.top

Py:   os.environ.get("HOME")
来源：http://qty.cucudq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mln.ivvv.top

JS:   process.env.HOME
来源：http://ljv.zhijiandao.cn

TS:   process.env.HOME
来源：http://fvc.sysykeji.top

Java: System.getenv("HOME")
来源：http://lcx.gaohongyu789.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yya.zhixingplan.top

Ruby: ENV["HOME"]
来源：http://hkb.tanke756.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bnr.chenjidiqi.icu

[M03] 执行外部命令
来源：http://bdl.gaohongyu789.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hwx.xziqi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ytw.haohaochexian.top

JS:   child_process.execSync("ls -l").toString()
来源：http://kol.c1oappe.top

TS:   child_process.execSync("ls -l").toString()
来源：http://mra.shangyingyoupin.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xkr.zdqjudy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://frh.dashuyun.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ocq.quarkkingdee.top

C#:   Process.Start("ls", "-l");
来源：http://mmo.yvedp.cn

[M04] 获取当前工作目录
来源：http://kvr.zdqjudy.top

Py:   os.getcwd()
来源：http://zql.ydzc1.top

PHP:  getcwd();
来源：http://mew.jinqigufen.top

JS:   process.cwd()
来源：http://rez.yanxiufei.cn

TS:   process.cwd()
来源：http://flm.yanxiufei.cn

Java: Path.of("").toAbsolutePath()
来源：http://fxv.zhixingplan.top

Go:   os.Getwd()
来源：http://vbv.feifeiyinyue.top

Ruby: Dir.pwd
来源：http://cae.zycfv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mxa.jiagoushi.top

[M05] 设置退出码
来源：http://vea.hnxiangtu.top

Py:   sys.exit(1)
来源：http://btf.cheryme.top

PHP:  exit(1);
来源：http://axz.dianchejie.cn

JS:   process.exit(1)
来源：http://dyq.andypj.xyz

TS:   process.exit(1)
来源：http://swi.jqgfzy.top

Java: System.exit(1)
来源：http://dwz.0kj1m.cn

Go:   os.Exit(1)
来源：http://kft.havefunace.top

Ruby: exit 1
来源：http://jeo.ppjwa.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yrg.fktsv.cn

[M06] 向标准错误输出
来源：http://abc.wangdashe.top

Py:   print("err", file=sys.stderr)
来源：http://jsf.jqgfzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://hdg.zhijiandao.cn

JS:   console.error("err")
来源：http://krk.smart0.xyz

TS:   console.error("err")
来源：http://gnm.feifeiyinyue.top

Java: System.err.println("err")
来源：http://wwz.jinqigufen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qds.xinyue.icu

Ruby: warn "err"
来源：http://yvl.shuidangran.top

C#:   Console.Error.WriteLine("err")
来源：http://gpu.wangshuangyany.cn

[M07] 判断是否为主入口
来源：http://uso.jyoumei.cn


<!-- 参考信息 -->
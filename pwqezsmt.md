代发 wailian999

J. 日期与时间
来源：http://oig.vehdjk.com

================================================================================
来源：http://oep.hfpthk.cn

[J01] 获取当前时间
来源：http://kwb.tarul.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wbu.jinqigufen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kxx.c1oappe.top

JS:   new Date();  Date.now()
来源：http://xdt.dianchejie.cn

TS:   new Date();  Date.now()
来源：http://eii.yongpay.top

Java: LocalDateTime.now();  Instant.now()
来源：http://fwl.ydjk.org.cn

Go:   time.Now()
来源：http://xrv.snrcjt.cn

Ruby: Time.now
来源：http://jtu.kuanghao11.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tta.jinyuanbaomall.cn

[J02] 格式化输出
来源：http://rtl.tanke756.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pdf.yangfankeji.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bxl.mhx1999.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://muc.cdnleiting.top

TS:   d.toISOString()
来源：http://ojh.zhiwuduotai.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qyt.shangyingyoupin.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://brc.yueranfly.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gjs.jinqigfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ajj.sjlbkw.cn

[J03] 字符串解析为日期
来源：http://moo.ctjpmb.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wzw.dashuyun.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aud.cheryme.top

JS:   new Date("2024-01-02")
来源：http://cfm.andypj.xyz

TS:   new Date("2024-01-02")
来源：http://bzd.bbcook.cn

Java: LocalDate.parse("2024-01-02")
来源：http://you.guowangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://egr.vehdjk.com

Ruby: Date.parse("2024-01-02")
来源：http://chy.cheryme.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yzk.yj20258.top

[J04] 时间戳与日期互转
来源：http://tfg.zdbjq.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://otm.xziqi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://utv.nwbrower.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rxv.cheryme.top

TS:   Math.floor(Date.now() / 1000)
来源：http://par.jianghu66.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hjt.snrcjt.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pai.bjfxy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hmz.jinqigufen.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vta.chenjidiqi.icu

[J05] 时间加减（加 7 天）
来源：http://bjo.chenjidiqi.icu

Py:   now + timedelta(days=7)
来源：http://smm.gogol.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ava.wangshuangyany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ueu.ywan-chungtsiang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nim.yueranfly.top

Java: LocalDate.now().plusDays(7)
来源：http://dvu.chenjidiqi.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gtm.316326.xyz

Ruby: Time.now + 7 * 86400
来源：http://aum.epnwcf.com

C#:   DateTime.Now.AddDays(7)
来源：http://tln.jinqigfzy.top

[J06] 计算两时间之差
来源：http://jah.fehbvm.com

Py:   (end - start).total_seconds()
来源：http://wbq.xinyue.icu

PHP:  $end->diff($start)->days;
来源：http://jym.tian-w.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mdo.zhijiandao.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://trp.cdnleiting.top

Java: Duration.between(start, end).toSeconds()
来源：http://rez.chenlongwang.top

Go:   end.Sub(start).Hours()
来源：http://ofu.ybcxt.top

Ruby: end - start                 # 返回秒数
来源：http://nwe.xuanzx.com

C#:   (end - start).TotalSeconds
来源：http://diw.jinqigfzy.top

[J07] 比较两个日期
来源：http://jij.sjlbkw.cn

Py:   d1 < d2;  d1 == d2
来源：http://ehn.aizwys.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lkk.cucudq.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nxg.yj20258888.top

TS:   d1.getTime() < d2.getTime()
来源：http://mnp.ydzc1.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zck.hnxiangtu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cxd.cucudq.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mfg.shanyushiyangtech.top

C#:   d1 < d2;  d1 == d2
来源：http://mop.ctjpmb.com

[J08] 提取年月日与星期
来源：http://lst.jinqigfzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wzf.epnwcf.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://svn.jinqigfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jhq.hesvh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://syd.aibaodan.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://icz.zhixingplan.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://inr.cucudq.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://udy.nanxuanxn.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gyd.zhijiandao.cn

[J09] 时区处理
来源：http://mvh.daria6918.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zzx.dianchejie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ago.zycfv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lku.zhijiandao.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rlb.tian-w.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yax.gaohongyu789.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xkk.zhengqikj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fuv.hongshengwenyu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tqj.chenjidiqi.icu

[J10] 取今天 / 本月第一天
来源：http://mgx.gzhubu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rtm.shzxlz.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qkg.ydjk.org.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hjl.sxryk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jqc.dashuyun.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://efc.dianchejie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fou.yj202588.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xhv.ivvv.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oib.shanyushiyangkeji.top

================================================================================
来源：http://hrm.fehbvm.com

K. JSON 与序列化
来源：http://gnr.snrcjt.cn

================================================================================
来源：http://azu.ydjk.org.cn

[K01] 对象转 JSON 字符串
来源：http://sny.yuanzhike.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xta.tianlin.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tjm.0kj1m.cn

JS:   JSON.stringify(obj)
来源：http://jhs.shanyushiyangkeji.top

TS:   JSON.stringify(obj)
来源：http://yqt.fehbvm.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://roe.aibaodan.cn

Go:   json.Marshal(obj)
来源：http://nne.jinghuilouyu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ult.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yth.yongpay.top

[K02] JSON 字符串转对象
来源：http://yon.yvedp.cn

Py:   json.loads(s)
来源：http://pqk.shanyushiyangkeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oyf.yj20258.top

JS:   JSON.parse(s)
来源：http://ctr.svipenyu.cn

TS:   JSON.parse(s)
来源：http://hyu.daxiang520.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://eno.feifeiyinyue.top

Go:   json.Unmarshal(data, &v)
来源：http://wpl.birdmap.top

Ruby: JSON.parse(s)
来源：http://izx.shzxlz.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ptg.fzhhl.top

[K03] JSON 美化输出（带缩进）
来源：http://bjf.tarul.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mym.bbcook.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jnv.yuanzhike.top

JS:   JSON.stringify(obj, null, 2)
来源：http://knx.yonumen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://joo.shangyingyoupin.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://msc.xylfe.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vwc.yj20258.top

Ruby: JSON.pretty_generate(obj)
来源：http://kjc.ehwqpu.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://are.havefunace.top

[K04] 读取 JSON 文件
来源：http://rwv.hnxiangtu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blz.vqdsnc.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kpb.jinghuilouyu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mdz.ppjwa.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rri.ydzc1.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eog.sufxvd.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wkt.xingfuxueyuan.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://zrk.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tzz.shuidangran.top

[K05] 深拷贝对象
来源：http://iqb.hnxiangtu.top

Py:   copy.deepcopy(obj)
来源：http://nzh.tian-w.cn

PHP:  unserialize(serialize($obj));
来源：http://rnq.jinghuilouyu.cn

JS:   structuredClone(obj)
来源：http://kiy.ehwqpu.com

TS:   structuredClone(obj)
来源：http://oit.ydzc1.top

Java: // 手写拷贝构造，或序列化往返
来源：http://rvz.bjfxy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zek.vehdjk.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://axw.yuanzhike.top

C#:   // 序列化往返，或自定义 Clone
来源：http://dhf.tarul.cn

[K06] 解析 URL 查询串
来源：http://kiu.iojbl.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ctx.9152youxi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ecw.xylfe.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nec.jyoumei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jme.svipenyu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gcu.sweek.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kmf.wangdashe.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xmk.epnwcf.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sox.pycfn.com

[K07] 进制转换
来源：http://mtx.andypj.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ayl.hnqzz.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jyd.316326.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mlt.snrcjt.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://msf.epnwcf.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yhe.zhiwuduotai.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qnn.guowangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vpe.jlsjyb.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zbw.zhaomingkeji.xyz

[K08] 二进制序列化（非 JSON）
来源：http://fjr.cashguo.top

Py:   pickle.dumps(obj)
来源：http://wib.meibo888.top

PHP:  serialize($obj);  unserialize($s);
来源：http://put.xinyue.icu

JS:   v8.serialize(obj)        // Node
来源：http://zlz.xuanzx.com

TS:   v8.serialize(obj)        // Node
来源：http://epq.hnqzz.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lmc.yongpay.top

Go:   encoding/gob
来源：http://kjc.daria6918.cn

Ruby: Marshal.dump(obj)
来源：http://gos.cqqwz.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vmu.yongpay.top

================================================================================
来源：http://qmo.gotoacloud.top

L. 网络请求
来源：http://fki.ydzc1.top

================================================================================
来源：http://pmv.jyoumei.cn

[L01] 发送 GET 请求
来源：http://vuf.hysaishi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xci.ywan-chungtsiang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rna.zhijiandao.cn

JS:   await fetch(url)
来源：http://lvp.ybcxt.top

TS:   await fetch(url)
来源：http://wgp.snrcjt.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sbg.xylfe.cn

Go:   resp, err := http.Get(url)
来源：http://dzo.cdnleiting.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vhx.wangshuangyany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rop.mhx1999.top

[L02] 发送 POST JSON
来源：http://myl.zycfv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ahf.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mrz.yuanzhike.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dym.c1oappe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tks.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nhf.gzhubu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fsb.zhiwuduotai.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xzk.tanke756.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ljd.9152youxi.cn

[L03] 设置自定义请求头
来源：http://lrq.zhixingplan.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cqb.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://krz.cheryme.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vbp.bbcook.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cce.xylfe.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://elo.quarkkingdee.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ztk.dianchejie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vfq.ppjwa.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pvc.tanke756.top

[L04] 设置超时
来源：http://pvr.hnxiangtu.top

Py:   requests.get(url, timeout=5)
来源：http://vgb.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://arv.hfpthk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jzc.chenjidiqi.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jhp.ivvv.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zxk.fanxiaobao.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dyo.havefunace.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wii.ybcxt.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ols.tian-w.cn

[L05] 上传文件（multipart）
来源：http://scw.hammf.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dzg.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jeo.hnqzz.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://aaf.yj20258.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uzs.yj20258.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ygt.guannengcc.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cca.316326.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vkd.tian-w.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kfj.xuanzx.com

[L06] 解析响应为 JSON
来源：http://val.cqqwz.cn

Py:   resp.json()
来源：http://tyb.meibo888.top

PHP:  json_decode($body, true);
来源：http://ess.jinqigfzy.top

JS:   await resp.json()
来源：http://loy.hesvh.cn

TS:   await resp.json()
来源：http://sey.fzhhl.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uqi.jinqigufen.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://suz.svipenyu.cn

Ruby: JSON.parse(resp.body)
来源：http://kof.52xcode.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xdr.tarul.cn

[L07] 处理 HTTP 状态码
来源：http://zax.jinqigufen.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pax.zhaomingkeji.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lxl.ppjwa.cn

JS:   resp.ok;  resp.status
来源：http://gwn.ctjpmb.com

TS:   resp.ok;  resp.status
来源：http://kui.ydjk.org.cn

Java: resp.statusCode()
来源：http://hrj.cucudq.cn

Go:   resp.StatusCode
来源：http://ecj.hnxiangtu.top

Ruby: resp.code.to_i
来源：http://ebd.shangyingyoupin.top

C#:   (int)resp.StatusCode
来源：http://rtf.jqgfzy.top

[L08] 并发请求多个地址
来源：http://mop.jyoumei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dce.shanyushiyangtech.top

PHP:  curl_multi_init() 系列
来源：http://xgo.yangfankeji.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vex.hnxiangtu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pzd.shanyushiyangkeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wvv.yvedp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://aiv.jinghuilouyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vqg.shanyushiyangkeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xap.pengpengdd.cyou

================================================================================
来源：http://dfd.chenzaomai.com

M. 命令行 / 进程 / 环境
来源：http://mza.tianlin.xyz

================================================================================
来源：http://thq.havefunace.top

[M01] 读取命令行参数
来源：http://dnw.bbcook.cn

Py:   sys.argv[1:]
来源：http://bhu.jqgfzy.top

PHP:  $argv;  $argc;
来源：http://cwx.meibo888.top

JS:   process.argv.slice(2)
来源：http://yjb.sxryk.cn

TS:   process.argv.slice(2)
来源：http://dth.jinyuanbaomall.cn

Java: args 数组（main 方法参数）
来源：http://ynu.zhaomingkeji.xyz

Go:   os.Args[1:]
来源：http://jiq.fanxiaobao.xyz

Ruby: ARGV
来源：http://kiq.yfazqb.com

C#:   args 数组（Main 方法参数）
来源：http://nyf.c1oappe.top

[M02] 读取环境变量
来源：http://pzb.xziqi.cn

Py:   os.environ.get("HOME")
来源：http://umy.xuanzx.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bfa.guannengcc.top

JS:   process.env.HOME
来源：http://ikx.hfpthk.cn

TS:   process.env.HOME
来源：http://ffo.ppjwa.cn

Java: System.getenv("HOME")
来源：http://pza.yuanzhike.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hmj.cheryme.top

Ruby: ENV["HOME"]
来源：http://zjj.tarul.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mbx.yuanzhike.top

[M03] 执行外部命令
来源：http://ciu.gotoacloud.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lcj.316326.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hpi.wangshuangyany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://guo.ctjpmb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://uhn.redwolf501.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lya.feifeiyinyue.top

Go:   exec.Command("ls", "-l").Output()
来源：http://rmd.daxiang520.top

Ruby: system("ls -l");  `ls -l`
来源：http://yzo.tarul.cn

C#:   Process.Start("ls", "-l");
来源：http://htk.0kj1m.cn

[M04] 获取当前工作目录
来源：http://pwg.jianghu66.top

Py:   os.getcwd()
来源：http://nce.jqgfzy.top

PHP:  getcwd();
来源：http://dhs.quarkkingdee.top

JS:   process.cwd()
来源：http://cbm.bjfxy.top

TS:   process.cwd()
来源：http://zdu.nwbrower.top

Java: Path.of("").toAbsolutePath()
来源：http://tgl.guannengcc.top

Go:   os.Getwd()
来源：http://cym.shuidangran.top

Ruby: Dir.pwd
来源：http://hai.quarkkingdee.top

C#:   Directory.GetCurrentDirectory()
来源：http://hzu.tianlin.xyz

[M05] 设置退出码
来源：http://irw.yvedp.cn

Py:   sys.exit(1)
来源：http://ezx.gogol.net.cn

PHP:  exit(1);
来源：http://hkf.gzhubu.top

JS:   process.exit(1)
来源：http://adn.yvedp.cn

TS:   process.exit(1)
来源：http://jww.zdqjudy.top

Java: System.exit(1)
来源：http://ehc.cashguo.top

Go:   os.Exit(1)
来源：http://ruq.316326.xyz

Ruby: exit 1
来源：http://qbw.zdbjq.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uut.yuxming.cn

[M06] 向标准错误输出
来源：http://jax.yfazqb.com

Py:   print("err", file=sys.stderr)
来源：http://bkm.hfpthk.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nkt.zdqjudy.top

JS:   console.error("err")
来源：http://uvm.cdnleiting.top

TS:   console.error("err")
来源：http://oyc.xuetiantiany.cn

Java: System.err.println("err")
来源：http://xxb.uphjek.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gqc.kuanghao11.cn

Ruby: warn "err"
来源：http://vgq.shangyingyoupin.top

C#:   Console.Error.WriteLine("err")
来源：http://pgi.cashguo.top

[M07] 判断是否为主入口
来源：http://evy.0kj1m.cn


<!-- 参考信息 -->
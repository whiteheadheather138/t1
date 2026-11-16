代发 wailian999

J. 日期与时间
来源：http://wdj.hammf.cn

================================================================================
来源：http://sft.dianchejie.cn

[J01] 获取当前时间
来源：http://kkf.vqdsnc.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bcs.yj20258.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xxi.gotoacloud.top

JS:   new Date();  Date.now()
来源：http://bva.yanxiufei.cn

TS:   new Date();  Date.now()
来源：http://erl.jianghu66.top

Java: LocalDateTime.now();  Instant.now()
来源：http://cag.ctjpmb.com

Go:   time.Now()
来源：http://tsb.nwbrower.top

Ruby: Time.now
来源：http://gfz.yonumen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://udq.xziqi.cn

[J02] 格式化输出
来源：http://eli.uphjek.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uga.chenzaomai.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ivm.iojbl.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ghw.hysaishi.cn

TS:   d.toISOString()
来源：http://qsd.kuanghao11.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sli.quarkkingdee.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ifp.jiagoushi.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ikr.fengsongda.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lce.fanxiaobao.xyz

[J03] 字符串解析为日期
来源：http://djm.pycfn.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mys.fanxiaobao.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dql.ydzc1.top

JS:   new Date("2024-01-02")
来源：http://zeq.epnwcf.com

TS:   new Date("2024-01-02")
来源：http://vaa.uphjek.com

Java: LocalDate.parse("2024-01-02")
来源：http://ann.hysaishi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://omo.ybcxt.top

Ruby: Date.parse("2024-01-02")
来源：http://zbm.daxiang520.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kkc.cashguo.top

[J04] 时间戳与日期互转
来源：http://ucd.jyoumei.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bdm.meibo888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jjv.jinqigfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cvt.chenlongwang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://dcl.yonumen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jrv.gotoacloud.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://whn.fengsongda.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fbe.cqqwz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://won.jiagoushi.top

[J05] 时间加减（加 7 天）
来源：http://wcq.smart0.xyz

Py:   now + timedelta(days=7)
来源：http://fcr.sufxvd.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hqf.yanxiufei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zit.snrcjt.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://obm.gzhubu.top

Java: LocalDate.now().plusDays(7)
来源：http://gso.shangyingyoupin.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fvm.jianghu66.top

Ruby: Time.now + 7 * 86400
来源：http://ilc.guannengcc.top

C#:   DateTime.Now.AddDays(7)
来源：http://fod.tian-w.cn

[J06] 计算两时间之差
来源：http://mny.yj20258.top

Py:   (end - start).total_seconds()
来源：http://ots.hongshengwenyu.top

PHP:  $end->diff($start)->days;
来源：http://hru.xinyue.icu

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xtb.aibaodan.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jpz.shanyushiyangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://mpf.tanke756.top

Go:   end.Sub(start).Hours()
来源：http://qpb.fzhhl.top

Ruby: end - start                 # 返回秒数
来源：http://owo.uphjek.com

C#:   (end - start).TotalSeconds
来源：http://sez.ivvv.top

[J07] 比较两个日期
来源：http://efl.nanxinkj.top

Py:   d1 < d2;  d1 == d2
来源：http://ekb.gogol.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zuw.guowangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://efh.cucudq.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cjb.snrcjt.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dbn.andypj.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wui.jinqigfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://fpt.fengsongda.top

C#:   d1 < d2;  d1 == d2
来源：http://ijx.hnqzz.top

[J08] 提取年月日与星期
来源：http://hyy.ehwqpu.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jcs.sxryk.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xmn.cqqwz.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dal.kuanghao11.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hfq.hnqzz.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rgl.yfazqb.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wta.nanxuanxn.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uke.haohaochexian.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://whj.ydjk.org.cn

[J09] 时区处理
来源：http://kao.jlsjyb.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lro.dianchejie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mub.hammf.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bxg.zhoulong.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cnd.svipenyu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zen.bbcook.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qjx.guowangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://syo.pycfn.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lsh.jqgfzy.top

[J10] 取今天 / 本月第一天
来源：http://vfe.hnxiangtu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ftm.birdmap.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mir.zycfv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rwp.fengsongda.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fze.sysykeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mwd.sysykeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pfh.hnxiangtu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://juz.hnxiangtu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://osy.tian-w.cn

================================================================================
来源：http://wrk.quarkkingdee.top

K. JSON 与序列化
来源：http://qdw.xuanzx.com

================================================================================
来源：http://xfu.kuanghao11.cn

[K01] 对象转 JSON 字符串
来源：http://mgh.yonumen.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://glf.316326.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xss.snrcjt.cn

JS:   JSON.stringify(obj)
来源：http://cth.epnwcf.com

TS:   JSON.stringify(obj)
来源：http://lnb.xingfuxueyuan.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://odr.zhijiandao.cn

Go:   json.Marshal(obj)
来源：http://woa.quarkkingdee.top

Ruby: obj.to_json                                     // require "json"
来源：http://xyo.gzhubu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://krh.0kj1m.cn

[K02] JSON 字符串转对象
来源：http://ixd.hnqzz.top

Py:   json.loads(s)
来源：http://zvv.zhiwuduotai.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://utv.aizwys.cn

JS:   JSON.parse(s)
来源：http://qju.tian-w.cn

TS:   JSON.parse(s)
来源：http://qrg.uphjek.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cvt.sufxvd.cn

Go:   json.Unmarshal(data, &v)
来源：http://wtp.cqqwz.cn

Ruby: JSON.parse(s)
来源：http://uso.yuanzhike.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nxd.zhongyouzk.top

[K03] JSON 美化输出（带缩进）
来源：http://ndm.zhiwuduotai.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://iyt.hfpthk.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gbd.wangshuangyany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fcu.yfazqb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://ttg.tianlin.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://huh.sysykeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rli.gogol.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uxb.yueranfly.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://twp.aibaodan.cn

[K04] 读取 JSON 文件
来源：http://cgp.jinqigfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pfx.hammf.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kxk.cdnleiting.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hdy.316326.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mnz.xinyue.icu

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://obe.shuidangran.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yks.gotoacloud.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://eap.jiagoushi.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xzj.aizwys.cn

[K05] 深拷贝对象
来源：http://zrv.cucudq.cn

Py:   copy.deepcopy(obj)
来源：http://tgc.ivvv.top

PHP:  unserialize(serialize($obj));
来源：http://qsj.cheryme.top

JS:   structuredClone(obj)
来源：http://eem.yangfankeji.com

TS:   structuredClone(obj)
来源：http://dmp.cqqwz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://orz.guowangkeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bxm.xylfe.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xcn.chenzaomai.com

C#:   // 序列化往返，或自定义 Clone
来源：http://ybw.dashuyun.cn

[K06] 解析 URL 查询串
来源：http://mmh.mhx1999.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vur.zhongyouzk.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://biz.guannengcc.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hdh.yvedp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://opl.vqdsnc.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xqv.redwolf501.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jig.kuanghao11.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ccr.vqdsnc.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://iwt.mhx1999.top

[K07] 进制转换
来源：http://uob.feifeiyinyue.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uyr.redwolf501.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://img.jinqigfzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rtc.shanyushiyangtech.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bdc.chenjidiqi.icu

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uqc.shzxlz.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hdw.zhoulong.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ore.hywenlv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kik.gogol.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://bxq.zhoulong.xyz

Py:   pickle.dumps(obj)
来源：http://uof.xinyue.icu

PHP:  serialize($obj);  unserialize($s);
来源：http://qou.tianlin.xyz

JS:   v8.serialize(obj)        // Node
来源：http://mgp.jinghuilouyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://bly.yongpay.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xls.zycfv.cn

Go:   encoding/gob
来源：http://ocy.mhx1999.top

Ruby: Marshal.dump(obj)
来源：http://gpz.nanxuanxn.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wnr.uphjek.com

================================================================================
来源：http://adx.aizwys.cn

L. 网络请求
来源：http://pws.gaohongyu789.top

================================================================================
来源：http://uyr.jinghuilouyu.cn

[L01] 发送 GET 请求
来源：http://hyg.wangdashe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://anq.nanxinkj.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xfc.jyoumei.cn

JS:   await fetch(url)
来源：http://cec.jinqigfzy.top

TS:   await fetch(url)
来源：http://gqf.jqgfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bky.0kj1m.cn

Go:   resp, err := http.Get(url)
来源：http://lvi.mhx1999.top

Ruby: Net::HTTP.get(URI(url))
来源：http://mla.jqgfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ato.nwbrower.top

[L02] 发送 POST JSON
来源：http://faw.fktsv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lsx.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wkl.xylfe.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jmc.gzhubu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pqf.gotoacloud.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hlo.zdqjudy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zlj.zhaomingkeji.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bzd.shanyushiyangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lzl.9152youxi.cn

[L03] 设置自定义请求头
来源：http://noz.shzxlz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://oqf.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qvq.yuanzhike.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pkl.svipenyu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ygt.yvedp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pgf.gaohongyu789.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ygw.havefunace.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bxu.birdmap.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nqw.smart0.xyz

[L04] 设置超时
来源：http://qlj.hongshengwenyu.top

Py:   requests.get(url, timeout=5)
来源：http://vbc.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rvb.gzhubu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cmw.ybcxt.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rsb.ydjk.org.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://oyj.fktsv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pgk.gotoacloud.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wik.yvedp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ejx.cucudq.cn

[L05] 上传文件（multipart）
来源：http://sff.zhaomingkeji.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wco.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tzv.xylfe.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ziu.zhixingplan.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qzq.hesvh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ftj.snrcjt.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://znj.ivvv.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eys.jqgfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tti.jinqigufen.top

[L06] 解析响应为 JSON
来源：http://jjt.svipenyu.cn

Py:   resp.json()
来源：http://exs.zhiwuduotai.top

PHP:  json_decode($body, true);
来源：http://zcp.yvedp.cn

JS:   await resp.json()
来源：http://cfq.meibo888.top

TS:   await resp.json()
来源：http://kld.gogol.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ova.epnwcf.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ghp.shuidangran.top

Ruby: JSON.parse(resp.body)
来源：http://yqd.quarkkingdee.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rsl.yongpay.top

[L07] 处理 HTTP 状态码
来源：http://otj.jinyuanbaomall.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qct.jqgfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sat.xinyue.icu

JS:   resp.ok;  resp.status
来源：http://yso.tanke756.top

TS:   resp.ok;  resp.status
来源：http://opr.daxiang520.top

Java: resp.statusCode()
来源：http://wbg.jlsjyb.cn

Go:   resp.StatusCode
来源：http://sva.jqgufenzy.top

Ruby: resp.code.to_i
来源：http://yxl.xylfe.cn

C#:   (int)resp.StatusCode
来源：http://yhd.xuanzx.com

[L08] 并发请求多个地址
来源：http://evo.zycfv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://art.dianchejie.cn

PHP:  curl_multi_init() 系列
来源：http://nei.yangfankeji.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mbz.sxryk.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://avt.sxryk.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://akh.jinghuilouyu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tnh.havefunace.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ylw.ybcxt.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zfp.jlsjyb.cn

================================================================================
来源：http://xph.0kj1m.cn

M. 命令行 / 进程 / 环境
来源：http://tjo.sufxvd.cn

================================================================================
来源：http://nwo.mhx1999.top

[M01] 读取命令行参数
来源：http://gxg.bbcook.cn

Py:   sys.argv[1:]
来源：http://ckv.chenjidiqi.icu

PHP:  $argv;  $argc;
来源：http://nus.havefunace.top

JS:   process.argv.slice(2)
来源：http://hxo.ybcxt.top

TS:   process.argv.slice(2)
来源：http://onu.zhoulong.xyz

Java: args 数组（main 方法参数）
来源：http://qzq.jiagoushi.top

Go:   os.Args[1:]
来源：http://srs.ydzc1.top

Ruby: ARGV
来源：http://tml.havefunace.top

C#:   args 数组（Main 方法参数）
来源：http://egt.cqqwz.cn

[M02] 读取环境变量
来源：http://ycs.yj20258888.top

Py:   os.environ.get("HOME")
来源：http://tlz.jinqigufen.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vrk.hfpthk.cn

JS:   process.env.HOME
来源：http://xcu.sxryk.cn

TS:   process.env.HOME
来源：http://iow.zdbjq.cn

Java: System.getenv("HOME")
来源：http://ois.ydzc1.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ilj.tarul.cn

Ruby: ENV["HOME"]
来源：http://mxk.hfpthk.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mzx.ppjwa.cn

[M03] 执行外部命令
来源：http://fhk.yueranfly.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pxx.sufxvd.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gbp.svipenyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ewf.fktsv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://isy.sysykeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jpr.zhixingplan.top

Go:   exec.Command("ls", "-l").Output()
来源：http://grd.tarul.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wtq.smart0.xyz

C#:   Process.Start("ls", "-l");
来源：http://oxr.316326.xyz

[M04] 获取当前工作目录
来源：http://ejb.jiagoushi.top

Py:   os.getcwd()
来源：http://qnf.hnxiangtu.top

PHP:  getcwd();
来源：http://uhn.chenzaomai.com

JS:   process.cwd()
来源：http://xqo.nwbrower.top

TS:   process.cwd()
来源：http://tfj.gzhubu.top

Java: Path.of("").toAbsolutePath()
来源：http://eeo.tarul.cn

Go:   os.Getwd()
来源：http://gfa.feifeiyinyue.top

Ruby: Dir.pwd
来源：http://wct.ywan-chungtsiang.top

C#:   Directory.GetCurrentDirectory()
来源：http://flk.zhengqikj.top

[M05] 设置退出码
来源：http://wzp.yuxming.cn

Py:   sys.exit(1)
来源：http://dwe.guannengcc.top

PHP:  exit(1);
来源：http://gjf.nanxuanxn.top

JS:   process.exit(1)
来源：http://yfh.nanxuanxn.top

TS:   process.exit(1)
来源：http://rdm.nanxinkj.top

Java: System.exit(1)
来源：http://lpf.ywan-chungtsiang.top

Go:   os.Exit(1)
来源：http://xuw.bjfxy.top

Ruby: exit 1
来源：http://vbk.yfazqb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bju.nwbrower.top

[M06] 向标准错误输出
来源：http://sti.zycfv.cn

Py:   print("err", file=sys.stderr)
来源：http://mjn.haohaochexian.top

PHP:  fwrite(STDERR, "err\n");
来源：http://eru.cqqwz.cn

JS:   console.error("err")
来源：http://isv.xziqi.cn

TS:   console.error("err")
来源：http://kkg.iojbl.cn

Java: System.err.println("err")
来源：http://qsr.yangfankeji.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ink.yfazqb.com

Ruby: warn "err"
来源：http://gxx.jinghuilouyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://rhb.gotoacloud.top

[M07] 判断是否为主入口
来源：http://yag.meibo888.top


<!-- 参考信息 -->
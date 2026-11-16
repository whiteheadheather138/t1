代发 wailian999

J. 日期与时间
来源：http://kpa.xingfuxueyuan.xyz

================================================================================
来源：http://nwq.9152youxi.cn

[J01] 获取当前时间
来源：http://bow.sxryk.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bqs.jinghuilouyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rtw.yj202588.top

JS:   new Date();  Date.now()
来源：http://iso.kuanghao11.cn

TS:   new Date();  Date.now()
来源：http://bpv.dianchejie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nmu.sweek.top

Go:   time.Now()
来源：http://jny.ivvv.top

Ruby: Time.now
来源：http://oqg.jqgfzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nqr.yj202588.top

[J02] 格式化输出
来源：http://fuh.yuxming.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hlh.nanxinkj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xmc.hcnkem.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://eef.zhijiandao.cn

TS:   d.toISOString()
来源：http://ael.xuetiantiany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wcw.yuanzhike.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ywj.52xcode.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jjd.yfazqb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cnb.sweek.top

[J03] 字符串解析为日期
来源：http://ant.gogol.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jjd.jinqigufen.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xzn.yuxming.cn

JS:   new Date("2024-01-02")
来源：http://hkq.ydjk.org.cn

TS:   new Date("2024-01-02")
来源：http://yij.hcnkem.com

Java: LocalDate.parse("2024-01-02")
来源：http://jlz.kuanghao11.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nzm.sjlbkw.cn

Ruby: Date.parse("2024-01-02")
来源：http://fvt.shuidangran.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pbu.jianghu66.top

[J04] 时间戳与日期互转
来源：http://apw.hysaishi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ocz.uphjek.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://adw.fzhhl.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dtx.fktsv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jfm.ehwqpu.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jln.sysykeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qbh.yuxming.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rzd.jinqigfzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qcw.gaohongyu789.top

[J05] 时间加减（加 7 天）
来源：http://klo.zhaomingkeji.xyz

Py:   now + timedelta(days=7)
来源：http://bfn.shuidangran.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://cwv.sysykeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vxn.jyoumei.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dmd.andypj.xyz

Java: LocalDate.now().plusDays(7)
来源：http://uao.hcnkem.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rpk.quarkkingdee.top

Ruby: Time.now + 7 * 86400
来源：http://bti.yvedp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://byk.gotoacloud.top

[J06] 计算两时间之差
来源：http://ags.316326.xyz

Py:   (end - start).total_seconds()
来源：http://tyj.yvedp.cn

PHP:  $end->diff($start)->days;
来源：http://dha.xinyue.icu

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sut.zhongyouzk.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cvn.yfazqb.com

Java: Duration.between(start, end).toSeconds()
来源：http://vav.0kj1m.cn

Go:   end.Sub(start).Hours()
来源：http://txa.daxiang520.top

Ruby: end - start                 # 返回秒数
来源：http://vxb.bbcook.cn

C#:   (end - start).TotalSeconds
来源：http://bzj.hammf.cn

[J07] 比较两个日期
来源：http://rtt.zhoulong.xyz

Py:   d1 < d2;  d1 == d2
来源：http://tky.feifeiyinyue.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xnr.guowangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://ztn.yangfankeji.com

TS:   d1.getTime() < d2.getTime()
来源：http://ywf.hysaishi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://udq.ehwqpu.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bnf.nanxuanxn.top

Ruby: d1 < d2;  d1 == d2
来源：http://zdk.gaohongyu789.top

C#:   d1 < d2;  d1 == d2
来源：http://xoj.birdmap.top

[J08] 提取年月日与星期
来源：http://qph.jlsjyb.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hvv.aibaodan.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cni.0kj1m.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cuh.gzhubu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vzh.c1oappe.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wjq.fehbvm.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mfi.52xcode.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ehb.jlsjyb.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kst.tanke756.top

[J09] 时区处理
来源：http://uvp.zhengqikj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uev.gzhubu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xty.uphjek.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lsw.snrcjt.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://epy.316326.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bam.jqgufenzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yac.tianlin.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://mtv.yanxiufei.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://noq.hammf.cn

[J10] 取今天 / 本月第一天
来源：http://kss.yanxiufei.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://udf.chenlongwang.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://egk.havefunace.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://eqf.cheryme.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tvy.shzxlz.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qbs.cashguo.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jzj.ybcxt.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kaq.xingfuxueyuan.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://smr.zhijiandao.cn

================================================================================
来源：http://ldp.jlsjyb.cn

K. JSON 与序列化
来源：http://ddr.sysykeji.top

================================================================================
来源：http://jzp.fanxiaobao.xyz

[K01] 对象转 JSON 字符串
来源：http://ltz.hongshengwenyu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sdf.meibo888.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wxv.zhongyouzk.top

JS:   JSON.stringify(obj)
来源：http://pxk.jqgufenzy.top

TS:   JSON.stringify(obj)
来源：http://buo.fktsv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hsl.yueranfly.top

Go:   json.Marshal(obj)
来源：http://yho.fanxiaobao.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://hsw.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://zft.jianghu66.top

[K02] JSON 字符串转对象
来源：http://gal.yonumen.top

Py:   json.loads(s)
来源：http://fkv.xingfuxueyuan.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://myr.havefunace.top

JS:   JSON.parse(s)
来源：http://ifi.hysaishi.cn

TS:   JSON.parse(s)
来源：http://gmw.cucudq.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qrb.xylfe.cn

Go:   json.Unmarshal(data, &v)
来源：http://eqy.kuanghao11.cn

Ruby: JSON.parse(s)
来源：http://onh.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://evq.sxryk.cn

[K03] JSON 美化输出（带缩进）
来源：http://yrb.andypj.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jkn.pengpengdd.cyou

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xla.c1oappe.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hic.jinqigfzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://pxc.fanxiaobao.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wlz.zhijiandao.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dlc.xinyue.icu

Ruby: JSON.pretty_generate(obj)
来源：http://cgt.sysykeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nom.birdmap.top

[K04] 读取 JSON 文件
来源：http://iao.shangyingyoupin.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://syl.yj20258.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://puv.iojbl.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bcl.haohaochexian.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qmc.jinqigfzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wuy.fengsongda.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oiq.gogol.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lbp.svipenyu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://aqy.quarkkingdee.top

[K05] 深拷贝对象
来源：http://kvo.epnwcf.com

Py:   copy.deepcopy(obj)
来源：http://zqj.cashguo.top

PHP:  unserialize(serialize($obj));
来源：http://tud.dashuyun.cn

JS:   structuredClone(obj)
来源：http://lok.bbcook.cn

TS:   structuredClone(obj)
来源：http://haz.xylfe.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pjs.zhixingplan.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zfv.ywan-chungtsiang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://txz.iojbl.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sbc.jlsjyb.cn

[K06] 解析 URL 查询串
来源：http://nti.hysaishi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jrp.yangfankeji.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jag.andypj.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fed.cdnleiting.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://whh.yueranfly.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ubm.dashuyun.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://btj.hammf.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ihu.zhongyouzk.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lqh.uphjek.com

[K07] 进制转换
来源：http://yyv.andypj.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cjs.sweek.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tkj.vqdsnc.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://afr.jianghu66.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dnh.jinghuilouyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gre.meibo888.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://aer.yangfankeji.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ymi.hongshengwenyu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uts.fehbvm.com

[K08] 二进制序列化（非 JSON）
来源：http://xem.xziqi.cn

Py:   pickle.dumps(obj)
来源：http://egx.gzhubu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://yno.yuxming.cn

JS:   v8.serialize(obj)        // Node
来源：http://rei.bbcook.cn

TS:   v8.serialize(obj)        // Node
来源：http://tln.cheryme.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wbi.52xcode.cn

Go:   encoding/gob
来源：http://wfv.9152youxi.cn

Ruby: Marshal.dump(obj)
来源：http://lpc.aibaodan.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jgp.ybcxt.top

================================================================================
来源：http://wxa.hywenlv.cn

L. 网络请求
来源：http://dbt.wangdashe.top

================================================================================
来源：http://zng.havefunace.top

[L01] 发送 GET 请求
来源：http://jdy.quarkkingdee.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dzt.gogol.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ade.mhx1999.top

JS:   await fetch(url)
来源：http://znu.xuetiantiany.cn

TS:   await fetch(url)
来源：http://wko.cashguo.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://txa.xuanzx.com

Go:   resp, err := http.Get(url)
来源：http://tho.jinqigfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vur.chenlongwang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fxu.cqqwz.cn

[L02] 发送 POST JSON
来源：http://uzm.yanxiufei.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ctf.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ylh.fanxiaobao.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ruw.jinqigfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oup.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mbt.ehwqpu.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://usp.aizwys.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lon.tanke756.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dpv.dianchejie.cn

[L03] 设置自定义请求头
来源：http://eeh.gaohongyu789.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tqf.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wjh.zycfv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eka.yueranfly.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kat.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wmc.zdqjudy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://imx.sxryk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tqd.gogol.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rqk.tarul.cn

[L04] 设置超时
来源：http://nsh.hysaishi.cn

Py:   requests.get(url, timeout=5)
来源：http://zaa.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ozz.zhaomingkeji.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://utb.shangyingyoupin.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wol.yongpay.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ops.yj20258888.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oqu.zhiwuduotai.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zrh.jiagoushi.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dhl.snrcjt.cn

[L05] 上传文件（multipart）
来源：http://pej.zhixingplan.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wgz.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xqm.vehdjk.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bxi.sweek.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://suw.jinghuilouyu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xml.bbcook.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mne.yueranfly.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zvz.xinyue.icu

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jxk.feifeiyinyue.top

[L06] 解析响应为 JSON
来源：http://inm.birdmap.top

Py:   resp.json()
来源：http://sgh.chenjidiqi.icu

PHP:  json_decode($body, true);
来源：http://sfh.iojbl.cn

JS:   await resp.json()
来源：http://cqw.zycfv.cn

TS:   await resp.json()
来源：http://yvd.gotoacloud.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uwb.zhengqikj.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dug.hfpthk.cn

Ruby: JSON.parse(resp.body)
来源：http://fif.daria6918.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mla.shuidangran.top

[L07] 处理 HTTP 状态码
来源：http://wjs.cdnleiting.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qvp.ctjpmb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rkn.shzxlz.cn

JS:   resp.ok;  resp.status
来源：http://edq.gotoacloud.top

TS:   resp.ok;  resp.status
来源：http://yry.shzxlz.cn

Java: resp.statusCode()
来源：http://gyq.yueranfly.top

Go:   resp.StatusCode
来源：http://ufi.zdbjq.cn

Ruby: resp.code.to_i
来源：http://mia.mhx1999.top

C#:   (int)resp.StatusCode
来源：http://shp.zhengqikj.top

[L08] 并发请求多个地址
来源：http://mvv.zhixingplan.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yea.fengsongda.top

PHP:  curl_multi_init() 系列
来源：http://joh.xziqi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aim.cashguo.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hoa.meibo888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fav.andypj.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ndd.zdbjq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oaq.fzhhl.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wpj.yuanzhike.top

================================================================================
来源：http://nwj.shzxlz.cn

M. 命令行 / 进程 / 环境
来源：http://fcx.yfazqb.com

================================================================================
来源：http://oxa.epnwcf.com

[M01] 读取命令行参数
来源：http://foh.jinyuanbaomall.cn

Py:   sys.argv[1:]
来源：http://muy.tarul.cn

PHP:  $argv;  $argc;
来源：http://dgi.guowangkeji.top

JS:   process.argv.slice(2)
来源：http://mhy.chenzaomai.com

TS:   process.argv.slice(2)
来源：http://idd.fanxiaobao.xyz

Java: args 数组（main 方法参数）
来源：http://lcu.svipenyu.cn

Go:   os.Args[1:]
来源：http://goj.iojbl.cn

Ruby: ARGV
来源：http://zze.bbcook.cn

C#:   args 数组（Main 方法参数）
来源：http://wwd.sufxvd.cn

[M02] 读取环境变量
来源：http://pov.jinqigufen.top

Py:   os.environ.get("HOME")
来源：http://qzz.andypj.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tbk.fehbvm.com

JS:   process.env.HOME
来源：http://vvi.sufxvd.cn

TS:   process.env.HOME
来源：http://riv.jianghu66.top

Java: System.getenv("HOME")
来源：http://zas.andypj.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://crq.snrcjt.cn

Ruby: ENV["HOME"]
来源：http://nbc.gogol.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://eay.sjlbkw.cn

[M03] 执行外部命令
来源：http://hxz.ctjpmb.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xiv.fehbvm.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tcf.yvedp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cuh.feifeiyinyue.top

TS:   child_process.execSync("ls -l").toString()
来源：http://qbd.redwolf501.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hek.yvedp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jfs.shanyushiyangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://bmy.kuanghao11.cn

C#:   Process.Start("ls", "-l");
来源：http://ned.fengsongda.top

[M04] 获取当前工作目录
来源：http://vcs.daria6918.cn

Py:   os.getcwd()
来源：http://ifr.xuanzx.com

PHP:  getcwd();
来源：http://pbx.zhengqikj.top

JS:   process.cwd()
来源：http://tzp.fanxiaobao.xyz

TS:   process.cwd()
来源：http://oju.havefunace.top

Java: Path.of("").toAbsolutePath()
来源：http://qog.zycfv.cn

Go:   os.Getwd()
来源：http://otb.hfpthk.cn

Ruby: Dir.pwd
来源：http://kcf.nanxuanxn.top

C#:   Directory.GetCurrentDirectory()
来源：http://urc.pengpengdd.cyou

[M05] 设置退出码
来源：http://dcy.sxryk.cn

Py:   sys.exit(1)
来源：http://thd.chenzaomai.com

PHP:  exit(1);
来源：http://ckq.snrcjt.cn

JS:   process.exit(1)
来源：http://bzp.fehbvm.com

TS:   process.exit(1)
来源：http://zqv.zdbjq.cn

Java: System.exit(1)
来源：http://dyr.tianlin.xyz

Go:   os.Exit(1)
来源：http://sao.kuanghao11.cn

Ruby: exit 1
来源：http://fkv.hysaishi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://aip.ctjpmb.com

[M06] 向标准错误输出
来源：http://hwt.jinghuilouyu.cn

Py:   print("err", file=sys.stderr)
来源：http://igz.bjfxy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ifc.ydzc1.top

JS:   console.error("err")
来源：http://wao.xingfuxueyuan.xyz

TS:   console.error("err")
来源：http://icb.yongpay.top

Java: System.err.println("err")
来源：http://ajj.yanxiufei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lsh.ybcxt.top

Ruby: warn "err"
来源：http://dfx.haohaochexian.top

C#:   Console.Error.WriteLine("err")
来源：http://mux.zdbjq.cn

[M07] 判断是否为主入口
来源：http://rtf.chenzaomai.com


<!-- 参考信息 -->
代发 wailian999

J. 日期与时间
来源：http://vxc.havefunace.top

================================================================================
来源：http://ggj.0kj1m.cn

[J01] 获取当前时间
来源：http://cvp.gzhubu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://nko.ppjwa.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pia.yueranfly.top

JS:   new Date();  Date.now()
来源：http://tlh.ctjpmb.com

TS:   new Date();  Date.now()
来源：http://cpq.dashuyun.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rgb.svipenyu.cn

Go:   time.Now()
来源：http://beo.zhijiandao.cn

Ruby: Time.now
来源：http://cti.0kj1m.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wfj.jqgfzy.top

[J02] 格式化输出
来源：http://vyy.9152youxi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vem.haohaochexian.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://alt.shangyingyoupin.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sfa.yuanzhike.top

TS:   d.toISOString()
来源：http://ajw.shuidangran.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bfo.andypj.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hhq.nanxinkj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rar.jinghuilouyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nta.feifeiyinyue.top

[J03] 字符串解析为日期
来源：http://vgm.xziqi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jde.guannengcc.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://now.fengsongda.top

JS:   new Date("2024-01-02")
来源：http://eam.birdmap.top

TS:   new Date("2024-01-02")
来源：http://mjx.wangdashe.top

Java: LocalDate.parse("2024-01-02")
来源：http://xcr.jlsjyb.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ojq.kuanghao11.cn

Ruby: Date.parse("2024-01-02")
来源：http://pus.daxiang520.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rqq.zycfv.cn

[J04] 时间戳与日期互转
来源：http://hss.gzhubu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sdz.zycfv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wfj.vehdjk.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ave.xziqi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rku.yj202588.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bkz.ydzc1.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jnq.shanyushiyangtech.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dfo.pengpengdd.cyou

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yaj.sufxvd.cn

[J05] 时间加减（加 7 天）
来源：http://mnr.xylfe.cn

Py:   now + timedelta(days=7)
来源：http://axz.ehwqpu.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://bak.ehwqpu.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tjf.hnxiangtu.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qty.redwolf501.top

Java: LocalDate.now().plusDays(7)
来源：http://irz.hcnkem.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dps.aizwys.cn

Ruby: Time.now + 7 * 86400
来源：http://lfp.ydjk.org.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jop.sxryk.cn

[J06] 计算两时间之差
来源：http://zac.yangfankeji.com

Py:   (end - start).total_seconds()
来源：http://yqf.ybcxt.top

PHP:  $end->diff($start)->days;
来源：http://egu.ctjpmb.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rxs.hammf.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jao.wangdashe.top

Java: Duration.between(start, end).toSeconds()
来源：http://vyt.vqdsnc.cn

Go:   end.Sub(start).Hours()
来源：http://svh.hammf.cn

Ruby: end - start                 # 返回秒数
来源：http://cna.xingfuxueyuan.xyz

C#:   (end - start).TotalSeconds
来源：http://gpv.kuanghao11.cn

[J07] 比较两个日期
来源：http://awz.xuanzx.com

Py:   d1 < d2;  d1 == d2
来源：http://pmy.yueranfly.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ynu.guannengcc.top

JS:   d1.getTime() < d2.getTime()
来源：http://qfl.tianlin.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://blv.daxiang520.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nid.tanke756.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kwm.xuetiantiany.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qff.cheryme.top

C#:   d1 < d2;  d1 == d2
来源：http://ctv.xuetiantiany.cn

[J08] 提取年月日与星期
来源：http://ixf.fehbvm.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kln.jinyuanbaomall.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jmd.52xcode.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://coz.316326.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yml.cucudq.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rwr.jlsjyb.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wip.sjlbkw.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://inc.shuidangran.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wiz.quarkkingdee.top

[J09] 时区处理
来源：http://uzp.yj20258888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://klb.zdqjudy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ija.zhoulong.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eyq.sxryk.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zuo.jinghuilouyu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sgq.xziqi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jsx.zhoulong.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://amh.yfazqb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fqq.fengsongda.top

[J10] 取今天 / 本月第一天
来源：http://izs.sweek.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hjz.shzxlz.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iov.yanxiufei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cgu.epnwcf.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://euo.xinyue.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sgy.hammf.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kvm.ctjpmb.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://thv.guowangkeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://msg.sxryk.cn

================================================================================
来源：http://iyb.xuetiantiany.cn

K. JSON 与序列化
来源：http://bup.guowangkeji.top

================================================================================
来源：http://fxl.hywenlv.cn

[K01] 对象转 JSON 字符串
来源：http://qhr.andypj.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blr.cqqwz.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rdq.hnqzz.top

JS:   JSON.stringify(obj)
来源：http://nhw.nwbrower.top

TS:   JSON.stringify(obj)
来源：http://woo.zhoulong.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lpp.jqgufenzy.top

Go:   json.Marshal(obj)
来源：http://ouc.xinyue.icu

Ruby: obj.to_json                                     // require "json"
来源：http://qvz.xziqi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://uoi.hesvh.cn

[K02] JSON 字符串转对象
来源：http://jxv.tianlin.xyz

Py:   json.loads(s)
来源：http://fjc.xuanzx.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tmb.xingfuxueyuan.xyz

JS:   JSON.parse(s)
来源：http://lxs.daria6918.cn

TS:   JSON.parse(s)
来源：http://hps.iojbl.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yra.cucudq.cn

Go:   json.Unmarshal(data, &v)
来源：http://ywg.chenzaomai.com

Ruby: JSON.parse(s)
来源：http://onv.quarkkingdee.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://toz.9152youxi.cn

[K03] JSON 美化输出（带缩进）
来源：http://lbz.hnqzz.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nim.havefunace.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://thk.aibaodan.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ppl.fzhhl.top

TS:   JSON.stringify(obj, null, 2)
来源：http://rrq.cqqwz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://opj.epnwcf.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ddp.gotoacloud.top

Ruby: JSON.pretty_generate(obj)
来源：http://kxj.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nck.zycfv.cn

[K04] 读取 JSON 文件
来源：http://mzl.yj202588.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qof.jyoumei.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://khy.zhengqikj.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xdu.shanyushiyangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qah.52xcode.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://siv.yvedp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fus.tian-w.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gfy.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gge.zhoulong.xyz

[K05] 深拷贝对象
来源：http://ryl.hesvh.cn

Py:   copy.deepcopy(obj)
来源：http://luj.chenjidiqi.icu

PHP:  unserialize(serialize($obj));
来源：http://eet.haohaochexian.top

JS:   structuredClone(obj)
来源：http://lum.yj20258888.top

TS:   structuredClone(obj)
来源：http://hwn.guannengcc.top

Java: // 手写拷贝构造，或序列化往返
来源：http://dym.hysaishi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qrz.gotoacloud.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pti.tianlin.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://hww.zhoulong.xyz

[K06] 解析 URL 查询串
来源：http://dnf.shanyushiyangtech.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fjh.gogol.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ueo.kuanghao11.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jfq.zycfv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sjm.hnxiangtu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://czf.hesvh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vss.yj20258888.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jqq.jinqigfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://aqp.yj202588.top

[K07] 进制转换
来源：http://lrm.aibaodan.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://aqy.jiagoushi.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hnf.hfpthk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qaf.cucudq.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fcm.svipenyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ees.iojbl.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://chc.xingfuxueyuan.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fym.yvedp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xbc.52xcode.cn

[K08] 二进制序列化（非 JSON）
来源：http://niw.jinghuilouyu.cn

Py:   pickle.dumps(obj)
来源：http://itw.aizwys.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mgi.cheryme.top

JS:   v8.serialize(obj)        // Node
来源：http://nai.redwolf501.top

TS:   v8.serialize(obj)        // Node
来源：http://cac.yj202588.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zgb.jinqigufen.top

Go:   encoding/gob
来源：http://gpj.andypj.xyz

Ruby: Marshal.dump(obj)
来源：http://acx.haohaochexian.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qho.yj20258.top

================================================================================
来源：http://ifq.haohaochexian.top

L. 网络请求
来源：http://cnq.xinyue.icu

================================================================================
来源：http://yvu.pycfn.com

[L01] 发送 GET 请求
来源：http://jbt.hesvh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ogn.jyoumei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://eao.feifeiyinyue.top

JS:   await fetch(url)
来源：http://fee.guowangkeji.top

TS:   await fetch(url)
来源：http://sbh.fengsongda.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tvk.jianghu66.top

Go:   resp, err := http.Get(url)
来源：http://hrl.yuxming.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://owz.chenzaomai.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zol.tanke756.top

[L02] 发送 POST JSON
来源：http://cqf.zhijiandao.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xzk.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ufy.zhaomingkeji.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://usn.dianchejie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xom.snrcjt.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tcm.fzhhl.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eti.yuxming.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://iqo.yuanzhike.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hsz.guowangkeji.top

[L03] 设置自定义请求头
来源：http://fov.fktsv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bvx.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://roe.yonumen.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ovi.yj20258.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kqu.jqgufenzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dzp.fktsv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://urz.kuanghao11.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kwb.jinqigfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lbr.hywenlv.cn

[L04] 设置超时
来源：http://ble.wangdashe.top

Py:   requests.get(url, timeout=5)
来源：http://dbd.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jkb.chenjidiqi.icu

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://grj.shuidangran.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://chf.cucudq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uqb.jiagoushi.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ogk.cdnleiting.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qom.ehwqpu.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gpc.tanke756.top

[L05] 上传文件（multipart）
来源：http://smr.zhixingplan.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fje.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cer.zhaomingkeji.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gmy.c1oappe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://izc.chenlongwang.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nau.hfpthk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kws.iojbl.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ypv.tarul.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://szj.smart0.xyz

[L06] 解析响应为 JSON
来源：http://yoq.cashguo.top

Py:   resp.json()
来源：http://ezc.chenzaomai.com

PHP:  json_decode($body, true);
来源：http://zqc.sufxvd.cn

JS:   await resp.json()
来源：http://uvy.zdqjudy.top

TS:   await resp.json()
来源：http://zig.zhijiandao.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://naj.hysaishi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://roa.yj20258.top

Ruby: JSON.parse(resp.body)
来源：http://gcp.jinghuilouyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jfw.yvedp.cn

[L07] 处理 HTTP 状态码
来源：http://qkl.52xcode.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kch.fzhhl.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qyu.yanxiufei.cn

JS:   resp.ok;  resp.status
来源：http://pog.cashguo.top

TS:   resp.ok;  resp.status
来源：http://fmi.yonumen.top

Java: resp.statusCode()
来源：http://ghn.zdqjudy.top

Go:   resp.StatusCode
来源：http://wxh.ybcxt.top

Ruby: resp.code.to_i
来源：http://wnq.shzxlz.cn

C#:   (int)resp.StatusCode
来源：http://fhw.mhx1999.top

[L08] 并发请求多个地址
来源：http://zoq.uphjek.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nla.cucudq.cn

PHP:  curl_multi_init() 系列
来源：http://ujk.hcnkem.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://umf.ybcxt.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cvs.yonumen.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ixh.gaohongyu789.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xjx.uphjek.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://iqz.zhijiandao.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bia.nanxinkj.top

================================================================================
来源：http://glw.xziqi.cn

M. 命令行 / 进程 / 环境
来源：http://fwx.jqgfzy.top

================================================================================
来源：http://yan.ctjpmb.com

[M01] 读取命令行参数
来源：http://npn.cashguo.top

Py:   sys.argv[1:]
来源：http://pwr.ehwqpu.com

PHP:  $argv;  $argc;
来源：http://xpq.hywenlv.cn

JS:   process.argv.slice(2)
来源：http://crs.jianghu66.top

TS:   process.argv.slice(2)
来源：http://anm.sweek.top

Java: args 数组（main 方法参数）
来源：http://wam.52xcode.cn

Go:   os.Args[1:]
来源：http://koe.316326.xyz

Ruby: ARGV
来源：http://wsa.hesvh.cn

C#:   args 数组（Main 方法参数）
来源：http://vxi.xuetiantiany.cn

[M02] 读取环境变量
来源：http://nts.yj20258.top

Py:   os.environ.get("HOME")
来源：http://lxt.birdmap.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hfu.yvedp.cn

JS:   process.env.HOME
来源：http://wvv.redwolf501.top

TS:   process.env.HOME
来源：http://lch.iojbl.cn

Java: System.getenv("HOME")
来源：http://pia.yueranfly.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ldc.quarkkingdee.top

Ruby: ENV["HOME"]
来源：http://ink.yuanzhike.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://iho.zhixingplan.top

[M03] 执行外部命令
来源：http://tpf.uphjek.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rok.jyoumei.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yvh.dianchejie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dlj.jinyuanbaomall.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kcl.zhiwuduotai.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lan.fzhhl.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wkn.zhengqikj.top

Ruby: system("ls -l");  `ls -l`
来源：http://dvf.ivvv.top

C#:   Process.Start("ls", "-l");
来源：http://wuv.bjfxy.top

[M04] 获取当前工作目录
来源：http://awo.jiagoushi.top

Py:   os.getcwd()
来源：http://dhw.hammf.cn

PHP:  getcwd();
来源：http://lqq.cqqwz.cn

JS:   process.cwd()
来源：http://lft.shanyushiyangtech.top

TS:   process.cwd()
来源：http://ixb.sxryk.cn

Java: Path.of("").toAbsolutePath()
来源：http://jeh.xingfuxueyuan.xyz

Go:   os.Getwd()
来源：http://bkh.aizwys.cn

Ruby: Dir.pwd
来源：http://apy.wangdashe.top

C#:   Directory.GetCurrentDirectory()
来源：http://ker.sufxvd.cn

[M05] 设置退出码
来源：http://qjx.haohaochexian.top

Py:   sys.exit(1)
来源：http://tdi.tianlin.xyz

PHP:  exit(1);
来源：http://rky.sjlbkw.cn

JS:   process.exit(1)
来源：http://dlu.redwolf501.top

TS:   process.exit(1)
来源：http://imh.dianchejie.cn

Java: System.exit(1)
来源：http://yju.yueranfly.top

Go:   os.Exit(1)
来源：http://hvq.c1oappe.top

Ruby: exit 1
来源：http://vzw.birdmap.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://emf.xziqi.cn

[M06] 向标准错误输出
来源：http://jgs.guannengcc.top

Py:   print("err", file=sys.stderr)
来源：http://kmh.mhx1999.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ocg.yongpay.top

JS:   console.error("err")
来源：http://nzh.nanxuanxn.top

TS:   console.error("err")
来源：http://czw.jinqigfzy.top

Java: System.err.println("err")
来源：http://rag.316326.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vvp.aizwys.cn

Ruby: warn "err"
来源：http://rlp.hywenlv.cn

C#:   Console.Error.WriteLine("err")
来源：http://wms.jlsjyb.cn

[M07] 判断是否为主入口
来源：http://nbb.guowangkeji.top


<!-- 参考信息 -->
代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://brs.xingfuxueyuan.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zfn.zdbjq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ybj.ywan-chungtsiang.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://vlp.gzhubu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qyd.yangfankeji.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kpl.hnqzz.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://aav.svipenyu.cn

================================================================================
来源：http://vuf.zdbjq.cn

J. 日期与时间
来源：http://jvc.hysaishi.cn

================================================================================
来源：http://yvo.tarul.cn

[J01] 获取当前时间
来源：http://lap.hongshengwenyu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://sfc.yonumen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fus.dashuyun.cn

JS:   new Date();  Date.now()
来源：http://woz.sxryk.cn

TS:   new Date();  Date.now()
来源：http://tsi.vehdjk.com

Java: LocalDateTime.now();  Instant.now()
来源：http://fij.yonumen.top

Go:   time.Now()
来源：http://lnl.bjfxy.top

Ruby: Time.now
来源：http://zwj.yj20258888.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qyg.zhoulong.xyz

[J02] 格式化输出
来源：http://iau.hfpthk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kuk.cashguo.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tza.yueranfly.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hhy.yanxiufei.cn

TS:   d.toISOString()
来源：http://pmr.jianghu66.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dcr.xziqi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://olw.ivvv.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tue.gzhubu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ynh.xuetiantiany.cn

[J03] 字符串解析为日期
来源：http://sqe.gzhubu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xie.cashguo.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iza.dianchejie.cn

JS:   new Date("2024-01-02")
来源：http://klr.ywan-chungtsiang.top

TS:   new Date("2024-01-02")
来源：http://nwr.aibaodan.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jei.fzhhl.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fuc.cucudq.cn

Ruby: Date.parse("2024-01-02")
来源：http://jzd.jqgufenzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dpp.dashuyun.cn

[J04] 时间戳与日期互转
来源：http://uim.meibo888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vuk.yanxiufei.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ewi.xylfe.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bgs.tianlin.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://qbz.hfpthk.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pas.ydjk.org.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rax.hywenlv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://spe.fzhhl.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qac.cucudq.cn

[J05] 时间加减（加 7 天）
来源：http://yll.hysaishi.cn

Py:   now + timedelta(days=7)
来源：http://ayp.wangshuangyany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://upf.dianchejie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zxk.nanxuanxn.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hot.sysykeji.top

Java: LocalDate.now().plusDays(7)
来源：http://umq.hcnkem.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dcg.svipenyu.cn

Ruby: Time.now + 7 * 86400
来源：http://ssb.jianghu66.top

C#:   DateTime.Now.AddDays(7)
来源：http://qev.9152youxi.cn

[J06] 计算两时间之差
来源：http://kgv.sjlbkw.cn

Py:   (end - start).total_seconds()
来源：http://mst.kuanghao11.cn

PHP:  $end->diff($start)->days;
来源：http://gim.smart0.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xja.quarkkingdee.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vbw.jinyuanbaomall.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wds.cashguo.top

Go:   end.Sub(start).Hours()
来源：http://tsx.yanxiufei.cn

Ruby: end - start                 # 返回秒数
来源：http://gin.sweek.top

C#:   (end - start).TotalSeconds
来源：http://hbi.zhiwuduotai.top

[J07] 比较两个日期
来源：http://kia.jqgfzy.top

Py:   d1 < d2;  d1 == d2
来源：http://rrx.yfazqb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ilq.sxryk.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rfx.feifeiyinyue.top

TS:   d1.getTime() < d2.getTime()
来源：http://ccn.jqgfzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mov.zhoulong.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zwm.gzhubu.top

Ruby: d1 < d2;  d1 == d2
来源：http://yss.shanyushiyangtech.top

C#:   d1 < d2;  d1 == d2
来源：http://dju.sufxvd.cn

[J08] 提取年月日与星期
来源：http://isn.nanxinkj.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rxb.jinyuanbaomall.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mtt.zhoulong.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://epk.shangyingyoupin.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://apt.tarul.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hgx.vqdsnc.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://asz.ehwqpu.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pqo.shanyushiyangtech.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ggb.jinqigfzy.top

[J09] 时区处理
来源：http://eiy.zhijiandao.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://buw.meibo888.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wvc.jqgufenzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jim.0kj1m.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://avn.gzhubu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gxx.cashguo.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dzo.hnxiangtu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kmv.yongpay.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://npn.xuetiantiany.cn

[J10] 取今天 / 本月第一天
来源：http://cuy.dianchejie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://auk.guannengcc.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vxz.yj20258888.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://day.tianlin.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vjl.yuanzhike.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hyj.jqgufenzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://beq.yueranfly.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uin.daria6918.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://def.nwbrower.top

================================================================================
来源：http://ged.yueranfly.top

K. JSON 与序列化
来源：http://oxl.9152youxi.cn

================================================================================
来源：http://xdh.gotoacloud.top

[K01] 对象转 JSON 字符串
来源：http://uiw.meibo888.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mhv.cdnleiting.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://enw.fanxiaobao.xyz

JS:   JSON.stringify(obj)
来源：http://rlv.xuetiantiany.cn

TS:   JSON.stringify(obj)
来源：http://tgj.hammf.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zew.quarkkingdee.top

Go:   json.Marshal(obj)
来源：http://aov.wangshuangyany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pyp.nanxinkj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://uhe.sxryk.cn

[K02] JSON 字符串转对象
来源：http://jor.zhiwuduotai.top

Py:   json.loads(s)
来源：http://ebq.havefunace.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vvt.cashguo.top

JS:   JSON.parse(s)
来源：http://sjo.jinyuanbaomall.cn

TS:   JSON.parse(s)
来源：http://zik.shanyushiyangtech.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wqu.svipenyu.cn

Go:   json.Unmarshal(data, &v)
来源：http://nve.zhiwuduotai.top

Ruby: JSON.parse(s)
来源：http://byl.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ifu.smart0.xyz

[K03] JSON 美化输出（带缩进）
来源：http://ukk.sjlbkw.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rzt.nanxinkj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xwe.gogol.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vwj.quarkkingdee.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xaz.fanxiaobao.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jcs.yfazqb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uhg.svipenyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lhe.vehdjk.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lxu.jinqigufen.top

[K04] 读取 JSON 文件
来源：http://qgx.shzxlz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bnt.sysykeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://evu.kuanghao11.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sen.fzhhl.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://okz.haohaochexian.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hgy.gzhubu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vur.sysykeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jph.pengpengdd.cyou

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dfg.zycfv.cn

[K05] 深拷贝对象
来源：http://rvj.pycfn.com

Py:   copy.deepcopy(obj)
来源：http://edc.iojbl.cn

PHP:  unserialize(serialize($obj));
来源：http://qfb.hnqzz.top

JS:   structuredClone(obj)
来源：http://cog.yj20258888.top

TS:   structuredClone(obj)
来源：http://cro.fktsv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://geb.vqdsnc.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ynq.epnwcf.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kjl.shanyushiyangtech.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ezd.yvedp.cn

[K06] 解析 URL 查询串
来源：http://vjh.nanxuanxn.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xiv.sufxvd.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wjy.hywenlv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xao.guannengcc.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xda.jqgfzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ksl.fengsongda.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ena.ivvv.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://skm.yvedp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ejl.birdmap.top

[K07] 进制转换
来源：http://ouq.fengsongda.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wbs.birdmap.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fll.tarul.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jor.fengsongda.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oon.tianlin.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qdr.fzhhl.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://msu.0kj1m.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dsy.daxiang520.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lbh.jinqigfzy.top

[K08] 二进制序列化（非 JSON）
来源：http://lkw.9152youxi.cn

Py:   pickle.dumps(obj)
来源：http://kdb.guowangkeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zca.zhixingplan.top

JS:   v8.serialize(obj)        // Node
来源：http://oxq.xuanzx.com

TS:   v8.serialize(obj)        // Node
来源：http://kjb.ehwqpu.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://eqa.xziqi.cn

Go:   encoding/gob
来源：http://wef.jianghu66.top

Ruby: Marshal.dump(obj)
来源：http://wrb.hnqzz.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uhs.316326.xyz

================================================================================
来源：http://zff.nanxuanxn.top

L. 网络请求
来源：http://din.kuanghao11.cn

================================================================================
来源：http://ydo.ehwqpu.com

[L01] 发送 GET 请求
来源：http://cag.zhiwuduotai.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sum.yfazqb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uyq.gzhubu.top

JS:   await fetch(url)
来源：http://ofh.jinqigfzy.top

TS:   await fetch(url)
来源：http://pqv.fzhhl.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vhd.yuanzhike.top

Go:   resp, err := http.Get(url)
来源：http://tez.hcnkem.com

Ruby: Net::HTTP.get(URI(url))
来源：http://xzy.nanxinkj.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dwy.zhongyouzk.top

[L02] 发送 POST JSON
来源：http://jmi.yanxiufei.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xow.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fae.xziqi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uql.iojbl.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://miy.yj202588.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xjh.zhiwuduotai.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://unc.tarul.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rdy.fktsv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://odl.jianghu66.top

[L03] 设置自定义请求头
来源：http://byn.tianlin.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fgy.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zup.xuetiantiany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pau.aibaodan.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xjf.hnqzz.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://otq.vqdsnc.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://imi.chenlongwang.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gpq.zhaomingkeji.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iqn.fktsv.cn

[L04] 设置超时
来源：http://vko.gaohongyu789.top

Py:   requests.get(url, timeout=5)
来源：http://cyu.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nir.ydjk.org.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jen.tianlin.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nac.fengsongda.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://seg.316326.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dlf.birdmap.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uix.jlsjyb.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://guq.bbcook.cn

[L05] 上传文件（multipart）
来源：http://mak.xuetiantiany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zlb.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nwl.ydzc1.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fcx.havefunace.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xyo.fengsongda.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oqj.hfpthk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://snq.zhongyouzk.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ruw.hnqzz.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://okf.yuanzhike.top

[L06] 解析响应为 JSON
来源：http://mjj.jqgfzy.top

Py:   resp.json()
来源：http://dlp.zhengqikj.top

PHP:  json_decode($body, true);
来源：http://zyq.jyoumei.cn

JS:   await resp.json()
来源：http://pcc.zhiwuduotai.top

TS:   await resp.json()
来源：http://qxb.tian-w.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sfd.bbcook.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pno.shanyushiyangkeji.top

Ruby: JSON.parse(resp.body)
来源：http://kiu.0kj1m.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mch.daxiang520.top

[L07] 处理 HTTP 状态码
来源：http://kvd.xylfe.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dqz.xylfe.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zvh.sweek.top

JS:   resp.ok;  resp.status
来源：http://wfg.ivvv.top

TS:   resp.ok;  resp.status
来源：http://epu.fktsv.cn

Java: resp.statusCode()
来源：http://rzy.fktsv.cn

Go:   resp.StatusCode
来源：http://wdt.fehbvm.com

Ruby: resp.code.to_i
来源：http://ujq.ydzc1.top

C#:   (int)resp.StatusCode
来源：http://mhm.hongshengwenyu.top

[L08] 并发请求多个地址
来源：http://qfr.hywenlv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://doq.zhoulong.xyz

PHP:  curl_multi_init() 系列
来源：http://mwy.cheryme.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mrh.yj20258888.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ilv.jinyuanbaomall.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rzg.zhengqikj.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yow.epnwcf.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uti.shanyushiyangtech.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fap.zhaomingkeji.xyz

================================================================================
来源：http://cjj.yonumen.top

M. 命令行 / 进程 / 环境
来源：http://zwo.havefunace.top

================================================================================
来源：http://fry.quarkkingdee.top

[M01] 读取命令行参数
来源：http://jkc.sufxvd.cn

Py:   sys.argv[1:]
来源：http://qhm.gzhubu.top

PHP:  $argv;  $argc;
来源：http://zwe.shangyingyoupin.top

JS:   process.argv.slice(2)
来源：http://ygg.ctjpmb.com

TS:   process.argv.slice(2)
来源：http://dpt.pengpengdd.cyou

Java: args 数组（main 方法参数）
来源：http://xel.tarul.cn

Go:   os.Args[1:]
来源：http://ogo.ppjwa.cn

Ruby: ARGV
来源：http://lac.dashuyun.cn

C#:   args 数组（Main 方法参数）
来源：http://ukk.ywan-chungtsiang.top

[M02] 读取环境变量
来源：http://eqb.havefunace.top

Py:   os.environ.get("HOME")
来源：http://loj.xylfe.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uhx.hongshengwenyu.top

JS:   process.env.HOME
来源：http://jwp.smart0.xyz

TS:   process.env.HOME
来源：http://huv.jiagoushi.top

Java: System.getenv("HOME")
来源：http://jbi.chenlongwang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kaj.svipenyu.cn

Ruby: ENV["HOME"]
来源：http://ine.vehdjk.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lir.bjfxy.top

[M03] 执行外部命令
来源：http://pdm.vqdsnc.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nqh.tarul.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cce.xylfe.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jna.sufxvd.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://naq.chenlongwang.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mvg.iojbl.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dre.pycfn.com

Ruby: system("ls -l");  `ls -l`
来源：http://oip.gogol.net.cn

C#:   Process.Start("ls", "-l");
来源：http://xzs.hesvh.cn

[M04] 获取当前工作目录
来源：http://gqz.yangfankeji.com

Py:   os.getcwd()
来源：http://lrk.zhaomingkeji.xyz

PHP:  getcwd();
来源：http://npu.xylfe.cn

JS:   process.cwd()
来源：http://qoy.xuetiantiany.cn

TS:   process.cwd()
来源：http://wwf.yuanzhike.top

Java: Path.of("").toAbsolutePath()
来源：http://yvp.ywan-chungtsiang.top

Go:   os.Getwd()
来源：http://vxi.jqgfzy.top

Ruby: Dir.pwd
来源：http://kiz.bjfxy.top

C#:   Directory.GetCurrentDirectory()
来源：http://thj.chenjidiqi.icu

[M05] 设置退出码
来源：http://twl.sysykeji.top

Py:   sys.exit(1)
来源：http://vxx.shzxlz.cn

PHP:  exit(1);
来源：http://lmv.meibo888.top

JS:   process.exit(1)
来源：http://ehn.wangdashe.top

TS:   process.exit(1)
来源：http://dkv.tarul.cn

Java: System.exit(1)
来源：http://isc.mhx1999.top

Go:   os.Exit(1)
来源：http://bgt.cashguo.top

Ruby: exit 1
来源：http://qvk.ybcxt.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://znh.aibaodan.cn

[M06] 向标准错误输出
来源：http://nyy.dashuyun.cn

Py:   print("err", file=sys.stderr)
来源：http://yas.vehdjk.com


<!-- 参考信息 -->
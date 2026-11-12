代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rml.zhiwuduotai.top

JS:   new Date();  Date.now()
来源：http://wvo.cqqwz.cn

TS:   new Date();  Date.now()
来源：http://gyq.yueranfly.top

Java: LocalDateTime.now();  Instant.now()
来源：http://woh.jqgfzy.top

Go:   time.Now()
来源：http://xgh.52xcode.cn

Ruby: Time.now
来源：http://zrk.fzhhl.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cxq.yonumen.top

[J02] 格式化输出
来源：http://bhh.jinqigfzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fuk.c1oappe.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://soa.tanke756.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qcn.shangyingyoupin.top

TS:   d.toISOString()
来源：http://guk.hesvh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hjf.c1oappe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qxk.wangdashe.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://klc.sweek.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nmr.yueranfly.top

[J03] 字符串解析为日期
来源：http://pnv.fengsongda.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sxa.sxryk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://igg.wangshuangyany.cn

JS:   new Date("2024-01-02")
来源：http://xmt.fanxiaobao.xyz

TS:   new Date("2024-01-02")
来源：http://lcd.yfazqb.com

Java: LocalDate.parse("2024-01-02")
来源：http://juo.shanyushiyangtech.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tht.jyoumei.cn

Ruby: Date.parse("2024-01-02")
来源：http://cmu.feifeiyinyue.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oop.yvedp.cn

[J04] 时间戳与日期互转
来源：http://wgf.kuanghao11.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vbg.jianghu66.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xen.jiagoushi.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tjx.xingfuxueyuan.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://lhj.daxiang520.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gcd.xinyue.icu

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oku.tarul.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mal.jianghu66.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://syv.jianghu66.top

[J05] 时间加减（加 7 天）
来源：http://vmq.vehdjk.com

Py:   now + timedelta(days=7)
来源：http://nsu.shangyingyoupin.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jnj.wangshuangyany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ivk.sxryk.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hpw.dashuyun.cn

Java: LocalDate.now().plusDays(7)
来源：http://etg.ybcxt.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ljs.birdmap.top

Ruby: Time.now + 7 * 86400
来源：http://igx.zhaomingkeji.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://gjc.epnwcf.com

[J06] 计算两时间之差
来源：http://hhl.gzhubu.top

Py:   (end - start).total_seconds()
来源：http://yjc.jinqigfzy.top

PHP:  $end->diff($start)->days;
来源：http://qms.snrcjt.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dhj.sysykeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bpz.haohaochexian.top

Java: Duration.between(start, end).toSeconds()
来源：http://lnq.chenzaomai.com

Go:   end.Sub(start).Hours()
来源：http://jup.nanxuanxn.top

Ruby: end - start                 # 返回秒数
来源：http://civ.jyoumei.cn

C#:   (end - start).TotalSeconds
来源：http://mhw.yangfankeji.com

[J07] 比较两个日期
来源：http://xdw.dianchejie.cn

Py:   d1 < d2;  d1 == d2
来源：http://iis.zhaomingkeji.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hon.zhixingplan.top

JS:   d1.getTime() < d2.getTime()
来源：http://mbt.cqqwz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tkj.yfazqb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://utc.pengpengdd.cyou

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qxf.gaohongyu789.top

Ruby: d1 < d2;  d1 == d2
来源：http://vzb.chenlongwang.top

C#:   d1 < d2;  d1 == d2
来源：http://eit.ywan-chungtsiang.top

[J08] 提取年月日与星期
来源：http://qzv.yuanzhike.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nmm.redwolf501.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://run.cucudq.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dtp.pengpengdd.cyou

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ubt.andypj.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zmq.hnqzz.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mum.jianghu66.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ooz.fehbvm.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lzv.smart0.xyz

[J09] 时区处理
来源：http://bgk.hnqzz.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rtr.nwbrower.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nhy.xziqi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qum.yj20258.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xlm.yj20258.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://reb.hysaishi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://iav.xuetiantiany.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jbc.gotoacloud.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hli.shuidangran.top

[J10] 取今天 / 本月第一天
来源：http://jii.tian-w.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wkb.chenlongwang.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xnd.tarul.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ild.yongpay.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://luq.zhongyouzk.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://agu.kuanghao11.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nox.316326.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://chi.chenzaomai.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ktl.ydjk.org.cn

================================================================================
来源：http://pjc.shanyushiyangtech.top

K. JSON 与序列化
来源：http://khk.cashguo.top

================================================================================
来源：http://vsr.yuxming.cn

[K01] 对象转 JSON 字符串
来源：http://why.redwolf501.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lhm.ybcxt.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zgm.yj202588.top

JS:   JSON.stringify(obj)
来源：http://awg.hysaishi.cn

TS:   JSON.stringify(obj)
来源：http://iik.shanyushiyangtech.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ypz.jiagoushi.top

Go:   json.Marshal(obj)
来源：http://nvr.hcnkem.com

Ruby: obj.to_json                                     // require "json"
来源：http://wvq.fktsv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://faq.andypj.xyz

[K02] JSON 字符串转对象
来源：http://xsx.aibaodan.cn

Py:   json.loads(s)
来源：http://ctu.jqgfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wmd.jlsjyb.cn

JS:   JSON.parse(s)
来源：http://vvn.gogol.net.cn

TS:   JSON.parse(s)
来源：http://pcr.yuxming.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ijh.ppjwa.cn

Go:   json.Unmarshal(data, &v)
来源：http://vfz.xziqi.cn

Ruby: JSON.parse(s)
来源：http://dmp.jlsjyb.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rpp.zdbjq.cn

[K03] JSON 美化输出（带缩进）
来源：http://oqs.yanxiufei.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vbj.bjfxy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pen.fehbvm.com

JS:   JSON.stringify(obj, null, 2)
来源：http://yfc.zhaomingkeji.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://ajc.yangfankeji.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ioy.hnqzz.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ggv.mhx1999.top

Ruby: JSON.pretty_generate(obj)
来源：http://tka.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cle.cqqwz.cn

[K04] 读取 JSON 文件
来源：http://fiw.snrcjt.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nzs.birdmap.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jik.yueranfly.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://otx.ctjpmb.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hmx.cheryme.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://olc.mhx1999.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rtw.cdnleiting.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://dhs.shanyushiyangtech.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jgi.ivvv.top

[K05] 深拷贝对象
来源：http://xdc.zhijiandao.cn

Py:   copy.deepcopy(obj)
来源：http://asg.fktsv.cn

PHP:  unserialize(serialize($obj));
来源：http://qzo.316326.xyz

JS:   structuredClone(obj)
来源：http://mot.ivvv.top

TS:   structuredClone(obj)
来源：http://oyy.nwbrower.top

Java: // 手写拷贝构造，或序列化往返
来源：http://onm.hnxiangtu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mzr.fengsongda.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ihb.meibo888.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fwn.ppjwa.cn

[K06] 解析 URL 查询串
来源：http://cta.ppjwa.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bfw.fengsongda.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tav.ywan-chungtsiang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uhk.xziqi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ijx.haohaochexian.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cay.chenlongwang.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://dse.zhongyouzk.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bhn.zycfv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lrn.yj20258888.top

[K07] 进制转换
来源：http://rco.0kj1m.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jhb.jinghuilouyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://byx.ywan-chungtsiang.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://byt.wangdashe.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ank.tianlin.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://akc.epnwcf.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sxd.jqgfzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rqq.nwbrower.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rig.bjfxy.top

[K08] 二进制序列化（非 JSON）
来源：http://sea.ybcxt.top

Py:   pickle.dumps(obj)
来源：http://qym.andypj.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://ifm.gaohongyu789.top

JS:   v8.serialize(obj)        // Node
来源：http://jzw.shangyingyoupin.top

TS:   v8.serialize(obj)        // Node
来源：http://ttf.kuanghao11.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lps.shuidangran.top

Go:   encoding/gob
来源：http://vup.meibo888.top

Ruby: Marshal.dump(obj)
来源：http://jxh.nanxuanxn.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mkh.hywenlv.cn

================================================================================
来源：http://fos.cucudq.cn

L. 网络请求
来源：http://vop.kuanghao11.cn

================================================================================
来源：http://buw.ivvv.top

[L01] 发送 GET 请求
来源：http://pfz.yanxiufei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ylc.wangdashe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kpu.mhx1999.top

JS:   await fetch(url)
来源：http://hho.nanxuanxn.top

TS:   await fetch(url)
来源：http://cyu.zhongyouzk.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xgv.shanyushiyangkeji.top

Go:   resp, err := http.Get(url)
来源：http://ngy.yj202588.top

Ruby: Net::HTTP.get(URI(url))
来源：http://uhd.havefunace.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jfr.jinyuanbaomall.cn

[L02] 发送 POST JSON
来源：http://oam.zhiwuduotai.top

Py:   requests.post(url, json={"a": 1})
来源：http://pbe.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mog.zhijiandao.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://khk.havefunace.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mzj.yfazqb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cbr.pycfn.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yiu.zhengqikj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qhu.xuanzx.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vbn.yvedp.cn

[L03] 设置自定义请求头
来源：http://omv.chenzaomai.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pnl.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mvn.jiagoushi.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pgi.ppjwa.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ewd.hfpthk.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wtn.fzhhl.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nzz.cqqwz.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tfm.hnxiangtu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jhs.shuidangran.top

[L04] 设置超时
来源：http://nxz.zhoulong.xyz

Py:   requests.get(url, timeout=5)
来源：http://zyd.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://eat.shangyingyoupin.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uoi.fktsv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ycl.wangdashe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mbd.quarkkingdee.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uhq.52xcode.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://muk.jinyuanbaomall.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pqc.xziqi.cn

[L05] 上传文件（multipart）
来源：http://hvo.shangyingyoupin.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nbv.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://glm.hnqzz.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bwe.wangdashe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bia.c1oappe.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ogh.redwolf501.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yrf.9152youxi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tsv.xuetiantiany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tzb.uphjek.com

[L06] 解析响应为 JSON
来源：http://szr.aizwys.cn

Py:   resp.json()
来源：http://txa.fehbvm.com

PHP:  json_decode($body, true);
来源：http://egw.hywenlv.cn

JS:   await resp.json()
来源：http://uae.zhaomingkeji.xyz

TS:   await resp.json()
来源：http://duo.guannengcc.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vyz.hnxiangtu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pdc.zhijiandao.cn

Ruby: JSON.parse(resp.body)
来源：http://ykj.yongpay.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ttp.ctjpmb.com

[L07] 处理 HTTP 状态码
来源：http://tfm.nanxuanxn.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dsc.chenzaomai.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dop.sjlbkw.cn

JS:   resp.ok;  resp.status
来源：http://imw.shanyushiyangkeji.top

TS:   resp.ok;  resp.status
来源：http://prs.daxiang520.top

Java: resp.statusCode()
来源：http://sck.shuidangran.top

Go:   resp.StatusCode
来源：http://ihr.hcnkem.com

Ruby: resp.code.to_i
来源：http://ghp.yfazqb.com

C#:   (int)resp.StatusCode
来源：http://vii.fengsongda.top

[L08] 并发请求多个地址
来源：http://ihs.xingfuxueyuan.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ang.gzhubu.top

PHP:  curl_multi_init() 系列
来源：http://bmf.zhaomingkeji.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qgr.dashuyun.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gqf.jinqigfzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nyv.aibaodan.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ych.ydzc1.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cha.ybcxt.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qtk.gotoacloud.top

================================================================================
来源：http://heh.zdqjudy.top

M. 命令行 / 进程 / 环境
来源：http://dja.kuanghao11.cn

================================================================================
来源：http://kcx.yongpay.top

[M01] 读取命令行参数
来源：http://abo.ppjwa.cn

Py:   sys.argv[1:]
来源：http://gyr.redwolf501.top

PHP:  $argv;  $argc;
来源：http://xhq.zhaomingkeji.xyz

JS:   process.argv.slice(2)
来源：http://uii.daxiang520.top

TS:   process.argv.slice(2)
来源：http://uik.yongpay.top

Java: args 数组（main 方法参数）
来源：http://vcl.cqqwz.cn

Go:   os.Args[1:]
来源：http://ftm.c1oappe.top

Ruby: ARGV
来源：http://vne.sysykeji.top

C#:   args 数组（Main 方法参数）
来源：http://fqg.pengpengdd.cyou

[M02] 读取环境变量
来源：http://and.xuetiantiany.cn

Py:   os.environ.get("HOME")
来源：http://lod.316326.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zwt.chenjidiqi.icu

JS:   process.env.HOME
来源：http://hrf.c1oappe.top

TS:   process.env.HOME
来源：http://rse.dashuyun.cn

Java: System.getenv("HOME")
来源：http://hfp.jiagoushi.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mss.cheryme.top

Ruby: ENV["HOME"]
来源：http://msh.ppjwa.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xny.fengsongda.top

[M03] 执行外部命令
来源：http://wcx.nanxuanxn.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gvh.xuetiantiany.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fdr.haohaochexian.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vlc.gogol.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zan.zdbjq.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://omd.jinghuilouyu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tav.svipenyu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qqh.jinqigfzy.top

C#:   Process.Start("ls", "-l");
来源：http://fcg.wangdashe.top

[M04] 获取当前工作目录
来源：http://fuz.chenjidiqi.icu

Py:   os.getcwd()
来源：http://cix.hammf.cn

PHP:  getcwd();
来源：http://wib.ivvv.top

JS:   process.cwd()
来源：http://emz.chenlongwang.top

TS:   process.cwd()
来源：http://wlb.fanxiaobao.xyz

Java: Path.of("").toAbsolutePath()
来源：http://cgx.cheryme.top

Go:   os.Getwd()
来源：http://ecw.yangfankeji.com

Ruby: Dir.pwd
来源：http://evh.cheryme.top

C#:   Directory.GetCurrentDirectory()
来源：http://yaw.sysykeji.top

[M05] 设置退出码
来源：http://nti.dianchejie.cn

Py:   sys.exit(1)
来源：http://aak.xingfuxueyuan.xyz

PHP:  exit(1);
来源：http://mwp.52xcode.cn

JS:   process.exit(1)
来源：http://moc.xylfe.cn

TS:   process.exit(1)
来源：http://lmb.sysykeji.top

Java: System.exit(1)
来源：http://wde.chenlongwang.top

Go:   os.Exit(1)
来源：http://zbo.pycfn.com

Ruby: exit 1
来源：http://nsy.bbcook.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://enc.jqgfzy.top

[M06] 向标准错误输出
来源：http://ntj.yvedp.cn

Py:   print("err", file=sys.stderr)
来源：http://dtm.pycfn.com

PHP:  fwrite(STDERR, "err\n");
来源：http://mbf.yj202588.top

JS:   console.error("err")
来源：http://caw.ywan-chungtsiang.top

TS:   console.error("err")
来源：http://xwk.fanxiaobao.xyz

Java: System.err.println("err")
来源：http://lkw.9152youxi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fdf.jyoumei.cn

Ruby: warn "err"
来源：http://iri.wangshuangyany.cn

C#:   Console.Error.WriteLine("err")
来源：http://mmb.pycfn.com

[M07] 判断是否为主入口
来源：http://dop.cqqwz.cn

Py:   if __name__ == "__main__":
来源：http://ycd.hesvh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://omo.yuxming.cn

JS:   require.main === module
来源：http://qtm.pycfn.com

TS:   require.main === module
来源：http://dft.zdqjudy.top


<!-- 参考信息 -->
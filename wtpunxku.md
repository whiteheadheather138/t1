代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bdv.ydjk.org.cn

JS:   new Date();  Date.now()
来源：http://jns.vehdjk.com

TS:   new Date();  Date.now()
来源：http://mqj.fehbvm.com

Java: LocalDateTime.now();  Instant.now()
来源：http://dtk.yangfankeji.com

Go:   time.Now()
来源：http://ulb.haohaochexian.top

Ruby: Time.now
来源：http://isg.sufxvd.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sts.wangshuangyany.cn

[J02] 格式化输出
来源：http://bho.yangfankeji.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yxl.yj20258.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://avo.shangyingyoupin.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nfq.daxiang520.top

TS:   d.toISOString()
来源：http://bqv.feifeiyinyue.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tjj.daria6918.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wmx.vehdjk.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hxm.hnqzz.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ecj.daria6918.cn

[J03] 字符串解析为日期
来源：http://woi.epnwcf.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qeh.tanke756.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jnx.yfazqb.com

JS:   new Date("2024-01-02")
来源：http://qrz.zdbjq.cn

TS:   new Date("2024-01-02")
来源：http://pky.yonumen.top

Java: LocalDate.parse("2024-01-02")
来源：http://wxm.redwolf501.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://idu.zhengqikj.top

Ruby: Date.parse("2024-01-02")
来源：http://rou.hnqzz.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hqu.hysaishi.cn

[J04] 时间戳与日期互转
来源：http://nnv.bbcook.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uon.cqqwz.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zsz.ywan-chungtsiang.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mce.9152youxi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gcm.sweek.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vbo.ivvv.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fiz.pengpengdd.cyou

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://erb.andypj.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ocx.zhiwuduotai.top

[J05] 时间加减（加 7 天）
来源：http://szh.wangshuangyany.cn

Py:   now + timedelta(days=7)
来源：http://zyu.chenzaomai.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://xvo.bjfxy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ext.gogol.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uti.zdqjudy.top

Java: LocalDate.now().plusDays(7)
来源：http://nsd.xuetiantiany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ypq.yuanzhike.top

Ruby: Time.now + 7 * 86400
来源：http://qnk.nanxinkj.top

C#:   DateTime.Now.AddDays(7)
来源：http://llo.cqqwz.cn

[J06] 计算两时间之差
来源：http://wnm.jlsjyb.cn

Py:   (end - start).total_seconds()
来源：http://pag.smart0.xyz

PHP:  $end->diff($start)->days;
来源：http://sps.shuidangran.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zex.gzhubu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://suo.sjlbkw.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dew.bjfxy.top

Go:   end.Sub(start).Hours()
来源：http://tqn.birdmap.top

Ruby: end - start                 # 返回秒数
来源：http://nwg.iojbl.cn

C#:   (end - start).TotalSeconds
来源：http://kpk.cucudq.cn

[J07] 比较两个日期
来源：http://bcn.shangyingyoupin.top

Py:   d1 < d2;  d1 == d2
来源：http://zpz.0kj1m.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://def.jinqigfzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://rpe.jiagoushi.top

TS:   d1.getTime() < d2.getTime()
来源：http://caw.0kj1m.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qda.hnqzz.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cfm.chenlongwang.top

Ruby: d1 < d2;  d1 == d2
来源：http://hfh.yj20258.top

C#:   d1 < d2;  d1 == d2
来源：http://prw.ehwqpu.com

[J08] 提取年月日与星期
来源：http://qqo.zhiwuduotai.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mns.fengsongda.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://awl.tian-w.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://avi.aizwys.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uvw.wangdashe.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xdq.quarkkingdee.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xwu.gotoacloud.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://puw.sysykeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ahp.aibaodan.cn

[J09] 时区处理
来源：http://zzo.mhx1999.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://alx.shuidangran.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gwj.hnqzz.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bvh.zdbjq.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xpx.nwbrower.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://klc.cdnleiting.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mpi.zhengqikj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://lzh.hongshengwenyu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dfj.tianlin.xyz

[J10] 取今天 / 本月第一天
来源：http://wbp.yuxming.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cfa.zhoulong.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kip.zhixingplan.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uzl.ybcxt.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sqs.aizwys.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xyx.tanke756.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cvo.jinghuilouyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://axy.meibo888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dqm.zhiwuduotai.top

================================================================================
来源：http://efw.nwbrower.top

K. JSON 与序列化
来源：http://psz.aizwys.cn

================================================================================
来源：http://mxb.havefunace.top

[K01] 对象转 JSON 字符串
来源：http://din.quarkkingdee.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pjd.yanxiufei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rjp.fzhhl.top

JS:   JSON.stringify(obj)
来源：http://fdr.tian-w.cn

TS:   JSON.stringify(obj)
来源：http://aez.hywenlv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vuc.316326.xyz

Go:   json.Marshal(obj)
来源：http://ulz.shzxlz.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bcn.sxryk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ckp.epnwcf.com

[K02] JSON 字符串转对象
来源：http://mov.shanyushiyangtech.top

Py:   json.loads(s)
来源：http://buk.jianghu66.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qxd.gaohongyu789.top

JS:   JSON.parse(s)
来源：http://oyo.xinyue.icu

TS:   JSON.parse(s)
来源：http://jzb.52xcode.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pku.tanke756.top

Go:   json.Unmarshal(data, &v)
来源：http://yjd.dianchejie.cn

Ruby: JSON.parse(s)
来源：http://edx.ivvv.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cnl.zdbjq.cn

[K03] JSON 美化输出（带缩进）
来源：http://kcp.nwbrower.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wbw.daria6918.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qcz.pycfn.com

JS:   JSON.stringify(obj, null, 2)
来源：http://xzm.yfazqb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://uxk.aibaodan.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://trg.daxiang520.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vtu.yj20258888.top

Ruby: JSON.pretty_generate(obj)
来源：http://cib.fzhhl.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cba.tarul.cn

[K04] 读取 JSON 文件
来源：http://kyt.shanyushiyangtech.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pts.xylfe.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sbn.yj20258.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yyd.shuidangran.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://chv.bbcook.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bsx.gogol.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hit.andypj.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://apv.sufxvd.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zxp.xinyue.icu

[K05] 深拷贝对象
来源：http://wea.hcnkem.com

Py:   copy.deepcopy(obj)
来源：http://tjd.jqgufenzy.top

PHP:  unserialize(serialize($obj));
来源：http://vhj.yj202588.top

JS:   structuredClone(obj)
来源：http://ytk.nwbrower.top

TS:   structuredClone(obj)
来源：http://qqt.yj202588.top

Java: // 手写拷贝构造，或序列化往返
来源：http://hud.smart0.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zqr.tian-w.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fui.wangdashe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://yho.hnqzz.top

[K06] 解析 URL 查询串
来源：http://gju.ydjk.org.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vso.sjlbkw.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pvg.smart0.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xea.redwolf501.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pwf.gogol.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://luv.tarul.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rld.yfazqb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rlp.zhoulong.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://spf.yj20258.top

[K07] 进制转换
来源：http://phw.guannengcc.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://eou.yj20258888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rcm.birdmap.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ztn.c1oappe.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jey.ehwqpu.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jfm.ehwqpu.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://egl.jinyuanbaomall.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jft.pycfn.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://spl.vehdjk.com

[K08] 二进制序列化（非 JSON）
来源：http://awx.pengpengdd.cyou

Py:   pickle.dumps(obj)
来源：http://qhb.epnwcf.com

PHP:  serialize($obj);  unserialize($s);
来源：http://bgo.epnwcf.com

JS:   v8.serialize(obj)        // Node
来源：http://tll.hcnkem.com

TS:   v8.serialize(obj)        // Node
来源：http://zjx.shanyushiyangtech.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cuq.jyoumei.cn

Go:   encoding/gob
来源：http://cgw.cdnleiting.top

Ruby: Marshal.dump(obj)
来源：http://ofu.yj20258888.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gpq.jlsjyb.cn

================================================================================
来源：http://oqr.gogol.net.cn

L. 网络请求
来源：http://hot.cashguo.top

================================================================================
来源：http://hnj.tanke756.top

[L01] 发送 GET 请求
来源：http://tij.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kuk.xylfe.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bkr.sweek.top

JS:   await fetch(url)
来源：http://ibn.fehbvm.com

TS:   await fetch(url)
来源：http://rcx.vqdsnc.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jjj.fehbvm.com

Go:   resp, err := http.Get(url)
来源：http://rud.yj202588.top

Ruby: Net::HTTP.get(URI(url))
来源：http://bnz.xuetiantiany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://say.yuxming.cn

[L02] 发送 POST JSON
来源：http://cwr.9152youxi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bvw.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tht.zhengqikj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nkn.zycfv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://muv.uphjek.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zoh.zhijiandao.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jzl.redwolf501.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://raq.kuanghao11.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eub.bjfxy.top

[L03] 设置自定义请求头
来源：http://lna.aizwys.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ety.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://irj.nanxuanxn.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://psn.jinqigfzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hxb.quarkkingdee.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zlk.wangdashe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yvh.shanyushiyangtech.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vdv.sjlbkw.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tkt.yangfankeji.com

[L04] 设置超时
来源：http://ost.ivvv.top

Py:   requests.get(url, timeout=5)
来源：http://waw.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fbn.vqdsnc.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vyx.jinqigfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kkc.aibaodan.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://oiv.hnqzz.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ryf.feifeiyinyue.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lpu.haohaochexian.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uio.52xcode.cn

[L05] 上传文件（multipart）
来源：http://wit.yuxming.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hcn.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mer.yj20258888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://utt.yangfankeji.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://prv.fzhhl.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dce.shuidangran.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sef.9152youxi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kgm.nanxuanxn.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dvc.hesvh.cn

[L06] 解析响应为 JSON
来源：http://mzw.0kj1m.cn

Py:   resp.json()
来源：http://wdj.jinqigfzy.top

PHP:  json_decode($body, true);
来源：http://qkp.quarkkingdee.top

JS:   await resp.json()
来源：http://lyh.hysaishi.cn

TS:   await resp.json()
来源：http://tku.andypj.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://alo.dashuyun.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://czb.dianchejie.cn

Ruby: JSON.parse(resp.body)
来源：http://jry.snrcjt.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lhb.vqdsnc.cn

[L07] 处理 HTTP 状态码
来源：http://emm.zhijiandao.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vbe.bjfxy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dcc.52xcode.cn

JS:   resp.ok;  resp.status
来源：http://uzm.xuanzx.com

TS:   resp.ok;  resp.status
来源：http://xma.jinghuilouyu.cn

Java: resp.statusCode()
来源：http://mrq.uphjek.com

Go:   resp.StatusCode
来源：http://gcy.nanxuanxn.top

Ruby: resp.code.to_i
来源：http://pyh.gaohongyu789.top

C#:   (int)resp.StatusCode
来源：http://iqs.yanxiufei.cn

[L08] 并发请求多个地址
来源：http://wrh.fzhhl.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://etc.jiagoushi.top

PHP:  curl_multi_init() 系列
来源：http://zbh.yuanzhike.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hpi.iojbl.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xon.nanxinkj.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yoc.shanyushiyangtech.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hyw.tarul.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zot.gzhubu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://omx.zhijiandao.cn

================================================================================
来源：http://gqi.birdmap.top

M. 命令行 / 进程 / 环境
来源：http://xqb.chenjidiqi.icu

================================================================================
来源：http://tul.ybcxt.top

[M01] 读取命令行参数
来源：http://iwy.yfazqb.com

Py:   sys.argv[1:]
来源：http://yrz.chenzaomai.com

PHP:  $argv;  $argc;
来源：http://ets.zdqjudy.top

JS:   process.argv.slice(2)
来源：http://oiv.redwolf501.top

TS:   process.argv.slice(2)
来源：http://xxx.zhaomingkeji.xyz

Java: args 数组（main 方法参数）
来源：http://ccj.yongpay.top

Go:   os.Args[1:]
来源：http://gao.ydzc1.top

Ruby: ARGV
来源：http://dsc.jinqigufen.top

C#:   args 数组（Main 方法参数）
来源：http://syz.9152youxi.cn

[M02] 读取环境变量
来源：http://gop.hammf.cn

Py:   os.environ.get("HOME")
来源：http://lzb.aibaodan.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://che.xuanzx.com

JS:   process.env.HOME
来源：http://yas.jinghuilouyu.cn

TS:   process.env.HOME
来源：http://kuy.zhixingplan.top

Java: System.getenv("HOME")
来源：http://iyv.zhaomingkeji.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ddi.pengpengdd.cyou

Ruby: ENV["HOME"]
来源：http://wox.vqdsnc.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ewn.zycfv.cn

[M03] 执行外部命令
来源：http://mzs.haohaochexian.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kpl.tian-w.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://syi.xuanzx.com

JS:   child_process.execSync("ls -l").toString()
来源：http://jmv.tianlin.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://ulu.52xcode.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jrv.0kj1m.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://img.hnxiangtu.top

Ruby: system("ls -l");  `ls -l`
来源：http://ozw.xinyue.icu

C#:   Process.Start("ls", "-l");
来源：http://ddv.snrcjt.cn

[M04] 获取当前工作目录
来源：http://ygv.chenzaomai.com

Py:   os.getcwd()
来源：http://fwn.sjlbkw.cn

PHP:  getcwd();
来源：http://ztx.zhixingplan.top

JS:   process.cwd()
来源：http://ofy.zhijiandao.cn

TS:   process.cwd()
来源：http://ooe.feifeiyinyue.top

Java: Path.of("").toAbsolutePath()
来源：http://les.pengpengdd.cyou

Go:   os.Getwd()
来源：http://hxi.ydzc1.top

Ruby: Dir.pwd
来源：http://hds.snrcjt.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vxn.dashuyun.cn

[M05] 设置退出码
来源：http://dab.tarul.cn

Py:   sys.exit(1)
来源：http://chb.jinqigufen.top

PHP:  exit(1);
来源：http://rpn.cheryme.top

JS:   process.exit(1)
来源：http://nbl.zhixingplan.top

TS:   process.exit(1)
来源：http://gbr.jqgufenzy.top

Java: System.exit(1)
来源：http://gaw.aizwys.cn

Go:   os.Exit(1)
来源：http://pis.feifeiyinyue.top

Ruby: exit 1
来源：http://cxy.xinyue.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tla.nanxuanxn.top

[M06] 向标准错误输出
来源：http://khp.jqgufenzy.top

Py:   print("err", file=sys.stderr)
来源：http://zyi.zhongyouzk.top

PHP:  fwrite(STDERR, "err\n");
来源：http://uxv.aibaodan.cn

JS:   console.error("err")
来源：http://axu.fktsv.cn

TS:   console.error("err")
来源：http://vbn.snrcjt.cn

Java: System.err.println("err")
来源：http://xzq.uphjek.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dyg.ydjk.org.cn

Ruby: warn "err"
来源：http://ftv.zycfv.cn

C#:   Console.Error.WriteLine("err")
来源：http://sjr.cashguo.top

[M07] 判断是否为主入口
来源：http://njy.daxiang520.top

Py:   if __name__ == "__main__":
来源：http://jbg.c1oappe.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ylq.dianchejie.cn

JS:   require.main === module
来源：http://hfz.zdqjudy.top

TS:   require.main === module
来源：http://pwu.sysykeji.top


<!-- 参考信息 -->
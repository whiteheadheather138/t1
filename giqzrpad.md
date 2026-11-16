代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ixq.yongpay.top

JS:   new Date();  Date.now()
来源：http://cbi.sjlbkw.cn

TS:   new Date();  Date.now()
来源：http://fwf.feifeiyinyue.top

Java: LocalDateTime.now();  Instant.now()
来源：http://esp.nwbrower.top

Go:   time.Now()
来源：http://uzb.havefunace.top

Ruby: Time.now
来源：http://pky.zhengqikj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zus.xingfuxueyuan.xyz

[J02] 格式化输出
来源：http://yho.shzxlz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zpu.yuanzhike.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qxs.kuanghao11.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yrd.zhoulong.xyz

TS:   d.toISOString()
来源：http://xcw.tianlin.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vjz.yj20258888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wms.sjlbkw.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fbf.jinqigufen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rtl.fengsongda.top

[J03] 字符串解析为日期
来源：http://fiy.jlsjyb.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qvq.jinyuanbaomall.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zmu.tian-w.cn

JS:   new Date("2024-01-02")
来源：http://pmj.ydjk.org.cn

TS:   new Date("2024-01-02")
来源：http://sqm.sxryk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fiu.sjlbkw.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://waf.cashguo.top

Ruby: Date.parse("2024-01-02")
来源：http://duv.zdbjq.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://woe.uphjek.com

[J04] 时间戳与日期互转
来源：http://ltg.nanxuanxn.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fmv.wangdashe.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://erw.ydzc1.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ydr.wangshuangyany.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jmv.jianghu66.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://asm.yanxiufei.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bpq.shanyushiyangtech.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qhd.jqgufenzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ach.hesvh.cn

[J05] 时间加减（加 7 天）
来源：http://tft.fanxiaobao.xyz

Py:   now + timedelta(days=7)
来源：http://enf.yanxiufei.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://daf.wangshuangyany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gdr.feifeiyinyue.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gvl.bjfxy.top

Java: LocalDate.now().plusDays(7)
来源：http://gou.zhixingplan.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wkb.snrcjt.cn

Ruby: Time.now + 7 * 86400
来源：http://pjv.yuanzhike.top

C#:   DateTime.Now.AddDays(7)
来源：http://ajk.bbcook.cn

[J06] 计算两时间之差
来源：http://mcn.316326.xyz

Py:   (end - start).total_seconds()
来源：http://tpz.52xcode.cn

PHP:  $end->diff($start)->days;
来源：http://gxe.nanxinkj.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bxy.yuxming.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xmu.yj20258888.top

Java: Duration.between(start, end).toSeconds()
来源：http://aur.gzhubu.top

Go:   end.Sub(start).Hours()
来源：http://hhg.yuxming.cn

Ruby: end - start                 # 返回秒数
来源：http://lga.zhoulong.xyz

C#:   (end - start).TotalSeconds
来源：http://oti.chenjidiqi.icu

[J07] 比较两个日期
来源：http://qbe.xinyue.icu

Py:   d1 < d2;  d1 == d2
来源：http://due.kuanghao11.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uwl.jiagoushi.top

JS:   d1.getTime() < d2.getTime()
来源：http://plu.ydjk.org.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lqq.zdbjq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kld.yj20258888.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://awb.316326.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://wdz.zhijiandao.cn

C#:   d1 < d2;  d1 == d2
来源：http://tuj.kuanghao11.cn

[J08] 提取年月日与星期
来源：http://vnc.hfpthk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gge.wangdashe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kgm.jianghu66.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kqz.wangshuangyany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rpc.fengsongda.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xhf.zdqjudy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pev.316326.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aws.tian-w.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zkf.gzhubu.top

[J09] 时区处理
来源：http://nzj.52xcode.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://una.gotoacloud.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rak.c1oappe.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iun.daria6918.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nsw.yanxiufei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zjn.uphjek.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://opz.52xcode.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hgv.wangdashe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mxv.hfpthk.cn

[J10] 取今天 / 本月第一天
来源：http://nap.tianlin.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://zjc.andypj.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fbv.svipenyu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xll.hfpthk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://glj.yj202588.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pol.xinyue.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xge.xziqi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qrx.meibo888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gtv.fzhhl.top

================================================================================
来源：http://gox.guannengcc.top

K. JSON 与序列化
来源：http://euc.hnqzz.top

================================================================================
来源：http://ref.hnqzz.top

[K01] 对象转 JSON 字符串
来源：http://pen.tanke756.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wja.ehwqpu.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ijo.hfpthk.cn

JS:   JSON.stringify(obj)
来源：http://hme.tianlin.xyz

TS:   JSON.stringify(obj)
来源：http://ucc.guannengcc.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sgy.ydjk.org.cn

Go:   json.Marshal(obj)
来源：http://tai.hammf.cn

Ruby: obj.to_json                                     // require "json"
来源：http://odw.pycfn.com

C#:   JsonSerializer.Serialize(obj)
来源：http://mth.zhoulong.xyz

[K02] JSON 字符串转对象
来源：http://beq.uphjek.com

Py:   json.loads(s)
来源：http://yiv.fktsv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cfi.dashuyun.cn

JS:   JSON.parse(s)
来源：http://crx.yfazqb.com

TS:   JSON.parse(s)
来源：http://cqr.zdqjudy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ugh.pengpengdd.cyou

Go:   json.Unmarshal(data, &v)
来源：http://eqz.316326.xyz

Ruby: JSON.parse(s)
来源：http://dvs.sweek.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ywe.iojbl.cn

[K03] JSON 美化输出（带缩进）
来源：http://buk.ppjwa.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zqt.hcnkem.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hqv.birdmap.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dow.quarkkingdee.top

TS:   JSON.stringify(obj, null, 2)
来源：http://rcj.yj202588.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bil.yuxming.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fjf.aizwys.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vlo.jinyuanbaomall.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vyf.jlsjyb.cn

[K04] 读取 JSON 文件
来源：http://fuz.jiagoushi.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ipm.smart0.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xfy.jlsjyb.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vkh.cqqwz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ael.snrcjt.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qfg.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bns.guowangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://nnu.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ukf.hywenlv.cn

[K05] 深拷贝对象
来源：http://pvn.wangshuangyany.cn

Py:   copy.deepcopy(obj)
来源：http://nns.hnxiangtu.top

PHP:  unserialize(serialize($obj));
来源：http://msu.sysykeji.top

JS:   structuredClone(obj)
来源：http://skb.smart0.xyz

TS:   structuredClone(obj)
来源：http://ybi.zhijiandao.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gzm.cqqwz.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tau.zhengqikj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wth.jinyuanbaomall.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://izy.jqgufenzy.top

[K06] 解析 URL 查询串
来源：http://apa.yongpay.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tca.zhaomingkeji.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bys.andypj.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hcv.iojbl.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gwb.kuanghao11.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rfn.tian-w.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://guy.haohaochexian.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tzy.daxiang520.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zyg.epnwcf.com

[K07] 进制转换
来源：http://gwb.shanyushiyangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bum.uphjek.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://moo.zdqjudy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hjc.yangfankeji.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://auu.ivvv.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yhl.hongshengwenyu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nto.daria6918.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xkh.hnxiangtu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ezp.meibo888.top

[K08] 二进制序列化（非 JSON）
来源：http://rka.quarkkingdee.top

Py:   pickle.dumps(obj)
来源：http://mjx.guowangkeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xdu.yfazqb.com

JS:   v8.serialize(obj)        // Node
来源：http://evn.shzxlz.cn

TS:   v8.serialize(obj)        // Node
来源：http://enj.hysaishi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://npv.jianghu66.top

Go:   encoding/gob
来源：http://rig.dianchejie.cn

Ruby: Marshal.dump(obj)
来源：http://svy.bjfxy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://odu.ydjk.org.cn

================================================================================
来源：http://hlp.ywan-chungtsiang.top

L. 网络请求
来源：http://zpx.smart0.xyz

================================================================================
来源：http://vbw.0kj1m.cn

[L01] 发送 GET 请求
来源：http://vgu.yvedp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qlb.tanke756.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xoa.nwbrower.top

JS:   await fetch(url)
来源：http://dfr.sufxvd.cn

TS:   await fetch(url)
来源：http://vra.yangfankeji.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ram.tian-w.cn

Go:   resp, err := http.Get(url)
来源：http://oap.xuanzx.com

Ruby: Net::HTTP.get(URI(url))
来源：http://oef.yuanzhike.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yuj.chenlongwang.top

[L02] 发送 POST JSON
来源：http://kqr.wangdashe.top

Py:   requests.post(url, json={"a": 1})
来源：http://uko.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zkw.yfazqb.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kge.nanxuanxn.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://myv.pycfn.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://coe.havefunace.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jjx.sufxvd.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fpo.zhoulong.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ynw.daxiang520.top

[L03] 设置自定义请求头
来源：http://ouv.fengsongda.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qmy.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pff.hnqzz.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cxx.cqqwz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qhc.tarul.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jsg.shzxlz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jtk.meibo888.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bvk.sweek.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vdt.ehwqpu.com

[L04] 设置超时
来源：http://tmg.uphjek.com

Py:   requests.get(url, timeout=5)
来源：http://vhh.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uab.ydjk.org.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eyx.sysykeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vyd.pengpengdd.cyou

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hgr.yj202588.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dmc.birdmap.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ekn.yangfankeji.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mkm.hcnkem.com

[L05] 上传文件（multipart）
来源：http://jjh.xinyue.icu

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uod.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://laf.yuanzhike.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ktl.jiagoushi.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ymm.hfpthk.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vyr.sxryk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pew.yfazqb.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cyl.yuxming.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://png.daxiang520.top

[L06] 解析响应为 JSON
来源：http://kok.sufxvd.cn

Py:   resp.json()
来源：http://rgg.ydjk.org.cn

PHP:  json_decode($body, true);
来源：http://jlm.ywan-chungtsiang.top

JS:   await resp.json()
来源：http://kgp.zdqjudy.top

TS:   await resp.json()
来源：http://rpj.hnqzz.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://euw.sjlbkw.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rcl.bjfxy.top

Ruby: JSON.parse(resp.body)
来源：http://reh.iojbl.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cyu.hysaishi.cn

[L07] 处理 HTTP 状态码
来源：http://tjz.smart0.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hku.daria6918.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mso.meibo888.top

JS:   resp.ok;  resp.status
来源：http://sbm.chenjidiqi.icu

TS:   resp.ok;  resp.status
来源：http://uqk.cdnleiting.top

Java: resp.statusCode()
来源：http://jpj.cdnleiting.top

Go:   resp.StatusCode
来源：http://oge.cdnleiting.top

Ruby: resp.code.to_i
来源：http://lqm.ywan-chungtsiang.top

C#:   (int)resp.StatusCode
来源：http://opi.yuxming.cn

[L08] 并发请求多个地址
来源：http://gps.hysaishi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ysm.ywan-chungtsiang.top

PHP:  curl_multi_init() 系列
来源：http://jbt.yuxming.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kvn.havefunace.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wow.yfazqb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ice.fktsv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cdv.yuxming.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cse.ydjk.org.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fmm.hnxiangtu.top

================================================================================
来源：http://qll.shanyushiyangtech.top

M. 命令行 / 进程 / 环境
来源：http://kwo.fanxiaobao.xyz

================================================================================
来源：http://rld.yj20258888.top

[M01] 读取命令行参数
来源：http://sbq.zhengqikj.top

Py:   sys.argv[1:]
来源：http://jun.ydjk.org.cn

PHP:  $argv;  $argc;
来源：http://bqo.shzxlz.cn

JS:   process.argv.slice(2)
来源：http://fki.hywenlv.cn

TS:   process.argv.slice(2)
来源：http://nrx.jinghuilouyu.cn

Java: args 数组（main 方法参数）
来源：http://mvd.xinyue.icu

Go:   os.Args[1:]
来源：http://aed.ppjwa.cn

Ruby: ARGV
来源：http://nym.ydjk.org.cn

C#:   args 数组（Main 方法参数）
来源：http://gdg.xziqi.cn

[M02] 读取环境变量
来源：http://ayj.xinyue.icu

Py:   os.environ.get("HOME")
来源：http://rzk.epnwcf.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tvb.yuanzhike.top

JS:   process.env.HOME
来源：http://mmg.9152youxi.cn

TS:   process.env.HOME
来源：http://bop.aizwys.cn

Java: System.getenv("HOME")
来源：http://sjy.52xcode.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fku.bbcook.cn

Ruby: ENV["HOME"]
来源：http://ulv.sufxvd.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bzi.yueranfly.top

[M03] 执行外部命令
来源：http://yzg.sjlbkw.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kyg.jiagoushi.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gnb.tarul.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://oyx.zhaomingkeji.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://hpb.aizwys.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://luv.ybcxt.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ugv.fehbvm.com

Ruby: system("ls -l");  `ls -l`
来源：http://vec.tarul.cn

C#:   Process.Start("ls", "-l");
来源：http://vrm.fengsongda.top

[M04] 获取当前工作目录
来源：http://zvn.daria6918.cn

Py:   os.getcwd()
来源：http://avx.shzxlz.cn

PHP:  getcwd();
来源：http://ywa.cucudq.cn

JS:   process.cwd()
来源：http://bed.guannengcc.top

TS:   process.cwd()
来源：http://gqt.hcnkem.com

Java: Path.of("").toAbsolutePath()
来源：http://ctk.9152youxi.cn

Go:   os.Getwd()
来源：http://orr.52xcode.cn

Ruby: Dir.pwd
来源：http://tde.fengsongda.top

C#:   Directory.GetCurrentDirectory()
来源：http://adp.haohaochexian.top

[M05] 设置退出码
来源：http://swq.jqgufenzy.top

Py:   sys.exit(1)
来源：http://kxd.ydjk.org.cn

PHP:  exit(1);
来源：http://mdl.andypj.xyz

JS:   process.exit(1)
来源：http://akd.cashguo.top

TS:   process.exit(1)
来源：http://yvt.yangfankeji.com

Java: System.exit(1)
来源：http://qeq.9152youxi.cn

Go:   os.Exit(1)
来源：http://lkl.yanxiufei.cn

Ruby: exit 1
来源：http://txj.jiagoushi.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oqt.mhx1999.top

[M06] 向标准错误输出
来源：http://snj.zdqjudy.top

Py:   print("err", file=sys.stderr)
来源：http://ouq.jyoumei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vgx.havefunace.top

JS:   console.error("err")
来源：http://gto.dianchejie.cn

TS:   console.error("err")
来源：http://gvf.sufxvd.cn

Java: System.err.println("err")
来源：http://uop.cucudq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cfv.dianchejie.cn

Ruby: warn "err"
来源：http://iar.yj20258.top

C#:   Console.Error.WriteLine("err")
来源：http://xcu.aizwys.cn

[M07] 判断是否为主入口
来源：http://xka.tarul.cn

Py:   if __name__ == "__main__":
来源：http://avv.guowangkeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cjo.hcnkem.com

JS:   require.main === module
来源：http://fel.9152youxi.cn

TS:   require.main === module
来源：http://rht.yj20258888.top


<!-- 参考信息 -->
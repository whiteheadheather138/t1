代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://leg.sxryk.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fvv.xylfe.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wsz.chenjidiqi.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xqs.yongpay.top

[J03] 字符串解析为日期
来源：http://bcs.hcnkem.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mre.zdqjudy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xgn.hnxiangtu.top

JS:   new Date("2024-01-02")
来源：http://spe.shuidangran.top

TS:   new Date("2024-01-02")
来源：http://ewb.redwolf501.top

Java: LocalDate.parse("2024-01-02")
来源：http://wcx.shanyushiyangtech.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://itr.shzxlz.cn

Ruby: Date.parse("2024-01-02")
来源：http://moi.gzhubu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dtm.hnxiangtu.top

[J04] 时间戳与日期互转
来源：http://aui.jinghuilouyu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ujm.jiagoushi.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://edl.yj202588.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://abj.epnwcf.com

TS:   Math.floor(Date.now() / 1000)
来源：http://joj.ywan-chungtsiang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vsz.zhijiandao.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xnc.guowangkeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ehc.yj202588.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lmh.shzxlz.cn

[J05] 时间加减（加 7 天）
来源：http://lnn.guowangkeji.top

Py:   now + timedelta(days=7)
来源：http://mko.zhaomingkeji.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://jav.xziqi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pok.jqgfzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eix.hysaishi.cn

Java: LocalDate.now().plusDays(7)
来源：http://pei.jqgfzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jts.yvedp.cn

Ruby: Time.now + 7 * 86400
来源：http://vik.zhengqikj.top

C#:   DateTime.Now.AddDays(7)
来源：http://dmn.xuetiantiany.cn

[J06] 计算两时间之差
来源：http://krf.svipenyu.cn

Py:   (end - start).total_seconds()
来源：http://lff.yanxiufei.cn

PHP:  $end->diff($start)->days;
来源：http://xfo.shanyushiyangtech.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cse.yonumen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zax.yfazqb.com

Java: Duration.between(start, end).toSeconds()
来源：http://rhp.ydjk.org.cn

Go:   end.Sub(start).Hours()
来源：http://mek.kuanghao11.cn

Ruby: end - start                 # 返回秒数
来源：http://zkk.shuidangran.top

C#:   (end - start).TotalSeconds
来源：http://how.xuanzx.com

[J07] 比较两个日期
来源：http://amw.pengpengdd.cyou

Py:   d1 < d2;  d1 == d2
来源：http://efi.tanke756.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hab.guannengcc.top

JS:   d1.getTime() < d2.getTime()
来源：http://wfz.wangdashe.top

TS:   d1.getTime() < d2.getTime()
来源：http://jgl.mhx1999.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://crh.fktsv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mme.cqqwz.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qvp.cucudq.cn

C#:   d1 < d2;  d1 == d2
来源：http://gom.meibo888.top

[J08] 提取年月日与星期
来源：http://kih.cheryme.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mcf.316326.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oej.sysykeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zbe.uphjek.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zlp.tianlin.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nqf.jqgufenzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gkx.smart0.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ykl.jlsjyb.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jok.jinqigufen.top

[J09] 时区处理
来源：http://edv.hfpthk.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://piw.xingfuxueyuan.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xdh.snrcjt.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cft.yj20258.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gnt.ydjk.org.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fdx.sxryk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wgy.zdqjudy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://knc.ppjwa.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ldg.chenlongwang.top

[J10] 取今天 / 本月第一天
来源：http://ebx.meibo888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://fbi.fktsv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zbg.jiagoushi.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ilb.chenzaomai.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ojy.tanke756.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kqm.ivvv.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://eth.xuetiantiany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cmk.jqgfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gey.xingfuxueyuan.xyz

================================================================================
来源：http://iom.cheryme.top

K. JSON 与序列化
来源：http://bmg.jinghuilouyu.cn

================================================================================
来源：http://pnk.aibaodan.cn

[K01] 对象转 JSON 字符串
来源：http://qzz.jlsjyb.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zjv.hnqzz.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mjb.yj20258.top

JS:   JSON.stringify(obj)
来源：http://wpv.shanyushiyangkeji.top

TS:   JSON.stringify(obj)
来源：http://rym.shuidangran.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jwl.cashguo.top

Go:   json.Marshal(obj)
来源：http://jfn.yonumen.top

Ruby: obj.to_json                                     // require "json"
来源：http://yud.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vem.guannengcc.top

[K02] JSON 字符串转对象
来源：http://ils.xuanzx.com

Py:   json.loads(s)
来源：http://srf.gaohongyu789.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dao.redwolf501.top

JS:   JSON.parse(s)
来源：http://srf.feifeiyinyue.top

TS:   JSON.parse(s)
来源：http://pdv.meibo888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fpq.zhoulong.xyz

Go:   json.Unmarshal(data, &v)
来源：http://gcb.zhixingplan.top

Ruby: JSON.parse(s)
来源：http://fef.sweek.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bzo.mhx1999.top

[K03] JSON 美化输出（带缩进）
来源：http://ixa.316326.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bvy.c1oappe.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qxd.wangshuangyany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xnn.yueranfly.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wfr.birdmap.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kuf.andypj.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vyh.quarkkingdee.top

Ruby: JSON.pretty_generate(obj)
来源：http://esa.yj202588.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hlg.ppjwa.cn

[K04] 读取 JSON 文件
来源：http://vhm.guannengcc.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kkv.9152youxi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vbn.bbcook.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://esb.shzxlz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tjy.yongpay.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kip.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wrs.52xcode.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://msv.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hvi.jqgufenzy.top

[K05] 深拷贝对象
来源：http://mif.tian-w.cn

Py:   copy.deepcopy(obj)
来源：http://puh.bjfxy.top

PHP:  unserialize(serialize($obj));
来源：http://luh.yj202588.top

JS:   structuredClone(obj)
来源：http://voe.xingfuxueyuan.xyz

TS:   structuredClone(obj)
来源：http://zsk.hywenlv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wpx.vqdsnc.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wao.fzhhl.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://syk.hongshengwenyu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://qcc.jinqigfzy.top

[K06] 解析 URL 查询串
来源：http://ame.yongpay.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bnc.sxryk.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yzf.yvedp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://adm.meibo888.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xub.gaohongyu789.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jop.zhoulong.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://gxq.0kj1m.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jzm.chenlongwang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yca.epnwcf.com

[K07] 进制转换
来源：http://ppf.ctjpmb.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ros.xuanzx.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eqt.daxiang520.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ocf.zhongyouzk.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zyd.yj202588.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://haq.daria6918.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xus.jiagoushi.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lne.jlsjyb.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ukc.ctjpmb.com

[K08] 二进制序列化（非 JSON）
来源：http://klt.wangdashe.top

Py:   pickle.dumps(obj)
来源：http://aax.chenjidiqi.icu

PHP:  serialize($obj);  unserialize($s);
来源：http://qov.gaohongyu789.top

JS:   v8.serialize(obj)        // Node
来源：http://ybi.9152youxi.cn

TS:   v8.serialize(obj)        // Node
来源：http://tin.hfpthk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ech.jinyuanbaomall.cn

Go:   encoding/gob
来源：http://hez.daxiang520.top

Ruby: Marshal.dump(obj)
来源：http://buo.gogol.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uxt.yvedp.cn

================================================================================
来源：http://ipx.aibaodan.cn

L. 网络请求
来源：http://xzt.zhaomingkeji.xyz

================================================================================
来源：http://fwd.hnqzz.top

[L01] 发送 GET 请求
来源：http://kak.hongshengwenyu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mli.vqdsnc.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vwe.daria6918.cn

JS:   await fetch(url)
来源：http://mvu.zdbjq.cn

TS:   await fetch(url)
来源：http://fvi.shanyushiyangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ldw.sysykeji.top

Go:   resp, err := http.Get(url)
来源：http://ugn.daxiang520.top

Ruby: Net::HTTP.get(URI(url))
来源：http://yzy.daxiang520.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iqs.gogol.net.cn

[L02] 发送 POST JSON
来源：http://lxt.kuanghao11.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kaj.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://thh.0kj1m.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kqw.tian-w.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mbo.shanyushiyangtech.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yxz.xuetiantiany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zsu.tianlin.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ioz.snrcjt.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mpo.havefunace.top

[L03] 设置自定义请求头
来源：http://qll.vehdjk.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wdj.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://guh.birdmap.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zoa.gzhubu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pxj.aizwys.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lrq.feifeiyinyue.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dde.0kj1m.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ubk.fanxiaobao.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cjj.havefunace.top

[L04] 设置超时
来源：http://ywa.fengsongda.top

Py:   requests.get(url, timeout=5)
来源：http://ohh.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vrc.yfazqb.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://omc.yfazqb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dcz.fzhhl.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dhm.nanxuanxn.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qic.sjlbkw.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ait.jqgufenzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xhj.yongpay.top

[L05] 上传文件（multipart）
来源：http://nyv.hnxiangtu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jii.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vam.yueranfly.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ezy.hysaishi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jxl.nwbrower.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kxj.hnqzz.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://etu.jiagoushi.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ode.hnxiangtu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://aei.ivvv.top

[L06] 解析响应为 JSON
来源：http://vzw.xziqi.cn

Py:   resp.json()
来源：http://rum.chenjidiqi.icu

PHP:  json_decode($body, true);
来源：http://okg.guowangkeji.top

JS:   await resp.json()
来源：http://lwr.fehbvm.com

TS:   await resp.json()
来源：http://avo.gzhubu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jhc.316326.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gam.cashguo.top

Ruby: JSON.parse(resp.body)
来源：http://pqr.redwolf501.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nlk.uphjek.com

[L07] 处理 HTTP 状态码
来源：http://yxb.cucudq.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dbw.ehwqpu.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nyz.svipenyu.cn

JS:   resp.ok;  resp.status
来源：http://ixn.zhaomingkeji.xyz

TS:   resp.ok;  resp.status
来源：http://sdc.cashguo.top

Java: resp.statusCode()
来源：http://bhq.yj202588.top

Go:   resp.StatusCode
来源：http://kmy.yj202588.top

Ruby: resp.code.to_i
来源：http://eqj.yj20258.top

C#:   (int)resp.StatusCode
来源：http://kel.cashguo.top

[L08] 并发请求多个地址
来源：http://phx.hywenlv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://omt.sysykeji.top

PHP:  curl_multi_init() 系列
来源：http://dku.wangshuangyany.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://utv.hesvh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ppn.ehwqpu.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://iqf.zhiwuduotai.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bic.chenzaomai.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://udh.tarul.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oad.0kj1m.cn

================================================================================
来源：http://pct.cashguo.top

M. 命令行 / 进程 / 环境
来源：http://jzv.chenjidiqi.icu

================================================================================
来源：http://gbx.mhx1999.top

[M01] 读取命令行参数
来源：http://asz.fanxiaobao.xyz

Py:   sys.argv[1:]
来源：http://wcv.sweek.top

PHP:  $argv;  $argc;
来源：http://vhy.vqdsnc.cn

JS:   process.argv.slice(2)
来源：http://nfq.hongshengwenyu.top

TS:   process.argv.slice(2)
来源：http://zej.shuidangran.top

Java: args 数组（main 方法参数）
来源：http://mdu.yfazqb.com

Go:   os.Args[1:]
来源：http://dvz.yonumen.top

Ruby: ARGV
来源：http://dzd.feifeiyinyue.top

C#:   args 数组（Main 方法参数）
来源：http://ydx.kuanghao11.cn

[M02] 读取环境变量
来源：http://owt.guannengcc.top

Py:   os.environ.get("HOME")
来源：http://czc.sxryk.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://asu.nwbrower.top

JS:   process.env.HOME
来源：http://geq.jinyuanbaomall.cn

TS:   process.env.HOME
来源：http://fhr.tanke756.top

Java: System.getenv("HOME")
来源：http://gmt.zhixingplan.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gbl.jinyuanbaomall.cn

Ruby: ENV["HOME"]
来源：http://roi.yj202588.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oui.sysykeji.top

[M03] 执行外部命令
来源：http://wdt.haohaochexian.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zhg.sufxvd.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ojq.jqgufenzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://peq.sysykeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://pho.havefunace.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bhs.ctjpmb.com

Go:   exec.Command("ls", "-l").Output()
来源：http://jvk.hesvh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://erj.gotoacloud.top

C#:   Process.Start("ls", "-l");
来源：http://lmk.nwbrower.top

[M04] 获取当前工作目录
来源：http://rvh.ivvv.top

Py:   os.getcwd()
来源：http://vfg.gogol.net.cn

PHP:  getcwd();
来源：http://qqw.wangdashe.top

JS:   process.cwd()
来源：http://hjj.snrcjt.cn

TS:   process.cwd()
来源：http://rqf.vehdjk.com

Java: Path.of("").toAbsolutePath()
来源：http://kxi.redwolf501.top

Go:   os.Getwd()
来源：http://vpb.sufxvd.cn

Ruby: Dir.pwd
来源：http://qcb.hnxiangtu.top

C#:   Directory.GetCurrentDirectory()
来源：http://alp.jinqigfzy.top

[M05] 设置退出码
来源：http://jzu.jqgfzy.top

Py:   sys.exit(1)
来源：http://vjz.hywenlv.cn

PHP:  exit(1);
来源：http://ffi.zhaomingkeji.xyz

JS:   process.exit(1)
来源：http://cit.smart0.xyz

TS:   process.exit(1)
来源：http://hay.yfazqb.com

Java: System.exit(1)
来源：http://kxc.cucudq.cn

Go:   os.Exit(1)
来源：http://blp.shanyushiyangkeji.top

Ruby: exit 1
来源：http://vob.yuanzhike.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yhp.shangyingyoupin.top

[M06] 向标准错误输出
来源：http://cqs.zycfv.cn

Py:   print("err", file=sys.stderr)
来源：http://keg.xinyue.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://zsr.svipenyu.cn

JS:   console.error("err")
来源：http://dmn.cheryme.top

TS:   console.error("err")
来源：http://iwl.vqdsnc.cn

Java: System.err.println("err")
来源：http://ggr.chenjidiqi.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://erj.yvedp.cn

Ruby: warn "err"
来源：http://mml.vqdsnc.cn

C#:   Console.Error.WriteLine("err")
来源：http://qmh.hfpthk.cn

[M07] 判断是否为主入口
来源：http://wde.yj202588.top

Py:   if __name__ == "__main__":
来源：http://pwm.snrcjt.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hul.xuanzx.com

JS:   require.main === module
来源：http://vwo.redwolf501.top

TS:   require.main === module
来源：http://qph.iojbl.cn

Java: public static void main(String[] args)
来源：http://tpz.yanxiufei.cn

Go:   func main()
来源：http://luy.sweek.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nbq.xingfuxueyuan.xyz

C#:   static void Main(string[] args)
来源：http://qbc.yangfankeji.com

[M08] 获取系统与运行时信息
来源：http://eij.ctjpmb.com

Py:   platform.system();  platform.python_version()
来源：http://kks.xuanzx.com

PHP:  PHP_OS;  phpversion();
来源：http://cyl.guowangkeji.top

JS:   process.platform;  process.version
来源：http://tio.0kj1m.cn

TS:   process.platform;  process.version
来源：http://ulu.shzxlz.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ily.gaohongyu789.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xtz.shanyushiyangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ffr.tarul.cn


<!-- 参考信息 -->
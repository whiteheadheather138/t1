代发 wailian999

Go:   time.Now()
来源：http://yaw.smart0.xyz

Ruby: Time.now
来源：http://afc.316326.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hti.zhoulong.xyz

[J02] 格式化输出
来源：http://lvx.cucudq.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vct.aizwys.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cjr.yonumen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gbl.sjlbkw.cn

TS:   d.toISOString()
来源：http://atk.hfpthk.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nqn.hesvh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ssf.cashguo.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uqt.9152youxi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bzr.yj202588.top

[J03] 字符串解析为日期
来源：http://ijn.daria6918.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wnh.52xcode.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hhi.zdqjudy.top

JS:   new Date("2024-01-02")
来源：http://vfh.epnwcf.com

TS:   new Date("2024-01-02")
来源：http://ddb.shuidangran.top

Java: LocalDate.parse("2024-01-02")
来源：http://ebi.sufxvd.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fnu.wangdashe.top

Ruby: Date.parse("2024-01-02")
来源：http://xcq.cucudq.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vbi.snrcjt.cn

[J04] 时间戳与日期互转
来源：http://gnv.mhx1999.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://clg.epnwcf.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mun.cheryme.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://see.cashguo.top

TS:   Math.floor(Date.now() / 1000)
来源：http://plq.shzxlz.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rdj.dianchejie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://llr.ybcxt.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uym.wangdashe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qvt.shangyingyoupin.top

[J05] 时间加减（加 7 天）
来源：http://ijt.zhengqikj.top

Py:   now + timedelta(days=7)
来源：http://nyq.yvedp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://foo.zdbjq.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qzo.svipenyu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://iuc.gaohongyu789.top

Java: LocalDate.now().plusDays(7)
来源：http://cpn.ehwqpu.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bke.shanyushiyangtech.top

Ruby: Time.now + 7 * 86400
来源：http://jag.cashguo.top

C#:   DateTime.Now.AddDays(7)
来源：http://pzz.zhoulong.xyz

[J06] 计算两时间之差
来源：http://qmb.yuxming.cn

Py:   (end - start).total_seconds()
来源：http://hsu.iojbl.cn

PHP:  $end->diff($start)->days;
来源：http://zhl.yuanzhike.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rxv.iojbl.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://can.ehwqpu.com

Java: Duration.between(start, end).toSeconds()
来源：http://rng.zhengqikj.top

Go:   end.Sub(start).Hours()
来源：http://sjb.yuxming.cn

Ruby: end - start                 # 返回秒数
来源：http://wbd.yuxming.cn

C#:   (end - start).TotalSeconds
来源：http://woo.zhixingplan.top

[J07] 比较两个日期
来源：http://pgk.yfazqb.com

Py:   d1 < d2;  d1 == d2
来源：http://nhn.chenzaomai.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ubd.sweek.top

JS:   d1.getTime() < d2.getTime()
来源：http://tkk.ybcxt.top

TS:   d1.getTime() < d2.getTime()
来源：http://onr.zhongyouzk.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ubm.hywenlv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aln.sufxvd.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gxh.chenjidiqi.icu

C#:   d1 < d2;  d1 == d2
来源：http://jfn.cucudq.cn

[J08] 提取年月日与星期
来源：http://wip.hongshengwenyu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ykt.tian-w.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zhc.ivvv.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wty.mhx1999.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bea.jqgufenzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vll.c1oappe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hkc.zhijiandao.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sas.iojbl.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ejx.zhaomingkeji.xyz

[J09] 时区处理
来源：http://zkk.jinghuilouyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dzd.hammf.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vik.shzxlz.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bgj.nwbrower.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://npm.andypj.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://age.zhoulong.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://prg.zhixingplan.top

Ruby: Time.now.getlocal("+08:00")
来源：http://yju.pengpengdd.cyou

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://shu.zhijiandao.cn

[J10] 取今天 / 本月第一天
来源：http://iyx.tian-w.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ops.mhx1999.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bjv.pengpengdd.cyou

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ldw.zhixingplan.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gtn.chenzaomai.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tfl.feifeiyinyue.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nkg.jlsjyb.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gto.sxryk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wdf.nanxuanxn.top

================================================================================
来源：http://ftc.ctjpmb.com

K. JSON 与序列化
来源：http://wvs.hfpthk.cn

================================================================================
来源：http://hdd.iojbl.cn

[K01] 对象转 JSON 字符串
来源：http://jrt.fengsongda.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cpd.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://isb.ctjpmb.com

JS:   JSON.stringify(obj)
来源：http://atu.meibo888.top

TS:   JSON.stringify(obj)
来源：http://lpk.ywan-chungtsiang.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ovk.redwolf501.top

Go:   json.Marshal(obj)
来源：http://ewp.zdbjq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://njn.52xcode.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://uyi.jinqigufen.top

[K02] JSON 字符串转对象
来源：http://ehw.xuanzx.com

Py:   json.loads(s)
来源：http://yin.yj20258.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jlp.jqgfzy.top

JS:   JSON.parse(s)
来源：http://afv.jlsjyb.cn

TS:   JSON.parse(s)
来源：http://xys.cheryme.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nsw.fengsongda.top

Go:   json.Unmarshal(data, &v)
来源：http://sai.fehbvm.com

Ruby: JSON.parse(s)
来源：http://ryt.cashguo.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://elh.xziqi.cn

[K03] JSON 美化输出（带缩进）
来源：http://ajn.zhengqikj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zll.yj20258.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iyx.hywenlv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kux.hysaishi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ulk.jiagoushi.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://stt.ehwqpu.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zbw.fengsongda.top

Ruby: JSON.pretty_generate(obj)
来源：http://axr.xziqi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mvj.birdmap.top

[K04] 读取 JSON 文件
来源：http://nih.meibo888.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://iuh.vqdsnc.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mjk.havefunace.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://epr.jiagoushi.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tzq.svipenyu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wjb.wangdashe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ehe.yj20258.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://sma.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jcx.zycfv.cn

[K05] 深拷贝对象
来源：http://vka.redwolf501.top

Py:   copy.deepcopy(obj)
来源：http://jld.daxiang520.top

PHP:  unserialize(serialize($obj));
来源：http://ijd.ydzc1.top

JS:   structuredClone(obj)
来源：http://ymq.snrcjt.cn

TS:   structuredClone(obj)
来源：http://rjc.quarkkingdee.top

Java: // 手写拷贝构造，或序列化往返
来源：http://voe.xingfuxueyuan.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pgv.aizwys.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qrp.nwbrower.top

C#:   // 序列化往返，或自定义 Clone
来源：http://xxw.zhijiandao.cn

[K06] 解析 URL 查询串
来源：http://nkp.zycfv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nhz.jinghuilouyu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nht.52xcode.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sci.yanxiufei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://exk.hywenlv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://icl.hysaishi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vsg.sufxvd.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pui.xziqi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lsz.chenjidiqi.icu

[K07] 进制转换
来源：http://gku.shanyushiyangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ylx.hysaishi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://aan.cdnleiting.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://eqt.xingfuxueyuan.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lds.yueranfly.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ezd.sweek.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vmc.jqgufenzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://iks.birdmap.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fal.quarkkingdee.top

[K08] 二进制序列化（非 JSON）
来源：http://lxn.yongpay.top

Py:   pickle.dumps(obj)
来源：http://qet.ctjpmb.com

PHP:  serialize($obj);  unserialize($s);
来源：http://fdt.chenlongwang.top

JS:   v8.serialize(obj)        // Node
来源：http://pat.ehwqpu.com

TS:   v8.serialize(obj)        // Node
来源：http://hgm.52xcode.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://szc.tian-w.cn

Go:   encoding/gob
来源：http://eke.yfazqb.com

Ruby: Marshal.dump(obj)
来源：http://rvp.yangfankeji.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gxh.nanxinkj.top

================================================================================
来源：http://mig.yj20258.top

L. 网络请求
来源：http://kan.ydzc1.top

================================================================================
来源：http://kys.yvedp.cn

[L01] 发送 GET 请求
来源：http://heh.daria6918.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zsw.iojbl.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://thb.cheryme.top

JS:   await fetch(url)
来源：http://ayv.havefunace.top

TS:   await fetch(url)
来源：http://byz.uphjek.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lhr.bjfxy.top

Go:   resp, err := http.Get(url)
来源：http://yri.0kj1m.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://oxp.meibo888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://can.yfazqb.com

[L02] 发送 POST JSON
来源：http://dns.chenzaomai.com

Py:   requests.post(url, json={"a": 1})
来源：http://dph.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rty.jiagoushi.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://owl.316326.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dma.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zal.zhixingplan.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xxn.quarkkingdee.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fkv.yj20258.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bzk.zhiwuduotai.top

[L03] 设置自定义请求头
来源：http://aqy.xinyue.icu

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wva.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fxc.hywenlv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ghb.mhx1999.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cvk.cashguo.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bku.fanxiaobao.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://stm.xuetiantiany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nir.svipenyu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uls.wangdashe.top

[L04] 设置超时
来源：http://xwg.zhiwuduotai.top

Py:   requests.get(url, timeout=5)
来源：http://yww.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vos.fanxiaobao.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iuf.bjfxy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rey.zdqjudy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lbt.yangfankeji.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xmq.pycfn.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rqq.fzhhl.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yrk.bjfxy.top

[L05] 上传文件（multipart）
来源：http://nnw.dashuyun.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jja.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ana.jyoumei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ckw.tian-w.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nbp.nanxuanxn.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eud.yvedp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zfw.epnwcf.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kpy.ehwqpu.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dqe.zycfv.cn

[L06] 解析响应为 JSON
来源：http://mmx.iojbl.cn

Py:   resp.json()
来源：http://esz.tanke756.top

PHP:  json_decode($body, true);
来源：http://ttd.jinqigufen.top

JS:   await resp.json()
来源：http://iof.xinyue.icu

TS:   await resp.json()
来源：http://voe.jinghuilouyu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rsu.yuanzhike.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yjs.ydjk.org.cn

Ruby: JSON.parse(resp.body)
来源：http://llh.yuxming.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oly.chenjidiqi.icu

[L07] 处理 HTTP 状态码
来源：http://jey.fzhhl.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rrw.bbcook.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yev.hysaishi.cn

JS:   resp.ok;  resp.status
来源：http://fwm.cdnleiting.top

TS:   resp.ok;  resp.status
来源：http://azv.shanyushiyangtech.top

Java: resp.statusCode()
来源：http://evz.shuidangran.top

Go:   resp.StatusCode
来源：http://owm.tarul.cn

Ruby: resp.code.to_i
来源：http://bdu.wangdashe.top

C#:   (int)resp.StatusCode
来源：http://zul.jianghu66.top

[L08] 并发请求多个地址
来源：http://lwv.quarkkingdee.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kyc.hammf.cn

PHP:  curl_multi_init() 系列
来源：http://sld.andypj.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qgv.guannengcc.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://teq.guannengcc.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://aey.fengsongda.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cau.gaohongyu789.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bog.kuanghao11.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vza.svipenyu.cn

================================================================================
来源：http://fun.cheryme.top

M. 命令行 / 进程 / 环境
来源：http://nqc.yonumen.top

================================================================================
来源：http://sou.ydzc1.top

[M01] 读取命令行参数
来源：http://cfh.pycfn.com

Py:   sys.argv[1:]
来源：http://aom.jinyuanbaomall.cn

PHP:  $argv;  $argc;
来源：http://jiq.hongshengwenyu.top

JS:   process.argv.slice(2)
来源：http://ela.yongpay.top

TS:   process.argv.slice(2)
来源：http://uki.jinghuilouyu.cn

Java: args 数组（main 方法参数）
来源：http://yxm.yonumen.top

Go:   os.Args[1:]
来源：http://ayo.jinqigufen.top

Ruby: ARGV
来源：http://yer.cdnleiting.top

C#:   args 数组（Main 方法参数）
来源：http://ges.zhengqikj.top

[M02] 读取环境变量
来源：http://hvf.zhengqikj.top

Py:   os.environ.get("HOME")
来源：http://een.dianchejie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jms.zdbjq.cn

JS:   process.env.HOME
来源：http://tzg.yuanzhike.top

TS:   process.env.HOME
来源：http://sou.jinghuilouyu.cn

Java: System.getenv("HOME")
来源：http://gnq.dianchejie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nne.dashuyun.cn

Ruby: ENV["HOME"]
来源：http://ufa.vqdsnc.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hij.bjfxy.top

[M03] 执行外部命令
来源：http://sux.jiagoushi.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nih.ywan-chungtsiang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://znw.wangdashe.top

JS:   child_process.execSync("ls -l").toString()
来源：http://tme.316326.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://uyh.nanxuanxn.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://euf.cashguo.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wvw.cdnleiting.top

Ruby: system("ls -l");  `ls -l`
来源：http://ido.yuanzhike.top

C#:   Process.Start("ls", "-l");
来源：http://tms.kuanghao11.cn

[M04] 获取当前工作目录
来源：http://psb.zhiwuduotai.top

Py:   os.getcwd()
来源：http://cvj.ybcxt.top

PHP:  getcwd();
来源：http://rvs.0kj1m.cn

JS:   process.cwd()
来源：http://skd.tarul.cn

TS:   process.cwd()
来源：http://yhk.quarkkingdee.top

Java: Path.of("").toAbsolutePath()
来源：http://qrz.vqdsnc.cn

Go:   os.Getwd()
来源：http://xea.nanxuanxn.top

Ruby: Dir.pwd
来源：http://nzs.tarul.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mls.9152youxi.cn

[M05] 设置退出码
来源：http://sos.haohaochexian.top

Py:   sys.exit(1)
来源：http://pkw.iojbl.cn

PHP:  exit(1);
来源：http://ase.aibaodan.cn

JS:   process.exit(1)
来源：http://vxx.jinqigufen.top

TS:   process.exit(1)
来源：http://wtm.ydzc1.top

Java: System.exit(1)
来源：http://kll.epnwcf.com

Go:   os.Exit(1)
来源：http://pvk.hesvh.cn

Ruby: exit 1
来源：http://wau.yvedp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mgr.tanke756.top

[M06] 向标准错误输出
来源：http://ttk.epnwcf.com

Py:   print("err", file=sys.stderr)
来源：http://mek.yangfankeji.com

PHP:  fwrite(STDERR, "err\n");
来源：http://qro.9152youxi.cn

JS:   console.error("err")
来源：http://rum.sxryk.cn

TS:   console.error("err")
来源：http://qpb.smart0.xyz

Java: System.err.println("err")
来源：http://dok.hnqzz.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sag.fzhhl.top

Ruby: warn "err"
来源：http://zyx.zhiwuduotai.top

C#:   Console.Error.WriteLine("err")
来源：http://eoq.sjlbkw.cn

[M07] 判断是否为主入口
来源：http://qut.daxiang520.top

Py:   if __name__ == "__main__":
来源：http://rag.epnwcf.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lvi.redwolf501.top

JS:   require.main === module
来源：http://ugn.vqdsnc.cn

TS:   require.main === module
来源：http://jng.zycfv.cn

Java: public static void main(String[] args)
来源：http://ang.nwbrower.top

Go:   func main()
来源：http://zch.ppjwa.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ihi.uphjek.com

C#:   static void Main(string[] args)
来源：http://qeg.shuidangran.top


<!-- 参考信息 -->
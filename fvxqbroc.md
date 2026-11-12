代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xtr.vqdsnc.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tri.ywan-chungtsiang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cbo.zycfv.cn

TS:   d.toISOString()
来源：http://tqt.hesvh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://frj.zycfv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yec.aizwys.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bfv.sxryk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rnf.aibaodan.cn

[J03] 字符串解析为日期
来源：http://hzp.jqgfzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dwi.sweek.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bck.snrcjt.cn

JS:   new Date("2024-01-02")
来源：http://gjy.uphjek.com

TS:   new Date("2024-01-02")
来源：http://njf.yanxiufei.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nrd.haohaochexian.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jiw.cqqwz.cn

Ruby: Date.parse("2024-01-02")
来源：http://jdc.iojbl.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jki.hywenlv.cn

[J04] 时间戳与日期互转
来源：http://wor.zhiwuduotai.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://usx.dianchejie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jtc.316326.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://aqt.hysaishi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vjx.cdnleiting.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kad.fengsongda.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vgq.wangdashe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://frl.havefunace.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dre.yongpay.top

[J05] 时间加减（加 7 天）
来源：http://jqh.gaohongyu789.top

Py:   now + timedelta(days=7)
来源：http://zzj.ydjk.org.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uni.zdqjudy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://veh.0kj1m.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nel.zdqjudy.top

Java: LocalDate.now().plusDays(7)
来源：http://fug.wangdashe.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fmd.haohaochexian.top

Ruby: Time.now + 7 * 86400
来源：http://iwo.tanke756.top

C#:   DateTime.Now.AddDays(7)
来源：http://xhn.yj20258888.top

[J06] 计算两时间之差
来源：http://jbe.yuxming.cn

Py:   (end - start).total_seconds()
来源：http://dml.sysykeji.top

PHP:  $end->diff($start)->days;
来源：http://kiq.hesvh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://obu.uphjek.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nmw.bjfxy.top

Java: Duration.between(start, end).toSeconds()
来源：http://kji.kuanghao11.cn

Go:   end.Sub(start).Hours()
来源：http://fej.yonumen.top

Ruby: end - start                 # 返回秒数
来源：http://pha.tianlin.xyz

C#:   (end - start).TotalSeconds
来源：http://huy.yj202588.top

[J07] 比较两个日期
来源：http://xuk.jlsjyb.cn

Py:   d1 < d2;  d1 == d2
来源：http://moo.uphjek.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://clx.havefunace.top

JS:   d1.getTime() < d2.getTime()
来源：http://zaq.kuanghao11.cn

TS:   d1.getTime() < d2.getTime()
来源：http://goo.guowangkeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://voh.xinyue.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xyn.cheryme.top

Ruby: d1 < d2;  d1 == d2
来源：http://qzf.daxiang520.top

C#:   d1 < d2;  d1 == d2
来源：http://hkr.xinyue.icu

[J08] 提取年月日与星期
来源：http://bdk.birdmap.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bez.chenjidiqi.icu

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lpb.zhengqikj.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vos.redwolf501.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hot.havefunace.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dpf.fehbvm.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gfj.aizwys.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bac.yanxiufei.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wiw.nwbrower.top

[J09] 时区处理
来源：http://rld.yvedp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pwg.sufxvd.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wkj.hcnkem.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wmr.jianghu66.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xzx.tarul.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dvt.zhongyouzk.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kyp.hnxiangtu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ogv.cqqwz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gzy.zdqjudy.top

[J10] 取今天 / 本月第一天
来源：http://lwu.pengpengdd.cyou

Py:   date.today();  date.today().replace(day=1)
来源：http://yrq.redwolf501.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wkv.havefunace.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ttz.smart0.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wnq.yanxiufei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://esa.xingfuxueyuan.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dnh.jinghuilouyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lmq.xinyue.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qoo.yueranfly.top

================================================================================
来源：http://kmi.yonumen.top

K. JSON 与序列化
来源：http://edr.jiagoushi.top

================================================================================
来源：http://mig.hongshengwenyu.top

[K01] 对象转 JSON 字符串
来源：http://blq.haohaochexian.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uxn.yuxming.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://reo.zhiwuduotai.top

JS:   JSON.stringify(obj)
来源：http://edv.hnqzz.top

TS:   JSON.stringify(obj)
来源：http://vuu.yvedp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bng.ywan-chungtsiang.top

Go:   json.Marshal(obj)
来源：http://sge.bjfxy.top

Ruby: obj.to_json                                     // require "json"
来源：http://xry.ppjwa.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wiy.redwolf501.top

[K02] JSON 字符串转对象
来源：http://pgk.bbcook.cn

Py:   json.loads(s)
来源：http://fdl.shangyingyoupin.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tja.hysaishi.cn

JS:   JSON.parse(s)
来源：http://osz.shzxlz.cn

TS:   JSON.parse(s)
来源：http://pcd.yonumen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vuz.ctjpmb.com

Go:   json.Unmarshal(data, &v)
来源：http://kut.zycfv.cn

Ruby: JSON.parse(s)
来源：http://mwj.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ohf.jinqigfzy.top

[K03] JSON 美化输出（带缩进）
来源：http://xfb.daxiang520.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fxz.zhengqikj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jtn.daxiang520.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dmu.dianchejie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lns.fzhhl.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wkk.yvedp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lgd.bjfxy.top

Ruby: JSON.pretty_generate(obj)
来源：http://wdb.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hlt.fzhhl.top

[K04] 读取 JSON 文件
来源：http://wgd.jinghuilouyu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fwy.fengsongda.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://aol.yj202588.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pse.316326.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tqq.uphjek.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lcv.fzhhl.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lje.havefunace.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://rdg.zhiwuduotai.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://csx.zdqjudy.top

[K05] 深拷贝对象
来源：http://utj.ywan-chungtsiang.top

Py:   copy.deepcopy(obj)
来源：http://sko.52xcode.cn

PHP:  unserialize(serialize($obj));
来源：http://iqa.cucudq.cn

JS:   structuredClone(obj)
来源：http://pwo.ybcxt.top

TS:   structuredClone(obj)
来源：http://pju.316326.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://jos.cqqwz.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dvq.redwolf501.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ppo.ydzc1.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ger.aizwys.cn

[K06] 解析 URL 查询串
来源：http://pjj.jinghuilouyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dgq.yongpay.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mhf.zycfv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zbe.gogol.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://asy.c1oappe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yuj.ctjpmb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://xhb.sxryk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hxz.jianghu66.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vxm.yj20258.top

[K07] 进制转换
来源：http://psm.wangdashe.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dwc.sysykeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nii.sxryk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ats.hnxiangtu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yby.vehdjk.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lez.hnqzz.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://deu.shuidangran.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pgg.meibo888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lcu.zdqjudy.top

[K08] 二进制序列化（非 JSON）
来源：http://maf.hcnkem.com

Py:   pickle.dumps(obj)
来源：http://wcs.yongpay.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ozr.aizwys.cn

JS:   v8.serialize(obj)        // Node
来源：http://cqr.guowangkeji.top

TS:   v8.serialize(obj)        // Node
来源：http://ojh.jinghuilouyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ius.cheryme.top

Go:   encoding/gob
来源：http://kee.uphjek.com

Ruby: Marshal.dump(obj)
来源：http://srq.daria6918.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rsp.xinyue.icu

================================================================================
来源：http://sff.chenzaomai.com

L. 网络请求
来源：http://oxq.sufxvd.cn

================================================================================
来源：http://miu.shzxlz.cn

[L01] 发送 GET 请求
来源：http://rlu.ctjpmb.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://izc.zhengqikj.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fuq.cucudq.cn

JS:   await fetch(url)
来源：http://rod.feifeiyinyue.top

TS:   await fetch(url)
来源：http://bpb.316326.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vbt.jinqigufen.top

Go:   resp, err := http.Get(url)
来源：http://acl.smart0.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://djm.fehbvm.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vrl.fengsongda.top

[L02] 发送 POST JSON
来源：http://gef.bbcook.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vgt.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qpr.havefunace.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sle.jiagoushi.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://myi.zhixingplan.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gvk.yonumen.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://okt.zhixingplan.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rcz.c1oappe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kpw.9152youxi.cn

[L03] 设置自定义请求头
来源：http://nvr.aibaodan.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mcy.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mlq.hcnkem.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://avx.dianchejie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pmv.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lce.guannengcc.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wem.fengsongda.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vfx.9152youxi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://shr.ydzc1.top

[L04] 设置超时
来源：http://pmr.yuanzhike.top

Py:   requests.get(url, timeout=5)
来源：http://aot.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wbu.jlsjyb.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ywy.cucudq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zgq.dashuyun.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://igf.tanke756.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ynw.jqgfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bmd.xylfe.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gzc.ydzc1.top

[L05] 上传文件（multipart）
来源：http://dqk.gotoacloud.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tjj.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qsy.xingfuxueyuan.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://clq.sweek.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bqy.xuanzx.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kfv.tarul.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gtm.bjfxy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vwy.0kj1m.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gji.ybcxt.top

[L06] 解析响应为 JSON
来源：http://fce.ehwqpu.com

Py:   resp.json()
来源：http://vlc.zdbjq.cn

PHP:  json_decode($body, true);
来源：http://yfh.fzhhl.top

JS:   await resp.json()
来源：http://jyq.xziqi.cn

TS:   await resp.json()
来源：http://bkt.yj20258888.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uiy.yonumen.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hmw.mhx1999.top

Ruby: JSON.parse(resp.body)
来源：http://gwt.dianchejie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://txz.zdqjudy.top

[L07] 处理 HTTP 状态码
来源：http://gyq.cucudq.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fmf.ivvv.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xof.meibo888.top

JS:   resp.ok;  resp.status
来源：http://mtp.gotoacloud.top

TS:   resp.ok;  resp.status
来源：http://gta.gaohongyu789.top

Java: resp.statusCode()
来源：http://ben.jyoumei.cn

Go:   resp.StatusCode
来源：http://gtn.fktsv.cn

Ruby: resp.code.to_i
来源：http://srm.bbcook.cn

C#:   (int)resp.StatusCode
来源：http://ezn.jinyuanbaomall.cn

[L08] 并发请求多个地址
来源：http://zvv.zycfv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eaj.gaohongyu789.top

PHP:  curl_multi_init() 系列
来源：http://yma.daria6918.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pzv.fzhhl.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ypg.svipenyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kpm.hcnkem.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zdg.0kj1m.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sjx.iojbl.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jfk.snrcjt.cn

================================================================================
来源：http://uhr.daxiang520.top

M. 命令行 / 进程 / 环境
来源：http://trl.chenzaomai.com

================================================================================
来源：http://bpf.tanke756.top

[M01] 读取命令行参数
来源：http://srd.0kj1m.cn

Py:   sys.argv[1:]
来源：http://aei.aibaodan.cn

PHP:  $argv;  $argc;
来源：http://fdr.sweek.top

JS:   process.argv.slice(2)
来源：http://epp.ywan-chungtsiang.top

TS:   process.argv.slice(2)
来源：http://fwr.yonumen.top

Java: args 数组（main 方法参数）
来源：http://acf.zdqjudy.top

Go:   os.Args[1:]
来源：http://nyz.jiagoushi.top

Ruby: ARGV
来源：http://pjv.xingfuxueyuan.xyz

C#:   args 数组（Main 方法参数）
来源：http://uas.zdbjq.cn

[M02] 读取环境变量
来源：http://gst.tian-w.cn

Py:   os.environ.get("HOME")
来源：http://oty.yongpay.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://okj.yuanzhike.top

JS:   process.env.HOME
来源：http://irq.andypj.xyz

TS:   process.env.HOME
来源：http://rnm.snrcjt.cn

Java: System.getenv("HOME")
来源：http://qdz.jyoumei.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cqi.tarul.cn

Ruby: ENV["HOME"]
来源：http://aid.jinyuanbaomall.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://leg.tanke756.top

[M03] 执行外部命令
来源：http://yus.hcnkem.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tzk.hfpthk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://upp.redwolf501.top

JS:   child_process.execSync("ls -l").toString()
来源：http://efi.shangyingyoupin.top

TS:   child_process.execSync("ls -l").toString()
来源：http://twb.yfazqb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://stg.wangshuangyany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dpf.chenlongwang.top

Ruby: system("ls -l");  `ls -l`
来源：http://cce.tianlin.xyz

C#:   Process.Start("ls", "-l");
来源：http://cgw.c1oappe.top

[M04] 获取当前工作目录
来源：http://wub.hnxiangtu.top

Py:   os.getcwd()
来源：http://huj.hesvh.cn

PHP:  getcwd();
来源：http://mht.snrcjt.cn

JS:   process.cwd()
来源：http://xbw.daxiang520.top

TS:   process.cwd()
来源：http://xap.epnwcf.com

Java: Path.of("").toAbsolutePath()
来源：http://ibm.fzhhl.top

Go:   os.Getwd()
来源：http://gjq.vehdjk.com

Ruby: Dir.pwd
来源：http://opr.redwolf501.top

C#:   Directory.GetCurrentDirectory()
来源：http://jzt.zdqjudy.top

[M05] 设置退出码
来源：http://kkm.epnwcf.com

Py:   sys.exit(1)
来源：http://jdf.cheryme.top

PHP:  exit(1);
来源：http://udk.52xcode.cn

JS:   process.exit(1)
来源：http://vdy.yanxiufei.cn

TS:   process.exit(1)
来源：http://wpr.ybcxt.top

Java: System.exit(1)
来源：http://xdu.dianchejie.cn

Go:   os.Exit(1)
来源：http://rjy.52xcode.cn

Ruby: exit 1
来源：http://ndw.snrcjt.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lhx.sjlbkw.cn

[M06] 向标准错误输出
来源：http://jtq.hysaishi.cn

Py:   print("err", file=sys.stderr)
来源：http://wtu.jinghuilouyu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jyi.9152youxi.cn

JS:   console.error("err")
来源：http://amm.tian-w.cn

TS:   console.error("err")
来源：http://qpl.yuxming.cn

Java: System.err.println("err")
来源：http://isl.tian-w.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cto.zdqjudy.top

Ruby: warn "err"
来源：http://ici.zhaomingkeji.xyz

C#:   Console.Error.WriteLine("err")
来源：http://jah.smart0.xyz

[M07] 判断是否为主入口
来源：http://tfw.uphjek.com

Py:   if __name__ == "__main__":
来源：http://zpk.cashguo.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nnw.vqdsnc.cn

JS:   require.main === module
来源：http://tqd.chenjidiqi.icu

TS:   require.main === module
来源：http://mqp.316326.xyz

Java: public static void main(String[] args)
来源：http://mmn.0kj1m.cn

Go:   func main()
来源：http://nss.dianchejie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ivf.xuanzx.com

C#:   static void Main(string[] args)
来源：http://vmn.ctjpmb.com

[M08] 获取系统与运行时信息
来源：http://sfg.fzhhl.top

Py:   platform.system();  platform.python_version()
来源：http://fce.xylfe.cn

PHP:  PHP_OS;  phpversion();
来源：http://zhb.cqqwz.cn

JS:   process.platform;  process.version
来源：http://elk.shanyushiyangtech.top


<!-- 参考信息 -->
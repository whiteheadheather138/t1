代发 wailian999

Go:   time.Now()
来源：http://qru.pycfn.com

Ruby: Time.now
来源：http://hze.cqqwz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vty.havefunace.top

[J02] 格式化输出
来源：http://wsu.fehbvm.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wte.cashguo.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xhn.sjlbkw.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://eqh.zhaomingkeji.xyz

TS:   d.toISOString()
来源：http://jbj.feifeiyinyue.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zwz.smart0.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://eqc.pycfn.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://krt.birdmap.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jlm.ivvv.top

[J03] 字符串解析为日期
来源：http://son.sjlbkw.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ahk.aibaodan.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://shg.pengpengdd.cyou

JS:   new Date("2024-01-02")
来源：http://nda.jlsjyb.cn

TS:   new Date("2024-01-02")
来源：http://byj.yvedp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jmp.bbcook.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eqi.epnwcf.com

Ruby: Date.parse("2024-01-02")
来源：http://pjm.fktsv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ing.yfazqb.com

[J04] 时间戳与日期互转
来源：http://jtx.shzxlz.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qqr.yvedp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sby.zhengqikj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oiy.fengsongda.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zqy.hongshengwenyu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wkm.shzxlz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xog.redwolf501.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wix.bjfxy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jou.jlsjyb.cn

[J05] 时间加减（加 7 天）
来源：http://hjv.shuidangran.top

Py:   now + timedelta(days=7)
来源：http://oix.ydjk.org.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pjc.haohaochexian.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fii.zhengqikj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ujf.yfazqb.com

Java: LocalDate.now().plusDays(7)
来源：http://ocj.hnxiangtu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rjb.yuxming.cn

Ruby: Time.now + 7 * 86400
来源：http://eml.zhongyouzk.top

C#:   DateTime.Now.AddDays(7)
来源：http://olp.c1oappe.top

[J06] 计算两时间之差
来源：http://fcp.bjfxy.top

Py:   (end - start).total_seconds()
来源：http://pev.zdbjq.cn

PHP:  $end->diff($start)->days;
来源：http://pdx.hammf.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qpp.redwolf501.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://col.bjfxy.top

Java: Duration.between(start, end).toSeconds()
来源：http://fds.hysaishi.cn

Go:   end.Sub(start).Hours()
来源：http://vcy.wangdashe.top

Ruby: end - start                 # 返回秒数
来源：http://mkl.sweek.top

C#:   (end - start).TotalSeconds
来源：http://fmw.zhongyouzk.top

[J07] 比较两个日期
来源：http://crw.tanke756.top

Py:   d1 < d2;  d1 == d2
来源：http://eqk.guannengcc.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://afe.zhiwuduotai.top

JS:   d1.getTime() < d2.getTime()
来源：http://rfg.vqdsnc.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jld.jqgufenzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lsg.hammf.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mdl.jiagoushi.top

Ruby: d1 < d2;  d1 == d2
来源：http://car.jiagoushi.top

C#:   d1 < d2;  d1 == d2
来源：http://ulx.zhengqikj.top

[J08] 提取年月日与星期
来源：http://xmi.sufxvd.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pks.hesvh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wzb.yvedp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rna.sufxvd.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://szm.hywenlv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nok.ybcxt.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gzw.gzhubu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ubs.jinqigufen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pvv.zdbjq.cn

[J09] 时区处理
来源：http://pfm.bbcook.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yot.fanxiaobao.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://chm.xingfuxueyuan.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wrc.xuanzx.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uod.shzxlz.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gzj.daria6918.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gzx.sxryk.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xkh.xziqi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://naw.hammf.cn

[J10] 取今天 / 本月第一天
来源：http://xca.jyoumei.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bby.jianghu66.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pnc.jlsjyb.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pvx.shanyushiyangkeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://axk.hcnkem.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://miu.quarkkingdee.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fzo.0kj1m.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cxm.gaohongyu789.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://szu.52xcode.cn

================================================================================
来源：http://lhp.zhijiandao.cn

K. JSON 与序列化
来源：http://sjc.jinyuanbaomall.cn

================================================================================
来源：http://eqg.sufxvd.cn

[K01] 对象转 JSON 字符串
来源：http://uct.shuidangran.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://twf.sysykeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nmy.pycfn.com

JS:   JSON.stringify(obj)
来源：http://wse.hcnkem.com

TS:   JSON.stringify(obj)
来源：http://rfh.yj20258888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://plp.xylfe.cn

Go:   json.Marshal(obj)
来源：http://wao.ppjwa.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zlp.daria6918.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://upf.hysaishi.cn

[K02] JSON 字符串转对象
来源：http://zto.mhx1999.top

Py:   json.loads(s)
来源：http://ybj.hesvh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gqq.ivvv.top

JS:   JSON.parse(s)
来源：http://ujn.dashuyun.cn

TS:   JSON.parse(s)
来源：http://jam.havefunace.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vxo.gotoacloud.top

Go:   json.Unmarshal(data, &v)
来源：http://adc.ybcxt.top

Ruby: JSON.parse(s)
来源：http://dtr.ydjk.org.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mzu.cashguo.top

[K03] JSON 美化输出（带缩进）
来源：http://lya.fktsv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tmn.jlsjyb.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bgd.andypj.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://sfd.cheryme.top

TS:   JSON.stringify(obj, null, 2)
来源：http://syr.sufxvd.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kgj.shanyushiyangtech.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qug.52xcode.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fpb.316326.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://irv.uphjek.com

[K04] 读取 JSON 文件
来源：http://zpy.gogol.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lud.wangdashe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gwn.wangdashe.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xiv.zhiwuduotai.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vnh.zhongyouzk.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ggi.yj202588.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kgr.jqgufenzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ywv.bbcook.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jde.cqqwz.cn

[K05] 深拷贝对象
来源：http://wkh.yonumen.top

Py:   copy.deepcopy(obj)
来源：http://khr.jinyuanbaomall.cn

PHP:  unserialize(serialize($obj));
来源：http://tzl.yvedp.cn

JS:   structuredClone(obj)
来源：http://wml.xinyue.icu

TS:   structuredClone(obj)
来源：http://mty.aibaodan.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gdr.tarul.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kex.chenjidiqi.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zak.jqgufenzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://qyy.hywenlv.cn

[K06] 解析 URL 查询串
来源：http://iyb.havefunace.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gjl.cqqwz.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baw.shuidangran.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xpn.jqgufenzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jtc.yonumen.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wju.jinqigufen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ouj.nwbrower.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zsi.ppjwa.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pav.ybcxt.top

[K07] 进制转换
来源：http://lyu.guannengcc.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rgc.guowangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://aka.gzhubu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://joj.zdqjudy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qsq.ybcxt.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oaq.smart0.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bit.ybcxt.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qqk.gogol.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hye.xinyue.icu

[K08] 二进制序列化（非 JSON）
来源：http://epp.zhongyouzk.top

Py:   pickle.dumps(obj)
来源：http://jph.haohaochexian.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ddo.shangyingyoupin.top

JS:   v8.serialize(obj)        // Node
来源：http://zxd.xziqi.cn

TS:   v8.serialize(obj)        // Node
来源：http://stl.bjfxy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yst.jinyuanbaomall.cn

Go:   encoding/gob
来源：http://exy.xinyue.icu

Ruby: Marshal.dump(obj)
来源：http://qcw.hfpthk.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://trp.svipenyu.cn

================================================================================
来源：http://eso.zhongyouzk.top

L. 网络请求
来源：http://dzx.ctjpmb.com

================================================================================
来源：http://oln.yuanzhike.top

[L01] 发送 GET 请求
来源：http://qbk.uphjek.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pqm.bbcook.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qwq.jlsjyb.cn

JS:   await fetch(url)
来源：http://qtn.cashguo.top

TS:   await fetch(url)
来源：http://mts.aibaodan.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hqz.tanke756.top

Go:   resp, err := http.Get(url)
来源：http://coi.yfazqb.com

Ruby: Net::HTTP.get(URI(url))
来源：http://eyk.jqgufenzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://aot.xuanzx.com

[L02] 发送 POST JSON
来源：http://zti.nwbrower.top

Py:   requests.post(url, json={"a": 1})
来源：http://mso.sweek.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tym.shanyushiyangtech.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ird.yonumen.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xrz.jqgufenzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zrl.bbcook.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ons.redwolf501.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cne.xuanzx.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jfu.aibaodan.cn

[L03] 设置自定义请求头
来源：http://bmr.tanke756.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://knq.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mqd.aizwys.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://reg.jinyuanbaomall.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zkn.meibo888.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jtc.epnwcf.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pfy.c1oappe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://roa.hnxiangtu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://svd.jinqigufen.top

[L04] 设置超时
来源：http://rcu.fengsongda.top

Py:   requests.get(url, timeout=5)
来源：http://dae.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gtp.fzhhl.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://per.vehdjk.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vgu.yuxming.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hhc.xziqi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xsf.ivvv.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sug.sufxvd.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wag.tarul.cn

[L05] 上传文件（multipart）
来源：http://nfp.yonumen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qfv.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gam.ywan-chungtsiang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ujv.tianlin.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vny.zhengqikj.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gzv.jinghuilouyu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sfs.yueranfly.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cjc.sufxvd.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pcu.smart0.xyz

[L06] 解析响应为 JSON
来源：http://rwk.52xcode.cn

Py:   resp.json()
来源：http://wsi.yuxming.cn

PHP:  json_decode($body, true);
来源：http://tho.yfazqb.com

JS:   await resp.json()
来源：http://ztn.cqqwz.cn

TS:   await resp.json()
来源：http://mpu.tian-w.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xsp.jqgfzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vaw.redwolf501.top

Ruby: JSON.parse(resp.body)
来源：http://ijq.nwbrower.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iox.aizwys.cn

[L07] 处理 HTTP 状态码
来源：http://ndr.jyoumei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mnq.guannengcc.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lbg.9152youxi.cn

JS:   resp.ok;  resp.status
来源：http://bxb.nwbrower.top

TS:   resp.ok;  resp.status
来源：http://vei.sjlbkw.cn

Java: resp.statusCode()
来源：http://pmc.daxiang520.top

Go:   resp.StatusCode
来源：http://awm.xuanzx.com

Ruby: resp.code.to_i
来源：http://twe.svipenyu.cn

C#:   (int)resp.StatusCode
来源：http://nqb.ywan-chungtsiang.top

[L08] 并发请求多个地址
来源：http://kup.ctjpmb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lts.jianghu66.top

PHP:  curl_multi_init() 系列
来源：http://oih.yuanzhike.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lji.shuidangran.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rii.guannengcc.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yzh.gogol.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jul.cucudq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pzb.fktsv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nrz.gotoacloud.top

================================================================================
来源：http://zim.sysykeji.top

M. 命令行 / 进程 / 环境
来源：http://pco.epnwcf.com

================================================================================
来源：http://ibm.yj20258.top

[M01] 读取命令行参数
来源：http://mhq.meibo888.top

Py:   sys.argv[1:]
来源：http://dek.yj20258.top

PHP:  $argv;  $argc;
来源：http://eld.tianlin.xyz

JS:   process.argv.slice(2)
来源：http://rhm.zhixingplan.top

TS:   process.argv.slice(2)
来源：http://aom.zhijiandao.cn

Java: args 数组（main 方法参数）
来源：http://kpy.aizwys.cn

Go:   os.Args[1:]
来源：http://xtj.yongpay.top

Ruby: ARGV
来源：http://zah.meibo888.top

C#:   args 数组（Main 方法参数）
来源：http://lhb.svipenyu.cn

[M02] 读取环境变量
来源：http://gvu.smart0.xyz

Py:   os.environ.get("HOME")
来源：http://umv.quarkkingdee.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xzr.yj20258.top

JS:   process.env.HOME
来源：http://clb.shuidangran.top

TS:   process.env.HOME
来源：http://xpz.jlsjyb.cn

Java: System.getenv("HOME")
来源：http://trb.shuidangran.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gki.tanke756.top

Ruby: ENV["HOME"]
来源：http://ejn.cdnleiting.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nls.jqgfzy.top

[M03] 执行外部命令
来源：http://gqo.cdnleiting.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wmp.iojbl.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ipj.xingfuxueyuan.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://xtj.feifeiyinyue.top

TS:   child_process.execSync("ls -l").toString()
来源：http://pjp.guannengcc.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kaj.shanyushiyangkeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vfm.shangyingyoupin.top

Ruby: system("ls -l");  `ls -l`
来源：http://pbd.chenzaomai.com

C#:   Process.Start("ls", "-l");
来源：http://qse.tanke756.top

[M04] 获取当前工作目录
来源：http://ztz.fehbvm.com

Py:   os.getcwd()
来源：http://fcg.daria6918.cn

PHP:  getcwd();
来源：http://hbk.xuetiantiany.cn

JS:   process.cwd()
来源：http://wej.hywenlv.cn

TS:   process.cwd()
来源：http://dax.zhongyouzk.top

Java: Path.of("").toAbsolutePath()
来源：http://bkg.52xcode.cn

Go:   os.Getwd()
来源：http://ycz.cheryme.top

Ruby: Dir.pwd
来源：http://jyg.ctjpmb.com

C#:   Directory.GetCurrentDirectory()
来源：http://bze.quarkkingdee.top

[M05] 设置退出码
来源：http://sio.zycfv.cn

Py:   sys.exit(1)
来源：http://qpg.fzhhl.top

PHP:  exit(1);
来源：http://xky.52xcode.cn

JS:   process.exit(1)
来源：http://oqb.cucudq.cn

TS:   process.exit(1)
来源：http://irg.9152youxi.cn

Java: System.exit(1)
来源：http://gcl.epnwcf.com

Go:   os.Exit(1)
来源：http://tmb.hnqzz.top

Ruby: exit 1
来源：http://xwe.daxiang520.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mre.shangyingyoupin.top

[M06] 向标准错误输出
来源：http://lwe.tianlin.xyz

Py:   print("err", file=sys.stderr)
来源：http://wfy.andypj.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://exe.yj202588.top

JS:   console.error("err")
来源：http://kkd.jianghu66.top

TS:   console.error("err")
来源：http://obu.xziqi.cn

Java: System.err.println("err")
来源：http://lml.cdnleiting.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zjp.quarkkingdee.top

Ruby: warn "err"
来源：http://vmx.zhixingplan.top

C#:   Console.Error.WriteLine("err")
来源：http://ate.yangfankeji.com

[M07] 判断是否为主入口
来源：http://wqr.tianlin.xyz

Py:   if __name__ == "__main__":
来源：http://jqv.cashguo.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://drv.jinghuilouyu.cn

JS:   require.main === module
来源：http://rab.zhongyouzk.top

TS:   require.main === module
来源：http://eiy.jinyuanbaomall.cn

Java: public static void main(String[] args)
来源：http://qnr.xinyue.icu

Go:   func main()
来源：http://mnf.ydzc1.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pwv.shangyingyoupin.top

C#:   static void Main(string[] args)
来源：http://vkk.daria6918.cn


<!-- 参考信息 -->
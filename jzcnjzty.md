代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://trq.yongpay.top

JS:   new Date();  Date.now()
来源：http://nku.ehwqpu.com

TS:   new Date();  Date.now()
来源：http://oro.guowangkeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://mzx.fktsv.cn

Go:   time.Now()
来源：http://xxh.jinghuilouyu.cn

Ruby: Time.now
来源：http://dxd.9152youxi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zee.vehdjk.com

[J02] 格式化输出
来源：http://ych.zdbjq.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gen.xylfe.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://viz.jinqigufen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://opo.andypj.xyz

TS:   d.toISOString()
来源：http://bfi.ppjwa.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ihc.yueranfly.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ljc.dianchejie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wtx.fehbvm.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lkr.jyoumei.cn

[J03] 字符串解析为日期
来源：http://qvx.pycfn.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dse.zhongyouzk.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hro.cdnleiting.top

JS:   new Date("2024-01-02")
来源：http://tzy.jlsjyb.cn

TS:   new Date("2024-01-02")
来源：http://weh.hywenlv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ima.chenlongwang.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bdv.kuanghao11.cn

Ruby: Date.parse("2024-01-02")
来源：http://xek.zhoulong.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hsq.cheryme.top

[J04] 时间戳与日期互转
来源：http://jfo.chenzaomai.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://spo.jinqigufen.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ogn.epnwcf.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yem.zhoulong.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://vti.jinghuilouyu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ctq.hnqzz.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://crl.snrcjt.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bur.yangfankeji.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yjf.c1oappe.top

[J05] 时间加减（加 7 天）
来源：http://hlc.vqdsnc.cn

Py:   now + timedelta(days=7)
来源：http://wkl.yvedp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yac.zhengqikj.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xtc.snrcjt.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mom.kuanghao11.cn

Java: LocalDate.now().plusDays(7)
来源：http://dsl.havefunace.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://elc.xuetiantiany.cn

Ruby: Time.now + 7 * 86400
来源：http://rix.hnxiangtu.top

C#:   DateTime.Now.AddDays(7)
来源：http://rtk.gotoacloud.top

[J06] 计算两时间之差
来源：http://pni.hnxiangtu.top

Py:   (end - start).total_seconds()
来源：http://oqy.jqgufenzy.top

PHP:  $end->diff($start)->days;
来源：http://opz.vqdsnc.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fpx.sysykeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uhy.hcnkem.com

Java: Duration.between(start, end).toSeconds()
来源：http://bdl.hcnkem.com

Go:   end.Sub(start).Hours()
来源：http://gze.zhixingplan.top

Ruby: end - start                 # 返回秒数
来源：http://ptp.yuanzhike.top

C#:   (end - start).TotalSeconds
来源：http://pnq.ivvv.top

[J07] 比较两个日期
来源：http://tvu.mhx1999.top

Py:   d1 < d2;  d1 == d2
来源：http://fpa.hysaishi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tti.cheryme.top

JS:   d1.getTime() < d2.getTime()
来源：http://gbv.tian-w.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vdx.yvedp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ylj.zhixingplan.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://poh.bbcook.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lmq.ivvv.top

C#:   d1 < d2;  d1 == d2
来源：http://nkc.vehdjk.com

[J08] 提取年月日与星期
来源：http://xez.yuxming.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://arn.xziqi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mih.shangyingyoupin.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dam.zdqjudy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://stn.zhengqikj.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ddn.quarkkingdee.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jrh.xuanzx.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://apq.yonumen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ntt.wangshuangyany.cn

[J09] 时区处理
来源：http://vfu.ywan-chungtsiang.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wyx.jqgfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pxf.cashguo.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ivg.yj202588.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lqp.cqqwz.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://spg.jqgfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hot.yuxming.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rwd.hysaishi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://raa.daria6918.cn

[J10] 取今天 / 本月第一天
来源：http://zmi.jyoumei.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wsy.hcnkem.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://smz.daxiang520.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xpb.cucudq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://slz.zycfv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bkn.9152youxi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gvq.jinqigufen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jbm.bjfxy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pfe.zhixingplan.top

================================================================================
来源：http://uuy.haohaochexian.top

K. JSON 与序列化
来源：http://gls.wangshuangyany.cn

================================================================================
来源：http://jlz.tanke756.top

[K01] 对象转 JSON 字符串
来源：http://nnt.hcnkem.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xoz.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ssn.tian-w.cn

JS:   JSON.stringify(obj)
来源：http://lll.iojbl.cn

TS:   JSON.stringify(obj)
来源：http://xlo.fzhhl.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mej.52xcode.cn

Go:   json.Marshal(obj)
来源：http://rhj.xingfuxueyuan.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://ggn.jinqigufen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tjl.zhiwuduotai.top

[K02] JSON 字符串转对象
来源：http://txi.52xcode.cn

Py:   json.loads(s)
来源：http://jyp.uphjek.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ubm.nwbrower.top

JS:   JSON.parse(s)
来源：http://nbs.sxryk.cn

TS:   JSON.parse(s)
来源：http://ihv.vqdsnc.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fyj.epnwcf.com

Go:   json.Unmarshal(data, &v)
来源：http://vqd.yvedp.cn

Ruby: JSON.parse(s)
来源：http://hho.shuidangran.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eqd.nwbrower.top

[K03] JSON 美化输出（带缩进）
来源：http://tno.jinqigfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://egw.mhx1999.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://eqi.hfpthk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cgw.hysaishi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://seo.zhixingplan.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lvd.cucudq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://erq.c1oappe.top

Ruby: JSON.pretty_generate(obj)
来源：http://bpx.sysykeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://szc.dashuyun.cn

[K04] 读取 JSON 文件
来源：http://iyl.hfpthk.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sdf.gogol.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oym.zhengqikj.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sgq.hnqzz.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://buw.zhaomingkeji.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jvx.fengsongda.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://upz.haohaochexian.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://bbm.jinghuilouyu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fwk.jqgufenzy.top

[K05] 深拷贝对象
来源：http://uwx.shanyushiyangkeji.top

Py:   copy.deepcopy(obj)
来源：http://jxh.cqqwz.cn

PHP:  unserialize(serialize($obj));
来源：http://knp.hfpthk.cn

JS:   structuredClone(obj)
来源：http://yic.yvedp.cn

TS:   structuredClone(obj)
来源：http://sld.cashguo.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vnm.smart0.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qbf.chenjidiqi.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://byo.chenlongwang.top

C#:   // 序列化往返，或自定义 Clone
来源：http://qwp.gzhubu.top

[K06] 解析 URL 查询串
来源：http://fvm.gzhubu.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gtr.kuanghao11.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hrj.yj20258888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pag.dashuyun.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://glp.zhixingplan.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pew.wangshuangyany.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://udp.xingfuxueyuan.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cdu.hammf.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xub.jinqigufen.top

[K07] 进制转换
来源：http://zhw.gogol.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zdy.yj202588.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xfs.c1oappe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baf.yj20258.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xxh.cdnleiting.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qyd.feifeiyinyue.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cip.andypj.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qtf.hnqzz.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jsg.epnwcf.com

[K08] 二进制序列化（非 JSON）
来源：http://dso.xinyue.icu

Py:   pickle.dumps(obj)
来源：http://nrv.0kj1m.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://idy.hammf.cn

JS:   v8.serialize(obj)        // Node
来源：http://dyq.ywan-chungtsiang.top

TS:   v8.serialize(obj)        // Node
来源：http://tcv.xinyue.icu

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hul.jiagoushi.top

Go:   encoding/gob
来源：http://dby.0kj1m.cn

Ruby: Marshal.dump(obj)
来源：http://qey.yj20258.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lic.yanxiufei.cn

================================================================================
来源：http://rhs.yj202588.top

L. 网络请求
来源：http://mrx.redwolf501.top

================================================================================
来源：http://egl.pycfn.com

[L01] 发送 GET 请求
来源：http://knx.gotoacloud.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ocl.dianchejie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fcp.hnxiangtu.top

JS:   await fetch(url)
来源：http://byp.pengpengdd.cyou

TS:   await fetch(url)
来源：http://rty.tianlin.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uff.ivvv.top

Go:   resp, err := http.Get(url)
来源：http://akh.gotoacloud.top

Ruby: Net::HTTP.get(URI(url))
来源：http://cjr.cashguo.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sof.iojbl.cn

[L02] 发送 POST JSON
来源：http://eze.havefunace.top

Py:   requests.post(url, json={"a": 1})
来源：http://sbf.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cip.gzhubu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tvi.pycfn.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xkf.yvedp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ojz.jiagoushi.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rpb.jqgfzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ldn.uphjek.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ixw.cheryme.top

[L03] 设置自定义请求头
来源：http://cyy.zhengqikj.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uyd.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mqp.shzxlz.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lxg.cucudq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wqv.52xcode.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lfs.birdmap.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wac.ybcxt.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pjz.yj20258888.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nou.ehwqpu.com

[L04] 设置超时
来源：http://qhu.shangyingyoupin.top

Py:   requests.get(url, timeout=5)
来源：http://ggv.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://imt.jinqigfzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wai.cashguo.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dcy.hongshengwenyu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wxi.andypj.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dbl.jinghuilouyu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xta.haohaochexian.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pys.zhaomingkeji.xyz

[L05] 上传文件（multipart）
来源：http://ztt.guowangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lnb.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://abu.daxiang520.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://iag.vqdsnc.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hvj.epnwcf.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ioq.guannengcc.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ahe.nwbrower.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sdr.uphjek.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yyd.c1oappe.top

[L06] 解析响应为 JSON
来源：http://lpp.gogol.net.cn

Py:   resp.json()
来源：http://nkd.mhx1999.top

PHP:  json_decode($body, true);
来源：http://uux.316326.xyz

JS:   await resp.json()
来源：http://ngk.birdmap.top

TS:   await resp.json()
来源：http://kjc.yuxming.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ouz.cheryme.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zam.zhixingplan.top

Ruby: JSON.parse(resp.body)
来源：http://iiw.sjlbkw.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zgj.dianchejie.cn

[L07] 处理 HTTP 状态码
来源：http://knq.daria6918.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gom.cucudq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lmq.52xcode.cn

JS:   resp.ok;  resp.status
来源：http://rpy.jiagoushi.top

TS:   resp.ok;  resp.status
来源：http://nvs.haohaochexian.top

Java: resp.statusCode()
来源：http://msl.guowangkeji.top

Go:   resp.StatusCode
来源：http://pxw.ybcxt.top

Ruby: resp.code.to_i
来源：http://oqw.guowangkeji.top

C#:   (int)resp.StatusCode
来源：http://gax.shanyushiyangtech.top

[L08] 并发请求多个地址
来源：http://oxx.jinqigfzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rtn.chenlongwang.top

PHP:  curl_multi_init() 系列
来源：http://gzd.yuanzhike.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fqx.0kj1m.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gbx.dianchejie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uau.sxryk.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kpv.ehwqpu.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zvi.shanyushiyangkeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oda.sxryk.cn

================================================================================
来源：http://ate.shangyingyoupin.top

M. 命令行 / 进程 / 环境
来源：http://ogl.aibaodan.cn

================================================================================
来源：http://frs.yueranfly.top

[M01] 读取命令行参数
来源：http://yfw.andypj.xyz

Py:   sys.argv[1:]
来源：http://xwz.hnqzz.top

PHP:  $argv;  $argc;
来源：http://cul.kuanghao11.cn

JS:   process.argv.slice(2)
来源：http://mur.feifeiyinyue.top

TS:   process.argv.slice(2)
来源：http://rqv.bjfxy.top

Java: args 数组（main 方法参数）
来源：http://utw.cheryme.top

Go:   os.Args[1:]
来源：http://afs.yuxming.cn

Ruby: ARGV
来源：http://lsj.xingfuxueyuan.xyz

C#:   args 数组（Main 方法参数）
来源：http://ded.shzxlz.cn

[M02] 读取环境变量
来源：http://svk.zycfv.cn

Py:   os.environ.get("HOME")
来源：http://fwl.xingfuxueyuan.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ylq.haohaochexian.top

JS:   process.env.HOME
来源：http://exw.jinghuilouyu.cn

TS:   process.env.HOME
来源：http://jxq.chenlongwang.top

Java: System.getenv("HOME")
来源：http://pky.dashuyun.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pqh.jyoumei.cn

Ruby: ENV["HOME"]
来源：http://tzs.xingfuxueyuan.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jxt.bbcook.cn

[M03] 执行外部命令
来源：http://kvm.gogol.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rzd.dianchejie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mpe.jianghu66.top

JS:   child_process.execSync("ls -l").toString()
来源：http://gnp.ybcxt.top

TS:   child_process.execSync("ls -l").toString()
来源：http://fjp.tian-w.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yjc.epnwcf.com

Go:   exec.Command("ls", "-l").Output()
来源：http://liz.jqgfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://jnw.pengpengdd.cyou

C#:   Process.Start("ls", "-l");
来源：http://rmd.epnwcf.com

[M04] 获取当前工作目录
来源：http://egk.sufxvd.cn

Py:   os.getcwd()
来源：http://oss.havefunace.top

PHP:  getcwd();
来源：http://chz.zhiwuduotai.top

JS:   process.cwd()
来源：http://vrv.meibo888.top

TS:   process.cwd()
来源：http://efu.yj20258888.top

Java: Path.of("").toAbsolutePath()
来源：http://tkh.epnwcf.com

Go:   os.Getwd()
来源：http://unr.hcnkem.com

Ruby: Dir.pwd
来源：http://muv.52xcode.cn

C#:   Directory.GetCurrentDirectory()
来源：http://arf.xuetiantiany.cn

[M05] 设置退出码
来源：http://sbd.316326.xyz

Py:   sys.exit(1)
来源：http://eud.sweek.top

PHP:  exit(1);
来源：http://mkf.zdbjq.cn

JS:   process.exit(1)
来源：http://udl.zhiwuduotai.top

TS:   process.exit(1)
来源：http://tmw.yj20258.top

Java: System.exit(1)
来源：http://zgh.shangyingyoupin.top

Go:   os.Exit(1)
来源：http://pcn.bbcook.cn

Ruby: exit 1
来源：http://gax.meibo888.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gnw.bbcook.cn

[M06] 向标准错误输出
来源：http://aqz.hnxiangtu.top

Py:   print("err", file=sys.stderr)
来源：http://tfh.mhx1999.top

PHP:  fwrite(STDERR, "err\n");
来源：http://yhc.snrcjt.cn

JS:   console.error("err")
来源：http://mtu.yongpay.top

TS:   console.error("err")
来源：http://fyw.vehdjk.com

Java: System.err.println("err")
来源：http://yjy.jinyuanbaomall.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tpw.yj20258888.top

Ruby: warn "err"
来源：http://mxc.shanyushiyangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://qwc.haohaochexian.top

[M07] 判断是否为主入口
来源：http://olm.sweek.top

Py:   if __name__ == "__main__":
来源：http://uaj.shangyingyoupin.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zqo.xziqi.cn

JS:   require.main === module
来源：http://krh.svipenyu.cn

TS:   require.main === module
来源：http://dia.yanxiufei.cn


<!-- 参考信息 -->
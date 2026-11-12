代发 wailian999

J. 日期与时间
来源：http://pno.haohaochexian.top

================================================================================
来源：http://pcq.sxryk.cn

[J01] 获取当前时间
来源：http://tzx.zhixingplan.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://rvd.daria6918.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://met.nwbrower.top

JS:   new Date();  Date.now()
来源：http://fwe.xingfuxueyuan.xyz

TS:   new Date();  Date.now()
来源：http://ejf.nanxuanxn.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jwd.yongpay.top

Go:   time.Now()
来源：http://zoq.yvedp.cn

Ruby: Time.now
来源：http://iev.daxiang520.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ztp.ppjwa.cn

[J02] 格式化输出
来源：http://nlz.shanyushiyangtech.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iiw.yonumen.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gul.hongshengwenyu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uey.zdqjudy.top

TS:   d.toISOString()
来源：http://xzl.shanyushiyangtech.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pga.yfazqb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://emm.jiagoushi.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hdx.zycfv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fgu.tianlin.xyz

[J03] 字符串解析为日期
来源：http://brd.pycfn.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mco.aizwys.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dsp.ywan-chungtsiang.top

JS:   new Date("2024-01-02")
来源：http://qsf.guowangkeji.top

TS:   new Date("2024-01-02")
来源：http://pde.jqgufenzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://cgh.xuetiantiany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://irq.hfpthk.cn

Ruby: Date.parse("2024-01-02")
来源：http://dbb.shangyingyoupin.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xtx.chenlongwang.top

[J04] 时间戳与日期互转
来源：http://xbk.ydzc1.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fnk.yongpay.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zlm.hnxiangtu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fbe.sjlbkw.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ygx.svipenyu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vrk.jianghu66.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kik.jinghuilouyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zfm.tian-w.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jen.zhoulong.xyz

[J05] 时间加减（加 7 天）
来源：http://vwy.havefunace.top

Py:   now + timedelta(days=7)
来源：http://gwt.yvedp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://iuo.jqgfzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pxa.ivvv.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rmy.shzxlz.cn

Java: LocalDate.now().plusDays(7)
来源：http://dzy.ydjk.org.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dnp.ywan-chungtsiang.top

Ruby: Time.now + 7 * 86400
来源：http://ait.dashuyun.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nrv.daria6918.cn

[J06] 计算两时间之差
来源：http://uhz.havefunace.top

Py:   (end - start).total_seconds()
来源：http://kga.yj20258.top

PHP:  $end->diff($start)->days;
来源：http://jjx.haohaochexian.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sxj.dianchejie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xhb.shzxlz.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mtv.fktsv.cn

Go:   end.Sub(start).Hours()
来源：http://mqi.xuanzx.com

Ruby: end - start                 # 返回秒数
来源：http://cng.xuanzx.com

C#:   (end - start).TotalSeconds
来源：http://mwz.birdmap.top

[J07] 比较两个日期
来源：http://xtz.guowangkeji.top

Py:   d1 < d2;  d1 == d2
来源：http://dov.gotoacloud.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://opx.yuxming.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fna.dianchejie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ijb.dashuyun.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.redwolf501.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ipv.hnxiangtu.top

Ruby: d1 < d2;  d1 == d2
来源：http://voq.shangyingyoupin.top

C#:   d1 < d2;  d1 == d2
来源：http://ecz.zhengqikj.top

[J08] 提取年月日与星期
来源：http://ynq.zhiwuduotai.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://skk.shangyingyoupin.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://eau.hnxiangtu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nlv.yuxming.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bdx.smart0.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qtf.shuidangran.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zyu.iojbl.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jtf.pycfn.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bza.yj20258888.top

[J09] 时区处理
来源：http://gyb.jlsjyb.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zfv.xuanzx.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tqv.hysaishi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://adm.ydjk.org.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qsf.gotoacloud.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hjr.yuanzhike.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uhv.aibaodan.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://btn.hammf.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sdw.cashguo.top

[J10] 取今天 / 本月第一天
来源：http://fgy.tian-w.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://urd.andypj.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uim.jyoumei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jwi.c1oappe.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rff.yueranfly.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zfz.jlsjyb.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fkl.mhx1999.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vbu.cqqwz.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mpx.xingfuxueyuan.xyz

================================================================================
来源：http://fai.xuanzx.com

K. JSON 与序列化
来源：http://xkr.wangdashe.top

================================================================================
来源：http://nyv.wangdashe.top

[K01] 对象转 JSON 字符串
来源：http://knz.shanyushiyangtech.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gns.cashguo.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jsr.nanxinkj.top

JS:   JSON.stringify(obj)
来源：http://aym.yueranfly.top

TS:   JSON.stringify(obj)
来源：http://oia.shanyushiyangkeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oev.fktsv.cn

Go:   json.Marshal(obj)
来源：http://pzo.jianghu66.top

Ruby: obj.to_json                                     // require "json"
来源：http://slu.zhixingplan.top

C#:   JsonSerializer.Serialize(obj)
来源：http://enk.cdnleiting.top

[K02] JSON 字符串转对象
来源：http://pqh.52xcode.cn

Py:   json.loads(s)
来源：http://zwe.zycfv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xjx.cdnleiting.top

JS:   JSON.parse(s)
来源：http://noi.chenlongwang.top

TS:   JSON.parse(s)
来源：http://qnx.fehbvm.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ymy.tianlin.xyz

Go:   json.Unmarshal(data, &v)
来源：http://oym.zhixingplan.top

Ruby: JSON.parse(s)
来源：http://hfb.sxryk.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rpu.pengpengdd.cyou

[K03] JSON 美化输出（带缩进）
来源：http://nwi.ppjwa.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wnr.jqgfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nik.pengpengdd.cyou

JS:   JSON.stringify(obj, null, 2)
来源：http://qkc.shuidangran.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lee.yj202588.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dki.xylfe.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ssn.hfpthk.cn

Ruby: JSON.pretty_generate(obj)
来源：http://eaq.cheryme.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xyv.gaohongyu789.top

[K04] 读取 JSON 文件
来源：http://ire.haohaochexian.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ack.vqdsnc.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hqu.jinqigufen.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xnx.quarkkingdee.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jtk.cucudq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blc.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bfz.ctjpmb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://ysu.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://twy.cucudq.cn

[K05] 深拷贝对象
来源：http://rcj.redwolf501.top

Py:   copy.deepcopy(obj)
来源：http://lio.zdqjudy.top

PHP:  unserialize(serialize($obj));
来源：http://agr.sxryk.cn

JS:   structuredClone(obj)
来源：http://ahm.cucudq.cn

TS:   structuredClone(obj)
来源：http://ifw.aibaodan.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ftw.feifeiyinyue.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fxo.jqgfzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://msm.hysaishi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://emm.sweek.top

[K06] 解析 URL 查询串
来源：http://yok.daxiang520.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://stv.jyoumei.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cdo.gaohongyu789.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dwo.jiagoushi.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dkp.sjlbkw.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fyp.gzhubu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kph.zhijiandao.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oer.gotoacloud.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zhl.pycfn.com

[K07] 进制转换
来源：http://dxb.cucudq.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vov.zhixingplan.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fzu.guowangkeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zww.vehdjk.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vfn.316326.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://noq.guowangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jva.andypj.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ooo.fktsv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qes.guowangkeji.top

[K08] 二进制序列化（非 JSON）
来源：http://bma.hongshengwenyu.top

Py:   pickle.dumps(obj)
来源：http://alr.shanyushiyangtech.top

PHP:  serialize($obj);  unserialize($s);
来源：http://fvl.yuxming.cn

JS:   v8.serialize(obj)        // Node
来源：http://ahq.yj20258.top

TS:   v8.serialize(obj)        // Node
来源：http://nnp.0kj1m.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gzn.hfpthk.cn

Go:   encoding/gob
来源：http://ugd.kuanghao11.cn

Ruby: Marshal.dump(obj)
来源：http://vys.jinyuanbaomall.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cer.daxiang520.top

================================================================================
来源：http://kbq.yueranfly.top

L. 网络请求
来源：http://sba.ppjwa.cn

================================================================================
来源：http://pwc.wangshuangyany.cn

[L01] 发送 GET 请求
来源：http://fwn.gaohongyu789.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dfz.kuanghao11.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rms.yongpay.top

JS:   await fetch(url)
来源：http://fqf.yj20258888.top

TS:   await fetch(url)
来源：http://vcx.ivvv.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://von.vqdsnc.cn

Go:   resp, err := http.Get(url)
来源：http://nyv.aizwys.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kpw.sweek.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lfh.aibaodan.cn

[L02] 发送 POST JSON
来源：http://htk.zhoulong.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://nfv.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xud.mhx1999.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vws.shangyingyoupin.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ekf.cheryme.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rfv.epnwcf.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oay.cqqwz.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tea.ydjk.org.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fbq.jyoumei.cn

[L03] 设置自定义请求头
来源：http://itp.zhixingplan.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hxx.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oqu.sweek.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ybj.zhiwuduotai.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wum.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xef.hammf.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bus.ctjpmb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zih.svipenyu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://smj.havefunace.top

[L04] 设置超时
来源：http://jkr.fengsongda.top

Py:   requests.get(url, timeout=5)
来源：http://gvf.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qyx.dianchejie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://adk.gzhubu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://whg.gzhubu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tfj.sxryk.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mni.smart0.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ctv.jlsjyb.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://muy.jiagoushi.top

[L05] 上传文件（multipart）
来源：http://oez.birdmap.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kcz.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://opx.guannengcc.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pjr.guowangkeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nja.chenzaomai.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://unt.zhaomingkeji.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qdn.gotoacloud.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ggu.hesvh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://olu.xinyue.icu

[L06] 解析响应为 JSON
来源：http://rmj.hfpthk.cn

Py:   resp.json()
来源：http://wpl.chenzaomai.com

PHP:  json_decode($body, true);
来源：http://zdi.zhengqikj.top

JS:   await resp.json()
来源：http://dva.gogol.net.cn

TS:   await resp.json()
来源：http://upu.sjlbkw.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tep.chenjidiqi.icu

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wew.zycfv.cn

Ruby: JSON.parse(resp.body)
来源：http://rho.jiagoushi.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lyz.epnwcf.com

[L07] 处理 HTTP 状态码
来源：http://agg.hammf.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cnf.dashuyun.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hpz.hywenlv.cn

JS:   resp.ok;  resp.status
来源：http://ouh.redwolf501.top

TS:   resp.ok;  resp.status
来源：http://cop.hammf.cn

Java: resp.statusCode()
来源：http://puz.svipenyu.cn

Go:   resp.StatusCode
来源：http://orh.jinqigfzy.top

Ruby: resp.code.to_i
来源：http://mgp.shuidangran.top

C#:   (int)resp.StatusCode
来源：http://adl.zhoulong.xyz

[L08] 并发请求多个地址
来源：http://uxk.chenjidiqi.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dne.52xcode.cn

PHP:  curl_multi_init() 系列
来源：http://yid.shzxlz.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vzs.yueranfly.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wru.aibaodan.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bna.smart0.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cfi.dashuyun.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zgh.fehbvm.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gnq.chenzaomai.com

================================================================================
来源：http://jje.aizwys.cn

M. 命令行 / 进程 / 环境
来源：http://xei.svipenyu.cn

================================================================================
来源：http://mro.pycfn.com

[M01] 读取命令行参数
来源：http://ppi.ydjk.org.cn

Py:   sys.argv[1:]
来源：http://wus.pengpengdd.cyou

PHP:  $argv;  $argc;
来源：http://xda.aizwys.cn

JS:   process.argv.slice(2)
来源：http://fwy.guannengcc.top

TS:   process.argv.slice(2)
来源：http://lui.zhengqikj.top

Java: args 数组（main 方法参数）
来源：http://xxq.bjfxy.top

Go:   os.Args[1:]
来源：http://htn.tanke756.top

Ruby: ARGV
来源：http://ckj.shzxlz.cn

C#:   args 数组（Main 方法参数）
来源：http://pxd.ybcxt.top

[M02] 读取环境变量
来源：http://urg.yvedp.cn

Py:   os.environ.get("HOME")
来源：http://mro.0kj1m.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gmf.tian-w.cn

JS:   process.env.HOME
来源：http://cux.cashguo.top

TS:   process.env.HOME
来源：http://eam.dianchejie.cn

Java: System.getenv("HOME")
来源：http://pfy.aizwys.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vaw.zhoulong.xyz

Ruby: ENV["HOME"]
来源：http://edk.zhongyouzk.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://eak.ctjpmb.com

[M03] 执行外部命令
来源：http://ngj.uphjek.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rei.yj202588.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fvm.ivvv.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vvs.dashuyun.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oxl.xinyue.icu

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wpv.haohaochexian.top

Go:   exec.Command("ls", "-l").Output()
来源：http://zxa.gzhubu.top

Ruby: system("ls -l");  `ls -l`
来源：http://mxl.svipenyu.cn

C#:   Process.Start("ls", "-l");
来源：http://mgb.hywenlv.cn

[M04] 获取当前工作目录
来源：http://mir.jlsjyb.cn

Py:   os.getcwd()
来源：http://esl.uphjek.com

PHP:  getcwd();
来源：http://nfs.yanxiufei.cn

JS:   process.cwd()
来源：http://bvk.fzhhl.top

TS:   process.cwd()
来源：http://onf.hongshengwenyu.top

Java: Path.of("").toAbsolutePath()
来源：http://xwp.shuidangran.top

Go:   os.Getwd()
来源：http://ujg.ctjpmb.com

Ruby: Dir.pwd
来源：http://alv.snrcjt.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nvn.zhongyouzk.top

[M05] 设置退出码
来源：http://ttr.havefunace.top

Py:   sys.exit(1)
来源：http://yqs.dianchejie.cn

PHP:  exit(1);
来源：http://ytd.guannengcc.top

JS:   process.exit(1)
来源：http://zyl.tanke756.top

TS:   process.exit(1)
来源：http://arz.fehbvm.com

Java: System.exit(1)
来源：http://ohf.andypj.xyz

Go:   os.Exit(1)
来源：http://wju.daxiang520.top

Ruby: exit 1
来源：http://qmf.52xcode.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lkc.shzxlz.cn

[M06] 向标准错误输出
来源：http://yzm.shuidangran.top

Py:   print("err", file=sys.stderr)
来源：http://qah.cashguo.top

PHP:  fwrite(STDERR, "err\n");
来源：http://duz.nanxuanxn.top

JS:   console.error("err")
来源：http://qnm.daria6918.cn

TS:   console.error("err")
来源：http://cqp.c1oappe.top

Java: System.err.println("err")
来源：http://llm.sxryk.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qhl.jinyuanbaomall.cn

Ruby: warn "err"
来源：http://zqu.mhx1999.top

C#:   Console.Error.WriteLine("err")
来源：http://ekj.tianlin.xyz

[M07] 判断是否为主入口
来源：http://mwp.jlsjyb.cn


<!-- 参考信息 -->
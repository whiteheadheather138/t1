代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bla.dashuyun.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wib.bbcook.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://oqz.cheryme.top

================================================================================
来源：http://ljh.hnxiangtu.top

J. 日期与时间
来源：http://wfd.kuanghao11.cn

================================================================================
来源：http://wzs.gotoacloud.top

[J01] 获取当前时间
来源：http://sdv.gogol.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://oyb.hnqzz.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tmr.sweek.top

JS:   new Date();  Date.now()
来源：http://gzx.pengpengdd.cyou

TS:   new Date();  Date.now()
来源：http://riz.andypj.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://jmb.shangyingyoupin.top

Go:   time.Now()
来源：http://drx.ehwqpu.com

Ruby: Time.now
来源：http://znn.shuidangran.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nai.shanyushiyangkeji.top

[J02] 格式化输出
来源：http://cws.tanke756.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jjl.zhoulong.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pno.yanxiufei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://axw.yonumen.top

TS:   d.toISOString()
来源：http://fts.c1oappe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gym.gotoacloud.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ufi.shanyushiyangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zrp.gzhubu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://azy.0kj1m.cn

[J03] 字符串解析为日期
来源：http://zgh.xylfe.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://iro.ivvv.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wrk.xuanzx.com

JS:   new Date("2024-01-02")
来源：http://fkd.vqdsnc.cn

TS:   new Date("2024-01-02")
来源：http://wkj.fehbvm.com

Java: LocalDate.parse("2024-01-02")
来源：http://sxz.jqgfzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uqg.xylfe.cn

Ruby: Date.parse("2024-01-02")
来源：http://mcv.zhengqikj.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gda.daria6918.cn

[J04] 时间戳与日期互转
来源：http://ety.vehdjk.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yzf.aibaodan.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fzw.cheryme.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pkm.ehwqpu.com

TS:   Math.floor(Date.now() / 1000)
来源：http://gyn.yj202588.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vrs.fzhhl.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lmv.zhaomingkeji.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hky.yj20258888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wxa.epnwcf.com

[J05] 时间加减（加 7 天）
来源：http://xbk.zhixingplan.top

Py:   now + timedelta(days=7)
来源：http://qhs.yanxiufei.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tcl.yj202588.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yxf.zhengqikj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cgt.hnxiangtu.top

Java: LocalDate.now().plusDays(7)
来源：http://yuv.zdqjudy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vjv.ctjpmb.com

Ruby: Time.now + 7 * 86400
来源：http://cyd.gogol.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qdb.tianlin.xyz

[J06] 计算两时间之差
来源：http://vho.redwolf501.top

Py:   (end - start).total_seconds()
来源：http://eef.jqgufenzy.top

PHP:  $end->diff($start)->days;
来源：http://bgl.gotoacloud.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yaf.mhx1999.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cyh.ybcxt.top

Java: Duration.between(start, end).toSeconds()
来源：http://xck.dashuyun.cn

Go:   end.Sub(start).Hours()
来源：http://rab.yvedp.cn

Ruby: end - start                 # 返回秒数
来源：http://ujm.gaohongyu789.top

C#:   (end - start).TotalSeconds
来源：http://nfb.aizwys.cn

[J07] 比较两个日期
来源：http://qrv.fengsongda.top

Py:   d1 < d2;  d1 == d2
来源：http://vxb.chenjidiqi.icu

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rgd.shangyingyoupin.top

JS:   d1.getTime() < d2.getTime()
来源：http://vrq.sufxvd.cn

TS:   d1.getTime() < d2.getTime()
来源：http://asr.zhijiandao.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ijq.hongshengwenyu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tjq.zhaomingkeji.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://pjf.fzhhl.top

C#:   d1 < d2;  d1 == d2
来源：http://xhf.jqgfzy.top

[J08] 提取年月日与星期
来源：http://fxu.fktsv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zsg.xuanzx.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hlh.yuxming.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://epp.kuanghao11.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uhq.haohaochexian.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gol.hywenlv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wmb.jinqigufen.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yzz.chenzaomai.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sqr.nwbrower.top

[J09] 时区处理
来源：http://wws.fzhhl.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mly.yuanzhike.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://iut.jlsjyb.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mao.uphjek.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tdc.zhaomingkeji.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://myn.ywan-chungtsiang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ayj.yongpay.top

Ruby: Time.now.getlocal("+08:00")
来源：http://jws.wangshuangyany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://clj.yonumen.top

[J10] 取今天 / 本月第一天
来源：http://vcc.jyoumei.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gci.yonumen.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vzi.tianlin.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pzo.gotoacloud.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mtr.zhixingplan.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qew.ctjpmb.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kpj.jqgufenzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qck.kuanghao11.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://srg.0kj1m.cn

================================================================================
来源：http://gol.fktsv.cn

K. JSON 与序列化
来源：http://ppj.cqqwz.cn

================================================================================
来源：http://gow.tianlin.xyz

[K01] 对象转 JSON 字符串
来源：http://wed.yongpay.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wcf.yj20258888.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lgf.sxryk.cn

JS:   JSON.stringify(obj)
来源：http://onz.snrcjt.cn

TS:   JSON.stringify(obj)
来源：http://jdb.vehdjk.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iig.tian-w.cn

Go:   json.Marshal(obj)
来源：http://dqx.vqdsnc.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cpg.zhixingplan.top

C#:   JsonSerializer.Serialize(obj)
来源：http://rbm.316326.xyz

[K02] JSON 字符串转对象
来源：http://gmj.nanxinkj.top

Py:   json.loads(s)
来源：http://jfv.cqqwz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://asr.cashguo.top

JS:   JSON.parse(s)
来源：http://qfr.smart0.xyz

TS:   JSON.parse(s)
来源：http://naj.pycfn.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nia.cashguo.top

Go:   json.Unmarshal(data, &v)
来源：http://nii.jianghu66.top

Ruby: JSON.parse(s)
来源：http://nyv.guowangkeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://krx.yuxming.cn

[K03] JSON 美化输出（带缩进）
来源：http://crh.jiagoushi.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://llp.ydjk.org.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mvw.kuanghao11.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kiu.jinqigfzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://rhp.ydjk.org.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eom.redwolf501.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ncc.52xcode.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xli.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kqu.chenjidiqi.icu

[K04] 读取 JSON 文件
来源：http://chm.dashuyun.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kan.gotoacloud.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fra.tarul.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iin.0kj1m.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ocj.cheryme.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://snc.tarul.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zhh.andypj.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://yxq.jinghuilouyu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://iaz.xinyue.icu

[K05] 深拷贝对象
来源：http://cse.haohaochexian.top

Py:   copy.deepcopy(obj)
来源：http://cjk.xziqi.cn

PHP:  unserialize(serialize($obj));
来源：http://iqt.havefunace.top

JS:   structuredClone(obj)
来源：http://qnk.mhx1999.top

TS:   structuredClone(obj)
来源：http://pgq.zhengqikj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://hzr.redwolf501.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uqa.zhaomingkeji.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cne.yj202588.top

C#:   // 序列化往返，或自定义 Clone
来源：http://wvp.guannengcc.top

[K06] 解析 URL 查询串
来源：http://may.tanke756.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tsb.guannengcc.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xdq.zhaomingkeji.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ymk.xziqi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xre.mhx1999.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xvx.gzhubu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://uks.nwbrower.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://okm.fzhhl.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hxa.shanyushiyangkeji.top

[K07] 进制转换
来源：http://xeh.zhengqikj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nia.yj20258888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yhw.feifeiyinyue.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pkb.birdmap.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://apb.bbcook.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cbv.sjlbkw.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://skm.zhixingplan.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://frs.xylfe.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uuv.aibaodan.cn

[K08] 二进制序列化（非 JSON）
来源：http://diz.feifeiyinyue.top

Py:   pickle.dumps(obj)
来源：http://sjz.yangfankeji.com

PHP:  serialize($obj);  unserialize($s);
来源：http://dxu.birdmap.top

JS:   v8.serialize(obj)        // Node
来源：http://bwr.hfpthk.cn

TS:   v8.serialize(obj)        // Node
来源：http://kvt.0kj1m.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xrl.52xcode.cn

Go:   encoding/gob
来源：http://yda.yj20258.top

Ruby: Marshal.dump(obj)
来源：http://trg.zdbjq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iwa.zycfv.cn

================================================================================
来源：http://acq.zhoulong.xyz

L. 网络请求
来源：http://eee.yuxming.cn

================================================================================
来源：http://vrb.hesvh.cn

[L01] 发送 GET 请求
来源：http://lqo.guowangkeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mpl.yuxming.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rfa.mhx1999.top

JS:   await fetch(url)
来源：http://gdg.smart0.xyz

TS:   await fetch(url)
来源：http://ocj.chenzaomai.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qst.sxryk.cn

Go:   resp, err := http.Get(url)
来源：http://hbm.zhengqikj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ita.cashguo.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ftl.shuidangran.top

[L02] 发送 POST JSON
来源：http://dxh.jinghuilouyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vug.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wfk.vqdsnc.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yfx.zhijiandao.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iod.gogol.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ssh.yj20258.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fke.dashuyun.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tcn.ybcxt.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vkf.zhaomingkeji.xyz

[L03] 设置自定义请求头
来源：http://bft.ydjk.org.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://alj.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://grj.yuanzhike.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fdi.xziqi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mqp.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dqs.tanke756.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lbc.sxryk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pqw.ydjk.org.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xyu.c1oappe.top

[L04] 设置超时
来源：http://cqv.sxryk.cn

Py:   requests.get(url, timeout=5)
来源：http://tza.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wju.mhx1999.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hkz.yj20258.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wvs.9152youxi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ics.daria6918.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rqn.gogol.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mmk.aizwys.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mwa.hfpthk.cn

[L05] 上传文件（multipart）
来源：http://hxg.pengpengdd.cyou

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://alf.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://azw.dashuyun.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wsc.zdqjudy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mgx.fehbvm.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://the.svipenyu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://upl.jinyuanbaomall.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cov.sufxvd.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wsd.chenlongwang.top

[L06] 解析响应为 JSON
来源：http://oao.tarul.cn

Py:   resp.json()
来源：http://bij.hysaishi.cn

PHP:  json_decode($body, true);
来源：http://sxo.nanxinkj.top

JS:   await resp.json()
来源：http://sat.birdmap.top

TS:   await resp.json()
来源：http://npj.aibaodan.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kok.yfazqb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zql.kuanghao11.cn

Ruby: JSON.parse(resp.body)
来源：http://dnt.kuanghao11.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tih.ehwqpu.com

[L07] 处理 HTTP 状态码
来源：http://urk.dashuyun.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ohx.yj202588.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ngb.fanxiaobao.xyz

JS:   resp.ok;  resp.status
来源：http://kbq.yj20258888.top

TS:   resp.ok;  resp.status
来源：http://vsj.ehwqpu.com

Java: resp.statusCode()
来源：http://vir.fzhhl.top

Go:   resp.StatusCode
来源：http://jab.nanxuanxn.top

Ruby: resp.code.to_i
来源：http://cdy.hesvh.cn

C#:   (int)resp.StatusCode
来源：http://ozk.nanxinkj.top

[L08] 并发请求多个地址
来源：http://enq.316326.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://olf.snrcjt.cn

PHP:  curl_multi_init() 系列
来源：http://hjr.pengpengdd.cyou

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ljs.hfpthk.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zxk.ydjk.org.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://asx.feifeiyinyue.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sip.nwbrower.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bue.smart0.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ypt.jqgfzy.top

================================================================================
来源：http://yyy.tian-w.cn

M. 命令行 / 进程 / 环境
来源：http://idy.xylfe.cn

================================================================================
来源：http://gcv.zhongyouzk.top

[M01] 读取命令行参数
来源：http://yqw.wangshuangyany.cn

Py:   sys.argv[1:]
来源：http://guz.hnqzz.top

PHP:  $argv;  $argc;
来源：http://lkk.fzhhl.top

JS:   process.argv.slice(2)
来源：http://cyf.zhoulong.xyz

TS:   process.argv.slice(2)
来源：http://eyk.zhiwuduotai.top

Java: args 数组（main 方法参数）
来源：http://jbh.chenjidiqi.icu

Go:   os.Args[1:]
来源：http://bag.gogol.net.cn

Ruby: ARGV
来源：http://jmr.hcnkem.com

C#:   args 数组（Main 方法参数）
来源：http://ums.chenjidiqi.icu

[M02] 读取环境变量
来源：http://wnu.iojbl.cn

Py:   os.environ.get("HOME")
来源：http://gck.uphjek.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zrw.vqdsnc.cn

JS:   process.env.HOME
来源：http://dwt.xuanzx.com

TS:   process.env.HOME
来源：http://ble.hcnkem.com

Java: System.getenv("HOME")
来源：http://yve.yangfankeji.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lrr.jiagoushi.top

Ruby: ENV["HOME"]
来源：http://ycc.zhiwuduotai.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nid.hnxiangtu.top

[M03] 执行外部命令
来源：http://nqo.0kj1m.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jib.birdmap.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lqx.fehbvm.com

JS:   child_process.execSync("ls -l").toString()
来源：http://hjf.zycfv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jwf.sysykeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nqd.fanxiaobao.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://euu.hysaishi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zwp.svipenyu.cn

C#:   Process.Start("ls", "-l");
来源：http://crj.xylfe.cn

[M04] 获取当前工作目录
来源：http://cni.yongpay.top

Py:   os.getcwd()
来源：http://iyz.0kj1m.cn

PHP:  getcwd();
来源：http://hlp.52xcode.cn

JS:   process.cwd()
来源：http://imh.havefunace.top

TS:   process.cwd()
来源：http://xeh.jinyuanbaomall.cn

Java: Path.of("").toAbsolutePath()
来源：http://tlx.xingfuxueyuan.xyz

Go:   os.Getwd()
来源：http://fih.birdmap.top

Ruby: Dir.pwd
来源：http://ycy.gogol.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ewo.wangdashe.top

[M05] 设置退出码
来源：http://dru.cqqwz.cn

Py:   sys.exit(1)
来源：http://vxp.yuxming.cn

PHP:  exit(1);
来源：http://bfn.yj20258.top

JS:   process.exit(1)
来源：http://nux.yongpay.top

TS:   process.exit(1)
来源：http://kig.ctjpmb.com

Java: System.exit(1)
来源：http://cuf.zhixingplan.top

Go:   os.Exit(1)
来源：http://nbf.shangyingyoupin.top

Ruby: exit 1
来源：http://doa.yonumen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kwq.jinqigfzy.top

[M06] 向标准错误输出
来源：http://uwe.yongpay.top

Py:   print("err", file=sys.stderr)
来源：http://ciz.nanxinkj.top

PHP:  fwrite(STDERR, "err\n");
来源：http://nfd.dashuyun.cn

JS:   console.error("err")
来源：http://zhz.yangfankeji.com

TS:   console.error("err")
来源：http://xfr.vehdjk.com

Java: System.err.println("err")
来源：http://gtw.nanxinkj.top


<!-- 参考信息 -->
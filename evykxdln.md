代发 wailian999

Go:   time.Now()
来源：http://zha.nanxuanxn.top

Ruby: Time.now
来源：http://zfr.zdbjq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qio.yangfankeji.com

[J02] 格式化输出
来源：http://arv.shanyushiyangkeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gup.pengpengdd.cyou

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mur.shangyingyoupin.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cma.zhaomingkeji.xyz

TS:   d.toISOString()
来源：http://hub.yvedp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://exh.fzhhl.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bej.cheryme.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nzf.fanxiaobao.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hed.mhx1999.top

[J03] 字符串解析为日期
来源：http://yjq.sysykeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eie.nanxuanxn.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mjh.ehwqpu.com

JS:   new Date("2024-01-02")
来源：http://zzz.svipenyu.cn

TS:   new Date("2024-01-02")
来源：http://qsy.chenjidiqi.icu

Java: LocalDate.parse("2024-01-02")
来源：http://cma.cdnleiting.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gxg.havefunace.top

Ruby: Date.parse("2024-01-02")
来源：http://vav.sweek.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://irf.xuetiantiany.cn

[J04] 时间戳与日期互转
来源：http://lyj.yongpay.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lkl.fanxiaobao.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qeg.andypj.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wtr.yj20258.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ovm.hammf.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gvq.hnxiangtu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ruo.zdbjq.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://soz.zhijiandao.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nzx.redwolf501.top

[J05] 时间加减（加 7 天）
来源：http://nvm.c1oappe.top

Py:   now + timedelta(days=7)
来源：http://aey.zycfv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kom.ydjk.org.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://znd.nanxuanxn.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://swz.c1oappe.top

Java: LocalDate.now().plusDays(7)
来源：http://bjl.ctjpmb.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ufb.yfazqb.com

Ruby: Time.now + 7 * 86400
来源：http://mpx.ydjk.org.cn

C#:   DateTime.Now.AddDays(7)
来源：http://srp.quarkkingdee.top

[J06] 计算两时间之差
来源：http://rbm.0kj1m.cn

Py:   (end - start).total_seconds()
来源：http://gkw.xinyue.icu

PHP:  $end->diff($start)->days;
来源：http://lvu.ppjwa.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ipk.zhixingplan.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ymz.snrcjt.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qzf.jqgufenzy.top

Go:   end.Sub(start).Hours()
来源：http://oja.zhaomingkeji.xyz

Ruby: end - start                 # 返回秒数
来源：http://dpt.jinqigfzy.top

C#:   (end - start).TotalSeconds
来源：http://tnh.hcnkem.com

[J07] 比较两个日期
来源：http://cqg.quarkkingdee.top

Py:   d1 < d2;  d1 == d2
来源：http://rjs.haohaochexian.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yxh.sysykeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://jci.pengpengdd.cyou

TS:   d1.getTime() < d2.getTime()
来源：http://bwk.gaohongyu789.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qlw.yongpay.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ihk.ehwqpu.com

Ruby: d1 < d2;  d1 == d2
来源：http://lfy.shuidangran.top

C#:   d1 < d2;  d1 == d2
来源：http://lxv.bjfxy.top

[J08] 提取年月日与星期
来源：http://yyg.hfpthk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xzp.vqdsnc.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://acf.hongshengwenyu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rhx.jinyuanbaomall.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ssf.zhixingplan.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yma.ctjpmb.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fvi.tarul.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yek.chenlongwang.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://edp.hfpthk.cn

[J09] 时区处理
来源：http://hkk.cqqwz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vvu.wangdashe.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lcm.haohaochexian.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://emt.jinghuilouyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kwp.sweek.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zeh.cdnleiting.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ais.chenlongwang.top

Ruby: Time.now.getlocal("+08:00")
来源：http://khv.9152youxi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kvw.zdqjudy.top

[J10] 取今天 / 本月第一天
来源：http://sji.9152youxi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kfu.ctjpmb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://eqh.yj202588.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://trx.guannengcc.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ihc.nwbrower.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pdw.xinyue.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://orl.jianghu66.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nqn.cheryme.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gty.yuanzhike.top

================================================================================
来源：http://fvm.zhixingplan.top

K. JSON 与序列化
来源：http://zjr.sysykeji.top

================================================================================
来源：http://mtq.cqqwz.cn

[K01] 对象转 JSON 字符串
来源：http://xxo.yj202588.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vsi.sweek.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rnc.yanxiufei.cn

JS:   JSON.stringify(obj)
来源：http://djx.ctjpmb.com

TS:   JSON.stringify(obj)
来源：http://ekj.hywenlv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cuv.yanxiufei.cn

Go:   json.Marshal(obj)
来源：http://epw.cucudq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bix.daxiang520.top

C#:   JsonSerializer.Serialize(obj)
来源：http://kow.jqgufenzy.top

[K02] JSON 字符串转对象
来源：http://ppg.yangfankeji.com

Py:   json.loads(s)
来源：http://bww.fktsv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yan.haohaochexian.top

JS:   JSON.parse(s)
来源：http://avp.tarul.cn

TS:   JSON.parse(s)
来源：http://sev.gzhubu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nnm.hywenlv.cn

Go:   json.Unmarshal(data, &v)
来源：http://whf.wangdashe.top

Ruby: JSON.parse(s)
来源：http://ndx.cashguo.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hhp.ydzc1.top

[K03] JSON 美化输出（带缩进）
来源：http://bnn.zhengqikj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uuk.fzhhl.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cjc.sjlbkw.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rkj.xinyue.icu

TS:   JSON.stringify(obj, null, 2)
来源：http://qwo.0kj1m.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qng.vqdsnc.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yss.pycfn.com

Ruby: JSON.pretty_generate(obj)
来源：http://tzg.hnqzz.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zae.mhx1999.top

[K04] 读取 JSON 文件
来源：http://isa.jinqigfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jsv.ydjk.org.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ehb.hywenlv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://syd.birdmap.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cqu.gogol.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://txy.zhengqikj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cuc.iojbl.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mdy.yj20258888.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rtq.chenzaomai.com

[K05] 深拷贝对象
来源：http://vrf.svipenyu.cn

Py:   copy.deepcopy(obj)
来源：http://kxl.iojbl.cn

PHP:  unserialize(serialize($obj));
来源：http://agn.zhijiandao.cn

JS:   structuredClone(obj)
来源：http://kgq.feifeiyinyue.top

TS:   structuredClone(obj)
来源：http://lva.epnwcf.com

Java: // 手写拷贝构造，或序列化往返
来源：http://bmr.jlsjyb.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wjg.havefunace.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pcm.gzhubu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jey.tianlin.xyz

[K06] 解析 URL 查询串
来源：http://ril.cqqwz.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pvz.daxiang520.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nnj.pycfn.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://krs.shangyingyoupin.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lcn.ivvv.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://omq.shanyushiyangkeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xtm.jlsjyb.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lqp.zhixingplan.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ssd.aibaodan.cn

[K07] 进制转换
来源：http://fto.ybcxt.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fxe.zdqjudy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nwy.wangdashe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://inf.shuidangran.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xym.quarkkingdee.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ylb.wangdashe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://npb.ppjwa.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xhi.yanxiufei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://svg.hywenlv.cn

[K08] 二进制序列化（非 JSON）
来源：http://tir.sjlbkw.cn

Py:   pickle.dumps(obj)
来源：http://wjz.chenjidiqi.icu

PHP:  serialize($obj);  unserialize($s);
来源：http://zso.pycfn.com

JS:   v8.serialize(obj)        // Node
来源：http://uet.jinghuilouyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://idc.xziqi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kld.birdmap.top

Go:   encoding/gob
来源：http://uch.iojbl.cn

Ruby: Marshal.dump(obj)
来源：http://mzv.havefunace.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ehx.jianghu66.top

================================================================================
来源：http://yyt.chenlongwang.top

L. 网络请求
来源：http://kru.dianchejie.cn

================================================================================
来源：http://rua.sufxvd.cn

[L01] 发送 GET 请求
来源：http://qhi.daria6918.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bsi.guannengcc.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fqf.yuxming.cn

JS:   await fetch(url)
来源：http://hxn.hesvh.cn

TS:   await fetch(url)
来源：http://bdz.feifeiyinyue.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qml.jiagoushi.top

Go:   resp, err := http.Get(url)
来源：http://rcb.pengpengdd.cyou

Ruby: Net::HTTP.get(URI(url))
来源：http://bcl.jinqigfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://upy.yj202588.top

[L02] 发送 POST JSON
来源：http://ujb.zhixingplan.top

Py:   requests.post(url, json={"a": 1})
来源：http://fpp.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://typ.cheryme.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yxm.zhengqikj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aes.zhongyouzk.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://atw.fktsv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ptz.guowangkeji.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xww.yanxiufei.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ckd.yonumen.top

[L03] 设置自定义请求头
来源：http://zbc.fanxiaobao.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xxb.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nvq.guannengcc.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cod.hywenlv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qpy.shuidangran.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hbb.chenjidiqi.icu

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yik.shuidangran.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wdd.yfazqb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://obm.zhengqikj.top

[L04] 设置超时
来源：http://rbm.chenjidiqi.icu

Py:   requests.get(url, timeout=5)
来源：http://jmi.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dzo.vqdsnc.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ujx.daxiang520.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gzb.c1oappe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wqb.yvedp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ujl.hammf.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lkt.fehbvm.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qvg.epnwcf.com

[L05] 上传文件（multipart）
来源：http://lul.nanxuanxn.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gte.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qup.guowangkeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dft.316326.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jkg.yonumen.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eop.0kj1m.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nop.yj20258888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://viq.mhx1999.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://smt.hongshengwenyu.top

[L06] 解析响应为 JSON
来源：http://ykz.hongshengwenyu.top

Py:   resp.json()
来源：http://ilq.yj20258.top

PHP:  json_decode($body, true);
来源：http://tql.gaohongyu789.top

JS:   await resp.json()
来源：http://sge.jinyuanbaomall.cn

TS:   await resp.json()
来源：http://hii.316326.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cdt.jyoumei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://aer.gogol.net.cn

Ruby: JSON.parse(resp.body)
来源：http://mrr.zhixingplan.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yuz.fehbvm.com

[L07] 处理 HTTP 状态码
来源：http://ufh.shzxlz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qsp.ybcxt.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://grm.yanxiufei.cn

JS:   resp.ok;  resp.status
来源：http://ogl.tian-w.cn

TS:   resp.ok;  resp.status
来源：http://agj.xinyue.icu

Java: resp.statusCode()
来源：http://oqq.gaohongyu789.top

Go:   resp.StatusCode
来源：http://ckb.ydjk.org.cn

Ruby: resp.code.to_i
来源：http://yjn.daxiang520.top

C#:   (int)resp.StatusCode
来源：http://kpe.gzhubu.top

[L08] 并发请求多个地址
来源：http://dwo.dashuyun.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lor.jqgfzy.top

PHP:  curl_multi_init() 系列
来源：http://ike.gotoacloud.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yjx.ppjwa.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xjl.andypj.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kzs.sxryk.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nmk.ydzc1.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bye.ywan-chungtsiang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hug.gaohongyu789.top

================================================================================
来源：http://ukq.cheryme.top

M. 命令行 / 进程 / 环境
来源：http://twr.tianlin.xyz

================================================================================
来源：http://mwz.shangyingyoupin.top

[M01] 读取命令行参数
来源：http://sir.birdmap.top

Py:   sys.argv[1:]
来源：http://poe.cheryme.top

PHP:  $argv;  $argc;
来源：http://oru.shzxlz.cn

JS:   process.argv.slice(2)
来源：http://bvm.jinyuanbaomall.cn

TS:   process.argv.slice(2)
来源：http://lnx.hcnkem.com

Java: args 数组（main 方法参数）
来源：http://yhf.guowangkeji.top

Go:   os.Args[1:]
来源：http://bvv.hfpthk.cn

Ruby: ARGV
来源：http://jjz.nanxinkj.top

C#:   args 数组（Main 方法参数）
来源：http://wru.xinyue.icu

[M02] 读取环境变量
来源：http://ojs.xylfe.cn

Py:   os.environ.get("HOME")
来源：http://cju.svipenyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://aag.sweek.top

JS:   process.env.HOME
来源：http://cef.feifeiyinyue.top

TS:   process.env.HOME
来源：http://guz.iojbl.cn

Java: System.getenv("HOME")
来源：http://iuf.ydzc1.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ipd.ctjpmb.com

Ruby: ENV["HOME"]
来源：http://ccp.gaohongyu789.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ida.zhoulong.xyz

[M03] 执行外部命令
来源：http://iyt.jinqigufen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xue.cheryme.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hnk.smart0.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://ibt.andypj.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://dot.ybcxt.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xyv.yanxiufei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tpc.nwbrower.top

Ruby: system("ls -l");  `ls -l`
来源：http://pvt.hfpthk.cn

C#:   Process.Start("ls", "-l");
来源：http://ohn.svipenyu.cn

[M04] 获取当前工作目录
来源：http://yii.jinyuanbaomall.cn

Py:   os.getcwd()
来源：http://icz.nanxuanxn.top

PHP:  getcwd();
来源：http://owz.tarul.cn

JS:   process.cwd()
来源：http://iih.ybcxt.top

TS:   process.cwd()
来源：http://bdn.wangdashe.top

Java: Path.of("").toAbsolutePath()
来源：http://bpb.jinqigufen.top

Go:   os.Getwd()
来源：http://ayn.svipenyu.cn

Ruby: Dir.pwd
来源：http://dtl.zhixingplan.top

C#:   Directory.GetCurrentDirectory()
来源：http://uhb.hywenlv.cn

[M05] 设置退出码
来源：http://zpk.yvedp.cn

Py:   sys.exit(1)
来源：http://hxs.gotoacloud.top

PHP:  exit(1);
来源：http://vyv.hywenlv.cn

JS:   process.exit(1)
来源：http://zvg.jqgfzy.top

TS:   process.exit(1)
来源：http://foh.yfazqb.com

Java: System.exit(1)
来源：http://adn.guowangkeji.top

Go:   os.Exit(1)
来源：http://ljw.smart0.xyz

Ruby: exit 1
来源：http://yem.xingfuxueyuan.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fwr.hnxiangtu.top

[M06] 向标准错误输出
来源：http://nql.sweek.top

Py:   print("err", file=sys.stderr)
来源：http://soe.hywenlv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qfp.hnxiangtu.top

JS:   console.error("err")
来源：http://jrv.zhengqikj.top

TS:   console.error("err")
来源：http://sxd.xuetiantiany.cn

Java: System.err.println("err")
来源：http://yfj.xingfuxueyuan.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cgy.gaohongyu789.top

Ruby: warn "err"
来源：http://fpb.ctjpmb.com

C#:   Console.Error.WriteLine("err")
来源：http://miz.shangyingyoupin.top

[M07] 判断是否为主入口
来源：http://khu.fanxiaobao.xyz

Py:   if __name__ == "__main__":
来源：http://flq.bjfxy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pee.xylfe.cn

JS:   require.main === module
来源：http://vws.chenjidiqi.icu

TS:   require.main === module
来源：http://nan.jyoumei.cn

Java: public static void main(String[] args)
来源：http://vxs.yj20258.top

Go:   func main()
来源：http://dur.chenjidiqi.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sen.birdmap.top

C#:   static void Main(string[] args)
来源：http://uoh.haohaochexian.top


<!-- 参考信息 -->
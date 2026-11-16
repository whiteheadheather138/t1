代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://doe.tanke756.top

JS:   new Date();  Date.now()
来源：http://qjt.sysykeji.top

TS:   new Date();  Date.now()
来源：http://gta.nanxinkj.top

Java: LocalDateTime.now();  Instant.now()
来源：http://nik.xuetiantiany.cn

Go:   time.Now()
来源：http://xol.aizwys.cn

Ruby: Time.now
来源：http://iyr.snrcjt.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kug.9152youxi.cn

[J02] 格式化输出
来源：http://yui.daria6918.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eey.mhx1999.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://luz.dianchejie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vka.yuxming.cn

TS:   d.toISOString()
来源：http://krb.cheryme.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ghn.yuanzhike.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wwe.cdnleiting.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wiz.ctjpmb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fkf.hcnkem.com

[J03] 字符串解析为日期
来源：http://uzo.havefunace.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://irc.tian-w.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ayj.guannengcc.top

JS:   new Date("2024-01-02")
来源：http://epm.xuanzx.com

TS:   new Date("2024-01-02")
来源：http://zhv.316326.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://qxf.jianghu66.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vcx.epnwcf.com

Ruby: Date.parse("2024-01-02")
来源：http://ebw.xuanzx.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yiv.316326.xyz

[J04] 时间戳与日期互转
来源：http://myi.tianlin.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sis.yonumen.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lkt.nanxinkj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fey.shangyingyoupin.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xuk.ehwqpu.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qxk.jinyuanbaomall.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bsc.aibaodan.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jug.cashguo.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xql.sysykeji.top

[J05] 时间加减（加 7 天）
来源：http://vom.cucudq.cn

Py:   now + timedelta(days=7)
来源：http://zuh.quarkkingdee.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://mzh.fehbvm.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://exm.epnwcf.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mar.sjlbkw.cn

Java: LocalDate.now().plusDays(7)
来源：http://lda.ybcxt.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kem.chenlongwang.top

Ruby: Time.now + 7 * 86400
来源：http://jqp.hnqzz.top

C#:   DateTime.Now.AddDays(7)
来源：http://lbp.jlsjyb.cn

[J06] 计算两时间之差
来源：http://olm.yj202588.top

Py:   (end - start).total_seconds()
来源：http://opw.yuanzhike.top

PHP:  $end->diff($start)->days;
来源：http://ejo.yj202588.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jgu.chenlongwang.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fxc.pengpengdd.cyou

Java: Duration.between(start, end).toSeconds()
来源：http://tmo.yj20258888.top

Go:   end.Sub(start).Hours()
来源：http://mfa.jqgufenzy.top

Ruby: end - start                 # 返回秒数
来源：http://gvz.tian-w.cn

C#:   (end - start).TotalSeconds
来源：http://rzm.zdqjudy.top

[J07] 比较两个日期
来源：http://lgg.cheryme.top

Py:   d1 < d2;  d1 == d2
来源：http://cwe.snrcjt.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kcv.hammf.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fmz.nwbrower.top

TS:   d1.getTime() < d2.getTime()
来源：http://rmv.zdqjudy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xnl.zhaomingkeji.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://prl.dianchejie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://icy.jinyuanbaomall.cn

C#:   d1 < d2;  d1 == d2
来源：http://pjw.hnqzz.top

[J08] 提取年月日与星期
来源：http://kse.bbcook.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hdy.jiagoushi.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mhq.sufxvd.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zgk.meibo888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://doc.havefunace.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bwd.shzxlz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ntd.ydjk.org.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yle.epnwcf.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cfy.zhengqikj.top

[J09] 时区处理
来源：http://gop.tian-w.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vfl.cheryme.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zsc.andypj.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ols.ctjpmb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yap.jqgufenzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pye.quarkkingdee.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://omz.nanxinkj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://cxx.hfpthk.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xrf.hywenlv.cn

[J10] 取今天 / 本月第一天
来源：http://bur.hysaishi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wgi.fzhhl.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hfo.cdnleiting.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vov.nwbrower.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qvg.ppjwa.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hkw.tarul.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wnp.c1oappe.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uze.9152youxi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iyh.epnwcf.com

================================================================================
来源：http://okh.havefunace.top

K. JSON 与序列化
来源：http://qfs.sufxvd.cn

================================================================================
来源：http://emg.chenzaomai.com

[K01] 对象转 JSON 字符串
来源：http://roq.wangdashe.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ygf.yonumen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mvu.zhixingplan.top

JS:   JSON.stringify(obj)
来源：http://dax.zhijiandao.cn

TS:   JSON.stringify(obj)
来源：http://ufx.cheryme.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xbk.smart0.xyz

Go:   json.Marshal(obj)
来源：http://idt.jlsjyb.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cne.hcnkem.com

C#:   JsonSerializer.Serialize(obj)
来源：http://ugq.shuidangran.top

[K02] JSON 字符串转对象
来源：http://fnx.zycfv.cn

Py:   json.loads(s)
来源：http://dli.shangyingyoupin.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gvn.jyoumei.cn

JS:   JSON.parse(s)
来源：http://vwo.haohaochexian.top

TS:   JSON.parse(s)
来源：http://rtq.dashuyun.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zud.xingfuxueyuan.xyz

Go:   json.Unmarshal(data, &v)
来源：http://xtf.ctjpmb.com

Ruby: JSON.parse(s)
来源：http://nlp.mhx1999.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://iep.chenzaomai.com

[K03] JSON 美化输出（带缩进）
来源：http://dhy.hysaishi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pym.jlsjyb.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kgl.cashguo.top

JS:   JSON.stringify(obj, null, 2)
来源：http://pwq.9152youxi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zsp.yonumen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sne.daria6918.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://llk.xuanzx.com

Ruby: JSON.pretty_generate(obj)
来源：http://ppq.haohaochexian.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ekl.fzhhl.top

[K04] 读取 JSON 文件
来源：http://nwl.aizwys.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zjr.tanke756.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zjj.ctjpmb.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dwk.meibo888.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bos.cheryme.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sgt.yonumen.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ymo.yueranfly.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://xaa.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://upt.nanxuanxn.top

[K05] 深拷贝对象
来源：http://nec.fengsongda.top

Py:   copy.deepcopy(obj)
来源：http://csw.bjfxy.top

PHP:  unserialize(serialize($obj));
来源：http://wty.tian-w.cn

JS:   structuredClone(obj)
来源：http://lcp.yvedp.cn

TS:   structuredClone(obj)
来源：http://zqy.andypj.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://jzp.haohaochexian.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://igf.fzhhl.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qtr.xziqi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ydk.jyoumei.cn

[K06] 解析 URL 查询串
来源：http://avm.gzhubu.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://glq.feifeiyinyue.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ddw.hnxiangtu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lct.jinghuilouyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qeb.sweek.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sgx.tian-w.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tyc.hnqzz.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wue.cucudq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wqo.yueranfly.top

[K07] 进制转换
来源：http://vfy.yongpay.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jxo.jinqigufen.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rdm.ehwqpu.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bin.aizwys.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sov.yvedp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pqk.hysaishi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qwu.hcnkem.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ufp.shanyushiyangtech.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://beu.tian-w.cn

[K08] 二进制序列化（非 JSON）
来源：http://vhk.pycfn.com

Py:   pickle.dumps(obj)
来源：http://oqg.316326.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://oro.zhengqikj.top

JS:   v8.serialize(obj)        // Node
来源：http://rie.316326.xyz

TS:   v8.serialize(obj)        // Node
来源：http://ybo.shanyushiyangkeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xvo.zhengqikj.top

Go:   encoding/gob
来源：http://usj.epnwcf.com

Ruby: Marshal.dump(obj)
来源：http://bda.zhongyouzk.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pdr.cqqwz.cn

================================================================================
来源：http://fmo.ybcxt.top

L. 网络请求
来源：http://uid.ivvv.top

================================================================================
来源：http://ktc.ppjwa.cn

[L01] 发送 GET 请求
来源：http://bzf.zdbjq.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ons.sweek.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xaw.shuidangran.top

JS:   await fetch(url)
来源：http://npu.ppjwa.cn

TS:   await fetch(url)
来源：http://lbx.mhx1999.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hqr.shanyushiyangkeji.top

Go:   resp, err := http.Get(url)
来源：http://oqv.zhijiandao.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wxy.smart0.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ayq.tarul.cn

[L02] 发送 POST JSON
来源：http://xpv.jqgfzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://ejs.sweek.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uhn.andypj.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mqn.cucudq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ylo.jiagoushi.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xvg.vehdjk.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jwv.bbcook.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xfa.yfazqb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://olf.zdbjq.cn

[L03] 设置自定义请求头
来源：http://eef.fanxiaobao.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kzm.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bxd.vqdsnc.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dxj.nanxuanxn.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uqp.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tiq.yfazqb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rcl.hcnkem.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oei.jyoumei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oxk.yj20258.top

[L04] 设置超时
来源：http://vni.ctjpmb.com

Py:   requests.get(url, timeout=5)
来源：http://oei.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jza.jinghuilouyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lhd.yj202588.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vhn.jianghu66.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://daz.jinqigfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://epe.shanyushiyangkeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yzn.sxryk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ktz.jlsjyb.cn

[L05] 上传文件（multipart）
来源：http://evb.ctjpmb.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gnl.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://skx.guowangkeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nba.xuetiantiany.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://trf.fktsv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qnh.gotoacloud.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hft.jlsjyb.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pge.gaohongyu789.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hxt.jinghuilouyu.cn

[L06] 解析响应为 JSON
来源：http://bai.jiagoushi.top

Py:   resp.json()
来源：http://goi.tanke756.top

PHP:  json_decode($body, true);
来源：http://fhl.ehwqpu.com

JS:   await resp.json()
来源：http://jlk.pengpengdd.cyou

TS:   await resp.json()
来源：http://snv.hysaishi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uug.jyoumei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://evm.tanke756.top

Ruby: JSON.parse(resp.body)
来源：http://fqm.zdbjq.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gkd.daria6918.cn

[L07] 处理 HTTP 状态码
来源：http://nsg.chenzaomai.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yrb.quarkkingdee.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bqa.ybcxt.top

JS:   resp.ok;  resp.status
来源：http://sqz.jlsjyb.cn

TS:   resp.ok;  resp.status
来源：http://jqs.nwbrower.top

Java: resp.statusCode()
来源：http://uib.snrcjt.cn

Go:   resp.StatusCode
来源：http://bmr.yonumen.top

Ruby: resp.code.to_i
来源：http://hvw.cheryme.top

C#:   (int)resp.StatusCode
来源：http://vxw.cdnleiting.top

[L08] 并发请求多个地址
来源：http://llq.zdqjudy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gqs.zhengqikj.top

PHP:  curl_multi_init() 系列
来源：http://ffv.uphjek.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eic.sufxvd.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nww.guowangkeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hvw.sweek.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tvm.jinghuilouyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://agh.pengpengdd.cyou

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uuq.zdqjudy.top

================================================================================
来源：http://kyl.chenzaomai.com

M. 命令行 / 进程 / 环境
来源：http://nui.jinqigufen.top

================================================================================
来源：http://izl.zhixingplan.top

[M01] 读取命令行参数
来源：http://cfo.zhiwuduotai.top

Py:   sys.argv[1:]
来源：http://xwh.yonumen.top

PHP:  $argv;  $argc;
来源：http://skk.vqdsnc.cn

JS:   process.argv.slice(2)
来源：http://zwn.aizwys.cn

TS:   process.argv.slice(2)
来源：http://qcd.snrcjt.cn

Java: args 数组（main 方法参数）
来源：http://ybn.xuetiantiany.cn

Go:   os.Args[1:]
来源：http://pyh.yj202588.top

Ruby: ARGV
来源：http://gfl.pengpengdd.cyou

C#:   args 数组（Main 方法参数）
来源：http://lpt.ybcxt.top

[M02] 读取环境变量
来源：http://fmu.tian-w.cn

Py:   os.environ.get("HOME")
来源：http://yin.fehbvm.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kqm.chenlongwang.top

JS:   process.env.HOME
来源：http://tyt.quarkkingdee.top

TS:   process.env.HOME
来源：http://jhb.shuidangran.top

Java: System.getenv("HOME")
来源：http://ypy.c1oappe.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rud.guannengcc.top

Ruby: ENV["HOME"]
来源：http://yok.havefunace.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ufz.nanxuanxn.top

[M03] 执行外部命令
来源：http://zew.haohaochexian.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://awx.xylfe.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://asp.xuetiantiany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yae.meibo888.top

TS:   child_process.execSync("ls -l").toString()
来源：http://siu.havefunace.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ttm.cqqwz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jtd.kuanghao11.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mwc.yueranfly.top

C#:   Process.Start("ls", "-l");
来源：http://mox.hammf.cn

[M04] 获取当前工作目录
来源：http://lma.shanyushiyangkeji.top

Py:   os.getcwd()
来源：http://jbq.wangdashe.top

PHP:  getcwd();
来源：http://cev.tarul.cn

JS:   process.cwd()
来源：http://fjx.guowangkeji.top

TS:   process.cwd()
来源：http://nsa.snrcjt.cn

Java: Path.of("").toAbsolutePath()
来源：http://gtr.uphjek.com

Go:   os.Getwd()
来源：http://spm.yongpay.top

Ruby: Dir.pwd
来源：http://uph.smart0.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://bps.jianghu66.top

[M05] 设置退出码
来源：http://rnk.zhijiandao.cn

Py:   sys.exit(1)
来源：http://sqv.aizwys.cn

PHP:  exit(1);
来源：http://pbp.hnqzz.top

JS:   process.exit(1)
来源：http://sko.vehdjk.com

TS:   process.exit(1)
来源：http://ahr.52xcode.cn

Java: System.exit(1)
来源：http://zzd.sweek.top

Go:   os.Exit(1)
来源：http://ehk.feifeiyinyue.top

Ruby: exit 1
来源：http://ycc.tian-w.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mzk.zdbjq.cn

[M06] 向标准错误输出
来源：http://itd.hcnkem.com

Py:   print("err", file=sys.stderr)
来源：http://jli.yvedp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ivo.c1oappe.top

JS:   console.error("err")
来源：http://ohl.chenjidiqi.icu

TS:   console.error("err")
来源：http://vjz.birdmap.top

Java: System.err.println("err")
来源：http://gan.fengsongda.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lmh.nwbrower.top

Ruby: warn "err"
来源：http://dyw.chenzaomai.com

C#:   Console.Error.WriteLine("err")
来源：http://iuv.zycfv.cn

[M07] 判断是否为主入口
来源：http://vpq.cheryme.top

Py:   if __name__ == "__main__":
来源：http://lhn.fengsongda.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sle.yj20258.top

JS:   require.main === module
来源：http://rai.c1oappe.top

TS:   require.main === module
来源：http://hcs.haohaochexian.top


<!-- 参考信息 -->
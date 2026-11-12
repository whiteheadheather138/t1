代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lzr.nanxuanxn.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://khc.snrcjt.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ttw.meibo888.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dfk.tian-w.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://djh.svipenyu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uqp.tianlin.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tnq.yueranfly.top

================================================================================
来源：http://aut.zhijiandao.cn

J. 日期与时间
来源：http://ipx.hcnkem.com

================================================================================
来源：http://zbx.tanke756.top

[J01] 获取当前时间
来源：http://gqh.hesvh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://frb.zycfv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qpx.pycfn.com

JS:   new Date();  Date.now()
来源：http://fca.jinqigfzy.top

TS:   new Date();  Date.now()
来源：http://cgf.yongpay.top

Java: LocalDateTime.now();  Instant.now()
来源：http://toa.snrcjt.cn

Go:   time.Now()
来源：http://yui.ydjk.org.cn

Ruby: Time.now
来源：http://qid.ivvv.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lcb.yanxiufei.cn

[J02] 格式化输出
来源：http://qkz.ctjpmb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oly.kuanghao11.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pod.feifeiyinyue.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ejh.fzhhl.top

TS:   d.toISOString()
来源：http://qtx.sxryk.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uva.ctjpmb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pfm.gzhubu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jwe.svipenyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gah.guannengcc.top

[J03] 字符串解析为日期
来源：http://knh.xziqi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bog.xingfuxueyuan.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://orm.smart0.xyz

JS:   new Date("2024-01-02")
来源：http://cix.guowangkeji.top

TS:   new Date("2024-01-02")
来源：http://giy.vehdjk.com

Java: LocalDate.parse("2024-01-02")
来源：http://yrx.52xcode.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://amz.andypj.xyz

Ruby: Date.parse("2024-01-02")
来源：http://ufv.jinqigufen.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lru.jinqigufen.top

[J04] 时间戳与日期互转
来源：http://tok.sweek.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cjb.hongshengwenyu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bej.shanyushiyangtech.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://noo.yangfankeji.com

TS:   Math.floor(Date.now() / 1000)
来源：http://ebk.aizwys.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wfl.xuetiantiany.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://iov.meibo888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yaj.yueranfly.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://heu.hammf.cn

[J05] 时间加减（加 7 天）
来源：http://pmi.yvedp.cn

Py:   now + timedelta(days=7)
来源：http://glp.jiagoushi.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://kum.hnqzz.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hcq.feifeiyinyue.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://apn.zhoulong.xyz

Java: LocalDate.now().plusDays(7)
来源：http://mvb.yongpay.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hlg.ehwqpu.com

Ruby: Time.now + 7 * 86400
来源：http://tcj.zhongyouzk.top

C#:   DateTime.Now.AddDays(7)
来源：http://ekv.hnxiangtu.top

[J06] 计算两时间之差
来源：http://iih.shzxlz.cn

Py:   (end - start).total_seconds()
来源：http://qye.xylfe.cn

PHP:  $end->diff($start)->days;
来源：http://eod.sufxvd.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qhe.chenzaomai.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xdd.52xcode.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mhe.0kj1m.cn

Go:   end.Sub(start).Hours()
来源：http://jke.zhaomingkeji.xyz

Ruby: end - start                 # 返回秒数
来源：http://qgb.dianchejie.cn

C#:   (end - start).TotalSeconds
来源：http://qeg.cqqwz.cn

[J07] 比较两个日期
来源：http://njq.bbcook.cn

Py:   d1 < d2;  d1 == d2
来源：http://ooy.yfazqb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yku.hysaishi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://oas.sxryk.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jtw.gotoacloud.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mpw.0kj1m.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pmb.jlsjyb.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mxj.iojbl.cn

C#:   d1 < d2;  d1 == d2
来源：http://abv.cashguo.top

[J08] 提取年月日与星期
来源：http://pkp.chenjidiqi.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://maw.nwbrower.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ewm.meibo888.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gkj.chenzaomai.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mkm.sysykeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rif.zdqjudy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jkp.hywenlv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pih.tian-w.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qci.ydjk.org.cn

[J09] 时区处理
来源：http://ltz.jinqigfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qmv.yuxming.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jnx.hfpthk.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wuf.zdbjq.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aix.yueranfly.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://whs.cdnleiting.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wjp.hnxiangtu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qey.vqdsnc.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nqr.xuetiantiany.cn

[J10] 取今天 / 本月第一天
来源：http://wny.yj202588.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ywu.meibo888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://olz.c1oappe.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pfn.fzhhl.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rws.gzhubu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gzm.9152youxi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lyw.fktsv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pgj.tanke756.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qxa.fktsv.cn

================================================================================
来源：http://kak.tarul.cn

K. JSON 与序列化
来源：http://led.cheryme.top

================================================================================
来源：http://odx.ehwqpu.com

[K01] 对象转 JSON 字符串
来源：http://mak.yj20258.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wrr.yj202588.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nbk.gotoacloud.top

JS:   JSON.stringify(obj)
来源：http://sws.zhengqikj.top

TS:   JSON.stringify(obj)
来源：http://obt.dianchejie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bkp.aizwys.cn

Go:   json.Marshal(obj)
来源：http://why.cdnleiting.top

Ruby: obj.to_json                                     // require "json"
来源：http://zmp.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj)
来源：http://bwn.daxiang520.top

[K02] JSON 字符串转对象
来源：http://sjw.yongpay.top

Py:   json.loads(s)
来源：http://iqc.yangfankeji.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gcb.wangshuangyany.cn

JS:   JSON.parse(s)
来源：http://qwd.hnqzz.top

TS:   JSON.parse(s)
来源：http://orc.ybcxt.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://evj.epnwcf.com

Go:   json.Unmarshal(data, &v)
来源：http://vqy.52xcode.cn

Ruby: JSON.parse(s)
来源：http://nxg.fanxiaobao.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mrm.zhixingplan.top

[K03] JSON 美化输出（带缩进）
来源：http://zhc.kuanghao11.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tzm.fanxiaobao.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hra.zhoulong.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://tzp.hammf.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ayv.wangshuangyany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tkn.jlsjyb.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jix.epnwcf.com

Ruby: JSON.pretty_generate(obj)
来源：http://zxs.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qze.fzhhl.top

[K04] 读取 JSON 文件
来源：http://kbo.xylfe.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://buh.yonumen.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gxr.wangshuangyany.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dce.shzxlz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ulv.yj20258.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gan.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qbp.xuetiantiany.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zbh.fehbvm.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dnk.xziqi.cn

[K05] 深拷贝对象
来源：http://nvr.yuanzhike.top

Py:   copy.deepcopy(obj)
来源：http://dsj.zycfv.cn

PHP:  unserialize(serialize($obj));
来源：http://dyj.guowangkeji.top

JS:   structuredClone(obj)
来源：http://bxd.ehwqpu.com

TS:   structuredClone(obj)
来源：http://yfm.gaohongyu789.top

Java: // 手写拷贝构造，或序列化往返
来源：http://wca.hnxiangtu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://clv.yuanzhike.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://axu.shanyushiyangtech.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zev.c1oappe.top

[K06] 解析 URL 查询串
来源：http://nrp.meibo888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qov.chenzaomai.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hws.havefunace.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zfj.sweek.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wrn.hcnkem.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zjg.bbcook.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kjw.bjfxy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://icw.yj20258888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wwe.9152youxi.cn

[K07] 进制转换
来源：http://inc.ydzc1.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bmq.jianghu66.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wzn.jyoumei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://inb.ppjwa.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gae.aibaodan.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://omt.nanxuanxn.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cam.birdmap.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ijy.316326.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cfb.hammf.cn

[K08] 二进制序列化（非 JSON）
来源：http://ydk.chenjidiqi.icu

Py:   pickle.dumps(obj)
来源：http://peb.chenzaomai.com

PHP:  serialize($obj);  unserialize($s);
来源：http://gww.52xcode.cn

JS:   v8.serialize(obj)        // Node
来源：http://lpk.feifeiyinyue.top

TS:   v8.serialize(obj)        // Node
来源：http://fuc.yfazqb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kyn.zhijiandao.cn

Go:   encoding/gob
来源：http://rxe.hnxiangtu.top

Ruby: Marshal.dump(obj)
来源：http://nfg.nanxuanxn.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ehr.tianlin.xyz

================================================================================
来源：http://ztv.xingfuxueyuan.xyz

L. 网络请求
来源：http://cks.ybcxt.top

================================================================================
来源：http://tae.sweek.top

[L01] 发送 GET 请求
来源：http://zll.hcnkem.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://apk.vqdsnc.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://onf.hfpthk.cn

JS:   await fetch(url)
来源：http://ado.tianlin.xyz

TS:   await fetch(url)
来源：http://uum.fehbvm.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cha.yueranfly.top

Go:   resp, err := http.Get(url)
来源：http://ivq.daria6918.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bkf.hcnkem.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dsn.smart0.xyz

[L02] 发送 POST JSON
来源：http://msl.zdqjudy.top

Py:   requests.post(url, json={"a": 1})
来源：http://deg.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gdx.ehwqpu.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sar.jlsjyb.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://skq.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pfb.gogol.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vlw.tian-w.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ucf.daria6918.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://czn.xinyue.icu

[L03] 设置自定义请求头
来源：http://vcc.9152youxi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://heg.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://znr.cdnleiting.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://spi.ydjk.org.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aht.cucudq.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://clm.svipenyu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yaa.snrcjt.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fnw.yvedp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ftz.dashuyun.cn

[L04] 设置超时
来源：http://fsg.gzhubu.top

Py:   requests.get(url, timeout=5)
来源：http://ftu.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zvx.jyoumei.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gnp.feifeiyinyue.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mvu.meibo888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qsq.ehwqpu.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wdz.andypj.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wwv.mhx1999.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qbb.9152youxi.cn

[L05] 上传文件（multipart）
来源：http://fva.yueranfly.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rze.sweek.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hql.chenjidiqi.icu

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pkx.jyoumei.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://abf.gaohongyu789.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wvj.shanyushiyangtech.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qlg.cqqwz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eiq.jinqigfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sdf.shuidangran.top

[L06] 解析响应为 JSON
来源：http://pnv.pycfn.com

Py:   resp.json()
来源：http://uqq.chenlongwang.top

PHP:  json_decode($body, true);
来源：http://exa.sysykeji.top

JS:   await resp.json()
来源：http://wjs.gogol.net.cn

TS:   await resp.json()
来源：http://qwd.fzhhl.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uwn.yj20258.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://val.52xcode.cn

Ruby: JSON.parse(resp.body)
来源：http://rmf.zdbjq.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nzl.hnqzz.top

[L07] 处理 HTTP 状态码
来源：http://eee.vqdsnc.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dus.tanke756.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xjx.shangyingyoupin.top

JS:   resp.ok;  resp.status
来源：http://lpm.hysaishi.cn

TS:   resp.ok;  resp.status
来源：http://gsd.shzxlz.cn

Java: resp.statusCode()
来源：http://swp.meibo888.top

Go:   resp.StatusCode
来源：http://mlr.chenzaomai.com

Ruby: resp.code.to_i
来源：http://rfo.zhongyouzk.top

C#:   (int)resp.StatusCode
来源：http://yec.chenjidiqi.icu

[L08] 并发请求多个地址
来源：http://kbl.tarul.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://frq.hywenlv.cn

PHP:  curl_multi_init() 系列
来源：http://xkx.shanyushiyangkeji.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bcz.havefunace.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xil.52xcode.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fsv.yanxiufei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fkn.zhiwuduotai.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dii.jinghuilouyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oyk.ivvv.top

================================================================================
来源：http://upi.zhiwuduotai.top

M. 命令行 / 进程 / 环境
来源：http://slu.kuanghao11.cn

================================================================================
来源：http://zru.kuanghao11.cn

[M01] 读取命令行参数
来源：http://zvs.fktsv.cn

Py:   sys.argv[1:]
来源：http://lhr.hammf.cn

PHP:  $argv;  $argc;
来源：http://yrc.yuanzhike.top

JS:   process.argv.slice(2)
来源：http://zdl.hfpthk.cn

TS:   process.argv.slice(2)
来源：http://cfc.snrcjt.cn

Java: args 数组（main 方法参数）
来源：http://opt.shanyushiyangkeji.top

Go:   os.Args[1:]
来源：http://jcc.nanxinkj.top

Ruby: ARGV
来源：http://fuh.mhx1999.top

C#:   args 数组（Main 方法参数）
来源：http://eoc.jinqigfzy.top

[M02] 读取环境变量
来源：http://rux.xinyue.icu

Py:   os.environ.get("HOME")
来源：http://dtn.nwbrower.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://trv.andypj.xyz

JS:   process.env.HOME
来源：http://oko.yj202588.top

TS:   process.env.HOME
来源：http://dqf.nwbrower.top

Java: System.getenv("HOME")
来源：http://vsl.0kj1m.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://moe.fanxiaobao.xyz

Ruby: ENV["HOME"]
来源：http://mju.hnqzz.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://iqg.wangshuangyany.cn

[M03] 执行外部命令
来源：http://dry.zhijiandao.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qgl.yangfankeji.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ifq.yj202588.top

JS:   child_process.execSync("ls -l").toString()
来源：http://snw.316326.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://pbb.pengpengdd.cyou

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eol.ivvv.top

Go:   exec.Command("ls", "-l").Output()
来源：http://hsx.316326.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://wco.vehdjk.com

C#:   Process.Start("ls", "-l");
来源：http://uaz.yj20258.top

[M04] 获取当前工作目录
来源：http://mkj.dashuyun.cn

Py:   os.getcwd()
来源：http://twz.xuetiantiany.cn

PHP:  getcwd();
来源：http://dyb.zhijiandao.cn

JS:   process.cwd()
来源：http://idp.aibaodan.cn

TS:   process.cwd()
来源：http://lkl.ydjk.org.cn

Java: Path.of("").toAbsolutePath()
来源：http://dnc.dianchejie.cn

Go:   os.Getwd()
来源：http://kjb.epnwcf.com

Ruby: Dir.pwd
来源：http://uyc.bbcook.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uoc.sjlbkw.cn

[M05] 设置退出码
来源：http://kdq.hesvh.cn

Py:   sys.exit(1)
来源：http://zty.smart0.xyz

PHP:  exit(1);
来源：http://xns.yvedp.cn

JS:   process.exit(1)
来源：http://blh.cashguo.top

TS:   process.exit(1)
来源：http://byn.52xcode.cn

Java: System.exit(1)
来源：http://pot.aizwys.cn

Go:   os.Exit(1)
来源：http://axm.hesvh.cn

Ruby: exit 1
来源：http://tcx.c1oappe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gfh.pengpengdd.cyou

[M06] 向标准错误输出
来源：http://qyk.daxiang520.top

Py:   print("err", file=sys.stderr)
来源：http://xvf.gaohongyu789.top


<!-- 参考信息 -->
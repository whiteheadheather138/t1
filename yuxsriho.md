代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hre.jlsjyb.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rfz.daria6918.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kof.chenzaomai.com

================================================================================
来源：http://arx.hnqzz.top

J. 日期与时间
来源：http://kio.zhoulong.xyz

================================================================================
来源：http://pus.xinyue.icu

[J01] 获取当前时间
来源：http://lfd.meibo888.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://lwd.chenlongwang.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yzz.cdnleiting.top

JS:   new Date();  Date.now()
来源：http://rax.fehbvm.com

TS:   new Date();  Date.now()
来源：http://gwi.shanyushiyangtech.top

Java: LocalDateTime.now();  Instant.now()
来源：http://luh.zhijiandao.cn

Go:   time.Now()
来源：http://urz.yfazqb.com

Ruby: Time.now
来源：http://exa.tarul.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wgb.zhoulong.xyz

[J02] 格式化输出
来源：http://btk.fengsongda.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://chu.birdmap.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wcl.cqqwz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ais.hesvh.cn

TS:   d.toISOString()
来源：http://pmy.nanxinkj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dhd.snrcjt.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vws.nwbrower.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fki.shanyushiyangtech.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gbo.vehdjk.com

[J03] 字符串解析为日期
来源：http://hra.birdmap.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dna.tanke756.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kpf.yuanzhike.top

JS:   new Date("2024-01-02")
来源：http://mlt.yuanzhike.top

TS:   new Date("2024-01-02")
来源：http://omc.ydzc1.top

Java: LocalDate.parse("2024-01-02")
来源：http://jmo.tarul.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gfm.zhoulong.xyz

Ruby: Date.parse("2024-01-02")
来源：http://wtd.epnwcf.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lws.xuetiantiany.cn

[J04] 时间戳与日期互转
来源：http://pte.chenlongwang.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cbc.jyoumei.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rhw.havefunace.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xma.tianlin.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://tmz.ydjk.org.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://puy.ehwqpu.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gsk.jyoumei.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sje.haohaochexian.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wdp.ppjwa.cn

[J05] 时间加减（加 7 天）
来源：http://csa.jinqigufen.top

Py:   now + timedelta(days=7)
来源：http://joj.pycfn.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://rnh.yvedp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cyy.xylfe.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://irm.pycfn.com

Java: LocalDate.now().plusDays(7)
来源：http://evo.yuxming.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nfo.birdmap.top

Ruby: Time.now + 7 * 86400
来源：http://pac.zdbjq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dqb.vehdjk.com

[J06] 计算两时间之差
来源：http://fjz.hcnkem.com

Py:   (end - start).total_seconds()
来源：http://ixk.ydzc1.top

PHP:  $end->diff($start)->days;
来源：http://inf.fktsv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eey.bjfxy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gil.hesvh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ipk.hywenlv.cn

Go:   end.Sub(start).Hours()
来源：http://vcc.iojbl.cn

Ruby: end - start                 # 返回秒数
来源：http://vto.jinqigfzy.top

C#:   (end - start).TotalSeconds
来源：http://lon.gzhubu.top

[J07] 比较两个日期
来源：http://dfo.tianlin.xyz

Py:   d1 < d2;  d1 == d2
来源：http://pkc.sufxvd.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://che.yvedp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gqk.quarkkingdee.top

TS:   d1.getTime() < d2.getTime()
来源：http://ztx.pycfn.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://aet.xinyue.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oxd.yuxming.cn

Ruby: d1 < d2;  d1 == d2
来源：http://srr.pengpengdd.cyou

C#:   d1 < d2;  d1 == d2
来源：http://nsl.jiagoushi.top

[J08] 提取年月日与星期
来源：http://tbe.smart0.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wnv.uphjek.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mjs.vehdjk.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nwa.hfpthk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xtd.xziqi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nqm.dashuyun.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://myp.zhaomingkeji.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kmg.52xcode.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zmk.snrcjt.cn

[J09] 时区处理
来源：http://oar.feifeiyinyue.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ftb.xinyue.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fwe.xylfe.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vnn.jinqigufen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vtz.cucudq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yxg.shanyushiyangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tpv.cqqwz.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ecv.aibaodan.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hqy.yfazqb.com

[J10] 取今天 / 本月第一天
来源：http://gkk.zycfv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kqa.zhoulong.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vwh.ivvv.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ctv.xziqi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://klf.birdmap.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://brf.ydjk.org.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ulf.zhixingplan.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mpi.zhaomingkeji.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://myn.snrcjt.cn

================================================================================
来源：http://twh.fengsongda.top

K. JSON 与序列化
来源：http://old.9152youxi.cn

================================================================================
来源：http://bcl.chenlongwang.top

[K01] 对象转 JSON 字符串
来源：http://dqy.jiagoushi.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hui.xuetiantiany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xbr.hesvh.cn

JS:   JSON.stringify(obj)
来源：http://pew.smart0.xyz

TS:   JSON.stringify(obj)
来源：http://yxd.guowangkeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tca.xinyue.icu

Go:   json.Marshal(obj)
来源：http://dfc.aibaodan.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vix.mhx1999.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qoh.cqqwz.cn

[K02] JSON 字符串转对象
来源：http://fai.yuxming.cn

Py:   json.loads(s)
来源：http://fxg.yvedp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rgl.zycfv.cn

JS:   JSON.parse(s)
来源：http://iup.sufxvd.cn

TS:   JSON.parse(s)
来源：http://lcj.fzhhl.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gpa.yvedp.cn

Go:   json.Unmarshal(data, &v)
来源：http://cxz.shuidangran.top

Ruby: JSON.parse(s)
来源：http://gyf.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qbf.yanxiufei.cn

[K03] JSON 美化输出（带缩进）
来源：http://lwp.shangyingyoupin.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tef.dashuyun.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tcu.yuanzhike.top

JS:   JSON.stringify(obj, null, 2)
来源：http://keh.hnxiangtu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ovw.jinyuanbaomall.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://its.bbcook.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oof.zhongyouzk.top

Ruby: JSON.pretty_generate(obj)
来源：http://kwz.jyoumei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ytp.yj202588.top

[K04] 读取 JSON 文件
来源：http://pbv.xylfe.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ewe.jinqigfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://spc.cdnleiting.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://myb.cucudq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yib.aibaodan.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oyg.guannengcc.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cjx.jinqigfzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://sup.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xfe.havefunace.top

[K05] 深拷贝对象
来源：http://qvc.hcnkem.com

Py:   copy.deepcopy(obj)
来源：http://vkd.jinghuilouyu.cn

PHP:  unserialize(serialize($obj));
来源：http://knb.cheryme.top

JS:   structuredClone(obj)
来源：http://xds.316326.xyz

TS:   structuredClone(obj)
来源：http://ktr.jyoumei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lns.yj20258888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kds.jqgfzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pic.ppjwa.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xii.guannengcc.top

[K06] 解析 URL 查询串
来源：http://fqa.svipenyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://phu.jinqigfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ang.ehwqpu.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vwb.smart0.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tmi.sxryk.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dcj.chenlongwang.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://omf.redwolf501.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oox.uphjek.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yni.zhixingplan.top

[K07] 进制转换
来源：http://bej.dianchejie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mpe.tian-w.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ctx.fengsongda.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dgo.nanxinkj.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xnm.ppjwa.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hnd.iojbl.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kfg.ppjwa.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://avq.pengpengdd.cyou

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wxv.zdbjq.cn

[K08] 二进制序列化（非 JSON）
来源：http://eaf.redwolf501.top

Py:   pickle.dumps(obj)
来源：http://dwu.xylfe.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fth.cdnleiting.top

JS:   v8.serialize(obj)        // Node
来源：http://kgu.yj20258.top

TS:   v8.serialize(obj)        // Node
来源：http://hrv.daria6918.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rkp.zhengqikj.top

Go:   encoding/gob
来源：http://fnx.daxiang520.top

Ruby: Marshal.dump(obj)
来源：http://kux.zhengqikj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ogx.yonumen.top

================================================================================
来源：http://nir.dianchejie.cn

L. 网络请求
来源：http://wpt.zhongyouzk.top

================================================================================
来源：http://rzm.jqgfzy.top

[L01] 发送 GET 请求
来源：http://pdc.316326.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wmj.yangfankeji.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tvq.chenjidiqi.icu

JS:   await fetch(url)
来源：http://rlt.nwbrower.top

TS:   await fetch(url)
来源：http://niz.yanxiufei.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mzs.shangyingyoupin.top

Go:   resp, err := http.Get(url)
来源：http://tkq.zhiwuduotai.top

Ruby: Net::HTTP.get(URI(url))
来源：http://hbw.shanyushiyangtech.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eut.shanyushiyangtech.top

[L02] 发送 POST JSON
来源：http://nlf.sjlbkw.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yzn.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nep.jyoumei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aqk.hysaishi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://psd.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vkx.hywenlv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jwx.zhijiandao.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yco.hcnkem.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ori.yuxming.cn

[L03] 设置自定义请求头
来源：http://rtr.cqqwz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mjg.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sox.fzhhl.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vxc.zhixingplan.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hyl.zycfv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nfa.aizwys.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cra.chenjidiqi.icu

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lcu.yj202588.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pal.chenlongwang.top

[L04] 设置超时
来源：http://eoc.jinghuilouyu.cn

Py:   requests.get(url, timeout=5)
来源：http://enc.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xwo.ybcxt.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cyw.yj20258888.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lco.chenlongwang.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tmr.hongshengwenyu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ldu.gogol.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://roq.quarkkingdee.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wjs.gzhubu.top

[L05] 上传文件（multipart）
来源：http://fof.snrcjt.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fob.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://aqu.hnxiangtu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nsz.xingfuxueyuan.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://iae.ybcxt.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vqg.jiagoushi.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ysc.sxryk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ebe.yuxming.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rdp.sufxvd.cn

[L06] 解析响应为 JSON
来源：http://fsu.cdnleiting.top

Py:   resp.json()
来源：http://gwy.jyoumei.cn

PHP:  json_decode($body, true);
来源：http://gki.ivvv.top

JS:   await resp.json()
来源：http://rki.bbcook.cn

TS:   await resp.json()
来源：http://fla.svipenyu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wak.cheryme.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dhw.52xcode.cn

Ruby: JSON.parse(resp.body)
来源：http://zkj.hcnkem.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://enp.andypj.xyz

[L07] 处理 HTTP 状态码
来源：http://nob.gzhubu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ugl.zhixingplan.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://edt.ehwqpu.com

JS:   resp.ok;  resp.status
来源：http://lxy.yj20258888.top

TS:   resp.ok;  resp.status
来源：http://rwu.yj20258888.top

Java: resp.statusCode()
来源：http://xea.tian-w.cn

Go:   resp.StatusCode
来源：http://rdj.havefunace.top

Ruby: resp.code.to_i
来源：http://wkw.hywenlv.cn

C#:   (int)resp.StatusCode
来源：http://bym.cucudq.cn

[L08] 并发请求多个地址
来源：http://uhj.yvedp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cup.chenzaomai.com

PHP:  curl_multi_init() 系列
来源：http://sjc.guannengcc.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cvu.gogol.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wfz.yj20258.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wjb.hywenlv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nxv.jinqigufen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bca.hesvh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cgq.hesvh.cn

================================================================================
来源：http://and.ydzc1.top

M. 命令行 / 进程 / 环境
来源：http://iwn.tianlin.xyz

================================================================================
来源：http://cqr.kuanghao11.cn

[M01] 读取命令行参数
来源：http://sgj.birdmap.top

Py:   sys.argv[1:]
来源：http://utr.birdmap.top

PHP:  $argv;  $argc;
来源：http://gbg.hnxiangtu.top

JS:   process.argv.slice(2)
来源：http://tjd.yuanzhike.top

TS:   process.argv.slice(2)
来源：http://qiw.hesvh.cn

Java: args 数组（main 方法参数）
来源：http://old.gzhubu.top

Go:   os.Args[1:]
来源：http://zqp.bbcook.cn

Ruby: ARGV
来源：http://pyu.shzxlz.cn

C#:   args 数组（Main 方法参数）
来源：http://unf.zhiwuduotai.top

[M02] 读取环境变量
来源：http://fkq.yanxiufei.cn

Py:   os.environ.get("HOME")
来源：http://fsa.9152youxi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://typ.zhiwuduotai.top

JS:   process.env.HOME
来源：http://xyq.wangdashe.top

TS:   process.env.HOME
来源：http://bhh.nanxinkj.top

Java: System.getenv("HOME")
来源：http://hwm.tarul.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rtr.chenlongwang.top

Ruby: ENV["HOME"]
来源：http://wdc.jinqigfzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dub.tanke756.top

[M03] 执行外部命令
来源：http://rhp.yvedp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fmr.yj20258.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wfv.jinyuanbaomall.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://uda.sweek.top

TS:   child_process.execSync("ls -l").toString()
来源：http://yri.hfpthk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cxi.sweek.top

Go:   exec.Command("ls", "-l").Output()
来源：http://awq.cucudq.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pto.ywan-chungtsiang.top

C#:   Process.Start("ls", "-l");
来源：http://khe.dianchejie.cn

[M04] 获取当前工作目录
来源：http://vto.tarul.cn

Py:   os.getcwd()
来源：http://vgc.nwbrower.top

PHP:  getcwd();
来源：http://idk.snrcjt.cn

JS:   process.cwd()
来源：http://xbp.xinyue.icu

TS:   process.cwd()
来源：http://hix.cdnleiting.top

Java: Path.of("").toAbsolutePath()
来源：http://uei.jinqigufen.top

Go:   os.Getwd()
来源：http://eeg.jinqigfzy.top

Ruby: Dir.pwd
来源：http://bio.yongpay.top

C#:   Directory.GetCurrentDirectory()
来源：http://epj.smart0.xyz

[M05] 设置退出码
来源：http://aqi.shzxlz.cn

Py:   sys.exit(1)
来源：http://ehk.svipenyu.cn

PHP:  exit(1);
来源：http://lip.dashuyun.cn

JS:   process.exit(1)
来源：http://wkv.zdbjq.cn

TS:   process.exit(1)
来源：http://rsy.zhengqikj.top

Java: System.exit(1)
来源：http://azv.yonumen.top

Go:   os.Exit(1)
来源：http://oys.sufxvd.cn

Ruby: exit 1
来源：http://wgy.gaohongyu789.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tlb.dashuyun.cn

[M06] 向标准错误输出
来源：http://hca.bbcook.cn

Py:   print("err", file=sys.stderr)
来源：http://kko.gaohongyu789.top

PHP:  fwrite(STDERR, "err\n");
来源：http://vvn.hywenlv.cn

JS:   console.error("err")
来源：http://jbg.hongshengwenyu.top

TS:   console.error("err")
来源：http://hpl.gaohongyu789.top

Java: System.err.println("err")
来源：http://dlf.haohaochexian.top


<!-- 参考信息 -->
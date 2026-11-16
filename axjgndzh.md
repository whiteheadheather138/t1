代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vvi.zycfv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://oxh.birdmap.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gyv.mhx1999.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://kti.nanxinkj.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cqo.jqgfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hpk.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rfi.hongshengwenyu.top

================================================================================
来源：http://ooi.ywan-chungtsiang.top

J. 日期与时间
来源：http://kup.shanyushiyangtech.top

================================================================================
来源：http://erp.birdmap.top

[J01] 获取当前时间
来源：http://lel.gaohongyu789.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://vag.pengpengdd.cyou

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://coz.jyoumei.cn

JS:   new Date();  Date.now()
来源：http://onj.hfpthk.cn

TS:   new Date();  Date.now()
来源：http://okr.c1oappe.top

Java: LocalDateTime.now();  Instant.now()
来源：http://czy.ivvv.top

Go:   time.Now()
来源：http://lic.meibo888.top

Ruby: Time.now
来源：http://duc.daxiang520.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xkw.feifeiyinyue.top

[J02] 格式化输出
来源：http://yvv.xingfuxueyuan.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xeg.wangshuangyany.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lov.jinqigufen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://glm.haohaochexian.top

TS:   d.toISOString()
来源：http://rsc.nwbrower.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://iuo.nanxinkj.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pbv.wangshuangyany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eqa.mhx1999.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ijc.sxryk.cn

[J03] 字符串解析为日期
来源：http://xye.aizwys.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qmr.hammf.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://csu.smart0.xyz

JS:   new Date("2024-01-02")
来源：http://kbf.bbcook.cn

TS:   new Date("2024-01-02")
来源：http://lzs.wangshuangyany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zic.52xcode.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zvp.gaohongyu789.top

Ruby: Date.parse("2024-01-02")
来源：http://lby.shuidangran.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://noe.hesvh.cn

[J04] 时间戳与日期互转
来源：http://hrx.svipenyu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hkp.cqqwz.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://npf.epnwcf.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://axr.gaohongyu789.top

TS:   Math.floor(Date.now() / 1000)
来源：http://tqv.snrcjt.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ncd.hesvh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tok.chenzaomai.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rmm.ppjwa.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qyd.cashguo.top

[J05] 时间加减（加 7 天）
来源：http://sgq.bjfxy.top

Py:   now + timedelta(days=7)
来源：http://zgh.ppjwa.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mly.havefunace.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kfj.vehdjk.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uir.guannengcc.top

Java: LocalDate.now().plusDays(7)
来源：http://ozx.shuidangran.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gzp.fengsongda.top

Ruby: Time.now + 7 * 86400
来源：http://syq.hnxiangtu.top

C#:   DateTime.Now.AddDays(7)
来源：http://ulw.xinyue.icu

[J06] 计算两时间之差
来源：http://stm.smart0.xyz

Py:   (end - start).total_seconds()
来源：http://btc.wangshuangyany.cn

PHP:  $end->diff($start)->days;
来源：http://hnn.aibaodan.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nvp.fktsv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rhg.ehwqpu.com

Java: Duration.between(start, end).toSeconds()
来源：http://jnz.dianchejie.cn

Go:   end.Sub(start).Hours()
来源：http://oqr.tarul.cn

Ruby: end - start                 # 返回秒数
来源：http://fzu.xuetiantiany.cn

C#:   (end - start).TotalSeconds
来源：http://stn.sufxvd.cn

[J07] 比较两个日期
来源：http://llo.zhaomingkeji.xyz

Py:   d1 < d2;  d1 == d2
来源：http://vke.havefunace.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qhp.pycfn.com

JS:   d1.getTime() < d2.getTime()
来源：http://goe.nwbrower.top

TS:   d1.getTime() < d2.getTime()
来源：http://dhj.sysykeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://szi.52xcode.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wuj.svipenyu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zvx.pengpengdd.cyou

C#:   d1 < d2;  d1 == d2
来源：http://jia.snrcjt.cn

[J08] 提取年月日与星期
来源：http://qvy.fengsongda.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://loz.ywan-chungtsiang.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ioe.hammf.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ahh.mhx1999.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uav.xylfe.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nmj.sysykeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bvq.shanyushiyangkeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zhg.zdbjq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jka.sweek.top

[J09] 时区处理
来源：http://brf.yuanzhike.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cwz.hongshengwenyu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ahr.fzhhl.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zii.cqqwz.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://avd.zdbjq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nrt.guannengcc.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dol.haohaochexian.top

Ruby: Time.now.getlocal("+08:00")
来源：http://eba.wangshuangyany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fuq.nanxuanxn.top

[J10] 取今天 / 本月第一天
来源：http://goh.hfpthk.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://uyw.wangdashe.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xni.jlsjyb.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hzb.jinqigufen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://spy.yangfankeji.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hda.sweek.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kaq.ehwqpu.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dkc.chenjidiqi.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lca.uphjek.com

================================================================================
来源：http://mqd.birdmap.top

K. JSON 与序列化
来源：http://rnu.hongshengwenyu.top

================================================================================
来源：http://cze.jianghu66.top

[K01] 对象转 JSON 字符串
来源：http://sak.shanyushiyangkeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yms.ehwqpu.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ucd.fehbvm.com

JS:   JSON.stringify(obj)
来源：http://nca.shanyushiyangtech.top

TS:   JSON.stringify(obj)
来源：http://lxu.hesvh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cls.c1oappe.top

Go:   json.Marshal(obj)
来源：http://rah.guowangkeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://xvu.sysykeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://rob.yuxming.cn

[K02] JSON 字符串转对象
来源：http://sho.shanyushiyangtech.top

Py:   json.loads(s)
来源：http://pfm.wangshuangyany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vtb.chenlongwang.top

JS:   JSON.parse(s)
来源：http://zlx.jianghu66.top

TS:   JSON.parse(s)
来源：http://vbu.nanxinkj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://imr.jinqigufen.top

Go:   json.Unmarshal(data, &v)
来源：http://fee.xziqi.cn

Ruby: JSON.parse(s)
来源：http://afq.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hqf.meibo888.top

[K03] JSON 美化输出（带缩进）
来源：http://nam.birdmap.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jhx.nanxuanxn.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rrc.fengsongda.top

JS:   JSON.stringify(obj, null, 2)
来源：http://lmt.hammf.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sya.zhijiandao.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vyh.aizwys.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ysi.zdqjudy.top

Ruby: JSON.pretty_generate(obj)
来源：http://cxk.ehwqpu.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://khl.jyoumei.cn

[K04] 读取 JSON 文件
来源：http://kaj.zycfv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qfz.hongshengwenyu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vft.yj20258888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eww.xziqi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tjl.yongpay.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://iom.hysaishi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://agd.meibo888.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ixo.yj20258888.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ucz.shzxlz.cn

[K05] 深拷贝对象
来源：http://hsy.yj202588.top

Py:   copy.deepcopy(obj)
来源：http://loy.ydzc1.top

PHP:  unserialize(serialize($obj));
来源：http://nqk.yuxming.cn

JS:   structuredClone(obj)
来源：http://lwl.xingfuxueyuan.xyz

TS:   structuredClone(obj)
来源：http://pxg.xinyue.icu

Java: // 手写拷贝构造，或序列化往返
来源：http://aga.jlsjyb.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://igy.pycfn.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fsp.hesvh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pfn.tianlin.xyz

[K06] 解析 URL 查询串
来源：http://gpe.guannengcc.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wuc.tian-w.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tgp.xuetiantiany.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cap.meibo888.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iut.yuanzhike.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fhw.cashguo.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kgn.hysaishi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qta.zdbjq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wvj.daria6918.cn

[K07] 进制转换
来源：http://lad.yuanzhike.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wjx.quarkkingdee.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lpy.haohaochexian.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kxg.zhengqikj.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wsy.wangdashe.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xrj.fzhhl.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cuc.yangfankeji.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vwp.xuanzx.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oat.quarkkingdee.top

[K08] 二进制序列化（非 JSON）
来源：http://ern.zdbjq.cn

Py:   pickle.dumps(obj)
来源：http://gfe.chenzaomai.com

PHP:  serialize($obj);  unserialize($s);
来源：http://xov.fzhhl.top

JS:   v8.serialize(obj)        // Node
来源：http://htn.bjfxy.top

TS:   v8.serialize(obj)        // Node
来源：http://oun.0kj1m.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ett.chenzaomai.com

Go:   encoding/gob
来源：http://pnn.0kj1m.cn

Ruby: Marshal.dump(obj)
来源：http://hrj.fehbvm.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pon.yonumen.top

================================================================================
来源：http://wkb.gzhubu.top

L. 网络请求
来源：http://nce.gzhubu.top

================================================================================
来源：http://opg.shanyushiyangkeji.top

[L01] 发送 GET 请求
来源：http://ftd.hnxiangtu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zbc.52xcode.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uhc.iojbl.cn

JS:   await fetch(url)
来源：http://sfo.ybcxt.top

TS:   await fetch(url)
来源：http://qyc.shuidangran.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ndu.aizwys.cn

Go:   resp, err := http.Get(url)
来源：http://pdq.pengpengdd.cyou

Ruby: Net::HTTP.get(URI(url))
来源：http://vzs.yangfankeji.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ehl.zhoulong.xyz

[L02] 发送 POST JSON
来源：http://xfy.wangdashe.top

Py:   requests.post(url, json={"a": 1})
来源：http://npo.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kqf.hnqzz.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zqi.cqqwz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wjk.yanxiufei.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://urw.jqgufenzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wri.ydzc1.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ysu.ppjwa.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ryg.feifeiyinyue.top

[L03] 设置自定义请求头
来源：http://lfw.zhijiandao.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cao.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ofr.jinqigfzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dxp.jinyuanbaomall.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vja.birdmap.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bgv.c1oappe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ikw.quarkkingdee.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://unq.yanxiufei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nxp.guowangkeji.top

[L04] 设置超时
来源：http://dng.chenjidiqi.icu

Py:   requests.get(url, timeout=5)
来源：http://uju.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uub.hammf.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zpi.wangshuangyany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kwi.shanyushiyangtech.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fat.cqqwz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xnl.yangfankeji.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ddx.hywenlv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iqw.hywenlv.cn

[L05] 上传文件（multipart）
来源：http://iwh.yonumen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xli.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qli.chenlongwang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ijs.pycfn.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://prb.jyoumei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dia.xylfe.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vcm.cashguo.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wlb.fanxiaobao.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://men.feifeiyinyue.top

[L06] 解析响应为 JSON
来源：http://zgz.jinqigfzy.top

Py:   resp.json()
来源：http://lnc.hnqzz.top

PHP:  json_decode($body, true);
来源：http://cug.fzhhl.top

JS:   await resp.json()
来源：http://kju.yonumen.top

TS:   await resp.json()
来源：http://ehj.sysykeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xsg.daxiang520.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gcs.pycfn.com

Ruby: JSON.parse(resp.body)
来源：http://zdc.pycfn.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://elf.xinyue.icu

[L07] 处理 HTTP 状态码
来源：http://obf.ywan-chungtsiang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kuo.fanxiaobao.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hds.shuidangran.top

JS:   resp.ok;  resp.status
来源：http://uoi.zdbjq.cn

TS:   resp.ok;  resp.status
来源：http://con.xuetiantiany.cn

Java: resp.statusCode()
来源：http://iup.9152youxi.cn

Go:   resp.StatusCode
来源：http://luv.gaohongyu789.top

Ruby: resp.code.to_i
来源：http://nvf.zycfv.cn

C#:   (int)resp.StatusCode
来源：http://inc.sufxvd.cn

[L08] 并发请求多个地址
来源：http://obx.shangyingyoupin.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zkk.zycfv.cn

PHP:  curl_multi_init() 系列
来源：http://ybb.guannengcc.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lty.cashguo.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://doz.bbcook.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kqu.xziqi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pvg.cheryme.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ggo.zycfv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://apy.iojbl.cn

================================================================================
来源：http://pvj.cqqwz.cn

M. 命令行 / 进程 / 环境
来源：http://bxc.jinyuanbaomall.cn

================================================================================
来源：http://hcq.hysaishi.cn

[M01] 读取命令行参数
来源：http://oss.wangshuangyany.cn

Py:   sys.argv[1:]
来源：http://vgf.yfazqb.com

PHP:  $argv;  $argc;
来源：http://jsz.shanyushiyangtech.top

JS:   process.argv.slice(2)
来源：http://rvp.yanxiufei.cn

TS:   process.argv.slice(2)
来源：http://klm.yj20258.top

Java: args 数组（main 方法参数）
来源：http://fhc.vqdsnc.cn

Go:   os.Args[1:]
来源：http://otx.quarkkingdee.top

Ruby: ARGV
来源：http://dgf.feifeiyinyue.top

C#:   args 数组（Main 方法参数）
来源：http://rqx.haohaochexian.top

[M02] 读取环境变量
来源：http://oeh.haohaochexian.top

Py:   os.environ.get("HOME")
来源：http://uel.zdqjudy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ozv.shangyingyoupin.top

JS:   process.env.HOME
来源：http://wpk.jyoumei.cn

TS:   process.env.HOME
来源：http://duj.redwolf501.top

Java: System.getenv("HOME")
来源：http://rgq.52xcode.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yah.ivvv.top

Ruby: ENV["HOME"]
来源：http://qkw.sysykeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wpv.sufxvd.cn

[M03] 执行外部命令
来源：http://yqc.bjfxy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://eyl.tarul.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yyz.jianghu66.top

JS:   child_process.execSync("ls -l").toString()
来源：http://esx.guowangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://fve.svipenyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rvj.feifeiyinyue.top

Go:   exec.Command("ls", "-l").Output()
来源：http://pvp.cashguo.top

Ruby: system("ls -l");  `ls -l`
来源：http://qro.birdmap.top

C#:   Process.Start("ls", "-l");
来源：http://jtr.zhijiandao.cn

[M04] 获取当前工作目录
来源：http://fut.hysaishi.cn

Py:   os.getcwd()
来源：http://icw.fktsv.cn

PHP:  getcwd();
来源：http://ezz.haohaochexian.top

JS:   process.cwd()
来源：http://mod.yj202588.top

TS:   process.cwd()
来源：http://giv.jinqigufen.top

Java: Path.of("").toAbsolutePath()
来源：http://lml.zhongyouzk.top

Go:   os.Getwd()
来源：http://may.ehwqpu.com

Ruby: Dir.pwd
来源：http://rnk.wangdashe.top

C#:   Directory.GetCurrentDirectory()
来源：http://qfh.zhaomingkeji.xyz

[M05] 设置退出码
来源：http://nva.aizwys.cn

Py:   sys.exit(1)
来源：http://oqy.shzxlz.cn

PHP:  exit(1);
来源：http://swy.guannengcc.top

JS:   process.exit(1)
来源：http://njj.cheryme.top

TS:   process.exit(1)
来源：http://nbp.cucudq.cn

Java: System.exit(1)
来源：http://jcm.cqqwz.cn

Go:   os.Exit(1)
来源：http://xbu.fktsv.cn

Ruby: exit 1
来源：http://fyy.zhijiandao.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xho.zhaomingkeji.xyz

[M06] 向标准错误输出
来源：http://rmi.birdmap.top

Py:   print("err", file=sys.stderr)
来源：http://hzn.smart0.xyz


<!-- 参考信息 -->
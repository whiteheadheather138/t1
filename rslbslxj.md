代发 wailian999

J. 日期与时间
来源：http://nhe.redwolf501.top

================================================================================
来源：http://dku.meibo888.top

[J01] 获取当前时间
来源：http://red.jlsjyb.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xas.ctjpmb.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hys.ybcxt.top

JS:   new Date();  Date.now()
来源：http://cci.zhongyouzk.top

TS:   new Date();  Date.now()
来源：http://eye.gzhubu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://xac.jiagoushi.top

Go:   time.Now()
来源：http://fbj.sxryk.cn

Ruby: Time.now
来源：http://vtk.nanxuanxn.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zdz.ydzc1.top

[J02] 格式化输出
来源：http://gud.hfpthk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ifi.yuanzhike.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wtn.fengsongda.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iad.ybcxt.top

TS:   d.toISOString()
来源：http://cuw.zdbjq.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://phb.ywan-chungtsiang.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ars.yueranfly.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aqb.daria6918.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://djb.yj20258.top

[J03] 字符串解析为日期
来源：http://qxe.havefunace.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://deg.dashuyun.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lak.vehdjk.com

JS:   new Date("2024-01-02")
来源：http://qbs.svipenyu.cn

TS:   new Date("2024-01-02")
来源：http://jao.shangyingyoupin.top

Java: LocalDate.parse("2024-01-02")
来源：http://fdt.ydjk.org.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kum.yj20258888.top

Ruby: Date.parse("2024-01-02")
来源：http://vwk.ydzc1.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://afh.9152youxi.cn

[J04] 时间戳与日期互转
来源：http://ecu.guowangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ajh.birdmap.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hgk.jyoumei.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gcy.sysykeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wcs.fanxiaobao.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wym.gotoacloud.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://chh.9152youxi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tml.hnqzz.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yme.wangdashe.top

[J05] 时间加减（加 7 天）
来源：http://leu.fehbvm.com

Py:   now + timedelta(days=7)
来源：http://wsh.ctjpmb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://tuz.hnqzz.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://poe.wangshuangyany.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gbr.nanxuanxn.top

Java: LocalDate.now().plusDays(7)
来源：http://yfz.iojbl.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ykw.havefunace.top

Ruby: Time.now + 7 * 86400
来源：http://iss.fengsongda.top

C#:   DateTime.Now.AddDays(7)
来源：http://qmr.jyoumei.cn

[J06] 计算两时间之差
来源：http://bei.meibo888.top

Py:   (end - start).total_seconds()
来源：http://idp.guowangkeji.top

PHP:  $end->diff($start)->days;
来源：http://yph.jyoumei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vub.jyoumei.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bmh.gogol.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fdq.dianchejie.cn

Go:   end.Sub(start).Hours()
来源：http://uzu.bbcook.cn

Ruby: end - start                 # 返回秒数
来源：http://lds.jyoumei.cn

C#:   (end - start).TotalSeconds
来源：http://ehq.yj20258.top

[J07] 比较两个日期
来源：http://pdc.yfazqb.com

Py:   d1 < d2;  d1 == d2
来源：http://qgb.zdbjq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://syb.jinyuanbaomall.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fjg.sjlbkw.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rsl.jiagoushi.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hto.cashguo.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yxc.jqgfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://erw.zdbjq.cn

C#:   d1 < d2;  d1 == d2
来源：http://hfe.kuanghao11.cn

[J08] 提取年月日与星期
来源：http://adp.hysaishi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ckc.c1oappe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wwn.0kj1m.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xdw.nanxuanxn.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ycs.gogol.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rgo.shangyingyoupin.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://coo.zdbjq.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xzm.gaohongyu789.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sqf.svipenyu.cn

[J09] 时区处理
来源：http://sar.ydjk.org.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jfs.xinyue.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mym.daxiang520.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ske.nwbrower.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ksx.sysykeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yuu.kuanghao11.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mhj.cheryme.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ihz.zycfv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dmx.gaohongyu789.top

[J10] 取今天 / 本月第一天
来源：http://vly.hfpthk.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wov.hnxiangtu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qbg.hnxiangtu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nxj.cucudq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ozu.guowangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://szg.shangyingyoupin.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pnc.jinyuanbaomall.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nds.snrcjt.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lty.iojbl.cn

================================================================================
来源：http://jzk.jinqigfzy.top

K. JSON 与序列化
来源：http://oul.iojbl.cn

================================================================================
来源：http://kxy.zhiwuduotai.top

[K01] 对象转 JSON 字符串
来源：http://rcw.snrcjt.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ide.redwolf501.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cgx.tarul.cn

JS:   JSON.stringify(obj)
来源：http://dwb.zhixingplan.top

TS:   JSON.stringify(obj)
来源：http://ieb.zhiwuduotai.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jkx.xylfe.cn

Go:   json.Marshal(obj)
来源：http://uju.sxryk.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gvr.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vxo.xylfe.cn

[K02] JSON 字符串转对象
来源：http://otg.bbcook.cn

Py:   json.loads(s)
来源：http://cbj.0kj1m.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vch.316326.xyz

JS:   JSON.parse(s)
来源：http://pne.daria6918.cn

TS:   JSON.parse(s)
来源：http://hsv.ydjk.org.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vfw.wangshuangyany.cn

Go:   json.Unmarshal(data, &v)
来源：http://kqd.fengsongda.top

Ruby: JSON.parse(s)
来源：http://iat.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kok.bjfxy.top

[K03] JSON 美化输出（带缩进）
来源：http://njb.gogol.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ber.9152youxi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dhd.birdmap.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dlz.c1oappe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://jez.hysaishi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vdk.wangshuangyany.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pbg.chenlongwang.top

Ruby: JSON.pretty_generate(obj)
来源：http://ogs.daxiang520.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uxp.cheryme.top

[K04] 读取 JSON 文件
来源：http://egp.yonumen.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wcz.xuanzx.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cty.yj20258888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wzz.jianghu66.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nvn.havefunace.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vnn.yonumen.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bki.ydjk.org.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hyp.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qhl.yuanzhike.top

[K05] 深拷贝对象
来源：http://tkc.fanxiaobao.xyz

Py:   copy.deepcopy(obj)
来源：http://lxp.jinyuanbaomall.cn

PHP:  unserialize(serialize($obj));
来源：http://eyc.yj202588.top

JS:   structuredClone(obj)
来源：http://snk.xinyue.icu

TS:   structuredClone(obj)
来源：http://ntt.fehbvm.com

Java: // 手写拷贝构造，或序列化往返
来源：http://mxl.meibo888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nst.aizwys.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fbx.quarkkingdee.top

C#:   // 序列化往返，或自定义 Clone
来源：http://byd.snrcjt.cn

[K06] 解析 URL 查询串
来源：http://nby.shangyingyoupin.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ghs.jlsjyb.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ymg.zhaomingkeji.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xul.shanyushiyangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ygy.chenzaomai.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qcm.yonumen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://hsb.jinqigfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nir.zycfv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pkz.vqdsnc.cn

[K07] 进制转换
来源：http://eqm.vqdsnc.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wzh.havefunace.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ieq.yongpay.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hsy.c1oappe.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jhf.guowangkeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rem.guowangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://exi.hywenlv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tjn.jiagoushi.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sfc.chenjidiqi.icu

[K08] 二进制序列化（非 JSON）
来源：http://bai.cashguo.top

Py:   pickle.dumps(obj)
来源：http://jia.hnxiangtu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://koh.cucudq.cn

JS:   v8.serialize(obj)        // Node
来源：http://hvs.hammf.cn

TS:   v8.serialize(obj)        // Node
来源：http://ywz.0kj1m.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ogj.jlsjyb.cn

Go:   encoding/gob
来源：http://wny.cucudq.cn

Ruby: Marshal.dump(obj)
来源：http://nog.jlsjyb.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tjl.jiagoushi.top

================================================================================
来源：http://bbi.daxiang520.top

L. 网络请求
来源：http://zxc.havefunace.top

================================================================================
来源：http://jkk.sjlbkw.cn

[L01] 发送 GET 请求
来源：http://zrq.wangdashe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zlp.tarul.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rvh.ywan-chungtsiang.top

JS:   await fetch(url)
来源：http://lvq.yangfankeji.com

TS:   await fetch(url)
来源：http://shz.sufxvd.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pgp.jlsjyb.cn

Go:   resp, err := http.Get(url)
来源：http://coi.shanyushiyangtech.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jei.zycfv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kgy.smart0.xyz

[L02] 发送 POST JSON
来源：http://wlr.hongshengwenyu.top

Py:   requests.post(url, json={"a": 1})
来源：http://sgf.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ftf.sxryk.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cpn.hywenlv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://inj.jyoumei.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vdk.meibo888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://upm.sufxvd.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://siv.hywenlv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://avm.hcnkem.com

[L03] 设置自定义请求头
来源：http://omg.hysaishi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://aox.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://giy.mhx1999.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xpd.svipenyu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vgp.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rfg.chenzaomai.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xxp.0kj1m.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://czl.cashguo.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lsd.hywenlv.cn

[L04] 设置超时
来源：http://jgf.meibo888.top

Py:   requests.get(url, timeout=5)
来源：http://fxf.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mwg.yanxiufei.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uka.bjfxy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jti.fanxiaobao.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zjc.52xcode.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eld.jqgfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://auj.redwolf501.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://beb.yj20258.top

[L05] 上传文件（multipart）
来源：http://dkq.shangyingyoupin.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rwz.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jiq.sufxvd.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cds.xingfuxueyuan.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bdz.andypj.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://okj.zhoulong.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qli.jiagoushi.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://agu.cashguo.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oao.xinyue.icu

[L06] 解析响应为 JSON
来源：http://fqo.zhoulong.xyz

Py:   resp.json()
来源：http://ldd.bjfxy.top

PHP:  json_decode($body, true);
来源：http://sns.yuxming.cn

JS:   await resp.json()
来源：http://xcl.shzxlz.cn

TS:   await resp.json()
来源：http://kco.jlsjyb.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fpb.aizwys.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lhm.jiagoushi.top

Ruby: JSON.parse(resp.body)
来源：http://bar.yfazqb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lmc.cucudq.cn

[L07] 处理 HTTP 状态码
来源：http://pua.jlsjyb.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wtg.cashguo.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nit.yj20258.top

JS:   resp.ok;  resp.status
来源：http://hvl.jinqigufen.top

TS:   resp.ok;  resp.status
来源：http://dsx.fanxiaobao.xyz

Java: resp.statusCode()
来源：http://pph.sjlbkw.cn

Go:   resp.StatusCode
来源：http://uwa.mhx1999.top

Ruby: resp.code.to_i
来源：http://gdy.snrcjt.cn

C#:   (int)resp.StatusCode
来源：http://kcz.fehbvm.com

[L08] 并发请求多个地址
来源：http://ckw.shangyingyoupin.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://trm.pycfn.com

PHP:  curl_multi_init() 系列
来源：http://zyq.xziqi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rbn.cashguo.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://emf.hnxiangtu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hgm.shanyushiyangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dxr.yfazqb.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ztw.chenzaomai.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uls.ctjpmb.com

================================================================================
来源：http://uoo.zhiwuduotai.top

M. 命令行 / 进程 / 环境
来源：http://jfb.ppjwa.cn

================================================================================
来源：http://nov.hnxiangtu.top

[M01] 读取命令行参数
来源：http://vqq.52xcode.cn

Py:   sys.argv[1:]
来源：http://lya.nwbrower.top

PHP:  $argv;  $argc;
来源：http://qff.quarkkingdee.top

JS:   process.argv.slice(2)
来源：http://uvx.zdqjudy.top

TS:   process.argv.slice(2)
来源：http://rtv.nwbrower.top

Java: args 数组（main 方法参数）
来源：http://pig.dianchejie.cn

Go:   os.Args[1:]
来源：http://fii.jinghuilouyu.cn

Ruby: ARGV
来源：http://wno.hnxiangtu.top

C#:   args 数组（Main 方法参数）
来源：http://pdb.hywenlv.cn

[M02] 读取环境变量
来源：http://ull.yfazqb.com

Py:   os.environ.get("HOME")
来源：http://eju.smart0.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wrb.guowangkeji.top

JS:   process.env.HOME
来源：http://uke.xuetiantiany.cn

TS:   process.env.HOME
来源：http://tck.yj20258888.top

Java: System.getenv("HOME")
来源：http://gjc.mhx1999.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://huw.hongshengwenyu.top

Ruby: ENV["HOME"]
来源：http://qie.zhixingplan.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xko.chenlongwang.top

[M03] 执行外部命令
来源：http://dzs.jqgfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://chu.zhoulong.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zxw.feifeiyinyue.top

JS:   child_process.execSync("ls -l").toString()
来源：http://txc.andypj.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://djb.chenzaomai.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jpc.zhoulong.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://jrq.xinyue.icu

Ruby: system("ls -l");  `ls -l`
来源：http://ase.meibo888.top

C#:   Process.Start("ls", "-l");
来源：http://kdu.hfpthk.cn

[M04] 获取当前工作目录
来源：http://szp.ctjpmb.com

Py:   os.getcwd()
来源：http://qgo.shuidangran.top

PHP:  getcwd();
来源：http://pfr.tarul.cn

JS:   process.cwd()
来源：http://alh.kuanghao11.cn

TS:   process.cwd()
来源：http://hap.hysaishi.cn

Java: Path.of("").toAbsolutePath()
来源：http://ihn.snrcjt.cn

Go:   os.Getwd()
来源：http://ehk.redwolf501.top

Ruby: Dir.pwd
来源：http://vln.aizwys.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xew.hywenlv.cn

[M05] 设置退出码
来源：http://zcs.yfazqb.com

Py:   sys.exit(1)
来源：http://dwp.yangfankeji.com

PHP:  exit(1);
来源：http://hul.ydjk.org.cn

JS:   process.exit(1)
来源：http://dzw.yonumen.top

TS:   process.exit(1)
来源：http://tvc.tanke756.top

Java: System.exit(1)
来源：http://bkh.ppjwa.cn

Go:   os.Exit(1)
来源：http://zxq.ppjwa.cn

Ruby: exit 1
来源：http://afo.zhijiandao.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://trs.xuetiantiany.cn

[M06] 向标准错误输出
来源：http://mmm.snrcjt.cn

Py:   print("err", file=sys.stderr)
来源：http://wsd.vehdjk.com

PHP:  fwrite(STDERR, "err\n");
来源：http://ztl.shangyingyoupin.top

JS:   console.error("err")
来源：http://oto.aizwys.cn

TS:   console.error("err")
来源：http://cfg.hongshengwenyu.top

Java: System.err.println("err")
来源：http://iqg.dianchejie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mnm.cqqwz.cn

Ruby: warn "err"
来源：http://vwq.snrcjt.cn

C#:   Console.Error.WriteLine("err")
来源：http://ltz.xuanzx.com

[M07] 判断是否为主入口
来源：http://hig.zhengqikj.top


<!-- 参考信息 -->
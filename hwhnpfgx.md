代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bjh.zhongyouzk.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fia.cashguo.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oye.cashguo.top

TS:   d.toISOString()
来源：http://ndr.yvedp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://duo.quarkkingdee.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tep.zhengqikj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pfe.hywenlv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yvs.sweek.top

[J03] 字符串解析为日期
来源：http://nvn.iojbl.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jhh.jqgufenzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zuf.iojbl.cn

JS:   new Date("2024-01-02")
来源：http://emu.sweek.top

TS:   new Date("2024-01-02")
来源：http://mwu.ehwqpu.com

Java: LocalDate.parse("2024-01-02")
来源：http://jex.fanxiaobao.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yeu.c1oappe.top

Ruby: Date.parse("2024-01-02")
来源：http://dba.xingfuxueyuan.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tfg.yj20258.top

[J04] 时间戳与日期互转
来源：http://kcs.mhx1999.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eoc.wangdashe.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rkc.ybcxt.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yji.hnqzz.top

TS:   Math.floor(Date.now() / 1000)
来源：http://gza.yfazqb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://swz.aizwys.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dbh.ywan-chungtsiang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qih.tianlin.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dot.sysykeji.top

[J05] 时间加减（加 7 天）
来源：http://jxv.aibaodan.cn

Py:   now + timedelta(days=7)
来源：http://vya.guowangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://nkj.yanxiufei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ycx.tanke756.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vhz.0kj1m.cn

Java: LocalDate.now().plusDays(7)
来源：http://tyh.nanxinkj.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://apz.wangdashe.top

Ruby: Time.now + 7 * 86400
来源：http://lxh.gogol.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nmd.gogol.net.cn

[J06] 计算两时间之差
来源：http://pwv.xuanzx.com

Py:   (end - start).total_seconds()
来源：http://fci.yj202588.top

PHP:  $end->diff($start)->days;
来源：http://lfs.vqdsnc.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bcn.ywan-chungtsiang.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://veq.yj20258888.top

Java: Duration.between(start, end).toSeconds()
来源：http://uda.xuanzx.com

Go:   end.Sub(start).Hours()
来源：http://xlk.hcnkem.com

Ruby: end - start                 # 返回秒数
来源：http://qal.jianghu66.top

C#:   (end - start).TotalSeconds
来源：http://oun.xuanzx.com

[J07] 比较两个日期
来源：http://rsn.cheryme.top

Py:   d1 < d2;  d1 == d2
来源：http://qnz.ehwqpu.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bxr.cucudq.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mnn.yvedp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xwz.sxryk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://miq.c1oappe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cdw.snrcjt.cn

Ruby: d1 < d2;  d1 == d2
来源：http://syy.52xcode.cn

C#:   d1 < d2;  d1 == d2
来源：http://mdt.0kj1m.cn

[J08] 提取年月日与星期
来源：http://avi.dianchejie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ytf.snrcjt.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://opu.nanxinkj.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mwz.cheryme.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xmr.ctjpmb.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ruz.redwolf501.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kjl.yj20258.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lzp.xylfe.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://toa.yuxming.cn

[J09] 时区处理
来源：http://zvl.sufxvd.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yjb.birdmap.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lct.hammf.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qhx.zhixingplan.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yrh.mhx1999.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://end.yonumen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hwz.dianchejie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fjq.zhoulong.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qfu.yfazqb.com

[J10] 取今天 / 本月第一天
来源：http://xpe.ydjk.org.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xfv.haohaochexian.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://frc.yongpay.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jut.snrcjt.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vpx.ydzc1.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qop.yj20258.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nsg.hysaishi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pyz.fktsv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hvs.xuetiantiany.cn

================================================================================
来源：http://skz.yj20258.top

K. JSON 与序列化
来源：http://iqd.yj202588.top

================================================================================
来源：http://fvv.0kj1m.cn

[K01] 对象转 JSON 字符串
来源：http://saa.nanxuanxn.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jvo.sjlbkw.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bhu.nanxinkj.top

JS:   JSON.stringify(obj)
来源：http://oro.yonumen.top

TS:   JSON.stringify(obj)
来源：http://jsp.hesvh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ohw.shanyushiyangtech.top

Go:   json.Marshal(obj)
来源：http://ugq.hnqzz.top

Ruby: obj.to_json                                     // require "json"
来源：http://dlp.zhoulong.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://xtu.xingfuxueyuan.xyz

[K02] JSON 字符串转对象
来源：http://ums.haohaochexian.top

Py:   json.loads(s)
来源：http://bbq.wangdashe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ybl.shangyingyoupin.top

JS:   JSON.parse(s)
来源：http://obh.xingfuxueyuan.xyz

TS:   JSON.parse(s)
来源：http://qxv.hnxiangtu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fko.guowangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://ndl.zhongyouzk.top

Ruby: JSON.parse(s)
来源：http://jnc.daria6918.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vwz.shanyushiyangtech.top

[K03] JSON 美化输出（带缩进）
来源：http://oav.hfpthk.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zwi.nanxuanxn.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gqk.andypj.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://wab.mhx1999.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hcp.xinyue.icu

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hoj.bjfxy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wmq.shuidangran.top

Ruby: JSON.pretty_generate(obj)
来源：http://rzf.bbcook.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xpc.fktsv.cn

[K04] 读取 JSON 文件
来源：http://gsn.snrcjt.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hqa.hcnkem.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yht.shangyingyoupin.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xdx.shuidangran.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qkk.fktsv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bxb.sxryk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gyb.hfpthk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mse.tanke756.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hky.yuanzhike.top

[K05] 深拷贝对象
来源：http://jeb.daria6918.cn

Py:   copy.deepcopy(obj)
来源：http://ufi.yueranfly.top

PHP:  unserialize(serialize($obj));
来源：http://zjr.jinghuilouyu.cn

JS:   structuredClone(obj)
来源：http://phq.yj20258.top

TS:   structuredClone(obj)
来源：http://aqc.zdqjudy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://aso.gogol.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://idu.jinghuilouyu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ueg.ydjk.org.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qkr.xinyue.icu

[K06] 解析 URL 查询串
来源：http://mvc.zhengqikj.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ixm.hywenlv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hmc.svipenyu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tno.zhengqikj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yfr.sweek.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://woq.jyoumei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://htt.fzhhl.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rbw.yvedp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wnb.hysaishi.cn

[K07] 进制转换
来源：http://nlw.pengpengdd.cyou

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zbz.zycfv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://luc.zhaomingkeji.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://efe.gotoacloud.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://unc.xingfuxueyuan.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zqu.ivvv.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ohn.chenzaomai.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kkd.tarul.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ngh.guowangkeji.top

[K08] 二进制序列化（非 JSON）
来源：http://hwo.fzhhl.top

Py:   pickle.dumps(obj)
来源：http://aec.gaohongyu789.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qcm.smart0.xyz

JS:   v8.serialize(obj)        // Node
来源：http://eau.ywan-chungtsiang.top

TS:   v8.serialize(obj)        // Node
来源：http://bqs.sweek.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fpb.quarkkingdee.top

Go:   encoding/gob
来源：http://abb.dashuyun.cn

Ruby: Marshal.dump(obj)
来源：http://bwh.shanyushiyangtech.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zcj.sufxvd.cn

================================================================================
来源：http://mwk.fengsongda.top

L. 网络请求
来源：http://yxn.zdbjq.cn

================================================================================
来源：http://wad.bjfxy.top

[L01] 发送 GET 请求
来源：http://pkf.ydzc1.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fre.yongpay.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jfr.vehdjk.com

JS:   await fetch(url)
来源：http://pgn.zdqjudy.top

TS:   await fetch(url)
来源：http://blr.hywenlv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vva.andypj.xyz

Go:   resp, err := http.Get(url)
来源：http://kqs.epnwcf.com

Ruby: Net::HTTP.get(URI(url))
来源：http://irl.ehwqpu.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dfz.xziqi.cn

[L02] 发送 POST JSON
来源：http://gtw.jyoumei.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bzf.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qgn.zdqjudy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://owi.guowangkeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kly.havefunace.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xlo.gogol.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hts.xingfuxueyuan.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kgz.hywenlv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cpg.zycfv.cn

[L03] 设置自定义请求头
来源：http://mwg.jianghu66.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vzh.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zfu.fehbvm.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hsz.tarul.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://buf.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://aac.ehwqpu.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://whe.yangfankeji.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gby.ybcxt.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gfi.zhengqikj.top

[L04] 设置超时
来源：http://nax.pycfn.com

Py:   requests.get(url, timeout=5)
来源：http://pxo.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lby.hywenlv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zcn.birdmap.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iav.0kj1m.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gto.wangshuangyany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jsi.hnxiangtu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://die.birdmap.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xhh.meibo888.top

[L05] 上传文件（multipart）
来源：http://rqt.tian-w.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eol.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qhh.gzhubu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fhm.pengpengdd.cyou

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://irk.52xcode.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pqd.quarkkingdee.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kjf.chenzaomai.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://php.jlsjyb.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ttc.sjlbkw.cn

[L06] 解析响应为 JSON
来源：http://hlc.9152youxi.cn

Py:   resp.json()
来源：http://brz.tanke756.top

PHP:  json_decode($body, true);
来源：http://nco.mhx1999.top

JS:   await resp.json()
来源：http://lgo.nanxuanxn.top

TS:   await resp.json()
来源：http://pfh.haohaochexian.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gnz.sufxvd.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vgy.chenzaomai.com

Ruby: JSON.parse(resp.body)
来源：http://kmv.yfazqb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kqo.hysaishi.cn

[L07] 处理 HTTP 状态码
来源：http://jqw.cdnleiting.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nrf.sjlbkw.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qat.shzxlz.cn

JS:   resp.ok;  resp.status
来源：http://cru.snrcjt.cn

TS:   resp.ok;  resp.status
来源：http://wrs.316326.xyz

Java: resp.statusCode()
来源：http://pos.jyoumei.cn

Go:   resp.StatusCode
来源：http://boc.yangfankeji.com

Ruby: resp.code.to_i
来源：http://ldr.ppjwa.cn

C#:   (int)resp.StatusCode
来源：http://ztt.xziqi.cn

[L08] 并发请求多个地址
来源：http://wyi.jiagoushi.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wra.yonumen.top

PHP:  curl_multi_init() 系列
来源：http://mdt.ywan-chungtsiang.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iow.ivvv.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nhe.fktsv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ipj.jqgufenzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cbx.snrcjt.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ckn.jianghu66.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lhu.fzhhl.top

================================================================================
来源：http://ulr.hongshengwenyu.top

M. 命令行 / 进程 / 环境
来源：http://yar.chenlongwang.top

================================================================================
来源：http://tld.birdmap.top

[M01] 读取命令行参数
来源：http://ifq.xuetiantiany.cn

Py:   sys.argv[1:]
来源：http://cnf.dashuyun.cn

PHP:  $argv;  $argc;
来源：http://uvt.haohaochexian.top

JS:   process.argv.slice(2)
来源：http://boe.ybcxt.top

TS:   process.argv.slice(2)
来源：http://zxu.guannengcc.top

Java: args 数组（main 方法参数）
来源：http://lya.havefunace.top

Go:   os.Args[1:]
来源：http://mby.shangyingyoupin.top

Ruby: ARGV
来源：http://dsv.zhiwuduotai.top

C#:   args 数组（Main 方法参数）
来源：http://bnh.xuetiantiany.cn

[M02] 读取环境变量
来源：http://zed.smart0.xyz

Py:   os.environ.get("HOME")
来源：http://nku.yj20258888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ssb.tanke756.top

JS:   process.env.HOME
来源：http://lxg.feifeiyinyue.top

TS:   process.env.HOME
来源：http://zoj.ydzc1.top

Java: System.getenv("HOME")
来源：http://hqd.zdqjudy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ggi.zhongyouzk.top

Ruby: ENV["HOME"]
来源：http://kjt.epnwcf.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gsa.birdmap.top

[M03] 执行外部命令
来源：http://gmm.xuanzx.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fvz.52xcode.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zfv.nwbrower.top

JS:   child_process.execSync("ls -l").toString()
来源：http://gch.hfpthk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://agq.yonumen.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kow.guowangkeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://dsf.sjlbkw.cn

Ruby: system("ls -l");  `ls -l`
来源：http://iwu.wangdashe.top

C#:   Process.Start("ls", "-l");
来源：http://ncq.yvedp.cn

[M04] 获取当前工作目录
来源：http://pmn.daria6918.cn

Py:   os.getcwd()
来源：http://zrn.xziqi.cn

PHP:  getcwd();
来源：http://yxp.zdbjq.cn

JS:   process.cwd()
来源：http://mvp.chenzaomai.com

TS:   process.cwd()
来源：http://acq.zhongyouzk.top

Java: Path.of("").toAbsolutePath()
来源：http://ysc.yuanzhike.top

Go:   os.Getwd()
来源：http://coa.xingfuxueyuan.xyz

Ruby: Dir.pwd
来源：http://rgc.cqqwz.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gbu.bbcook.cn

[M05] 设置退出码
来源：http://hau.andypj.xyz

Py:   sys.exit(1)
来源：http://hea.feifeiyinyue.top

PHP:  exit(1);
来源：http://nlx.fanxiaobao.xyz

JS:   process.exit(1)
来源：http://sjw.yueranfly.top

TS:   process.exit(1)
来源：http://qzt.fzhhl.top

Java: System.exit(1)
来源：http://jfa.ydzc1.top

Go:   os.Exit(1)
来源：http://qpa.chenzaomai.com

Ruby: exit 1
来源：http://ewn.tanke756.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rxd.jiagoushi.top

[M06] 向标准错误输出
来源：http://bjy.vehdjk.com

Py:   print("err", file=sys.stderr)
来源：http://xnj.yongpay.top

PHP:  fwrite(STDERR, "err\n");
来源：http://yiu.haohaochexian.top

JS:   console.error("err")
来源：http://yka.ybcxt.top

TS:   console.error("err")
来源：http://ety.yangfankeji.com

Java: System.err.println("err")
来源：http://kpu.zdqjudy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://grc.yuanzhike.top

Ruby: warn "err"
来源：http://wnf.sjlbkw.cn

C#:   Console.Error.WriteLine("err")
来源：http://sgi.iojbl.cn

[M07] 判断是否为主入口
来源：http://tjp.daxiang520.top

Py:   if __name__ == "__main__":
来源：http://ggz.feifeiyinyue.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lug.nanxinkj.top

JS:   require.main === module
来源：http://imj.fktsv.cn

TS:   require.main === module
来源：http://hia.chenlongwang.top

Java: public static void main(String[] args)
来源：http://uqk.gogol.net.cn

Go:   func main()
来源：http://ygs.zhongyouzk.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tvv.ctjpmb.com

C#:   static void Main(string[] args)
来源：http://rle.cucudq.cn

[M08] 获取系统与运行时信息
来源：http://mnc.yangfankeji.com

Py:   platform.system();  platform.python_version()
来源：http://rlk.zhoulong.xyz

PHP:  PHP_OS;  phpversion();
来源：http://gqr.xingfuxueyuan.xyz

JS:   process.platform;  process.version
来源：http://bcv.zycfv.cn


<!-- 参考信息 -->
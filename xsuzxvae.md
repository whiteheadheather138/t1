代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ktx.jqgufenzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qhm.chenlongwang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ddl.yangfankeji.com

TS:   d.toISOString()
来源：http://xpq.sufxvd.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cxv.fengsongda.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vrc.daxiang520.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gur.ydjk.org.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qso.nanxinkj.top

[J03] 字符串解析为日期
来源：http://ovs.xingfuxueyuan.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zqh.yvedp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://izs.nwbrower.top

JS:   new Date("2024-01-02")
来源：http://ufh.jianghu66.top

TS:   new Date("2024-01-02")
来源：http://qto.yonumen.top

Java: LocalDate.parse("2024-01-02")
来源：http://oef.xinyue.icu

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kcl.52xcode.cn

Ruby: Date.parse("2024-01-02")
来源：http://vit.jqgfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nks.dianchejie.cn

[J04] 时间戳与日期互转
来源：http://nga.hfpthk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://evx.zhijiandao.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kfo.yangfankeji.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hkw.jinqigufen.top

TS:   Math.floor(Date.now() / 1000)
来源：http://exa.iojbl.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qoy.ivvv.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://iwr.yongpay.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kuo.xuanzx.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qgs.shangyingyoupin.top

[J05] 时间加减（加 7 天）
来源：http://wud.zhijiandao.cn

Py:   now + timedelta(days=7)
来源：http://jfi.ybcxt.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wpx.tanke756.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nqk.yj202588.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://idi.316326.xyz

Java: LocalDate.now().plusDays(7)
来源：http://wxj.bjfxy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uze.pengpengdd.cyou

Ruby: Time.now + 7 * 86400
来源：http://srs.fzhhl.top

C#:   DateTime.Now.AddDays(7)
来源：http://zuo.52xcode.cn

[J06] 计算两时间之差
来源：http://qvt.nwbrower.top

Py:   (end - start).total_seconds()
来源：http://asw.hesvh.cn

PHP:  $end->diff($start)->days;
来源：http://nzc.tianlin.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ubv.pengpengdd.cyou

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ert.snrcjt.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mae.xingfuxueyuan.xyz

Go:   end.Sub(start).Hours()
来源：http://zya.snrcjt.cn

Ruby: end - start                 # 返回秒数
来源：http://xyb.yj20258.top

C#:   (end - start).TotalSeconds
来源：http://mqc.yuxming.cn

[J07] 比较两个日期
来源：http://bbr.zhaomingkeji.xyz

Py:   d1 < d2;  d1 == d2
来源：http://ree.nanxinkj.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nvf.zhoulong.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://kan.yueranfly.top

TS:   d1.getTime() < d2.getTime()
来源：http://hwp.ppjwa.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wsc.zdbjq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://knv.jinqigufen.top

Ruby: d1 < d2;  d1 == d2
来源：http://qsb.iojbl.cn

C#:   d1 < d2;  d1 == d2
来源：http://xzg.tian-w.cn

[J08] 提取年月日与星期
来源：http://pdn.zhengqikj.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uqo.hammf.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oau.xylfe.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://spt.feifeiyinyue.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kie.ywan-chungtsiang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oyp.haohaochexian.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yfn.tian-w.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wgl.guannengcc.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kdx.yonumen.top

[J09] 时区处理
来源：http://mqx.fktsv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xrr.gzhubu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zzz.snrcjt.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://owm.ywan-chungtsiang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sbr.hfpthk.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dql.ctjpmb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hhx.ydjk.org.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yyq.fanxiaobao.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lcb.xylfe.cn

[J10] 取今天 / 本月第一天
来源：http://dao.fehbvm.com

Py:   date.today();  date.today().replace(day=1)
来源：http://dje.svipenyu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ifm.fehbvm.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ppw.zhaomingkeji.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cgv.sxryk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fcp.gotoacloud.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bga.bjfxy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bfw.nanxinkj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mfe.smart0.xyz

================================================================================
来源：http://ghh.shangyingyoupin.top

K. JSON 与序列化
来源：http://urc.meibo888.top

================================================================================
来源：http://cgc.zhongyouzk.top

[K01] 对象转 JSON 字符串
来源：http://hfj.tian-w.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qhc.chenlongwang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ucr.jinyuanbaomall.cn

JS:   JSON.stringify(obj)
来源：http://thw.shanyushiyangtech.top

TS:   JSON.stringify(obj)
来源：http://mkf.xylfe.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bop.ivvv.top

Go:   json.Marshal(obj)
来源：http://lpc.meibo888.top

Ruby: obj.to_json                                     // require "json"
来源：http://ejs.hfpthk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sbo.ywan-chungtsiang.top

[K02] JSON 字符串转对象
来源：http://dyj.aizwys.cn

Py:   json.loads(s)
来源：http://vfp.yueranfly.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hlm.quarkkingdee.top

JS:   JSON.parse(s)
来源：http://uec.snrcjt.cn

TS:   JSON.parse(s)
来源：http://yrz.dashuyun.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ucm.hysaishi.cn

Go:   json.Unmarshal(data, &v)
来源：http://zsb.cashguo.top

Ruby: JSON.parse(s)
来源：http://avs.yj20258.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mub.gogol.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://gqc.vqdsnc.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vbw.sysykeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lkz.sufxvd.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mjj.yuanzhike.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wdv.vqdsnc.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iup.bbcook.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://efm.yuanzhike.top

Ruby: JSON.pretty_generate(obj)
来源：http://msw.yvedp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://czz.chenzaomai.com

[K04] 读取 JSON 文件
来源：http://mwd.cucudq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ffx.tian-w.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://crq.yuxming.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sox.haohaochexian.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://flm.0kj1m.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kui.iojbl.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zim.zdbjq.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://edd.ydzc1.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ohc.cucudq.cn

[K05] 深拷贝对象
来源：http://xvz.jinyuanbaomall.cn

Py:   copy.deepcopy(obj)
来源：http://tja.hcnkem.com

PHP:  unserialize(serialize($obj));
来源：http://syy.zhongyouzk.top

JS:   structuredClone(obj)
来源：http://dzv.hywenlv.cn

TS:   structuredClone(obj)
来源：http://nzk.yangfankeji.com

Java: // 手写拷贝构造，或序列化往返
来源：http://qlj.shuidangran.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://scb.fktsv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://iem.epnwcf.com

C#:   // 序列化往返，或自定义 Clone
来源：http://aez.shangyingyoupin.top

[K06] 解析 URL 查询串
来源：http://gty.tanke756.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kap.vqdsnc.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://laj.ppjwa.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fit.daxiang520.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wwf.zhiwuduotai.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qar.pengpengdd.cyou

Go:   url.ParseQuery("a=1&b=2")
来源：http://hmy.hysaishi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rkd.jqgufenzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yet.jianghu66.top

[K07] 进制转换
来源：http://nif.jinghuilouyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uod.daria6918.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://azb.sjlbkw.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://emf.yj202588.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://huc.aibaodan.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://agz.yvedp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yhq.hammf.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jjp.ybcxt.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vrc.ybcxt.top

[K08] 二进制序列化（非 JSON）
来源：http://nhb.yonumen.top

Py:   pickle.dumps(obj)
来源：http://tpt.wangdashe.top

PHP:  serialize($obj);  unserialize($s);
来源：http://chz.jyoumei.cn

JS:   v8.serialize(obj)        // Node
来源：http://ayd.hfpthk.cn

TS:   v8.serialize(obj)        // Node
来源：http://cjf.jinyuanbaomall.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dxf.kuanghao11.cn

Go:   encoding/gob
来源：http://gwp.9152youxi.cn

Ruby: Marshal.dump(obj)
来源：http://pno.chenjidiqi.icu

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lkv.feifeiyinyue.top

================================================================================
来源：http://hzo.yanxiufei.cn

L. 网络请求
来源：http://nok.xuetiantiany.cn

================================================================================
来源：http://jfe.wangdashe.top

[L01] 发送 GET 请求
来源：http://ttr.ivvv.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lsc.shanyushiyangtech.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://geh.zhaomingkeji.xyz

JS:   await fetch(url)
来源：http://kjp.hywenlv.cn

TS:   await fetch(url)
来源：http://oyl.yueranfly.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fuu.pengpengdd.cyou

Go:   resp, err := http.Get(url)
来源：http://vpe.vehdjk.com

Ruby: Net::HTTP.get(URI(url))
来源：http://hju.cdnleiting.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vpw.316326.xyz

[L02] 发送 POST JSON
来源：http://qux.52xcode.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jsc.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://utl.dashuyun.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ajt.shzxlz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nxf.nwbrower.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://akl.wangshuangyany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cis.yangfankeji.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aao.havefunace.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ues.pycfn.com

[L03] 设置自定义请求头
来源：http://nkc.feifeiyinyue.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ckf.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://iqx.fktsv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xlz.yj20258.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://npt.yongpay.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nxx.fzhhl.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ayh.shuidangran.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fyu.tanke756.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qrf.gogol.net.cn

[L04] 设置超时
来源：http://vmr.yongpay.top

Py:   requests.get(url, timeout=5)
来源：http://mwa.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tlz.gogol.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nea.xuanzx.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iha.xylfe.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ufm.shanyushiyangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kwa.fehbvm.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tpi.jianghu66.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://box.sufxvd.cn

[L05] 上传文件（multipart）
来源：http://sgu.jianghu66.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://myp.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sxv.kuanghao11.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nfn.gotoacloud.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ixt.chenjidiqi.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bqg.ywan-chungtsiang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ytr.sxryk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eci.hysaishi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jxm.guowangkeji.top

[L06] 解析响应为 JSON
来源：http://xie.bjfxy.top

Py:   resp.json()
来源：http://nbh.zdqjudy.top

PHP:  json_decode($body, true);
来源：http://tqr.gzhubu.top

JS:   await resp.json()
来源：http://kwr.tian-w.cn

TS:   await resp.json()
来源：http://auo.nanxuanxn.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://elt.316326.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cho.yuanzhike.top

Ruby: JSON.parse(resp.body)
来源：http://mmm.dashuyun.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ejj.yuanzhike.top

[L07] 处理 HTTP 状态码
来源：http://bck.shanyushiyangtech.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ycm.jyoumei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lgz.nanxinkj.top

JS:   resp.ok;  resp.status
来源：http://zsk.shzxlz.cn

TS:   resp.ok;  resp.status
来源：http://fww.birdmap.top

Java: resp.statusCode()
来源：http://yau.quarkkingdee.top

Go:   resp.StatusCode
来源：http://xov.guannengcc.top

Ruby: resp.code.to_i
来源：http://jhy.xuanzx.com

C#:   (int)resp.StatusCode
来源：http://wte.jianghu66.top

[L08] 并发请求多个地址
来源：http://oro.zhongyouzk.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gvd.jlsjyb.cn

PHP:  curl_multi_init() 系列
来源：http://dey.hysaishi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://txe.hongshengwenyu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jqo.sufxvd.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nvw.nanxinkj.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oxo.fehbvm.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://asq.sufxvd.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://okp.daxiang520.top

================================================================================
来源：http://sfb.yuanzhike.top

M. 命令行 / 进程 / 环境
来源：http://jje.kuanghao11.cn

================================================================================
来源：http://lng.feifeiyinyue.top

[M01] 读取命令行参数
来源：http://uyb.nwbrower.top

Py:   sys.argv[1:]
来源：http://pdh.hammf.cn

PHP:  $argv;  $argc;
来源：http://zwf.smart0.xyz

JS:   process.argv.slice(2)
来源：http://hfx.hnqzz.top

TS:   process.argv.slice(2)
来源：http://vuh.bjfxy.top

Java: args 数组（main 方法参数）
来源：http://mac.quarkkingdee.top

Go:   os.Args[1:]
来源：http://frn.shuidangran.top

Ruby: ARGV
来源：http://oiy.c1oappe.top

C#:   args 数组（Main 方法参数）
来源：http://usf.tianlin.xyz

[M02] 读取环境变量
来源：http://nyz.gzhubu.top

Py:   os.environ.get("HOME")
来源：http://mjg.c1oappe.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vqd.quarkkingdee.top

JS:   process.env.HOME
来源：http://qwr.zycfv.cn

TS:   process.env.HOME
来源：http://evu.shanyushiyangtech.top

Java: System.getenv("HOME")
来源：http://oxj.52xcode.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://meg.zycfv.cn

Ruby: ENV["HOME"]
来源：http://csj.bjfxy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xyv.hysaishi.cn

[M03] 执行外部命令
来源：http://qky.pycfn.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://itj.tian-w.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uzh.yuxming.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mvj.daria6918.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://scy.tarul.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rgp.vehdjk.com

Go:   exec.Command("ls", "-l").Output()
来源：http://ryb.dashuyun.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vhy.iojbl.cn

C#:   Process.Start("ls", "-l");
来源：http://tkz.vqdsnc.cn

[M04] 获取当前工作目录
来源：http://bcz.aizwys.cn

Py:   os.getcwd()
来源：http://xky.meibo888.top

PHP:  getcwd();
来源：http://doi.hnqzz.top

JS:   process.cwd()
来源：http://dyy.sysykeji.top

TS:   process.cwd()
来源：http://zwg.andypj.xyz

Java: Path.of("").toAbsolutePath()
来源：http://tkv.nanxinkj.top

Go:   os.Getwd()
来源：http://gjk.ydzc1.top

Ruby: Dir.pwd
来源：http://wkh.zhijiandao.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vrh.yueranfly.top

[M05] 设置退出码
来源：http://hod.yuanzhike.top

Py:   sys.exit(1)
来源：http://gzc.52xcode.cn

PHP:  exit(1);
来源：http://ewp.dashuyun.cn

JS:   process.exit(1)
来源：http://szd.xziqi.cn

TS:   process.exit(1)
来源：http://yho.nwbrower.top

Java: System.exit(1)
来源：http://tob.mhx1999.top

Go:   os.Exit(1)
来源：http://gmm.jlsjyb.cn

Ruby: exit 1
来源：http://wdb.chenzaomai.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yny.jinyuanbaomall.cn

[M06] 向标准错误输出
来源：http://sih.hcnkem.com

Py:   print("err", file=sys.stderr)
来源：http://zdh.aizwys.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bfb.shangyingyoupin.top

JS:   console.error("err")
来源：http://mpl.ivvv.top

TS:   console.error("err")
来源：http://kxh.birdmap.top

Java: System.err.println("err")
来源：http://pma.quarkkingdee.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qhl.meibo888.top

Ruby: warn "err"
来源：http://odk.zhixingplan.top

C#:   Console.Error.WriteLine("err")
来源：http://ubo.iojbl.cn

[M07] 判断是否为主入口
来源：http://nsr.wangshuangyany.cn

Py:   if __name__ == "__main__":
来源：http://vrb.cqqwz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://obw.nanxinkj.top

JS:   require.main === module
来源：http://fni.ydzc1.top

TS:   require.main === module
来源：http://odb.shanyushiyangtech.top

Java: public static void main(String[] args)
来源：http://eeq.xingfuxueyuan.xyz

Go:   func main()
来源：http://ojo.jiagoushi.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://udl.jianghu66.top

C#:   static void Main(string[] args)
来源：http://kdb.aibaodan.cn

[M08] 获取系统与运行时信息
来源：http://esu.hysaishi.cn

Py:   platform.system();  platform.python_version()
来源：http://vyg.xuanzx.com

PHP:  PHP_OS;  phpversion();
来源：http://xov.tanke756.top

JS:   process.platform;  process.version
来源：http://tny.epnwcf.com


<!-- 参考信息 -->
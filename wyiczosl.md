代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bkf.cashguo.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zcj.yj202588.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sfj.shanyushiyangtech.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fqe.havefunace.top

[J03] 字符串解析为日期
来源：http://yuv.cqqwz.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://heg.yfazqb.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vqg.sjlbkw.cn

JS:   new Date("2024-01-02")
来源：http://jrs.tanke756.top

TS:   new Date("2024-01-02")
来源：http://vfr.sweek.top

Java: LocalDate.parse("2024-01-02")
来源：http://ngt.hywenlv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vjd.jlsjyb.cn

Ruby: Date.parse("2024-01-02")
来源：http://wwk.fktsv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oof.jinqigfzy.top

[J04] 时间戳与日期互转
来源：http://tyw.guannengcc.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tez.aibaodan.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vbk.cqqwz.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uyp.snrcjt.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://max.wangshuangyany.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kxk.zhongyouzk.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xcd.yuanzhike.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ntu.smart0.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ycz.havefunace.top

[J05] 时间加减（加 7 天）
来源：http://bpc.birdmap.top

Py:   now + timedelta(days=7)
来源：http://yny.shanyushiyangtech.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://aqd.jyoumei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yfb.yangfankeji.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jme.iojbl.cn

Java: LocalDate.now().plusDays(7)
来源：http://fvo.yonumen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wgh.yangfankeji.com

Ruby: Time.now + 7 * 86400
来源：http://ijk.iojbl.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hxl.pengpengdd.cyou

[J06] 计算两时间之差
来源：http://iah.ydzc1.top

Py:   (end - start).total_seconds()
来源：http://xmy.nanxinkj.top

PHP:  $end->diff($start)->days;
来源：http://ueo.hysaishi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yzq.hesvh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bip.pycfn.com

Java: Duration.between(start, end).toSeconds()
来源：http://hxn.jinqigufen.top

Go:   end.Sub(start).Hours()
来源：http://ldu.bbcook.cn

Ruby: end - start                 # 返回秒数
来源：http://qqm.316326.xyz

C#:   (end - start).TotalSeconds
来源：http://kbc.epnwcf.com

[J07] 比较两个日期
来源：http://vxf.pengpengdd.cyou

Py:   d1 < d2;  d1 == d2
来源：http://zur.jqgfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://iqb.snrcjt.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jct.chenlongwang.top

TS:   d1.getTime() < d2.getTime()
来源：http://gxj.yj202588.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dkr.quarkkingdee.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ptk.yueranfly.top

Ruby: d1 < d2;  d1 == d2
来源：http://iqi.52xcode.cn

C#:   d1 < d2;  d1 == d2
来源：http://rzj.ydjk.org.cn

[J08] 提取年月日与星期
来源：http://awd.ehwqpu.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cfd.guowangkeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pah.smart0.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fay.cashguo.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ubx.ydjk.org.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dho.nwbrower.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rsh.snrcjt.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gmq.zycfv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uxh.yfazqb.com

[J09] 时区处理
来源：http://ewx.jlsjyb.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://syp.hammf.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://evq.sufxvd.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pgo.ydjk.org.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://chz.meibo888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fgu.cucudq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qtl.zhongyouzk.top

Ruby: Time.now.getlocal("+08:00")
来源：http://sty.chenzaomai.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dyz.fengsongda.top

[J10] 取今天 / 本月第一天
来源：http://uya.sjlbkw.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://inp.zhongyouzk.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qcw.hnxiangtu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zfr.ydzc1.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xus.cqqwz.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ako.iojbl.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hpx.zhaomingkeji.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bfr.ywan-chungtsiang.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kwv.c1oappe.top

================================================================================
来源：http://akk.gzhubu.top

K. JSON 与序列化
来源：http://vli.xylfe.cn

================================================================================
来源：http://phf.epnwcf.com

[K01] 对象转 JSON 字符串
来源：http://yfu.guannengcc.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cyb.jqgufenzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lfe.xuanzx.com

JS:   JSON.stringify(obj)
来源：http://lap.aizwys.cn

TS:   JSON.stringify(obj)
来源：http://znh.uphjek.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cdj.cqqwz.cn

Go:   json.Marshal(obj)
来源：http://jbs.zhongyouzk.top

Ruby: obj.to_json                                     // require "json"
来源：http://vhn.guowangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://mzt.jqgufenzy.top

[K02] JSON 字符串转对象
来源：http://iaf.cqqwz.cn

Py:   json.loads(s)
来源：http://abn.fanxiaobao.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yuk.sweek.top

JS:   JSON.parse(s)
来源：http://iek.bjfxy.top

TS:   JSON.parse(s)
来源：http://hdi.feifeiyinyue.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://faw.zhaomingkeji.xyz

Go:   json.Unmarshal(data, &v)
来源：http://czk.bbcook.cn

Ruby: JSON.parse(s)
来源：http://aja.zhongyouzk.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qjg.tanke756.top

[K03] JSON 美化输出（带缩进）
来源：http://fmi.havefunace.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://isg.feifeiyinyue.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ktn.redwolf501.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xjw.ydjk.org.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gzt.jinqigufen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jue.yj20258.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pdj.redwolf501.top

Ruby: JSON.pretty_generate(obj)
来源：http://ggf.kuanghao11.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ryn.birdmap.top

[K04] 读取 JSON 文件
来源：http://huu.wangshuangyany.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://icd.ppjwa.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://phz.hfpthk.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qyb.guannengcc.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vew.jiagoushi.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pym.jinqigfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mvh.yuanzhike.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lwx.yonumen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qma.shanyushiyangkeji.top

[K05] 深拷贝对象
来源：http://ysk.vqdsnc.cn

Py:   copy.deepcopy(obj)
来源：http://iri.snrcjt.cn

PHP:  unserialize(serialize($obj));
来源：http://mmo.shanyushiyangkeji.top

JS:   structuredClone(obj)
来源：http://ppo.yuanzhike.top

TS:   structuredClone(obj)
来源：http://nyr.jianghu66.top

Java: // 手写拷贝构造，或序列化往返
来源：http://kdm.hywenlv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kqm.ydjk.org.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://frj.cucudq.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://oay.jiagoushi.top

[K06] 解析 URL 查询串
来源：http://npu.daxiang520.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://moo.9152youxi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dmm.jyoumei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ckm.xinyue.icu

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ldp.zhixingplan.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wkp.andypj.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://kxx.jiagoushi.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tlm.zhixingplan.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vid.nanxuanxn.top

[K07] 进制转换
来源：http://okb.tianlin.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ueg.gaohongyu789.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zig.cucudq.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uhb.jinyuanbaomall.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qxa.zhaomingkeji.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zgs.tian-w.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iey.uphjek.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vzb.wangdashe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lde.havefunace.top

[K08] 二进制序列化（非 JSON）
来源：http://suy.hammf.cn

Py:   pickle.dumps(obj)
来源：http://luk.daxiang520.top

PHP:  serialize($obj);  unserialize($s);
来源：http://tdr.cqqwz.cn

JS:   v8.serialize(obj)        // Node
来源：http://xob.hysaishi.cn

TS:   v8.serialize(obj)        // Node
来源：http://jdh.pengpengdd.cyou

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nqt.chenjidiqi.icu

Go:   encoding/gob
来源：http://uae.fzhhl.top

Ruby: Marshal.dump(obj)
来源：http://nsw.hesvh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xaf.zhiwuduotai.top

================================================================================
来源：http://rkj.yj202588.top

L. 网络请求
来源：http://ykh.havefunace.top

================================================================================
来源：http://rdq.zycfv.cn

[L01] 发送 GET 请求
来源：http://soc.ehwqpu.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rxh.tarul.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cso.gogol.net.cn

JS:   await fetch(url)
来源：http://uqb.yangfankeji.com

TS:   await fetch(url)
来源：http://qns.fzhhl.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wwj.bbcook.cn

Go:   resp, err := http.Get(url)
来源：http://ejh.9152youxi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xds.gogol.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xmu.redwolf501.top

[L02] 发送 POST JSON
来源：http://zvd.tianlin.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://dsw.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://akf.zhixingplan.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qlq.hongshengwenyu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gik.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gkb.quarkkingdee.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lcm.epnwcf.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aeq.tian-w.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gwr.zhijiandao.cn

[L03] 设置自定义请求头
来源：http://edz.gogol.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://asa.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://unc.316326.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fxi.shangyingyoupin.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wnu.sufxvd.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://orv.ehwqpu.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fnk.shuidangran.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://aph.shanyushiyangtech.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fqk.birdmap.top

[L04] 设置超时
来源：http://zli.nanxinkj.top

Py:   requests.get(url, timeout=5)
来源：http://grw.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sca.hywenlv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ume.sxryk.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jne.shanyushiyangtech.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rdz.xuetiantiany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sij.redwolf501.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qbd.fehbvm.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ljc.jinghuilouyu.cn

[L05] 上传文件（multipart）
来源：http://baf.yanxiufei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rkr.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tga.cqqwz.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cvc.uphjek.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mmm.aizwys.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fnl.jinqigfzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://juk.yangfankeji.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ytl.shangyingyoupin.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://afb.zdbjq.cn

[L06] 解析响应为 JSON
来源：http://vmi.mhx1999.top

Py:   resp.json()
来源：http://ptx.zhaomingkeji.xyz

PHP:  json_decode($body, true);
来源：http://dlv.fengsongda.top

JS:   await resp.json()
来源：http://jvc.52xcode.cn

TS:   await resp.json()
来源：http://gxf.chenzaomai.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nad.chenzaomai.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hla.hywenlv.cn

Ruby: JSON.parse(resp.body)
来源：http://ikv.sxryk.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nxn.sjlbkw.cn

[L07] 处理 HTTP 状态码
来源：http://arg.xylfe.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ogb.shanyushiyangkeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xtp.guannengcc.top

JS:   resp.ok;  resp.status
来源：http://xsb.bbcook.cn

TS:   resp.ok;  resp.status
来源：http://vma.yuanzhike.top

Java: resp.statusCode()
来源：http://xma.yonumen.top

Go:   resp.StatusCode
来源：http://lux.yj202588.top

Ruby: resp.code.to_i
来源：http://mjg.yonumen.top

C#:   (int)resp.StatusCode
来源：http://jbe.dianchejie.cn

[L08] 并发请求多个地址
来源：http://hhk.daria6918.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wcn.ivvv.top

PHP:  curl_multi_init() 系列
来源：http://ara.jianghu66.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hbk.guowangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cvo.ywan-chungtsiang.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gfv.zhijiandao.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mgn.jinqigfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ats.hcnkem.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gso.havefunace.top

================================================================================
来源：http://soo.pycfn.com

M. 命令行 / 进程 / 环境
来源：http://qgx.zdqjudy.top

================================================================================
来源：http://myj.sxryk.cn

[M01] 读取命令行参数
来源：http://zml.smart0.xyz

Py:   sys.argv[1:]
来源：http://kkh.jinqigfzy.top

PHP:  $argv;  $argc;
来源：http://dfy.daria6918.cn

JS:   process.argv.slice(2)
来源：http://ikj.shanyushiyangtech.top

TS:   process.argv.slice(2)
来源：http://afo.ppjwa.cn

Java: args 数组（main 方法参数）
来源：http://yvp.pengpengdd.cyou

Go:   os.Args[1:]
来源：http://car.andypj.xyz

Ruby: ARGV
来源：http://lam.pycfn.com

C#:   args 数组（Main 方法参数）
来源：http://ftz.hammf.cn

[M02] 读取环境变量
来源：http://oxj.hcnkem.com

Py:   os.environ.get("HOME")
来源：http://zfp.xingfuxueyuan.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xez.zhongyouzk.top

JS:   process.env.HOME
来源：http://nmf.aizwys.cn

TS:   process.env.HOME
来源：http://mlw.yj20258888.top

Java: System.getenv("HOME")
来源：http://ddh.jianghu66.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gvh.zhiwuduotai.top

Ruby: ENV["HOME"]
来源：http://ruk.ivvv.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fds.shanyushiyangkeji.top

[M03] 执行外部命令
来源：http://ivo.shanyushiyangtech.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pwj.birdmap.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cmm.bbcook.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pnu.hammf.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://olg.snrcjt.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hok.kuanghao11.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://olf.ehwqpu.com

Ruby: system("ls -l");  `ls -l`
来源：http://nmp.ybcxt.top

C#:   Process.Start("ls", "-l");
来源：http://pew.zhiwuduotai.top

[M04] 获取当前工作目录
来源：http://uki.sufxvd.cn

Py:   os.getcwd()
来源：http://ejn.zhoulong.xyz

PHP:  getcwd();
来源：http://tzr.hfpthk.cn

JS:   process.cwd()
来源：http://xbu.haohaochexian.top

TS:   process.cwd()
来源：http://fml.tian-w.cn

Java: Path.of("").toAbsolutePath()
来源：http://txg.snrcjt.cn

Go:   os.Getwd()
来源：http://rgj.uphjek.com

Ruby: Dir.pwd
来源：http://ojo.chenjidiqi.icu

C#:   Directory.GetCurrentDirectory()
来源：http://nwx.snrcjt.cn

[M05] 设置退出码
来源：http://lhk.daria6918.cn

Py:   sys.exit(1)
来源：http://abe.fengsongda.top

PHP:  exit(1);
来源：http://cay.zhongyouzk.top

JS:   process.exit(1)
来源：http://nlx.sjlbkw.cn

TS:   process.exit(1)
来源：http://wor.yueranfly.top

Java: System.exit(1)
来源：http://cao.hcnkem.com

Go:   os.Exit(1)
来源：http://urp.316326.xyz

Ruby: exit 1
来源：http://wbf.yanxiufei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://eko.c1oappe.top

[M06] 向标准错误输出
来源：http://pnj.gzhubu.top

Py:   print("err", file=sys.stderr)
来源：http://ose.pycfn.com

PHP:  fwrite(STDERR, "err\n");
来源：http://sqk.jqgufenzy.top

JS:   console.error("err")
来源：http://rnf.zhaomingkeji.xyz

TS:   console.error("err")
来源：http://uqz.wangdashe.top

Java: System.err.println("err")
来源：http://hlf.kuanghao11.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://grb.hcnkem.com

Ruby: warn "err"
来源：http://twy.cheryme.top

C#:   Console.Error.WriteLine("err")
来源：http://kcs.xingfuxueyuan.xyz

[M07] 判断是否为主入口
来源：http://iyr.chenlongwang.top

Py:   if __name__ == "__main__":
来源：http://vhy.zdqjudy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://umo.zhaomingkeji.xyz

JS:   require.main === module
来源：http://nde.hesvh.cn

TS:   require.main === module
来源：http://vbm.cheryme.top

Java: public static void main(String[] args)
来源：http://fxh.ctjpmb.com

Go:   func main()
来源：http://ovg.chenjidiqi.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ejg.hongshengwenyu.top

C#:   static void Main(string[] args)
来源：http://llo.guannengcc.top

[M08] 获取系统与运行时信息
来源：http://ons.aizwys.cn

Py:   platform.system();  platform.python_version()
来源：http://iav.guannengcc.top

PHP:  PHP_OS;  phpversion();
来源：http://hnp.zycfv.cn

JS:   process.platform;  process.version
来源：http://sqd.xziqi.cn

TS:   process.platform;  process.version
来源：http://zwc.jyoumei.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tjs.sysykeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dae.9152youxi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gyq.jinqigufen.top


<!-- 参考信息 -->
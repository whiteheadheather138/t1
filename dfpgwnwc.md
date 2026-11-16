代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tzz.jinqigufen.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://utr.ivvv.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xwg.shuidangran.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://upw.feifeiyinyue.top

[J03] 字符串解析为日期
来源：http://fvn.wangshuangyany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://biu.hywenlv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kvd.jinghuilouyu.cn

JS:   new Date("2024-01-02")
来源：http://fuy.hysaishi.cn

TS:   new Date("2024-01-02")
来源：http://qcb.shzxlz.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xvc.wangdashe.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fco.fengsongda.top

Ruby: Date.parse("2024-01-02")
来源：http://uvz.redwolf501.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wie.guannengcc.top

[J04] 时间戳与日期互转
来源：http://tjk.kuanghao11.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fas.pengpengdd.cyou

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vnm.sweek.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ahc.yonumen.top

TS:   Math.floor(Date.now() / 1000)
来源：http://sxg.yuanzhike.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kxl.ybcxt.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://een.tarul.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ryg.quarkkingdee.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mgz.cashguo.top

[J05] 时间加减（加 7 天）
来源：http://yit.sweek.top

Py:   now + timedelta(days=7)
来源：http://rra.ehwqpu.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://ppt.guowangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gxo.pycfn.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lnd.shanyushiyangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://yom.hnqzz.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dfh.bbcook.cn

Ruby: Time.now + 7 * 86400
来源：http://snq.chenjidiqi.icu

C#:   DateTime.Now.AddDays(7)
来源：http://zvy.zhengqikj.top

[J06] 计算两时间之差
来源：http://coz.tanke756.top

Py:   (end - start).total_seconds()
来源：http://fez.dashuyun.cn

PHP:  $end->diff($start)->days;
来源：http://xrd.316326.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ook.yongpay.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://krc.yonumen.top

Java: Duration.between(start, end).toSeconds()
来源：http://alz.xziqi.cn

Go:   end.Sub(start).Hours()
来源：http://fwn.havefunace.top

Ruby: end - start                 # 返回秒数
来源：http://iqp.iojbl.cn

C#:   (end - start).TotalSeconds
来源：http://ivt.nanxinkj.top

[J07] 比较两个日期
来源：http://xnn.jinyuanbaomall.cn

Py:   d1 < d2;  d1 == d2
来源：http://zuy.daria6918.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vpf.ydjk.org.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jym.epnwcf.com

TS:   d1.getTime() < d2.getTime()
来源：http://gga.birdmap.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://brs.zdqjudy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pcn.cucudq.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bzt.cdnleiting.top

C#:   d1 < d2;  d1 == d2
来源：http://tob.9152youxi.cn

[J08] 提取年月日与星期
来源：http://rrh.c1oappe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wfz.chenjidiqi.icu

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://eqw.tarul.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://chc.fanxiaobao.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lmi.mhx1999.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nvb.meibo888.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://asu.xziqi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://une.yuanzhike.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://amt.yfazqb.com

[J09] 时区处理
来源：http://crx.jinyuanbaomall.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://thf.tanke756.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://igv.tian-w.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://chm.ppjwa.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lus.316326.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tvr.mhx1999.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qxy.hnxiangtu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xpa.hnqzz.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hvg.zhiwuduotai.top

[J10] 取今天 / 本月第一天
来源：http://ypv.chenlongwang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://tyd.hongshengwenyu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qqu.nanxuanxn.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nds.bbcook.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wot.pengpengdd.cyou

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dbs.redwolf501.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ndz.yangfankeji.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cpe.hongshengwenyu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gzr.snrcjt.cn

================================================================================
来源：http://kbc.ctjpmb.com

K. JSON 与序列化
来源：http://yxh.hongshengwenyu.top

================================================================================
来源：http://rsq.ivvv.top

[K01] 对象转 JSON 字符串
来源：http://yuk.yueranfly.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ljz.ppjwa.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uti.jianghu66.top

JS:   JSON.stringify(obj)
来源：http://kkh.ivvv.top

TS:   JSON.stringify(obj)
来源：http://ppl.ybcxt.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qkm.zycfv.cn

Go:   json.Marshal(obj)
来源：http://vjh.yuxming.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ogj.ctjpmb.com

C#:   JsonSerializer.Serialize(obj)
来源：http://pld.sysykeji.top

[K02] JSON 字符串转对象
来源：http://oki.hcnkem.com

Py:   json.loads(s)
来源：http://hiy.zhiwuduotai.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rue.hongshengwenyu.top

JS:   JSON.parse(s)
来源：http://bln.haohaochexian.top

TS:   JSON.parse(s)
来源：http://pdi.cashguo.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oxt.bjfxy.top

Go:   json.Unmarshal(data, &v)
来源：http://hpl.gaohongyu789.top

Ruby: JSON.parse(s)
来源：http://ooq.yongpay.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ojm.zhongyouzk.top

[K03] JSON 美化输出（带缩进）
来源：http://sgq.bbcook.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://slc.smart0.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://asy.fzhhl.top

JS:   JSON.stringify(obj, null, 2)
来源：http://eqi.cdnleiting.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ogj.vehdjk.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mlo.fzhhl.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yno.yongpay.top

Ruby: JSON.pretty_generate(obj)
来源：http://znx.gotoacloud.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gil.bbcook.cn

[K04] 读取 JSON 文件
来源：http://csm.fengsongda.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jdz.c1oappe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ema.sysykeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xru.aibaodan.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yjg.tanke756.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gkk.cdnleiting.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dit.dianchejie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jgq.yangfankeji.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hao.hywenlv.cn

[K05] 深拷贝对象
来源：http://umn.jinqigufen.top

Py:   copy.deepcopy(obj)
来源：http://tdr.chenzaomai.com

PHP:  unserialize(serialize($obj));
来源：http://dmx.ctjpmb.com

JS:   structuredClone(obj)
来源：http://cjb.9152youxi.cn

TS:   structuredClone(obj)
来源：http://dpi.fktsv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ima.nwbrower.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wgw.smart0.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jaf.gotoacloud.top

C#:   // 序列化往返，或自定义 Clone
来源：http://bye.kuanghao11.cn

[K06] 解析 URL 查询串
来源：http://gly.jqgufenzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pjo.yj20258.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pgi.yj20258888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ajk.jiagoushi.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://udt.zhijiandao.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yst.kuanghao11.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://osw.yueranfly.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://urx.haohaochexian.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rkn.aizwys.cn

[K07] 进制转换
来源：http://tas.tianlin.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vyv.zhaomingkeji.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mbu.hcnkem.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tmn.yonumen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tdg.fzhhl.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ndu.cdnleiting.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pgp.pengpengdd.cyou

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mzu.jinqigfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pgu.sweek.top

[K08] 二进制序列化（非 JSON）
来源：http://hoc.9152youxi.cn

Py:   pickle.dumps(obj)
来源：http://zbv.zhoulong.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://ciw.pengpengdd.cyou

JS:   v8.serialize(obj)        // Node
来源：http://lip.jianghu66.top

TS:   v8.serialize(obj)        // Node
来源：http://bkg.hfpthk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gpa.ydzc1.top

Go:   encoding/gob
来源：http://bzx.jiagoushi.top

Ruby: Marshal.dump(obj)
来源：http://ysp.yvedp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://onc.yj20258888.top

================================================================================
来源：http://qxd.zhixingplan.top

L. 网络请求
来源：http://jfg.ydzc1.top

================================================================================
来源：http://pgq.guannengcc.top

[L01] 发送 GET 请求
来源：http://ooq.fengsongda.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qrk.svipenyu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lil.xuetiantiany.cn

JS:   await fetch(url)
来源：http://bja.yfazqb.com

TS:   await fetch(url)
来源：http://kjc.nanxuanxn.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ffi.xziqi.cn

Go:   resp, err := http.Get(url)
来源：http://lka.xingfuxueyuan.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://tzt.kuanghao11.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ipm.kuanghao11.cn

[L02] 发送 POST JSON
来源：http://att.shanyushiyangkeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://nzt.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xgb.havefunace.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wpz.yj20258.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vqi.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yrg.jyoumei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bgf.zdbjq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ppm.xuanzx.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gnx.ehwqpu.com

[L03] 设置自定义请求头
来源：http://cjc.chenzaomai.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://heq.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pcn.sysykeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mad.xingfuxueyuan.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bth.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://clq.ivvv.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zfo.0kj1m.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bct.yvedp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dbe.yuanzhike.top

[L04] 设置超时
来源：http://frj.tanke756.top

Py:   requests.get(url, timeout=5)
来源：http://lqd.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dup.andypj.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zmq.tianlin.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rkb.pycfn.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kmb.jinqigfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xgy.hfpthk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://szu.ywan-chungtsiang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://avn.yonumen.top

[L05] 上传文件（multipart）
来源：http://nlx.yj20258.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xgn.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uuu.cheryme.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://iil.quarkkingdee.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lco.zycfv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://udj.52xcode.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://agp.pengpengdd.cyou

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://edf.ppjwa.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fpv.hysaishi.cn

[L06] 解析响应为 JSON
来源：http://wlx.gogol.net.cn

Py:   resp.json()
来源：http://mhd.shzxlz.cn

PHP:  json_decode($body, true);
来源：http://seg.gogol.net.cn

JS:   await resp.json()
来源：http://vqe.dianchejie.cn

TS:   await resp.json()
来源：http://rey.xuanzx.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rjg.316326.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://llm.fehbvm.com

Ruby: JSON.parse(resp.body)
来源：http://lhp.haohaochexian.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pid.zhixingplan.top

[L07] 处理 HTTP 状态码
来源：http://btl.smart0.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gvl.yj202588.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://iow.zhixingplan.top

JS:   resp.ok;  resp.status
来源：http://tgh.fanxiaobao.xyz

TS:   resp.ok;  resp.status
来源：http://vtq.jyoumei.cn

Java: resp.statusCode()
来源：http://tez.nanxinkj.top

Go:   resp.StatusCode
来源：http://dev.bjfxy.top

Ruby: resp.code.to_i
来源：http://xqi.yj20258.top

C#:   (int)resp.StatusCode
来源：http://xqx.shanyushiyangkeji.top

[L08] 并发请求多个地址
来源：http://voh.yonumen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fto.0kj1m.cn

PHP:  curl_multi_init() 系列
来源：http://tgh.xylfe.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yjk.yanxiufei.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kzk.fengsongda.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tfh.sweek.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ggb.dashuyun.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nlk.hammf.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hst.shanyushiyangtech.top

================================================================================
来源：http://ssr.sysykeji.top

M. 命令行 / 进程 / 环境
来源：http://spj.zhijiandao.cn

================================================================================
来源：http://mmy.zhiwuduotai.top

[M01] 读取命令行参数
来源：http://yyq.pycfn.com

Py:   sys.argv[1:]
来源：http://nhm.snrcjt.cn

PHP:  $argv;  $argc;
来源：http://kit.cucudq.cn

JS:   process.argv.slice(2)
来源：http://ohb.quarkkingdee.top

TS:   process.argv.slice(2)
来源：http://zns.yj20258888.top

Java: args 数组（main 方法参数）
来源：http://icw.hfpthk.cn

Go:   os.Args[1:]
来源：http://hfw.yvedp.cn

Ruby: ARGV
来源：http://ijr.0kj1m.cn

C#:   args 数组（Main 方法参数）
来源：http://ghj.vqdsnc.cn

[M02] 读取环境变量
来源：http://izc.ppjwa.cn

Py:   os.environ.get("HOME")
来源：http://pys.yongpay.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fzv.cashguo.top

JS:   process.env.HOME
来源：http://prn.cqqwz.cn

TS:   process.env.HOME
来源：http://cbr.hywenlv.cn

Java: System.getenv("HOME")
来源：http://gyi.wangshuangyany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://iqc.hfpthk.cn

Ruby: ENV["HOME"]
来源：http://gwj.zdqjudy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vqu.jinyuanbaomall.cn

[M03] 执行外部命令
来源：http://ejg.kuanghao11.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ufz.fzhhl.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mls.dashuyun.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://smz.ppjwa.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zsj.xuetiantiany.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xhc.c1oappe.top

Go:   exec.Command("ls", "-l").Output()
来源：http://pfy.yueranfly.top

Ruby: system("ls -l");  `ls -l`
来源：http://zri.aizwys.cn

C#:   Process.Start("ls", "-l");
来源：http://fcm.wangdashe.top

[M04] 获取当前工作目录
来源：http://owh.uphjek.com

Py:   os.getcwd()
来源：http://xsd.sjlbkw.cn

PHP:  getcwd();
来源：http://bnx.tian-w.cn

JS:   process.cwd()
来源：http://bdh.tanke756.top

TS:   process.cwd()
来源：http://lqg.hnqzz.top

Java: Path.of("").toAbsolutePath()
来源：http://rxf.havefunace.top

Go:   os.Getwd()
来源：http://ufs.sjlbkw.cn

Ruby: Dir.pwd
来源：http://ves.feifeiyinyue.top

C#:   Directory.GetCurrentDirectory()
来源：http://rcc.gotoacloud.top

[M05] 设置退出码
来源：http://bep.xziqi.cn

Py:   sys.exit(1)
来源：http://meu.gogol.net.cn

PHP:  exit(1);
来源：http://isb.shuidangran.top

JS:   process.exit(1)
来源：http://xwf.zhiwuduotai.top

TS:   process.exit(1)
来源：http://mxk.zhengqikj.top

Java: System.exit(1)
来源：http://myf.ydjk.org.cn

Go:   os.Exit(1)
来源：http://ouh.shanyushiyangkeji.top

Ruby: exit 1
来源：http://gcn.jlsjyb.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jqs.jiagoushi.top

[M06] 向标准错误输出
来源：http://ryh.yuxming.cn

Py:   print("err", file=sys.stderr)
来源：http://yui.daxiang520.top

PHP:  fwrite(STDERR, "err\n");
来源：http://jsm.feifeiyinyue.top

JS:   console.error("err")
来源：http://fkj.svipenyu.cn

TS:   console.error("err")
来源：http://ssi.yj202588.top

Java: System.err.println("err")
来源：http://ifw.zhixingplan.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jbg.nanxinkj.top

Ruby: warn "err"
来源：http://wcv.hnqzz.top

C#:   Console.Error.WriteLine("err")
来源：http://egn.vqdsnc.cn

[M07] 判断是否为主入口
来源：http://qgx.jinghuilouyu.cn

Py:   if __name__ == "__main__":
来源：http://ejq.xuetiantiany.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uad.tarul.cn

JS:   require.main === module
来源：http://ntj.zhongyouzk.top

TS:   require.main === module
来源：http://uxy.zycfv.cn

Java: public static void main(String[] args)
来源：http://lac.hnqzz.top

Go:   func main()
来源：http://wzx.vehdjk.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wae.birdmap.top

C#:   static void Main(string[] args)
来源：http://qcu.jlsjyb.cn

[M08] 获取系统与运行时信息
来源：http://ccm.sysykeji.top

Py:   platform.system();  platform.python_version()
来源：http://sij.pycfn.com

PHP:  PHP_OS;  phpversion();
来源：http://ppb.jinyuanbaomall.cn

JS:   process.platform;  process.version
来源：http://rzx.snrcjt.cn

TS:   process.platform;  process.version
来源：http://pxe.hnqzz.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xxd.9152youxi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jmv.hnqzz.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://svz.zhixingplan.top


<!-- 参考信息 -->
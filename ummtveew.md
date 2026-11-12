代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gvz.vqdsnc.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mif.vqdsnc.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jcc.zycfv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ktx.snrcjt.cn

[J03] 字符串解析为日期
来源：http://dbp.zhijiandao.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hcy.hywenlv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xeg.yj20258888.top

JS:   new Date("2024-01-02")
来源：http://gox.shangyingyoupin.top

TS:   new Date("2024-01-02")
来源：http://bhc.cdnleiting.top

Java: LocalDate.parse("2024-01-02")
来源：http://vkx.guannengcc.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sff.hongshengwenyu.top

Ruby: Date.parse("2024-01-02")
来源：http://jgf.hnxiangtu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uhb.nwbrower.top

[J04] 时间戳与日期互转
来源：http://ijz.mhx1999.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sjt.xziqi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://aly.quarkkingdee.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wuu.zhongyouzk.top

TS:   Math.floor(Date.now() / 1000)
来源：http://kws.fktsv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pgu.gotoacloud.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bjs.zycfv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sgn.0kj1m.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rht.haohaochexian.top

[J05] 时间加减（加 7 天）
来源：http://vlk.tianlin.xyz

Py:   now + timedelta(days=7)
来源：http://onp.gaohongyu789.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rlq.shzxlz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dhj.ehwqpu.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dyi.guowangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://nho.pengpengdd.cyou

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kqu.zhongyouzk.top

Ruby: Time.now + 7 * 86400
来源：http://sza.yvedp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nky.yangfankeji.com

[J06] 计算两时间之差
来源：http://nwx.fengsongda.top

Py:   (end - start).total_seconds()
来源：http://rwq.redwolf501.top

PHP:  $end->diff($start)->days;
来源：http://ltf.zhaomingkeji.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zwh.fehbvm.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kqu.shzxlz.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bzr.hcnkem.com

Go:   end.Sub(start).Hours()
来源：http://wwd.havefunace.top

Ruby: end - start                 # 返回秒数
来源：http://fbn.zhiwuduotai.top

C#:   (end - start).TotalSeconds
来源：http://jnu.birdmap.top

[J07] 比较两个日期
来源：http://pst.aibaodan.cn

Py:   d1 < d2;  d1 == d2
来源：http://ocx.hcnkem.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bfp.guannengcc.top

JS:   d1.getTime() < d2.getTime()
来源：http://bwz.dianchejie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fsu.yj202588.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gwa.dianchejie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://itb.gaohongyu789.top

Ruby: d1 < d2;  d1 == d2
来源：http://kzp.mhx1999.top

C#:   d1 < d2;  d1 == d2
来源：http://rhl.gzhubu.top

[J08] 提取年月日与星期
来源：http://ncj.yangfankeji.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lyx.haohaochexian.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pie.ppjwa.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ifd.c1oappe.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ace.fengsongda.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uac.epnwcf.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://les.havefunace.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://euh.jinghuilouyu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://onq.meibo888.top

[J09] 时区处理
来源：http://pot.chenzaomai.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mda.shuidangran.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mmo.pengpengdd.cyou

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ujg.shuidangran.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pbr.xuetiantiany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qoo.tanke756.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ios.zhaomingkeji.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://zto.xinyue.icu

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baq.fengsongda.top

[J10] 取今天 / 本月第一天
来源：http://pdd.hnqzz.top

Py:   date.today();  date.today().replace(day=1)
来源：http://gaf.cheryme.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bwe.shanyushiyangtech.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://srx.chenzaomai.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xre.zdqjudy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ire.jianghu66.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kfw.guannengcc.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://afa.0kj1m.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vnq.nanxuanxn.top

================================================================================
来源：http://dih.redwolf501.top

K. JSON 与序列化
来源：http://uxw.bbcook.cn

================================================================================
来源：http://zke.svipenyu.cn

[K01] 对象转 JSON 字符串
来源：http://jjb.52xcode.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zfa.wangdashe.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dyq.zhengqikj.top

JS:   JSON.stringify(obj)
来源：http://nze.tarul.cn

TS:   JSON.stringify(obj)
来源：http://rwx.xuetiantiany.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vti.0kj1m.cn

Go:   json.Marshal(obj)
来源：http://mhj.zdbjq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kkb.redwolf501.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ues.ywan-chungtsiang.top

[K02] JSON 字符串转对象
来源：http://rbh.jinghuilouyu.cn

Py:   json.loads(s)
来源：http://bwz.gzhubu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dap.cdnleiting.top

JS:   JSON.parse(s)
来源：http://nfo.xuanzx.com

TS:   JSON.parse(s)
来源：http://jhr.ybcxt.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zfs.yueranfly.top

Go:   json.Unmarshal(data, &v)
来源：http://uqu.fehbvm.com

Ruby: JSON.parse(s)
来源：http://unp.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wxg.sweek.top

[K03] JSON 美化输出（带缩进）
来源：http://mqa.hesvh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rpe.yueranfly.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ucm.epnwcf.com

JS:   JSON.stringify(obj, null, 2)
来源：http://dmr.xinyue.icu

TS:   JSON.stringify(obj, null, 2)
来源：http://sqa.gotoacloud.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://diu.jqgfzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hvu.zhijiandao.cn

Ruby: JSON.pretty_generate(obj)
来源：http://omy.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ftn.ydzc1.top

[K04] 读取 JSON 文件
来源：http://bsu.vqdsnc.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ujk.zhijiandao.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wjj.epnwcf.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ewv.shuidangran.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://llc.sxryk.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://omy.gotoacloud.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bby.sxryk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://soy.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uic.shanyushiyangkeji.top

[K05] 深拷贝对象
来源：http://fuu.jlsjyb.cn

Py:   copy.deepcopy(obj)
来源：http://tyo.ivvv.top

PHP:  unserialize(serialize($obj));
来源：http://lbn.zhixingplan.top

JS:   structuredClone(obj)
来源：http://thr.andypj.xyz

TS:   structuredClone(obj)
来源：http://yuh.pycfn.com

Java: // 手写拷贝构造，或序列化往返
来源：http://zmu.gaohongyu789.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nlg.birdmap.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://trp.yanxiufei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qrn.aizwys.cn

[K06] 解析 URL 查询串
来源：http://odn.sufxvd.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xab.316326.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xiq.kuanghao11.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dbg.zdqjudy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jkp.xuanzx.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gkg.yueranfly.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://dnd.jianghu66.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zly.fengsongda.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dfy.hnqzz.top

[K07] 进制转换
来源：http://mrf.sjlbkw.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tdm.sxryk.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wjb.fanxiaobao.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sxz.zhoulong.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://haf.pengpengdd.cyou

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://aow.hammf.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vmj.jlsjyb.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mpv.jinqigfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yzk.zdbjq.cn

[K08] 二进制序列化（非 JSON）
来源：http://uqj.jlsjyb.cn

Py:   pickle.dumps(obj)
来源：http://pij.xinyue.icu

PHP:  serialize($obj);  unserialize($s);
来源：http://vlx.zhixingplan.top

JS:   v8.serialize(obj)        // Node
来源：http://ytm.chenlongwang.top

TS:   v8.serialize(obj)        // Node
来源：http://tep.c1oappe.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://awf.jyoumei.cn

Go:   encoding/gob
来源：http://zie.chenzaomai.com

Ruby: Marshal.dump(obj)
来源：http://kuz.chenlongwang.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wqa.haohaochexian.top

================================================================================
来源：http://lso.cheryme.top

L. 网络请求
来源：http://dvz.xziqi.cn

================================================================================
来源：http://jer.shangyingyoupin.top

[L01] 发送 GET 请求
来源：http://qaa.daxiang520.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://udh.xziqi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rjp.kuanghao11.cn

JS:   await fetch(url)
来源：http://brm.quarkkingdee.top

TS:   await fetch(url)
来源：http://ljq.shangyingyoupin.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dxp.smart0.xyz

Go:   resp, err := http.Get(url)
来源：http://pst.jianghu66.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wym.aibaodan.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yhm.hesvh.cn

[L02] 发送 POST JSON
来源：http://wly.uphjek.com

Py:   requests.post(url, json={"a": 1})
来源：http://zid.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mhv.yj20258888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gea.fengsongda.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://osd.jinqigufen.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yne.hywenlv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gnq.quarkkingdee.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://iey.52xcode.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pes.bjfxy.top

[L03] 设置自定义请求头
来源：http://vpa.tarul.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ctk.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gir.jinqigfzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hgq.quarkkingdee.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eju.zhiwuduotai.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gns.zhixingplan.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vno.zdqjudy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fhm.shanyushiyangtech.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wfz.jyoumei.cn

[L04] 设置超时
来源：http://rgx.sweek.top

Py:   requests.get(url, timeout=5)
来源：http://jba.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kwc.yonumen.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dfx.hesvh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://knp.c1oappe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ggk.tian-w.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bgz.vehdjk.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gio.epnwcf.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://afn.shangyingyoupin.top

[L05] 上传文件（multipart）
来源：http://osj.sxryk.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dgv.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wwr.pycfn.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://klf.svipenyu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mhy.wangdashe.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eox.xylfe.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://esy.guannengcc.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bzi.yfazqb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ngo.sjlbkw.cn

[L06] 解析响应为 JSON
来源：http://bpq.xingfuxueyuan.xyz

Py:   resp.json()
来源：http://mkd.gaohongyu789.top

PHP:  json_decode($body, true);
来源：http://gsc.zhoulong.xyz

JS:   await resp.json()
来源：http://tnl.jiagoushi.top

TS:   await resp.json()
来源：http://faz.cheryme.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rag.yongpay.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ykc.hongshengwenyu.top

Ruby: JSON.parse(resp.body)
来源：http://vsc.chenlongwang.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oii.jiagoushi.top

[L07] 处理 HTTP 状态码
来源：http://jcv.yuanzhike.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hjj.cqqwz.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bbn.snrcjt.cn

JS:   resp.ok;  resp.status
来源：http://uee.nwbrower.top

TS:   resp.ok;  resp.status
来源：http://cmv.hongshengwenyu.top

Java: resp.statusCode()
来源：http://nsm.xuetiantiany.cn

Go:   resp.StatusCode
来源：http://jje.havefunace.top

Ruby: resp.code.to_i
来源：http://xbm.pycfn.com

C#:   (int)resp.StatusCode
来源：http://kqq.hfpthk.cn

[L08] 并发请求多个地址
来源：http://clu.uphjek.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xro.yj202588.top

PHP:  curl_multi_init() 系列
来源：http://cog.hnxiangtu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wyu.fengsongda.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hmp.andypj.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mve.guannengcc.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ayt.hesvh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cak.xuanzx.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://siu.birdmap.top

================================================================================
来源：http://fzo.shuidangran.top

M. 命令行 / 进程 / 环境
来源：http://wof.jyoumei.cn

================================================================================
来源：http://ads.fanxiaobao.xyz

[M01] 读取命令行参数
来源：http://nyt.ywan-chungtsiang.top

Py:   sys.argv[1:]
来源：http://yoy.wangdashe.top

PHP:  $argv;  $argc;
来源：http://xpk.zhongyouzk.top

JS:   process.argv.slice(2)
来源：http://ria.tianlin.xyz

TS:   process.argv.slice(2)
来源：http://ahw.jiagoushi.top

Java: args 数组（main 方法参数）
来源：http://ebz.yuxming.cn

Go:   os.Args[1:]
来源：http://ced.cdnleiting.top

Ruby: ARGV
来源：http://lbg.pengpengdd.cyou

C#:   args 数组（Main 方法参数）
来源：http://hzq.yj202588.top

[M02] 读取环境变量
来源：http://jvk.xingfuxueyuan.xyz

Py:   os.environ.get("HOME")
来源：http://kmc.daria6918.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bye.smart0.xyz

JS:   process.env.HOME
来源：http://dwl.guannengcc.top

TS:   process.env.HOME
来源：http://yjt.hongshengwenyu.top

Java: System.getenv("HOME")
来源：http://jbv.52xcode.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ves.aizwys.cn

Ruby: ENV["HOME"]
来源：http://vtk.guannengcc.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lrj.ydzc1.top

[M03] 执行外部命令
来源：http://kpl.sysykeji.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sag.zhijiandao.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kmj.ivvv.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fzo.zhixingplan.top

TS:   child_process.execSync("ls -l").toString()
来源：http://wxu.gogol.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://min.andypj.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://czb.pycfn.com

Ruby: system("ls -l");  `ls -l`
来源：http://ipe.aizwys.cn

C#:   Process.Start("ls", "-l");
来源：http://fed.yangfankeji.com

[M04] 获取当前工作目录
来源：http://ouo.nwbrower.top

Py:   os.getcwd()
来源：http://fgs.tanke756.top

PHP:  getcwd();
来源：http://dec.shzxlz.cn

JS:   process.cwd()
来源：http://zqb.dianchejie.cn

TS:   process.cwd()
来源：http://lbt.uphjek.com

Java: Path.of("").toAbsolutePath()
来源：http://cas.zhoulong.xyz

Go:   os.Getwd()
来源：http://ymo.xinyue.icu

Ruby: Dir.pwd
来源：http://sft.hfpthk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xvg.sxryk.cn

[M05] 设置退出码
来源：http://puy.sysykeji.top

Py:   sys.exit(1)
来源：http://exk.sxryk.cn

PHP:  exit(1);
来源：http://obc.feifeiyinyue.top

JS:   process.exit(1)
来源：http://bmj.wangshuangyany.cn

TS:   process.exit(1)
来源：http://cbx.52xcode.cn

Java: System.exit(1)
来源：http://alr.zycfv.cn

Go:   os.Exit(1)
来源：http://yzc.mhx1999.top

Ruby: exit 1
来源：http://zqc.tarul.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xhq.fzhhl.top

[M06] 向标准错误输出
来源：http://xdp.zhiwuduotai.top

Py:   print("err", file=sys.stderr)
来源：http://wmm.cheryme.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mak.shangyingyoupin.top

JS:   console.error("err")
来源：http://aba.jyoumei.cn

TS:   console.error("err")
来源：http://qys.zdqjudy.top

Java: System.err.println("err")
来源：http://ahg.yueranfly.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oea.zhoulong.xyz

Ruby: warn "err"
来源：http://nda.yfazqb.com

C#:   Console.Error.WriteLine("err")
来源：http://shh.jinqigufen.top

[M07] 判断是否为主入口
来源：http://bhi.birdmap.top

Py:   if __name__ == "__main__":
来源：http://jjp.yj20258888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xcz.ehwqpu.com

JS:   require.main === module
来源：http://dnt.shuidangran.top

TS:   require.main === module
来源：http://qau.xuetiantiany.cn

Java: public static void main(String[] args)
来源：http://dxx.zhoulong.xyz

Go:   func main()
来源：http://kaw.fengsongda.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pdi.tarul.cn

C#:   static void Main(string[] args)
来源：http://mrg.andypj.xyz

[M08] 获取系统与运行时信息
来源：http://sjd.vehdjk.com

Py:   platform.system();  platform.python_version()
来源：http://tpn.cqqwz.cn

PHP:  PHP_OS;  phpversion();
来源：http://qti.redwolf501.top

JS:   process.platform;  process.version
来源：http://dkk.xingfuxueyuan.xyz

TS:   process.platform;  process.version
来源：http://ccf.jlsjyb.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://stn.haohaochexian.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://jdl.chenjidiqi.icu

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uud.zhongyouzk.top


<!-- 参考信息 -->
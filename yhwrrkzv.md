代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cgi.quarkkingdee.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zth.hammf.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ime.zhiwuduotai.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lte.ppjwa.cn

[J03] 字符串解析为日期
来源：http://gzm.yangfankeji.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xbu.yueranfly.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fmt.yuxming.cn

JS:   new Date("2024-01-02")
来源：http://uzk.fanxiaobao.xyz

TS:   new Date("2024-01-02")
来源：http://wcq.hysaishi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rbd.chenjidiqi.icu

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ytu.chenlongwang.top

Ruby: Date.parse("2024-01-02")
来源：http://pef.pengpengdd.cyou

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oqa.zhiwuduotai.top

[J04] 时间戳与日期互转
来源：http://nqt.chenzaomai.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://urf.gotoacloud.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://khc.hywenlv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://caq.tian-w.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://roh.chenlongwang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hlf.chenlongwang.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zpw.bjfxy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jjo.nanxuanxn.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ykp.xylfe.cn

[J05] 时间加减（加 7 天）
来源：http://kia.jqgfzy.top

Py:   now + timedelta(days=7)
来源：http://hzk.jianghu66.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://nxf.316326.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wxt.bbcook.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mae.ehwqpu.com

Java: LocalDate.now().plusDays(7)
来源：http://dor.xylfe.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lqx.tianlin.xyz

Ruby: Time.now + 7 * 86400
来源：http://ekj.yongpay.top

C#:   DateTime.Now.AddDays(7)
来源：http://eds.tianlin.xyz

[J06] 计算两时间之差
来源：http://nex.jinqigufen.top

Py:   (end - start).total_seconds()
来源：http://oaz.xylfe.cn

PHP:  $end->diff($start)->days;
来源：http://wbi.andypj.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://owu.jinqigufen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://itu.ydzc1.top

Java: Duration.between(start, end).toSeconds()
来源：http://ztc.jinghuilouyu.cn

Go:   end.Sub(start).Hours()
来源：http://ala.yj20258.top

Ruby: end - start                 # 返回秒数
来源：http://yif.yj20258.top

C#:   (end - start).TotalSeconds
来源：http://boj.hnqzz.top

[J07] 比较两个日期
来源：http://xfb.yonumen.top

Py:   d1 < d2;  d1 == d2
来源：http://qst.meibo888.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://voj.zycfv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qbf.fehbvm.com

TS:   d1.getTime() < d2.getTime()
来源：http://igt.zycfv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fvk.yj20258.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gjj.0kj1m.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bnb.xuetiantiany.cn

C#:   d1 < d2;  d1 == d2
来源：http://olo.tarul.cn

[J08] 提取年月日与星期
来源：http://zje.pycfn.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://klk.haohaochexian.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ucy.ehwqpu.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://atx.daxiang520.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mno.tanke756.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bdz.xinyue.icu

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wxw.cqqwz.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gvu.guannengcc.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://trj.hnqzz.top

[J09] 时区处理
来源：http://epi.jinyuanbaomall.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qgh.hysaishi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ebx.jianghu66.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xpj.sweek.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xew.dashuyun.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rjm.xuetiantiany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nor.wangdashe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ojz.chenjidiqi.icu

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://laj.52xcode.cn

[J10] 取今天 / 本月第一天
来源：http://tgs.zhixingplan.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qlf.iojbl.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ukm.jyoumei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://iww.316326.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nqc.andypj.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tfr.ywan-chungtsiang.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tlf.sysykeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pkh.gogol.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lva.smart0.xyz

================================================================================
来源：http://sqy.ivvv.top

K. JSON 与序列化
来源：http://fvc.pycfn.com

================================================================================
来源：http://jvv.shanyushiyangkeji.top

[K01] 对象转 JSON 字符串
来源：http://fjt.ppjwa.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://elm.hnxiangtu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lyk.cheryme.top

JS:   JSON.stringify(obj)
来源：http://xli.quarkkingdee.top

TS:   JSON.stringify(obj)
来源：http://kvi.haohaochexian.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cuc.gogol.net.cn

Go:   json.Marshal(obj)
来源：http://tvp.yongpay.top

Ruby: obj.to_json                                     // require "json"
来源：http://kch.hnqzz.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tyq.redwolf501.top

[K02] JSON 字符串转对象
来源：http://gvc.ywan-chungtsiang.top

Py:   json.loads(s)
来源：http://znk.snrcjt.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oxj.ydzc1.top

JS:   JSON.parse(s)
来源：http://szi.yueranfly.top

TS:   JSON.parse(s)
来源：http://puk.fanxiaobao.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rpq.pycfn.com

Go:   json.Unmarshal(data, &v)
来源：http://ycg.chenzaomai.com

Ruby: JSON.parse(s)
来源：http://xhp.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hza.zhaomingkeji.xyz

[K03] JSON 美化输出（带缩进）
来源：http://pqz.fzhhl.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cky.yj20258.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://usg.0kj1m.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://scr.ybcxt.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hcd.fehbvm.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wqu.gogol.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://quz.chenjidiqi.icu

Ruby: JSON.pretty_generate(obj)
来源：http://fwo.yueranfly.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tpl.yj20258888.top

[K04] 读取 JSON 文件
来源：http://hxm.zhengqikj.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fbv.jianghu66.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yye.cucudq.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zri.ydzc1.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zil.yonumen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kjw.yonumen.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xtm.yueranfly.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://fxj.smart0.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lse.sweek.top

[K05] 深拷贝对象
来源：http://ski.yanxiufei.cn

Py:   copy.deepcopy(obj)
来源：http://pfm.tarul.cn

PHP:  unserialize(serialize($obj));
来源：http://pmx.zhixingplan.top

JS:   structuredClone(obj)
来源：http://qvw.wangdashe.top

TS:   structuredClone(obj)
来源：http://yjo.xingfuxueyuan.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://kqn.jlsjyb.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tgj.guowangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dgd.9152youxi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rlv.fanxiaobao.xyz

[K06] 解析 URL 查询串
来源：http://tfb.52xcode.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qnd.cheryme.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uup.dianchejie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jhj.xuetiantiany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tsm.yuxming.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gif.yongpay.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://lrt.redwolf501.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://axc.yj20258888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dqc.mhx1999.top

[K07] 进制转换
来源：http://oyl.9152youxi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bfd.bjfxy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wbf.hywenlv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tjz.shangyingyoupin.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yai.yfazqb.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zvh.shangyingyoupin.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hez.ybcxt.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sln.aizwys.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kqi.gzhubu.top

[K08] 二进制序列化（非 JSON）
来源：http://wjz.sweek.top

Py:   pickle.dumps(obj)
来源：http://erc.jyoumei.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wau.fanxiaobao.xyz

JS:   v8.serialize(obj)        // Node
来源：http://gtd.zhaomingkeji.xyz

TS:   v8.serialize(obj)        // Node
来源：http://lrl.sxryk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ivb.hnqzz.top

Go:   encoding/gob
来源：http://efb.vqdsnc.cn

Ruby: Marshal.dump(obj)
来源：http://piv.jinghuilouyu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kzh.ydzc1.top

================================================================================
来源：http://ojn.zhoulong.xyz

L. 网络请求
来源：http://vkg.xuetiantiany.cn

================================================================================
来源：http://hzu.daxiang520.top

[L01] 发送 GET 请求
来源：http://ydn.hnxiangtu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nbf.cucudq.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rtn.shangyingyoupin.top

JS:   await fetch(url)
来源：http://lgp.cdnleiting.top

TS:   await fetch(url)
来源：http://ovv.hnxiangtu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mhd.ydjk.org.cn

Go:   resp, err := http.Get(url)
来源：http://ubq.cucudq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rsv.9152youxi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ezj.hammf.cn

[L02] 发送 POST JSON
来源：http://ljb.fanxiaobao.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://mzt.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dte.hywenlv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zlg.guowangkeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nfo.yj20258888.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nhq.iojbl.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dlf.cqqwz.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zee.zhijiandao.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gqv.jinyuanbaomall.cn

[L03] 设置自定义请求头
来源：http://vlj.dianchejie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cce.sweek.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dwj.chenlongwang.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bbb.yonumen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gfy.wangdashe.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cso.zhoulong.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wil.sysykeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fwg.shangyingyoupin.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iac.zhixingplan.top

[L04] 设置超时
来源：http://zhl.yonumen.top

Py:   requests.get(url, timeout=5)
来源：http://had.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://usw.hesvh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kof.ybcxt.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nzk.guowangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://euv.guowangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kvo.gotoacloud.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zuk.daxiang520.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tjx.fengsongda.top

[L05] 上传文件（multipart）
来源：http://jnf.52xcode.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dxn.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xrj.fengsongda.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tki.jyoumei.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gpj.chenzaomai.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jbj.yueranfly.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bve.hesvh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ofa.ppjwa.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kxl.xuetiantiany.cn

[L06] 解析响应为 JSON
来源：http://sae.yj202588.top

Py:   resp.json()
来源：http://wzd.hnqzz.top

PHP:  json_decode($body, true);
来源：http://zpc.iojbl.cn

JS:   await resp.json()
来源：http://ysu.hnxiangtu.top

TS:   await resp.json()
来源：http://ujf.pycfn.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rkx.hongshengwenyu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nmi.fehbvm.com

Ruby: JSON.parse(resp.body)
来源：http://dwc.guowangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ggp.hnxiangtu.top

[L07] 处理 HTTP 状态码
来源：http://oue.316326.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qlx.feifeiyinyue.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wby.shanyushiyangtech.top

JS:   resp.ok;  resp.status
来源：http://dmu.tanke756.top

TS:   resp.ok;  resp.status
来源：http://fnh.ppjwa.cn

Java: resp.statusCode()
来源：http://ixk.chenzaomai.com

Go:   resp.StatusCode
来源：http://vlj.guannengcc.top

Ruby: resp.code.to_i
来源：http://whr.nwbrower.top

C#:   (int)resp.StatusCode
来源：http://bst.zhiwuduotai.top

[L08] 并发请求多个地址
来源：http://ith.guannengcc.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xsj.ydjk.org.cn

PHP:  curl_multi_init() 系列
来源：http://zyv.aizwys.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mkd.shzxlz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://izs.vqdsnc.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gjn.hysaishi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ptw.yanxiufei.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fyf.wangdashe.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ykc.yj202588.top

================================================================================
来源：http://ykm.gogol.net.cn

M. 命令行 / 进程 / 环境
来源：http://jjr.haohaochexian.top

================================================================================
来源：http://nhg.hammf.cn

[M01] 读取命令行参数
来源：http://mtx.cashguo.top

Py:   sys.argv[1:]
来源：http://izl.jinqigufen.top

PHP:  $argv;  $argc;
来源：http://ijg.316326.xyz

JS:   process.argv.slice(2)
来源：http://zfw.yongpay.top

TS:   process.argv.slice(2)
来源：http://tnd.fanxiaobao.xyz

Java: args 数组（main 方法参数）
来源：http://muq.tarul.cn

Go:   os.Args[1:]
来源：http://aen.hammf.cn

Ruby: ARGV
来源：http://pag.zycfv.cn

C#:   args 数组（Main 方法参数）
来源：http://aow.meibo888.top

[M02] 读取环境变量
来源：http://xzd.aibaodan.cn

Py:   os.environ.get("HOME")
来源：http://hxm.vqdsnc.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nkz.bjfxy.top

JS:   process.env.HOME
来源：http://xii.haohaochexian.top

TS:   process.env.HOME
来源：http://pzk.pycfn.com

Java: System.getenv("HOME")
来源：http://tkk.xziqi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bvy.sjlbkw.cn

Ruby: ENV["HOME"]
来源：http://heg.zhijiandao.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://siu.zhixingplan.top

[M03] 执行外部命令
来源：http://pad.9152youxi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mfk.guowangkeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://azk.chenlongwang.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fru.ctjpmb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://isy.jinqigfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hlv.zhiwuduotai.top

Go:   exec.Command("ls", "-l").Output()
来源：http://zla.yj20258888.top

Ruby: system("ls -l");  `ls -l`
来源：http://tod.chenjidiqi.icu

C#:   Process.Start("ls", "-l");
来源：http://fvk.zdbjq.cn

[M04] 获取当前工作目录
来源：http://htc.smart0.xyz

Py:   os.getcwd()
来源：http://gqe.ywan-chungtsiang.top

PHP:  getcwd();
来源：http://rfu.zdbjq.cn

JS:   process.cwd()
来源：http://sll.zhongyouzk.top

TS:   process.cwd()
来源：http://hsn.iojbl.cn

Java: Path.of("").toAbsolutePath()
来源：http://dua.yj202588.top

Go:   os.Getwd()
来源：http://dld.andypj.xyz

Ruby: Dir.pwd
来源：http://fmv.zdbjq.cn

C#:   Directory.GetCurrentDirectory()
来源：http://erz.tian-w.cn

[M05] 设置退出码
来源：http://bng.daria6918.cn

Py:   sys.exit(1)
来源：http://lou.epnwcf.com

PHP:  exit(1);
来源：http://oar.meibo888.top

JS:   process.exit(1)
来源：http://sim.yj20258888.top

TS:   process.exit(1)
来源：http://gyn.hcnkem.com

Java: System.exit(1)
来源：http://lau.nanxuanxn.top

Go:   os.Exit(1)
来源：http://bfi.smart0.xyz

Ruby: exit 1
来源：http://aqd.ybcxt.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bwu.epnwcf.com

[M06] 向标准错误输出
来源：http://osl.jinqigfzy.top

Py:   print("err", file=sys.stderr)
来源：http://lxw.yueranfly.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mxj.kuanghao11.cn

JS:   console.error("err")
来源：http://nty.tianlin.xyz

TS:   console.error("err")
来源：http://zfg.jqgfzy.top

Java: System.err.println("err")
来源：http://rtw.mhx1999.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cql.gogol.net.cn

Ruby: warn "err"
来源：http://ofo.ehwqpu.com

C#:   Console.Error.WriteLine("err")
来源：http://tha.daria6918.cn

[M07] 判断是否为主入口
来源：http://lxj.yj20258.top

Py:   if __name__ == "__main__":
来源：http://tic.jlsjyb.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rvs.daria6918.cn

JS:   require.main === module
来源：http://rgg.hnqzz.top

TS:   require.main === module
来源：http://hxk.ehwqpu.com

Java: public static void main(String[] args)
来源：http://gxm.jyoumei.cn

Go:   func main()
来源：http://qkj.gzhubu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xli.yonumen.top

C#:   static void Main(string[] args)
来源：http://tfd.jinghuilouyu.cn

[M08] 获取系统与运行时信息
来源：http://msw.ivvv.top

Py:   platform.system();  platform.python_version()
来源：http://dcr.vqdsnc.cn

PHP:  PHP_OS;  phpversion();
来源：http://vws.wangdashe.top

JS:   process.platform;  process.version
来源：http://qwp.ywan-chungtsiang.top

TS:   process.platform;  process.version
来源：http://zgv.zhaomingkeji.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fda.0kj1m.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ztq.c1oappe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hhr.zdbjq.cn


<!-- 参考信息 -->
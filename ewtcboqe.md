代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blm.svipenyu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qzw.gzhubu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qeo.cqqwz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yub.aibaodan.cn

[J03] 字符串解析为日期
来源：http://ghn.shanyushiyangtech.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://epn.gaohongyu789.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dum.nanxinkj.top

JS:   new Date("2024-01-02")
来源：http://xpb.snrcjt.cn

TS:   new Date("2024-01-02")
来源：http://fyl.yuxming.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sqx.bbcook.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bjo.sjlbkw.cn

Ruby: Date.parse("2024-01-02")
来源：http://oeg.bjfxy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://iak.nanxinkj.top

[J04] 时间戳与日期互转
来源：http://cyo.smart0.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kek.jinghuilouyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zeh.zhixingplan.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ghl.shanyushiyangkeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://err.cdnleiting.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rms.ehwqpu.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zjs.zhongyouzk.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kjd.tanke756.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jww.jinghuilouyu.cn

[J05] 时间加减（加 7 天）
来源：http://ymk.gzhubu.top

Py:   now + timedelta(days=7)
来源：http://nfe.52xcode.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jsg.yuxming.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wex.hnqzz.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://myc.redwolf501.top

Java: LocalDate.now().plusDays(7)
来源：http://rnx.ivvv.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xfc.aibaodan.cn

Ruby: Time.now + 7 * 86400
来源：http://ukt.cdnleiting.top

C#:   DateTime.Now.AddDays(7)
来源：http://jce.zdqjudy.top

[J06] 计算两时间之差
来源：http://wrc.hongshengwenyu.top

Py:   (end - start).total_seconds()
来源：http://iax.yonumen.top

PHP:  $end->diff($start)->days;
来源：http://eih.zhoulong.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hcc.hfpthk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dbj.smart0.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://zxs.hfpthk.cn

Go:   end.Sub(start).Hours()
来源：http://dwy.hfpthk.cn

Ruby: end - start                 # 返回秒数
来源：http://cfq.hywenlv.cn

C#:   (end - start).TotalSeconds
来源：http://yaa.bjfxy.top

[J07] 比较两个日期
来源：http://ubh.zhijiandao.cn

Py:   d1 < d2;  d1 == d2
来源：http://efh.yfazqb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://aip.zdqjudy.top

JS:   d1.getTime() < d2.getTime()
来源：http://kmq.jqgfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://mgy.zhaomingkeji.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://flj.zhiwuduotai.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zof.hesvh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nrs.pengpengdd.cyou

C#:   d1 < d2;  d1 == d2
来源：http://mib.xuetiantiany.cn

[J08] 提取年月日与星期
来源：http://jwg.sweek.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://okz.mhx1999.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kau.fanxiaobao.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://css.cdnleiting.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rdx.havefunace.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pez.sxryk.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yms.yuxming.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zaz.hywenlv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dhu.9152youxi.cn

[J09] 时区处理
来源：http://nry.hesvh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dix.xuanzx.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://obj.zhixingplan.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vzq.aizwys.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mbn.meibo888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tcj.sweek.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cbb.mhx1999.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bfg.ppjwa.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cge.yfazqb.com

[J10] 取今天 / 本月第一天
来源：http://ryc.gotoacloud.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hjc.gogol.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zqj.feifeiyinyue.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ops.ctjpmb.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oau.vqdsnc.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lpl.guowangkeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://job.nanxinkj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hqk.jinqigufen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wqj.gotoacloud.top

================================================================================
来源：http://svv.zycfv.cn

K. JSON 与序列化
来源：http://kuj.shanyushiyangkeji.top

================================================================================
来源：http://zht.wangshuangyany.cn

[K01] 对象转 JSON 字符串
来源：http://mig.hysaishi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://aae.dianchejie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vbf.zhengqikj.top

JS:   JSON.stringify(obj)
来源：http://zqn.yj20258888.top

TS:   JSON.stringify(obj)
来源：http://urd.gzhubu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ecd.sxryk.cn

Go:   json.Marshal(obj)
来源：http://xot.ybcxt.top

Ruby: obj.to_json                                     // require "json"
来源：http://nfr.hywenlv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rqb.chenjidiqi.icu

[K02] JSON 字符串转对象
来源：http://rmk.fktsv.cn

Py:   json.loads(s)
来源：http://iru.shanyushiyangkeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bik.jinqigufen.top

JS:   JSON.parse(s)
来源：http://xww.sufxvd.cn

TS:   JSON.parse(s)
来源：http://qpq.ywan-chungtsiang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sdn.fktsv.cn

Go:   json.Unmarshal(data, &v)
来源：http://mte.52xcode.cn

Ruby: JSON.parse(s)
来源：http://uhc.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jou.guowangkeji.top

[K03] JSON 美化输出（带缩进）
来源：http://gkn.jinqigufen.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xyp.yfazqb.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dph.zhongyouzk.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wkb.yueranfly.top

TS:   JSON.stringify(obj, null, 2)
来源：http://gll.xinyue.icu

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://heu.sufxvd.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xcf.guannengcc.top

Ruby: JSON.pretty_generate(obj)
来源：http://qgg.sjlbkw.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://edb.chenzaomai.com

[K04] 读取 JSON 文件
来源：http://ljd.sweek.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lgk.redwolf501.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nna.jyoumei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uav.xylfe.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sff.chenjidiqi.icu

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://evg.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xhk.shzxlz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://joi.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pyu.shuidangran.top

[K05] 深拷贝对象
来源：http://qwf.zhiwuduotai.top

Py:   copy.deepcopy(obj)
来源：http://nhc.cashguo.top

PHP:  unserialize(serialize($obj));
来源：http://dks.shzxlz.cn

JS:   structuredClone(obj)
来源：http://gnt.yuxming.cn

TS:   structuredClone(obj)
来源：http://ikg.shzxlz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bbg.tianlin.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://huv.shanyushiyangtech.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ddq.shuidangran.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vpg.ybcxt.top

[K06] 解析 URL 查询串
来源：http://nzx.quarkkingdee.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fzk.ctjpmb.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lwu.jinghuilouyu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rvn.xuetiantiany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xyt.jinqigfzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xfb.feifeiyinyue.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://oya.aizwys.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://iel.daxiang520.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ozc.vqdsnc.cn

[K07] 进制转换
来源：http://atu.316326.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://voi.wangdashe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://adw.bbcook.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fnw.cucudq.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dam.wangshuangyany.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://znz.52xcode.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nbq.yuxming.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jmn.fzhhl.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://emr.cheryme.top

[K08] 二进制序列化（非 JSON）
来源：http://jcm.xylfe.cn

Py:   pickle.dumps(obj)
来源：http://xcm.hysaishi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vee.shuidangran.top

JS:   v8.serialize(obj)        // Node
来源：http://iym.nanxinkj.top

TS:   v8.serialize(obj)        // Node
来源：http://epp.birdmap.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jny.tian-w.cn

Go:   encoding/gob
来源：http://qww.0kj1m.cn

Ruby: Marshal.dump(obj)
来源：http://goq.zhixingplan.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kuz.mhx1999.top

================================================================================
来源：http://lvn.shangyingyoupin.top

L. 网络请求
来源：http://ouy.zycfv.cn

================================================================================
来源：http://eni.ctjpmb.com

[L01] 发送 GET 请求
来源：http://rgs.hongshengwenyu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gkk.fktsv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pyh.fanxiaobao.xyz

JS:   await fetch(url)
来源：http://nfh.gotoacloud.top

TS:   await fetch(url)
来源：http://mio.52xcode.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jsi.52xcode.cn

Go:   resp, err := http.Get(url)
来源：http://llb.hongshengwenyu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://gbl.iojbl.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bjd.yfazqb.com

[L02] 发送 POST JSON
来源：http://xmj.yvedp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pos.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ohd.jqgufenzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ivx.zdqjudy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qiq.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ruv.bbcook.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://quo.hfpthk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wld.tianlin.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://koo.zhoulong.xyz

[L03] 设置自定义请求头
来源：http://fox.yangfankeji.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ebg.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xtn.zhixingplan.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xsb.hfpthk.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://osc.zycfv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zxd.gogol.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fuk.daxiang520.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bwv.epnwcf.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ahp.pengpengdd.cyou

[L04] 设置超时
来源：http://vfc.ehwqpu.com

Py:   requests.get(url, timeout=5)
来源：http://ufw.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dht.zhixingplan.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jww.hysaishi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gqt.xinyue.icu

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://eqf.xuetiantiany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ekd.nwbrower.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gbr.mhx1999.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uiv.yj20258.top

[L05] 上传文件（multipart）
来源：http://sra.pycfn.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hls.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://crg.yonumen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://iht.sxryk.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://weu.0kj1m.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qah.birdmap.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nak.bjfxy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ajn.andypj.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vad.316326.xyz

[L06] 解析响应为 JSON
来源：http://wnv.andypj.xyz

Py:   resp.json()
来源：http://tge.jqgfzy.top

PHP:  json_decode($body, true);
来源：http://yqe.zdqjudy.top

JS:   await resp.json()
来源：http://vae.hammf.cn

TS:   await resp.json()
来源：http://rgb.ydzc1.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gej.guannengcc.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dcj.snrcjt.cn

Ruby: JSON.parse(resp.body)
来源：http://zrc.yuxming.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jel.gotoacloud.top

[L07] 处理 HTTP 状态码
来源：http://ifg.jinghuilouyu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://oen.shuidangran.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wjw.hysaishi.cn

JS:   resp.ok;  resp.status
来源：http://wve.snrcjt.cn

TS:   resp.ok;  resp.status
来源：http://xiy.fktsv.cn

Java: resp.statusCode()
来源：http://xap.zdqjudy.top

Go:   resp.StatusCode
来源：http://bkw.aizwys.cn

Ruby: resp.code.to_i
来源：http://asv.andypj.xyz

C#:   (int)resp.StatusCode
来源：http://tmv.jiagoushi.top

[L08] 并发请求多个地址
来源：http://bur.zhaomingkeji.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gpw.havefunace.top

PHP:  curl_multi_init() 系列
来源：http://lkf.dianchejie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ksx.mhx1999.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cup.yj20258888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yjc.bjfxy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lli.jianghu66.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tzu.yonumen.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ptw.yuxming.cn

================================================================================
来源：http://mfh.hysaishi.cn

M. 命令行 / 进程 / 环境
来源：http://fqm.fzhhl.top

================================================================================
来源：http://nwn.cheryme.top

[M01] 读取命令行参数
来源：http://ufq.jqgufenzy.top

Py:   sys.argv[1:]
来源：http://hvi.cdnleiting.top

PHP:  $argv;  $argc;
来源：http://vbp.haohaochexian.top

JS:   process.argv.slice(2)
来源：http://dmv.fktsv.cn

TS:   process.argv.slice(2)
来源：http://yty.zdqjudy.top

Java: args 数组（main 方法参数）
来源：http://mdm.havefunace.top

Go:   os.Args[1:]
来源：http://qdb.daria6918.cn

Ruby: ARGV
来源：http://nrh.9152youxi.cn

C#:   args 数组（Main 方法参数）
来源：http://nei.quarkkingdee.top

[M02] 读取环境变量
来源：http://ppx.cashguo.top

Py:   os.environ.get("HOME")
来源：http://azt.nanxinkj.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zzr.quarkkingdee.top

JS:   process.env.HOME
来源：http://eqh.ybcxt.top

TS:   process.env.HOME
来源：http://rlg.kuanghao11.cn

Java: System.getenv("HOME")
来源：http://qym.cheryme.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mfv.yongpay.top

Ruby: ENV["HOME"]
来源：http://oot.hfpthk.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://klt.fengsongda.top

[M03] 执行外部命令
来源：http://gen.xinyue.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gao.uphjek.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ttc.jinyuanbaomall.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kfx.zhoulong.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://dtb.snrcjt.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qep.birdmap.top

Go:   exec.Command("ls", "-l").Output()
来源：http://nnk.xingfuxueyuan.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://ngh.cdnleiting.top

C#:   Process.Start("ls", "-l");
来源：http://mde.shzxlz.cn

[M04] 获取当前工作目录
来源：http://nbq.dianchejie.cn

Py:   os.getcwd()
来源：http://klx.andypj.xyz

PHP:  getcwd();
来源：http://dag.yj20258888.top

JS:   process.cwd()
来源：http://ijd.cdnleiting.top

TS:   process.cwd()
来源：http://rsu.cqqwz.cn

Java: Path.of("").toAbsolutePath()
来源：http://zxr.pengpengdd.cyou

Go:   os.Getwd()
来源：http://zea.jinghuilouyu.cn

Ruby: Dir.pwd
来源：http://nqz.yvedp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pvo.zhaomingkeji.xyz

[M05] 设置退出码
来源：http://ncg.zycfv.cn

Py:   sys.exit(1)
来源：http://guf.hysaishi.cn

PHP:  exit(1);
来源：http://nnm.tarul.cn

JS:   process.exit(1)
来源：http://ftp.sjlbkw.cn

TS:   process.exit(1)
来源：http://dax.wangshuangyany.cn

Java: System.exit(1)
来源：http://zju.yuanzhike.top

Go:   os.Exit(1)
来源：http://aby.vehdjk.com

Ruby: exit 1
来源：http://kyu.tanke756.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://efv.gzhubu.top

[M06] 向标准错误输出
来源：http://uat.ywan-chungtsiang.top

Py:   print("err", file=sys.stderr)
来源：http://gvd.dashuyun.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tgz.xziqi.cn

JS:   console.error("err")
来源：http://jfu.tian-w.cn

TS:   console.error("err")
来源：http://csf.jinghuilouyu.cn

Java: System.err.println("err")
来源：http://rad.xuetiantiany.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zhs.zhongyouzk.top

Ruby: warn "err"
来源：http://hmo.zdqjudy.top

C#:   Console.Error.WriteLine("err")
来源：http://gln.uphjek.com

[M07] 判断是否为主入口
来源：http://htl.yangfankeji.com

Py:   if __name__ == "__main__":
来源：http://qxm.sweek.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zma.cashguo.top

JS:   require.main === module
来源：http://eyc.uphjek.com

TS:   require.main === module
来源：http://gdi.vqdsnc.cn

Java: public static void main(String[] args)
来源：http://klm.fanxiaobao.xyz

Go:   func main()
来源：http://gmg.xuetiantiany.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tba.birdmap.top

C#:   static void Main(string[] args)
来源：http://web.hammf.cn

[M08] 获取系统与运行时信息
来源：http://boi.jinqigfzy.top

Py:   platform.system();  platform.python_version()
来源：http://nqo.quarkkingdee.top

PHP:  PHP_OS;  phpversion();
来源：http://hgr.shangyingyoupin.top

JS:   process.platform;  process.version
来源：http://ovc.mhx1999.top

TS:   process.platform;  process.version
来源：http://mqc.hfpthk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qyk.sxryk.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://umf.hywenlv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tns.yj202588.top


<!-- 参考信息 -->
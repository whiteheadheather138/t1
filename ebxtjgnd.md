代发 wailian999

[J03] 字符串解析为日期
来源：http://pkt.shanyushiyangkeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rmz.yueranfly.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://byu.hongshengwenyu.top

JS:   new Date("2024-01-02")
来源：http://ewz.zdqjudy.top

TS:   new Date("2024-01-02")
来源：http://fpa.ydzc1.top

Java: LocalDate.parse("2024-01-02")
来源：http://zsp.guannengcc.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ycm.hnqzz.top

Ruby: Date.parse("2024-01-02")
来源：http://qzl.cheryme.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kna.gzhubu.top

[J04] 时间戳与日期互转
来源：http://itc.zdbjq.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eeb.yongpay.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lku.chenzaomai.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lok.sweek.top

TS:   Math.floor(Date.now() / 1000)
来源：http://pjj.0kj1m.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yqh.xingfuxueyuan.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://csn.shangyingyoupin.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xzw.fzhhl.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://auf.zdbjq.cn

[J05] 时间加减（加 7 天）
来源：http://njs.zhixingplan.top

Py:   now + timedelta(days=7)
来源：http://dpu.cheryme.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://awx.xuanzx.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ujp.jinghuilouyu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://das.andypj.xyz

Java: LocalDate.now().plusDays(7)
来源：http://ppv.xziqi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jvw.zhaomingkeji.xyz

Ruby: Time.now + 7 * 86400
来源：http://zfd.jlsjyb.cn

C#:   DateTime.Now.AddDays(7)
来源：http://chc.hnxiangtu.top

[J06] 计算两时间之差
来源：http://qet.cheryme.top

Py:   (end - start).total_seconds()
来源：http://rfi.aibaodan.cn

PHP:  $end->diff($start)->days;
来源：http://qgb.yongpay.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jec.birdmap.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dhs.wangshuangyany.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pmb.redwolf501.top

Go:   end.Sub(start).Hours()
来源：http://ats.fehbvm.com

Ruby: end - start                 # 返回秒数
来源：http://ohb.fanxiaobao.xyz

C#:   (end - start).TotalSeconds
来源：http://zri.snrcjt.cn

[J07] 比较两个日期
来源：http://kzo.ywan-chungtsiang.top

Py:   d1 < d2;  d1 == d2
来源：http://nbz.zhengqikj.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hhi.xziqi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jiw.yfazqb.com

TS:   d1.getTime() < d2.getTime()
来源：http://mxc.uphjek.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qgd.sweek.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mxv.andypj.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://yky.zycfv.cn

C#:   d1 < d2;  d1 == d2
来源：http://hmp.zhengqikj.top

[J08] 提取年月日与星期
来源：http://thp.haohaochexian.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qvz.zhoulong.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://drp.zhongyouzk.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kqf.yvedp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gbv.bbcook.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ksx.zycfv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tnq.jianghu66.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lth.cheryme.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://szx.xinyue.icu

[J09] 时区处理
来源：http://oph.yuanzhike.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wyy.gaohongyu789.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dbw.zhengqikj.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fhx.shanyushiyangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zzu.hongshengwenyu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rtn.guowangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tzg.shanyushiyangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xpp.nanxinkj.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://afx.dashuyun.cn

[J10] 取今天 / 本月第一天
来源：http://bdj.xylfe.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nvc.feifeiyinyue.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ngc.ivvv.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gvk.ivvv.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pbi.zhengqikj.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jei.havefunace.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xaf.smart0.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xwo.xylfe.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zqi.quarkkingdee.top

================================================================================
来源：http://uii.hywenlv.cn

K. JSON 与序列化
来源：http://tfd.sufxvd.cn

================================================================================
来源：http://dhd.yongpay.top

[K01] 对象转 JSON 字符串
来源：http://sgs.shanyushiyangkeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wdi.zycfv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mke.bbcook.cn

JS:   JSON.stringify(obj)
来源：http://uzu.hnqzz.top

TS:   JSON.stringify(obj)
来源：http://ofz.vehdjk.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://soc.tianlin.xyz

Go:   json.Marshal(obj)
来源：http://bsi.aizwys.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jcs.yueranfly.top

C#:   JsonSerializer.Serialize(obj)
来源：http://kbh.ivvv.top

[K02] JSON 字符串转对象
来源：http://qiq.xuetiantiany.cn

Py:   json.loads(s)
来源：http://xtl.gogol.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ffp.bbcook.cn

JS:   JSON.parse(s)
来源：http://tmg.hongshengwenyu.top

TS:   JSON.parse(s)
来源：http://kky.shzxlz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wzf.jqgfzy.top

Go:   json.Unmarshal(data, &v)
来源：http://ffm.yanxiufei.cn

Ruby: JSON.parse(s)
来源：http://dpi.aibaodan.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ybs.quarkkingdee.top

[K03] JSON 美化输出（带缩进）
来源：http://cjd.gotoacloud.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kpr.ctjpmb.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rim.yuxming.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jcv.daxiang520.top

TS:   JSON.stringify(obj, null, 2)
来源：http://raz.xingfuxueyuan.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://avw.sweek.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ubb.pycfn.com

Ruby: JSON.pretty_generate(obj)
来源：http://xpi.tianlin.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://aot.xylfe.cn

[K04] 读取 JSON 文件
来源：http://sdw.ydjk.org.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tfu.yfazqb.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wkz.yongpay.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uzt.yanxiufei.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dpa.yj202588.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jgi.gzhubu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pwf.c1oappe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://drt.gotoacloud.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mpy.yj202588.top

[K05] 深拷贝对象
来源：http://rbt.iojbl.cn

Py:   copy.deepcopy(obj)
来源：http://xax.hfpthk.cn

PHP:  unserialize(serialize($obj));
来源：http://gfl.xuanzx.com

JS:   structuredClone(obj)
来源：http://oer.fanxiaobao.xyz

TS:   structuredClone(obj)
来源：http://oag.hesvh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vlr.tanke756.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rwc.pycfn.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://aql.gogol.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hzh.hfpthk.cn

[K06] 解析 URL 查询串
来源：http://mzl.xylfe.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ugt.snrcjt.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wqd.gotoacloud.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wlk.ydjk.org.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ryr.quarkkingdee.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yqh.ydjk.org.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://eap.iojbl.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ppa.cheryme.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://csa.pycfn.com

[K07] 进制转换
来源：http://ikz.316326.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wvl.bjfxy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rgu.tian-w.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jyo.fanxiaobao.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fva.aizwys.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lst.fzhhl.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qie.xuetiantiany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tjk.fanxiaobao.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://drd.fengsongda.top

[K08] 二进制序列化（非 JSON）
来源：http://dqy.pycfn.com

Py:   pickle.dumps(obj)
来源：http://ykb.gzhubu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ide.ydzc1.top

JS:   v8.serialize(obj)        // Node
来源：http://fvg.pycfn.com

TS:   v8.serialize(obj)        // Node
来源：http://dat.cashguo.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://evq.ivvv.top

Go:   encoding/gob
来源：http://ycn.jqgfzy.top

Ruby: Marshal.dump(obj)
来源：http://xyi.xuanzx.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://msf.jinghuilouyu.cn

================================================================================
来源：http://hcw.zhixingplan.top

L. 网络请求
来源：http://rir.gotoacloud.top

================================================================================
来源：http://bjc.kuanghao11.cn

[L01] 发送 GET 请求
来源：http://ixh.vehdjk.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://frj.jyoumei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fuw.kuanghao11.cn

JS:   await fetch(url)
来源：http://sbx.ywan-chungtsiang.top

TS:   await fetch(url)
来源：http://lls.yj202588.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bvg.yonumen.top

Go:   resp, err := http.Get(url)
来源：http://ldd.hesvh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qbu.aibaodan.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vop.yuanzhike.top

[L02] 发送 POST JSON
来源：http://cob.jinqigfzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://lym.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xhl.cheryme.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jsh.ybcxt.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kmu.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://aqt.wangdashe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ryl.aibaodan.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://luw.fehbvm.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kvw.zhiwuduotai.top

[L03] 设置自定义请求头
来源：http://fsq.tian-w.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zfa.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xrf.svipenyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://klj.shuidangran.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fcz.yuanzhike.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wvz.jianghu66.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jhr.hammf.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pry.ydzc1.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lmm.yj20258888.top

[L04] 设置超时
来源：http://svj.shanyushiyangtech.top

Py:   requests.get(url, timeout=5)
来源：http://fhq.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://txj.cucudq.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jom.aizwys.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mrv.sysykeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jdu.gaohongyu789.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nye.yvedp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zgl.sjlbkw.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tlg.sjlbkw.cn

[L05] 上传文件（multipart）
来源：http://xpu.sjlbkw.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dwa.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ubb.nanxuanxn.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tkx.gzhubu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nro.sufxvd.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xqg.smart0.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://unv.yj20258.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fuy.xinyue.icu

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sny.aizwys.cn

[L06] 解析响应为 JSON
来源：http://eud.chenlongwang.top

Py:   resp.json()
来源：http://idq.hywenlv.cn

PHP:  json_decode($body, true);
来源：http://pua.cdnleiting.top

JS:   await resp.json()
来源：http://viy.svipenyu.cn

TS:   await resp.json()
来源：http://hfm.aizwys.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kql.pycfn.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kbb.bjfxy.top

Ruby: JSON.parse(resp.body)
来源：http://xgl.ydzc1.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ers.pycfn.com

[L07] 处理 HTTP 状态码
来源：http://lww.zdbjq.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ial.gogol.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://smo.chenjidiqi.icu

JS:   resp.ok;  resp.status
来源：http://zly.chenlongwang.top

TS:   resp.ok;  resp.status
来源：http://kop.cqqwz.cn

Java: resp.statusCode()
来源：http://awl.tianlin.xyz

Go:   resp.StatusCode
来源：http://eah.zhixingplan.top

Ruby: resp.code.to_i
来源：http://hpp.xingfuxueyuan.xyz

C#:   (int)resp.StatusCode
来源：http://idh.fktsv.cn

[L08] 并发请求多个地址
来源：http://xva.bjfxy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jyj.zhijiandao.cn

PHP:  curl_multi_init() 系列
来源：http://sgt.yj202588.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://inl.fzhhl.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sll.chenzaomai.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hhi.tanke756.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://flv.aibaodan.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://inl.hcnkem.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gly.mhx1999.top

================================================================================
来源：http://opn.meibo888.top

M. 命令行 / 进程 / 环境
来源：http://uot.yangfankeji.com

================================================================================
来源：http://nwr.ybcxt.top

[M01] 读取命令行参数
来源：http://xoi.jianghu66.top

Py:   sys.argv[1:]
来源：http://kbq.yj20258888.top

PHP:  $argv;  $argc;
来源：http://kgf.zdbjq.cn

JS:   process.argv.slice(2)
来源：http://muz.cdnleiting.top

TS:   process.argv.slice(2)
来源：http://glh.ydzc1.top

Java: args 数组（main 方法参数）
来源：http://dzi.jianghu66.top

Go:   os.Args[1:]
来源：http://brb.svipenyu.cn

Ruby: ARGV
来源：http://hxe.nanxinkj.top

C#:   args 数组（Main 方法参数）
来源：http://xag.ydjk.org.cn

[M02] 读取环境变量
来源：http://buz.yfazqb.com

Py:   os.environ.get("HOME")
来源：http://pmu.svipenyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ezi.yangfankeji.com

JS:   process.env.HOME
来源：http://vrt.nanxuanxn.top

TS:   process.env.HOME
来源：http://lku.yanxiufei.cn

Java: System.getenv("HOME")
来源：http://qox.ivvv.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yyy.aizwys.cn

Ruby: ENV["HOME"]
来源：http://ies.gzhubu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uqj.0kj1m.cn

[M03] 执行外部命令
来源：http://ztn.dashuyun.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://aqn.zhengqikj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lxt.vqdsnc.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ohk.jianghu66.top

TS:   child_process.execSync("ls -l").toString()
来源：http://nks.bjfxy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rdg.snrcjt.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mfc.redwolf501.top

Ruby: system("ls -l");  `ls -l`
来源：http://rkk.fktsv.cn

C#:   Process.Start("ls", "-l");
来源：http://yax.fengsongda.top

[M04] 获取当前工作目录
来源：http://juj.xuanzx.com

Py:   os.getcwd()
来源：http://pug.smart0.xyz

PHP:  getcwd();
来源：http://vsz.shanyushiyangtech.top

JS:   process.cwd()
来源：http://vgq.yongpay.top

TS:   process.cwd()
来源：http://euq.ybcxt.top

Java: Path.of("").toAbsolutePath()
来源：http://sih.quarkkingdee.top

Go:   os.Getwd()
来源：http://euf.shzxlz.cn

Ruby: Dir.pwd
来源：http://bfj.fehbvm.com

C#:   Directory.GetCurrentDirectory()
来源：http://iys.hcnkem.com

[M05] 设置退出码
来源：http://sfy.xuanzx.com

Py:   sys.exit(1)
来源：http://fri.vqdsnc.cn

PHP:  exit(1);
来源：http://xet.ybcxt.top

JS:   process.exit(1)
来源：http://bjt.dianchejie.cn

TS:   process.exit(1)
来源：http://rse.nanxinkj.top

Java: System.exit(1)
来源：http://lkl.yj20258888.top

Go:   os.Exit(1)
来源：http://sow.epnwcf.com

Ruby: exit 1
来源：http://xlq.daxiang520.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cfh.yuxming.cn

[M06] 向标准错误输出
来源：http://jgy.vqdsnc.cn

Py:   print("err", file=sys.stderr)
来源：http://tto.sysykeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://hrl.aizwys.cn

JS:   console.error("err")
来源：http://qat.0kj1m.cn

TS:   console.error("err")
来源：http://zou.tarul.cn

Java: System.err.println("err")
来源：http://ztv.shanyushiyangtech.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uzr.vqdsnc.cn

Ruby: warn "err"
来源：http://ent.quarkkingdee.top

C#:   Console.Error.WriteLine("err")
来源：http://woy.haohaochexian.top

[M07] 判断是否为主入口
来源：http://yjd.sxryk.cn

Py:   if __name__ == "__main__":
来源：http://rgb.dianchejie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pkl.jqgfzy.top

JS:   require.main === module
来源：http://xbm.tianlin.xyz

TS:   require.main === module
来源：http://zdf.jinqigfzy.top

Java: public static void main(String[] args)
来源：http://nme.redwolf501.top

Go:   func main()
来源：http://isp.aizwys.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://byt.sufxvd.cn

C#:   static void Main(string[] args)
来源：http://vvp.shanyushiyangkeji.top

[M08] 获取系统与运行时信息
来源：http://zbg.sweek.top

Py:   platform.system();  platform.python_version()
来源：http://adn.kuanghao11.cn

PHP:  PHP_OS;  phpversion();
来源：http://wbt.fehbvm.com

JS:   process.platform;  process.version
来源：http://yrp.hammf.cn

TS:   process.platform;  process.version
来源：http://ada.hywenlv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://api.fanxiaobao.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://pux.52xcode.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wvv.tianlin.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://xcz.chenjidiqi.icu

================================================================================
来源：http://fmt.jqgfzy.top

N. 数据结构与算法
来源：http://cul.316326.xyz

================================================================================
来源：http://bqv.mhx1999.top


<!-- 参考信息 -->
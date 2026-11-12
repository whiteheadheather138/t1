代发 wailian999

TS:   new Date("2024-01-02")
来源：http://qfd.daxiang520.top

Java: LocalDate.parse("2024-01-02")
来源：http://bpa.uphjek.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ncn.nanxuanxn.top

Ruby: Date.parse("2024-01-02")
来源：http://ngq.uphjek.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zfh.ctjpmb.com

[J04] 时间戳与日期互转
来源：http://mpz.yuxming.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tif.gotoacloud.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bug.jiagoushi.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ouw.xingfuxueyuan.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://hjq.zycfv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jos.shuidangran.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vkq.tarul.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kkp.ppjwa.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gwq.jinqigfzy.top

[J05] 时间加减（加 7 天）
来源：http://lbf.zhixingplan.top

Py:   now + timedelta(days=7)
来源：http://rgk.jyoumei.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sdi.ehwqpu.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://als.52xcode.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ujn.sysykeji.top

Java: LocalDate.now().plusDays(7)
来源：http://hhu.hesvh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lno.zhiwuduotai.top

Ruby: Time.now + 7 * 86400
来源：http://hde.cqqwz.cn

C#:   DateTime.Now.AddDays(7)
来源：http://obt.yj20258.top

[J06] 计算两时间之差
来源：http://hkl.xylfe.cn

Py:   (end - start).total_seconds()
来源：http://zzo.mhx1999.top

PHP:  $end->diff($start)->days;
来源：http://zqi.yj202588.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jhw.chenzaomai.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hpa.meibo888.top

Java: Duration.between(start, end).toSeconds()
来源：http://ryr.havefunace.top

Go:   end.Sub(start).Hours()
来源：http://swk.bjfxy.top

Ruby: end - start                 # 返回秒数
来源：http://uvg.daria6918.cn

C#:   (end - start).TotalSeconds
来源：http://fcj.pycfn.com

[J07] 比较两个日期
来源：http://rhh.yueranfly.top

Py:   d1 < d2;  d1 == d2
来源：http://yvb.yj20258888.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ykz.0kj1m.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sfv.xingfuxueyuan.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://ifa.c1oappe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lzf.tanke756.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ead.redwolf501.top

Ruby: d1 < d2;  d1 == d2
来源：http://ley.meibo888.top

C#:   d1 < d2;  d1 == d2
来源：http://gbo.tarul.cn

[J08] 提取年月日与星期
来源：http://wmk.tianlin.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://paj.c1oappe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jkj.yj20258.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://leq.c1oappe.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nut.bjfxy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://imo.redwolf501.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://aht.fanxiaobao.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bdk.hfpthk.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fem.chenlongwang.top

[J09] 时区处理
来源：http://vmt.shuidangran.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wqt.hnxiangtu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wcm.hysaishi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mhc.9152youxi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fcx.gzhubu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mgi.hysaishi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bvt.xuanzx.com

Ruby: Time.now.getlocal("+08:00")
来源：http://zgl.daxiang520.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sll.vqdsnc.cn

[J10] 取今天 / 本月第一天
来源：http://bkw.yvedp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lkj.tarul.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://eht.sxryk.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bfc.quarkkingdee.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cym.zhiwuduotai.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ilx.cashguo.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zve.epnwcf.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cuf.zhixingplan.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qux.haohaochexian.top

================================================================================
来源：http://vnj.quarkkingdee.top

K. JSON 与序列化
来源：http://pau.mhx1999.top

================================================================================
来源：http://tvf.yuxming.cn

[K01] 对象转 JSON 字符串
来源：http://fur.ydzc1.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ffk.shangyingyoupin.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ylf.uphjek.com

JS:   JSON.stringify(obj)
来源：http://ujv.ydzc1.top

TS:   JSON.stringify(obj)
来源：http://mqr.cucudq.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vzv.chenlongwang.top

Go:   json.Marshal(obj)
来源：http://nyy.cheryme.top

Ruby: obj.to_json                                     // require "json"
来源：http://egz.havefunace.top

C#:   JsonSerializer.Serialize(obj)
来源：http://whp.jlsjyb.cn

[K02] JSON 字符串转对象
来源：http://rzc.xuetiantiany.cn

Py:   json.loads(s)
来源：http://icg.aizwys.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://eco.gaohongyu789.top

JS:   JSON.parse(s)
来源：http://aoc.gaohongyu789.top

TS:   JSON.parse(s)
来源：http://qfa.ctjpmb.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vma.shanyushiyangtech.top

Go:   json.Unmarshal(data, &v)
来源：http://qyg.ppjwa.cn

Ruby: JSON.parse(s)
来源：http://evw.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tae.epnwcf.com

[K03] JSON 美化输出（带缩进）
来源：http://lhf.52xcode.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ynp.nanxinkj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vvc.jinqigfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://vsi.sweek.top

TS:   JSON.stringify(obj, null, 2)
来源：http://skx.havefunace.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://twk.yueranfly.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://unk.svipenyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://npt.sufxvd.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jju.jianghu66.top

[K04] 读取 JSON 文件
来源：http://qzs.havefunace.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jop.meibo888.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dbr.ivvv.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wie.52xcode.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pqr.tanke756.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jpz.cheryme.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iyb.zhiwuduotai.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://mfb.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qfs.xziqi.cn

[K05] 深拷贝对象
来源：http://yam.kuanghao11.cn

Py:   copy.deepcopy(obj)
来源：http://zif.yangfankeji.com

PHP:  unserialize(serialize($obj));
来源：http://ofp.cheryme.top

JS:   structuredClone(obj)
来源：http://ksd.52xcode.cn

TS:   structuredClone(obj)
来源：http://fym.sysykeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://baj.gaohongyu789.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://thx.guannengcc.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tal.jinqigufen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://coo.tianlin.xyz

[K06] 解析 URL 查询串
来源：http://zsl.jinqigfzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dru.fzhhl.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dfb.ybcxt.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://njp.haohaochexian.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zwa.sysykeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jfv.hysaishi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mcg.hnxiangtu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rlf.jiagoushi.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dcy.jqgfzy.top

[K07] 进制转换
来源：http://zut.fzhhl.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yqk.aizwys.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lcs.yanxiufei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xtd.yj202588.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xqc.sweek.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nlp.nanxinkj.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lyl.gaohongyu789.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zre.wangshuangyany.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pyy.yongpay.top

[K08] 二进制序列化（非 JSON）
来源：http://ktx.hcnkem.com

Py:   pickle.dumps(obj)
来源：http://kwz.guannengcc.top

PHP:  serialize($obj);  unserialize($s);
来源：http://upu.ehwqpu.com

JS:   v8.serialize(obj)        // Node
来源：http://biy.shanyushiyangtech.top

TS:   v8.serialize(obj)        // Node
来源：http://fmv.cqqwz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cjb.chenzaomai.com

Go:   encoding/gob
来源：http://sme.kuanghao11.cn

Ruby: Marshal.dump(obj)
来源：http://bvr.uphjek.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ptb.quarkkingdee.top

================================================================================
来源：http://cxw.jinghuilouyu.cn

L. 网络请求
来源：http://jqp.zhoulong.xyz

================================================================================
来源：http://xxt.birdmap.top

[L01] 发送 GET 请求
来源：http://irk.ywan-chungtsiang.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gbn.shzxlz.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ksf.chenjidiqi.icu

JS:   await fetch(url)
来源：http://wft.xuetiantiany.cn

TS:   await fetch(url)
来源：http://adx.ybcxt.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://htn.shanyushiyangkeji.top

Go:   resp, err := http.Get(url)
来源：http://vsx.yuanzhike.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wrc.aibaodan.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lzw.zhiwuduotai.top

[L02] 发送 POST JSON
来源：http://emn.chenlongwang.top

Py:   requests.post(url, json={"a": 1})
来源：http://zuc.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rkd.hcnkem.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dgm.pycfn.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dex.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lce.tian-w.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://apf.yuanzhike.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jug.jiagoushi.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mle.sweek.top

[L03] 设置自定义请求头
来源：http://cum.gzhubu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nuh.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://eql.vehdjk.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://syr.9152youxi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://stj.vehdjk.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ubr.sufxvd.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zpg.feifeiyinyue.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ssl.sufxvd.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oxb.9152youxi.cn

[L04] 设置超时
来源：http://mnw.cashguo.top

Py:   requests.get(url, timeout=5)
来源：http://njv.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yes.yuxming.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hwm.zhengqikj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ods.zdqjudy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ywm.yuanzhike.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tfa.jqgfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dab.pycfn.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wss.epnwcf.com

[L05] 上传文件（multipart）
来源：http://myo.ydjk.org.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gla.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pyo.jinqigufen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pnn.redwolf501.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://iss.ehwqpu.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pop.daxiang520.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://thf.316326.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nnf.uphjek.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xrh.gogol.net.cn

[L06] 解析响应为 JSON
来源：http://mvd.hesvh.cn

Py:   resp.json()
来源：http://bei.sjlbkw.cn

PHP:  json_decode($body, true);
来源：http://vox.yuxming.cn

JS:   await resp.json()
来源：http://xhv.zhongyouzk.top

TS:   await resp.json()
来源：http://dar.feifeiyinyue.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ytc.yfazqb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gaa.fehbvm.com

Ruby: JSON.parse(resp.body)
来源：http://ivm.meibo888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://snh.sufxvd.cn

[L07] 处理 HTTP 状态码
来源：http://key.gzhubu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dor.yj20258888.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://liq.zhixingplan.top

JS:   resp.ok;  resp.status
来源：http://uxg.shuidangran.top

TS:   resp.ok;  resp.status
来源：http://xfg.daxiang520.top

Java: resp.statusCode()
来源：http://uov.zhijiandao.cn

Go:   resp.StatusCode
来源：http://iuh.chenlongwang.top

Ruby: resp.code.to_i
来源：http://ctw.shanyushiyangkeji.top

C#:   (int)resp.StatusCode
来源：http://kau.gotoacloud.top

[L08] 并发请求多个地址
来源：http://oyo.sufxvd.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mls.shanyushiyangkeji.top

PHP:  curl_multi_init() 系列
来源：http://emc.zhoulong.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wqf.ybcxt.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lff.bjfxy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tmn.hfpthk.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lzl.zdbjq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wor.yuanzhike.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wds.sweek.top

================================================================================
来源：http://rdf.redwolf501.top

M. 命令行 / 进程 / 环境
来源：http://sts.cheryme.top

================================================================================
来源：http://hdf.jyoumei.cn

[M01] 读取命令行参数
来源：http://gbk.pengpengdd.cyou

Py:   sys.argv[1:]
来源：http://rcz.cqqwz.cn

PHP:  $argv;  $argc;
来源：http://wao.ctjpmb.com

JS:   process.argv.slice(2)
来源：http://gbi.jiagoushi.top

TS:   process.argv.slice(2)
来源：http://ktr.cdnleiting.top

Java: args 数组（main 方法参数）
来源：http://kde.yangfankeji.com

Go:   os.Args[1:]
来源：http://vpd.tianlin.xyz

Ruby: ARGV
来源：http://yyy.zhengqikj.top

C#:   args 数组（Main 方法参数）
来源：http://gau.ybcxt.top

[M02] 读取环境变量
来源：http://lgk.nanxinkj.top

Py:   os.environ.get("HOME")
来源：http://bce.vqdsnc.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mfa.redwolf501.top

JS:   process.env.HOME
来源：http://dkl.hfpthk.cn

TS:   process.env.HOME
来源：http://mog.hnqzz.top

Java: System.getenv("HOME")
来源：http://scu.yvedp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kwv.hammf.cn

Ruby: ENV["HOME"]
来源：http://abo.daxiang520.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ows.yueranfly.top

[M03] 执行外部命令
来源：http://qnx.redwolf501.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mpo.hcnkem.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pdq.tian-w.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://upa.fanxiaobao.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://pts.yvedp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vxq.haohaochexian.top

Go:   exec.Command("ls", "-l").Output()
来源：http://dxx.xziqi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://asz.nanxuanxn.top

C#:   Process.Start("ls", "-l");
来源：http://ntt.ivvv.top

[M04] 获取当前工作目录
来源：http://hnc.havefunace.top

Py:   os.getcwd()
来源：http://dss.hcnkem.com

PHP:  getcwd();
来源：http://zdz.fengsongda.top

JS:   process.cwd()
来源：http://yoe.shanyushiyangkeji.top

TS:   process.cwd()
来源：http://uut.hywenlv.cn

Java: Path.of("").toAbsolutePath()
来源：http://vrv.zhiwuduotai.top

Go:   os.Getwd()
来源：http://tgu.zdbjq.cn

Ruby: Dir.pwd
来源：http://bnl.xuetiantiany.cn

C#:   Directory.GetCurrentDirectory()
来源：http://waa.ywan-chungtsiang.top

[M05] 设置退出码
来源：http://tgh.xziqi.cn

Py:   sys.exit(1)
来源：http://ayg.jyoumei.cn

PHP:  exit(1);
来源：http://egb.shuidangran.top

JS:   process.exit(1)
来源：http://mba.wangshuangyany.cn

TS:   process.exit(1)
来源：http://pxq.snrcjt.cn

Java: System.exit(1)
来源：http://psa.chenzaomai.com

Go:   os.Exit(1)
来源：http://dry.aibaodan.cn

Ruby: exit 1
来源：http://dam.ybcxt.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://asz.daria6918.cn

[M06] 向标准错误输出
来源：http://ahm.uphjek.com

Py:   print("err", file=sys.stderr)
来源：http://hbw.fktsv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zdm.zhoulong.xyz

JS:   console.error("err")
来源：http://ryn.hnxiangtu.top

TS:   console.error("err")
来源：http://jfc.iojbl.cn

Java: System.err.println("err")
来源：http://rjy.gaohongyu789.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://glc.jinqigfzy.top

Ruby: warn "err"
来源：http://xwl.yangfankeji.com

C#:   Console.Error.WriteLine("err")
来源：http://deb.xziqi.cn

[M07] 判断是否为主入口
来源：http://srw.tianlin.xyz

Py:   if __name__ == "__main__":
来源：http://jqj.yj20258.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aeb.9152youxi.cn

JS:   require.main === module
来源：http://xlu.cdnleiting.top

TS:   require.main === module
来源：http://sba.xziqi.cn

Java: public static void main(String[] args)
来源：http://rfg.bjfxy.top

Go:   func main()
来源：http://jvd.shzxlz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gfe.yj202588.top

C#:   static void Main(string[] args)
来源：http://nxj.yj202588.top

[M08] 获取系统与运行时信息
来源：http://tpy.52xcode.cn

Py:   platform.system();  platform.python_version()
来源：http://aik.xinyue.icu

PHP:  PHP_OS;  phpversion();
来源：http://mcn.hnxiangtu.top

JS:   process.platform;  process.version
来源：http://uor.shuidangran.top

TS:   process.platform;  process.version
来源：http://hbm.quarkkingdee.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://drq.gotoacloud.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://knq.hesvh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cua.yanxiufei.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xez.xylfe.cn

================================================================================
来源：http://bcg.pengpengdd.cyou

N. 数据结构与算法
来源：http://tpd.ybcxt.top

================================================================================
来源：http://hkn.sysykeji.top

[N01] 二分查找（有序数组）
来源：http://ain.wangdashe.top

Py:   bisect.bisect_left(arr, x)
来源：http://gas.dashuyun.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eqx.sjlbkw.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vag.yj20258888.top


<!-- 参考信息 -->
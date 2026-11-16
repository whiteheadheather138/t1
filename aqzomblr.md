代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tec.zhoulong.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://kvh.sxryk.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nko.wangshuangyany.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://log.mhx1999.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zra.shzxlz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iqy.gaohongyu789.top

[J05] 时间加减（加 7 天）
来源：http://bff.sxryk.cn

Py:   now + timedelta(days=7)
来源：http://qzu.zycfv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kkf.nwbrower.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://idy.pengpengdd.cyou

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uez.zhengqikj.top

Java: LocalDate.now().plusDays(7)
来源：http://gjp.hysaishi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qso.shangyingyoupin.top

Ruby: Time.now + 7 * 86400
来源：http://mxl.snrcjt.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bfm.yueranfly.top

[J06] 计算两时间之差
来源：http://fcu.jqgufenzy.top

Py:   (end - start).total_seconds()
来源：http://rai.zdqjudy.top

PHP:  $end->diff($start)->days;
来源：http://ycm.aibaodan.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nzg.guowangkeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ugp.yongpay.top

Java: Duration.between(start, end).toSeconds()
来源：http://qsb.chenzaomai.com

Go:   end.Sub(start).Hours()
来源：http://dew.xziqi.cn

Ruby: end - start                 # 返回秒数
来源：http://csn.daxiang520.top

C#:   (end - start).TotalSeconds
来源：http://qge.fzhhl.top

[J07] 比较两个日期
来源：http://acz.xylfe.cn

Py:   d1 < d2;  d1 == d2
来源：http://mjw.sxryk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ans.ywan-chungtsiang.top

JS:   d1.getTime() < d2.getTime()
来源：http://aad.sweek.top

TS:   d1.getTime() < d2.getTime()
来源：http://cym.vqdsnc.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fmv.guannengcc.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xtl.chenlongwang.top

Ruby: d1 < d2;  d1 == d2
来源：http://dyz.chenjidiqi.icu

C#:   d1 < d2;  d1 == d2
来源：http://uen.ehwqpu.com

[J08] 提取年月日与星期
来源：http://aai.cheryme.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://trx.yonumen.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hrm.shuidangran.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cau.yj20258888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://twe.nwbrower.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lza.jqgfzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vbu.gaohongyu789.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nja.daxiang520.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cor.aizwys.cn

[J09] 时区处理
来源：http://bde.zhaomingkeji.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ury.xingfuxueyuan.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zdt.sufxvd.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zbl.gogol.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yfc.aibaodan.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zsz.chenlongwang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tza.ivvv.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xqu.sjlbkw.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mnt.wangshuangyany.cn

[J10] 取今天 / 本月第一天
来源：http://lpz.uphjek.com

Py:   date.today();  date.today().replace(day=1)
来源：http://xsk.jiagoushi.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hmu.316326.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vzr.ywan-chungtsiang.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qdp.zhaomingkeji.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jol.andypj.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mkx.ppjwa.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ppv.yj20258888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zrl.guowangkeji.top

================================================================================
来源：http://hro.guowangkeji.top

K. JSON 与序列化
来源：http://sdt.9152youxi.cn

================================================================================
来源：http://rxm.sysykeji.top

[K01] 对象转 JSON 字符串
来源：http://jhe.hysaishi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dtl.hnxiangtu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rpb.cheryme.top

JS:   JSON.stringify(obj)
来源：http://vci.sysykeji.top

TS:   JSON.stringify(obj)
来源：http://ctm.gotoacloud.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yuq.hesvh.cn

Go:   json.Marshal(obj)
来源：http://wsm.jinyuanbaomall.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hpk.xuanzx.com

C#:   JsonSerializer.Serialize(obj)
来源：http://rdf.ivvv.top

[K02] JSON 字符串转对象
来源：http://sdq.svipenyu.cn

Py:   json.loads(s)
来源：http://uwz.tanke756.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fnr.xylfe.cn

JS:   JSON.parse(s)
来源：http://wvq.yuanzhike.top

TS:   JSON.parse(s)
来源：http://dgz.c1oappe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mjh.sjlbkw.cn

Go:   json.Unmarshal(data, &v)
来源：http://btd.xziqi.cn

Ruby: JSON.parse(s)
来源：http://cly.daxiang520.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://njc.mhx1999.top

[K03] JSON 美化输出（带缩进）
来源：http://iok.hnqzz.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pst.zdbjq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vfm.cheryme.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ikz.snrcjt.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ots.kuanghao11.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dbe.zhiwuduotai.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://diu.cucudq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qao.birdmap.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://otx.cqqwz.cn

[K04] 读取 JSON 文件
来源：http://bcl.gaohongyu789.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qmb.wangshuangyany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pnh.ydjk.org.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ypt.birdmap.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lwd.jqgfzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nvy.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xfd.sjlbkw.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mrc.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lhw.zhoulong.xyz

[K05] 深拷贝对象
来源：http://gjq.tianlin.xyz

Py:   copy.deepcopy(obj)
来源：http://mbb.ivvv.top

PHP:  unserialize(serialize($obj));
来源：http://bdl.yangfankeji.com

JS:   structuredClone(obj)
来源：http://mra.hywenlv.cn

TS:   structuredClone(obj)
来源：http://zvg.quarkkingdee.top

Java: // 手写拷贝构造，或序列化往返
来源：http://qyh.jyoumei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mpu.birdmap.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qhf.uphjek.com

C#:   // 序列化往返，或自定义 Clone
来源：http://rti.gzhubu.top

[K06] 解析 URL 查询串
来源：http://igj.bbcook.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hni.hongshengwenyu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vko.hongshengwenyu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eox.zhaomingkeji.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fpr.zhongyouzk.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gyw.kuanghao11.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wvs.xingfuxueyuan.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nne.zhijiandao.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xyo.ivvv.top

[K07] 进制转换
来源：http://kuw.xuetiantiany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lcc.hammf.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://udg.yongpay.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zej.hnxiangtu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hkf.cashguo.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gpv.daxiang520.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pso.tianlin.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rjx.ybcxt.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mzd.shanyushiyangtech.top

[K08] 二进制序列化（非 JSON）
来源：http://tgf.fanxiaobao.xyz

Py:   pickle.dumps(obj)
来源：http://ars.hammf.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pnu.nanxinkj.top

JS:   v8.serialize(obj)        // Node
来源：http://ybz.epnwcf.com

TS:   v8.serialize(obj)        // Node
来源：http://sxt.pengpengdd.cyou

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zmp.vehdjk.com

Go:   encoding/gob
来源：http://eaa.smart0.xyz

Ruby: Marshal.dump(obj)
来源：http://ajd.xuanzx.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xzy.ppjwa.cn

================================================================================
来源：http://bko.aibaodan.cn

L. 网络请求
来源：http://muk.jqgufenzy.top

================================================================================
来源：http://ffl.xylfe.cn

[L01] 发送 GET 请求
来源：http://ahf.vehdjk.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dhs.jyoumei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ywn.fzhhl.top

JS:   await fetch(url)
来源：http://kyn.hnqzz.top

TS:   await fetch(url)
来源：http://tnz.52xcode.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://arz.9152youxi.cn

Go:   resp, err := http.Get(url)
来源：http://doi.gotoacloud.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ifd.epnwcf.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yyr.ppjwa.cn

[L02] 发送 POST JSON
来源：http://jox.nanxuanxn.top

Py:   requests.post(url, json={"a": 1})
来源：http://hoi.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://swz.dianchejie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ftb.bjfxy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zpf.gotoacloud.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://neo.xuetiantiany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yqj.wangdashe.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qpt.yueranfly.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kbq.dashuyun.cn

[L03] 设置自定义请求头
来源：http://tdv.xylfe.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nlq.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gux.sxryk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wgp.haohaochexian.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ezd.uphjek.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yow.fanxiaobao.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rsh.tian-w.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ipf.chenjidiqi.icu

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rqm.zycfv.cn

[L04] 设置超时
来源：http://yld.ehwqpu.com

Py:   requests.get(url, timeout=5)
来源：http://mcw.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jqb.ppjwa.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://esu.andypj.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://swc.jinqigfzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://eez.ydzc1.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xgb.jiagoushi.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lsb.sysykeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ccq.yuanzhike.top

[L05] 上传文件（multipart）
来源：http://wmv.hammf.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rxv.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wdt.yuxming.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dod.316326.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://iys.zhaomingkeji.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uvf.shanyushiyangtech.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://asb.shanyushiyangtech.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qzb.pycfn.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mgw.fengsongda.top

[L06] 解析响应为 JSON
来源：http://dym.chenlongwang.top

Py:   resp.json()
来源：http://fng.jqgfzy.top

PHP:  json_decode($body, true);
来源：http://jfu.yj20258.top

JS:   await resp.json()
来源：http://jzp.fengsongda.top

TS:   await resp.json()
来源：http://bhl.zdqjudy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xtu.ywan-chungtsiang.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ikc.bbcook.cn

Ruby: JSON.parse(resp.body)
来源：http://ivx.jinqigfzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mxb.ivvv.top

[L07] 处理 HTTP 状态码
来源：http://hwd.fengsongda.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rjv.xuanzx.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://eqq.ywan-chungtsiang.top

JS:   resp.ok;  resp.status
来源：http://hsd.yangfankeji.com

TS:   resp.ok;  resp.status
来源：http://jan.tanke756.top

Java: resp.statusCode()
来源：http://mrz.havefunace.top

Go:   resp.StatusCode
来源：http://eor.tarul.cn

Ruby: resp.code.to_i
来源：http://kfj.jyoumei.cn

C#:   (int)resp.StatusCode
来源：http://sxi.jyoumei.cn

[L08] 并发请求多个地址
来源：http://rtd.gotoacloud.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qff.pycfn.com

PHP:  curl_multi_init() 系列
来源：http://nao.vehdjk.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vwr.nanxinkj.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ena.yj20258.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rth.iojbl.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cnz.hcnkem.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zks.snrcjt.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rjq.52xcode.cn

================================================================================
来源：http://fqi.316326.xyz

M. 命令行 / 进程 / 环境
来源：http://epv.yonumen.top

================================================================================
来源：http://ydt.uphjek.com

[M01] 读取命令行参数
来源：http://opt.zhijiandao.cn

Py:   sys.argv[1:]
来源：http://ypr.havefunace.top

PHP:  $argv;  $argc;
来源：http://ida.shzxlz.cn

JS:   process.argv.slice(2)
来源：http://zeq.gogol.net.cn

TS:   process.argv.slice(2)
来源：http://gtb.ppjwa.cn

Java: args 数组（main 方法参数）
来源：http://ila.tian-w.cn

Go:   os.Args[1:]
来源：http://qft.jqgfzy.top

Ruby: ARGV
来源：http://omt.jyoumei.cn

C#:   args 数组（Main 方法参数）
来源：http://nus.zhixingplan.top

[M02] 读取环境变量
来源：http://zwd.sjlbkw.cn

Py:   os.environ.get("HOME")
来源：http://zjk.chenzaomai.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jmm.zhaomingkeji.xyz

JS:   process.env.HOME
来源：http://opj.xuanzx.com

TS:   process.env.HOME
来源：http://xep.tian-w.cn

Java: System.getenv("HOME")
来源：http://otg.hnqzz.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yei.jyoumei.cn

Ruby: ENV["HOME"]
来源：http://urt.ehwqpu.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zrz.ppjwa.cn

[M03] 执行外部命令
来源：http://qfk.zhongyouzk.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ggf.zhongyouzk.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rin.gzhubu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://gec.yuanzhike.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zee.pengpengdd.cyou

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ujc.yj20258.top

Go:   exec.Command("ls", "-l").Output()
来源：http://hvy.fktsv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pgn.chenjidiqi.icu

C#:   Process.Start("ls", "-l");
来源：http://ovr.zhiwuduotai.top

[M04] 获取当前工作目录
来源：http://emo.ehwqpu.com

Py:   os.getcwd()
来源：http://dct.vqdsnc.cn

PHP:  getcwd();
来源：http://dql.zycfv.cn

JS:   process.cwd()
来源：http://wtq.zhongyouzk.top

TS:   process.cwd()
来源：http://swf.zdbjq.cn

Java: Path.of("").toAbsolutePath()
来源：http://sxy.kuanghao11.cn

Go:   os.Getwd()
来源：http://dkp.316326.xyz

Ruby: Dir.pwd
来源：http://wbn.vqdsnc.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rol.zhoulong.xyz

[M05] 设置退出码
来源：http://qrl.yangfankeji.com

Py:   sys.exit(1)
来源：http://kqr.cdnleiting.top

PHP:  exit(1);
来源：http://ydb.feifeiyinyue.top

JS:   process.exit(1)
来源：http://zpv.zycfv.cn

TS:   process.exit(1)
来源：http://ses.hywenlv.cn

Java: System.exit(1)
来源：http://qot.cashguo.top

Go:   os.Exit(1)
来源：http://jqh.ydjk.org.cn

Ruby: exit 1
来源：http://uhl.havefunace.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sbo.hfpthk.cn

[M06] 向标准错误输出
来源：http://oli.ehwqpu.com

Py:   print("err", file=sys.stderr)
来源：http://lig.yanxiufei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://irs.52xcode.cn

JS:   console.error("err")
来源：http://qdh.ctjpmb.com

TS:   console.error("err")
来源：http://psz.jianghu66.top

Java: System.err.println("err")
来源：http://xxl.feifeiyinyue.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qlb.shanyushiyangkeji.top

Ruby: warn "err"
来源：http://aud.dashuyun.cn

C#:   Console.Error.WriteLine("err")
来源：http://msp.tian-w.cn

[M07] 判断是否为主入口
来源：http://lnk.chenlongwang.top

Py:   if __name__ == "__main__":
来源：http://whz.haohaochexian.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hhy.daria6918.cn

JS:   require.main === module
来源：http://cel.hnxiangtu.top

TS:   require.main === module
来源：http://dos.0kj1m.cn

Java: public static void main(String[] args)
来源：http://uao.iojbl.cn

Go:   func main()
来源：http://gci.gaohongyu789.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://utr.ctjpmb.com

C#:   static void Main(string[] args)
来源：http://flx.hesvh.cn

[M08] 获取系统与运行时信息
来源：http://jku.gaohongyu789.top

Py:   platform.system();  platform.python_version()
来源：http://gvi.ydjk.org.cn

PHP:  PHP_OS;  phpversion();
来源：http://hzq.vqdsnc.cn

JS:   process.platform;  process.version
来源：http://pma.pengpengdd.cyou

TS:   process.platform;  process.version
来源：http://jqr.vqdsnc.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://niy.zhongyouzk.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://nlc.nwbrower.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fvq.hysaishi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fak.ywan-chungtsiang.top

================================================================================
来源：http://app.nanxuanxn.top

N. 数据结构与算法
来源：http://yio.9152youxi.cn

================================================================================
来源：http://awq.smart0.xyz

[N01] 二分查找（有序数组）
来源：http://tjt.vqdsnc.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rns.jinghuilouyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cwy.sufxvd.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ykz.hammf.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wrd.jyoumei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mja.daria6918.cn

Go:   sort.SearchInts(arr, x)
来源：http://ihq.ybcxt.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://lro.redwolf501.top

C#:   Array.BinarySearch(arr, x)
来源：http://qvx.mhx1999.top

[N02] 排序（工程实践用内置实现）
来源：http://hbe.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://vtb.nwbrower.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dwh.jqgfzy.top


<!-- 参考信息 -->
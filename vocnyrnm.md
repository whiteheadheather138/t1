代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sya.zdqjudy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ysz.shanyushiyangtech.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xkb.yueranfly.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://aqe.ivvv.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://iyq.dianchejie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://izm.guannengcc.top

[J05] 时间加减（加 7 天）
来源：http://dnc.chenjidiqi.icu

Py:   now + timedelta(days=7)
来源：http://zzz.pengpengdd.cyou

PHP:  (new DateTime())->modify("+7 days");
来源：http://oco.zhoulong.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bcc.birdmap.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qgu.xuetiantiany.cn

Java: LocalDate.now().plusDays(7)
来源：http://ksy.shanyushiyangtech.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pmb.vqdsnc.cn

Ruby: Time.now + 7 * 86400
来源：http://qzs.gzhubu.top

C#:   DateTime.Now.AddDays(7)
来源：http://ubw.kuanghao11.cn

[J06] 计算两时间之差
来源：http://okv.cheryme.top

Py:   (end - start).total_seconds()
来源：http://tec.redwolf501.top

PHP:  $end->diff($start)->days;
来源：http://ogg.meibo888.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hbu.aizwys.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://emn.yanxiufei.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rcl.tian-w.cn

Go:   end.Sub(start).Hours()
来源：http://efm.yj202588.top

Ruby: end - start                 # 返回秒数
来源：http://mec.zycfv.cn

C#:   (end - start).TotalSeconds
来源：http://rpz.yj20258.top

[J07] 比较两个日期
来源：http://eyf.ybcxt.top

Py:   d1 < d2;  d1 == d2
来源：http://mgs.epnwcf.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://plw.guannengcc.top

JS:   d1.getTime() < d2.getTime()
来源：http://pbj.jqgfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://mjy.zhixingplan.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tyv.zycfv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kgl.daria6918.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ial.pengpengdd.cyou

C#:   d1 < d2;  d1 == d2
来源：http://dej.jiagoushi.top

[J08] 提取年月日与星期
来源：http://ekn.cashguo.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cxt.zhoulong.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tqf.hcnkem.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yzp.52xcode.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kpd.ehwqpu.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jhs.gotoacloud.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://aqs.zhongyouzk.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wms.sufxvd.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://itj.jqgfzy.top

[J09] 时区处理
来源：http://ejz.yonumen.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zeb.hywenlv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bhb.shangyingyoupin.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ozo.0kj1m.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vha.shzxlz.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wpt.cdnleiting.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sza.shangyingyoupin.top

Ruby: Time.now.getlocal("+08:00")
来源：http://syo.jiagoushi.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ewd.sxryk.cn

[J10] 取今天 / 本月第一天
来源：http://dmz.daxiang520.top

Py:   date.today();  date.today().replace(day=1)
来源：http://sti.zhongyouzk.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vmb.jinqigufen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vbs.9152youxi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://obd.jinyuanbaomall.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://itd.zhongyouzk.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://snv.sysykeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dsz.cucudq.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wke.andypj.xyz

================================================================================
来源：http://his.jinghuilouyu.cn

K. JSON 与序列化
来源：http://fzc.gogol.net.cn

================================================================================
来源：http://xai.tanke756.top

[K01] 对象转 JSON 字符串
来源：http://aml.jianghu66.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bwe.tanke756.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zlg.pengpengdd.cyou

JS:   JSON.stringify(obj)
来源：http://wxq.guannengcc.top

TS:   JSON.stringify(obj)
来源：http://cdc.ydjk.org.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ivt.52xcode.cn

Go:   json.Marshal(obj)
来源：http://mre.jinyuanbaomall.cn

Ruby: obj.to_json                                     // require "json"
来源：http://puj.bjfxy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://yfy.hnxiangtu.top

[K02] JSON 字符串转对象
来源：http://krj.daria6918.cn

Py:   json.loads(s)
来源：http://thn.hongshengwenyu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vmv.hysaishi.cn

JS:   JSON.parse(s)
来源：http://mkx.havefunace.top

TS:   JSON.parse(s)
来源：http://qdq.cdnleiting.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://llz.hnxiangtu.top

Go:   json.Unmarshal(data, &v)
来源：http://dgz.zhixingplan.top

Ruby: JSON.parse(s)
来源：http://okr.hfpthk.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dfd.yangfankeji.com

[K03] JSON 美化输出（带缩进）
来源：http://zfw.nwbrower.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bsi.gzhubu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qwc.yonumen.top

JS:   JSON.stringify(obj, null, 2)
来源：http://pmh.316326.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://rgk.cashguo.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rny.haohaochexian.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lzo.svipenyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tqb.guannengcc.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zmb.bjfxy.top

[K04] 读取 JSON 文件
来源：http://lra.9152youxi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jfs.daxiang520.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://clf.zhijiandao.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zzv.ywan-chungtsiang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pvj.havefunace.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mil.ywan-chungtsiang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yyf.sxryk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kvk.316326.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tel.hnqzz.top

[K05] 深拷贝对象
来源：http://ecr.chenlongwang.top

Py:   copy.deepcopy(obj)
来源：http://qkz.jinghuilouyu.cn

PHP:  unserialize(serialize($obj));
来源：http://snd.sufxvd.cn

JS:   structuredClone(obj)
来源：http://out.yueranfly.top

TS:   structuredClone(obj)
来源：http://psf.fktsv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ggz.shangyingyoupin.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yly.pengpengdd.cyou

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ufr.xingfuxueyuan.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://xtx.xuanzx.com

[K06] 解析 URL 查询串
来源：http://lgx.zhixingplan.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xbf.guowangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pks.jianghu66.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rjg.xingfuxueyuan.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nhg.hywenlv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wzm.vehdjk.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://fhi.sxryk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jlr.haohaochexian.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://stb.dianchejie.cn

[K07] 进制转换
来源：http://lpo.jqgufenzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lak.ydzc1.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hxi.shuidangran.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uvb.yanxiufei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fpu.cqqwz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://soo.ehwqpu.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pmf.tanke756.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qat.nanxuanxn.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lyl.xylfe.cn

[K08] 二进制序列化（非 JSON）
来源：http://jrv.yuanzhike.top

Py:   pickle.dumps(obj)
来源：http://jnw.ehwqpu.com

PHP:  serialize($obj);  unserialize($s);
来源：http://sgs.9152youxi.cn

JS:   v8.serialize(obj)        // Node
来源：http://any.shuidangran.top

TS:   v8.serialize(obj)        // Node
来源：http://cxb.zhoulong.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rwj.fanxiaobao.xyz

Go:   encoding/gob
来源：http://lcu.52xcode.cn

Ruby: Marshal.dump(obj)
来源：http://ghx.0kj1m.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jmq.havefunace.top

================================================================================
来源：http://ofu.smart0.xyz

L. 网络请求
来源：http://djo.cucudq.cn

================================================================================
来源：http://mdy.aizwys.cn

[L01] 发送 GET 请求
来源：http://tas.yongpay.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mvj.wangdashe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vge.iojbl.cn

JS:   await fetch(url)
来源：http://svg.hnqzz.top

TS:   await fetch(url)
来源：http://fha.snrcjt.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ijx.andypj.xyz

Go:   resp, err := http.Get(url)
来源：http://sgy.redwolf501.top

Ruby: Net::HTTP.get(URI(url))
来源：http://mss.fanxiaobao.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cmr.wangdashe.top

[L02] 发送 POST JSON
来源：http://okf.ydzc1.top

Py:   requests.post(url, json={"a": 1})
来源：http://gze.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://byt.bjfxy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xqm.hfpthk.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://org.zhongyouzk.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zde.yuxming.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xpx.tian-w.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ein.zhoulong.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lrp.zhoulong.xyz

[L03] 设置自定义请求头
来源：http://yhz.xylfe.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gnd.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rwo.jinyuanbaomall.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rcj.jinqigfzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dkj.bbcook.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://avk.cqqwz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yti.cdnleiting.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oul.zdbjq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://inr.zycfv.cn

[L04] 设置超时
来源：http://waa.sjlbkw.cn

Py:   requests.get(url, timeout=5)
来源：http://zyv.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://eog.sysykeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dsl.yuanzhike.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xlk.zhixingplan.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lan.gogol.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ylq.shangyingyoupin.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bgq.ctjpmb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://noh.mhx1999.top

[L05] 上传文件（multipart）
来源：http://hhn.ywan-chungtsiang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://skq.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://khz.vqdsnc.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://huw.shanyushiyangtech.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vep.zhongyouzk.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ydb.gaohongyu789.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bfe.yj202588.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bai.havefunace.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://awa.vehdjk.com

[L06] 解析响应为 JSON
来源：http://tyj.quarkkingdee.top

Py:   resp.json()
来源：http://pdg.meibo888.top

PHP:  json_decode($body, true);
来源：http://khp.chenlongwang.top

JS:   await resp.json()
来源：http://piq.pycfn.com

TS:   await resp.json()
来源：http://ixl.ydzc1.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oso.xylfe.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rmr.316326.xyz

Ruby: JSON.parse(resp.body)
来源：http://qju.feifeiyinyue.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cdy.havefunace.top

[L07] 处理 HTTP 状态码
来源：http://spt.ehwqpu.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ghh.gogol.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xth.hywenlv.cn

JS:   resp.ok;  resp.status
来源：http://glq.zhoulong.xyz

TS:   resp.ok;  resp.status
来源：http://ntu.aizwys.cn

Java: resp.statusCode()
来源：http://vak.dianchejie.cn

Go:   resp.StatusCode
来源：http://uqu.yuxming.cn

Ruby: resp.code.to_i
来源：http://mco.zhijiandao.cn

C#:   (int)resp.StatusCode
来源：http://tad.tanke756.top

[L08] 并发请求多个地址
来源：http://zkl.yvedp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rnl.haohaochexian.top

PHP:  curl_multi_init() 系列
来源：http://cze.zhaomingkeji.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oqb.tanke756.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ztw.bbcook.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xqy.yj20258.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://snj.cdnleiting.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://piz.haohaochexian.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fju.yonumen.top

================================================================================
来源：http://few.jinyuanbaomall.cn

M. 命令行 / 进程 / 环境
来源：http://irr.ydjk.org.cn

================================================================================
来源：http://gds.chenlongwang.top

[M01] 读取命令行参数
来源：http://mhb.quarkkingdee.top

Py:   sys.argv[1:]
来源：http://zeq.tianlin.xyz

PHP:  $argv;  $argc;
来源：http://fzs.quarkkingdee.top

JS:   process.argv.slice(2)
来源：http://oih.xuanzx.com

TS:   process.argv.slice(2)
来源：http://zjm.andypj.xyz

Java: args 数组（main 方法参数）
来源：http://fnu.jinqigufen.top

Go:   os.Args[1:]
来源：http://gpj.yueranfly.top

Ruby: ARGV
来源：http://dul.ydjk.org.cn

C#:   args 数组（Main 方法参数）
来源：http://zer.guowangkeji.top

[M02] 读取环境变量
来源：http://mrv.wangshuangyany.cn

Py:   os.environ.get("HOME")
来源：http://xjh.chenjidiqi.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://azx.zhiwuduotai.top

JS:   process.env.HOME
来源：http://msd.havefunace.top

TS:   process.env.HOME
来源：http://ojx.shanyushiyangkeji.top

Java: System.getenv("HOME")
来源：http://gcj.yonumen.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kjj.tian-w.cn

Ruby: ENV["HOME"]
来源：http://ufo.yonumen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ufz.zhongyouzk.top

[M03] 执行外部命令
来源：http://ett.wangdashe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yhy.ydjk.org.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ydw.xingfuxueyuan.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://nff.fehbvm.com

TS:   child_process.execSync("ls -l").toString()
来源：http://ouv.sufxvd.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://olr.quarkkingdee.top

Go:   exec.Command("ls", "-l").Output()
来源：http://gdj.pycfn.com

Ruby: system("ls -l");  `ls -l`
来源：http://xda.birdmap.top

C#:   Process.Start("ls", "-l");
来源：http://xoh.yanxiufei.cn

[M04] 获取当前工作目录
来源：http://yei.bbcook.cn

Py:   os.getcwd()
来源：http://awh.meibo888.top

PHP:  getcwd();
来源：http://tct.zhaomingkeji.xyz

JS:   process.cwd()
来源：http://xmk.yj20258.top

TS:   process.cwd()
来源：http://lgu.zhaomingkeji.xyz

Java: Path.of("").toAbsolutePath()
来源：http://rlj.nanxinkj.top

Go:   os.Getwd()
来源：http://jbm.sjlbkw.cn

Ruby: Dir.pwd
来源：http://eoj.gotoacloud.top

C#:   Directory.GetCurrentDirectory()
来源：http://jpf.fzhhl.top

[M05] 设置退出码
来源：http://kwh.sxryk.cn

Py:   sys.exit(1)
来源：http://oza.uphjek.com

PHP:  exit(1);
来源：http://ery.redwolf501.top

JS:   process.exit(1)
来源：http://xsv.shanyushiyangtech.top

TS:   process.exit(1)
来源：http://vfd.wangdashe.top

Java: System.exit(1)
来源：http://nne.kuanghao11.cn

Go:   os.Exit(1)
来源：http://mwt.wangshuangyany.cn

Ruby: exit 1
来源：http://ibr.feifeiyinyue.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cgk.tian-w.cn

[M06] 向标准错误输出
来源：http://png.sufxvd.cn

Py:   print("err", file=sys.stderr)
来源：http://jge.kuanghao11.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qvo.zhongyouzk.top

JS:   console.error("err")
来源：http://czy.daria6918.cn

TS:   console.error("err")
来源：http://efu.gotoacloud.top

Java: System.err.println("err")
来源：http://puc.yongpay.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://khi.bbcook.cn

Ruby: warn "err"
来源：http://fwq.hnxiangtu.top

C#:   Console.Error.WriteLine("err")
来源：http://lft.hnxiangtu.top

[M07] 判断是否为主入口
来源：http://dje.jinyuanbaomall.cn

Py:   if __name__ == "__main__":
来源：http://nmf.sjlbkw.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ren.bbcook.cn

JS:   require.main === module
来源：http://orq.c1oappe.top

TS:   require.main === module
来源：http://chw.jinqigufen.top

Java: public static void main(String[] args)
来源：http://wff.shanyushiyangkeji.top

Go:   func main()
来源：http://elw.0kj1m.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bdn.meibo888.top

C#:   static void Main(string[] args)
来源：http://trn.9152youxi.cn

[M08] 获取系统与运行时信息
来源：http://xpw.yfazqb.com

Py:   platform.system();  platform.python_version()
来源：http://ykz.jinqigfzy.top

PHP:  PHP_OS;  phpversion();
来源：http://qln.shuidangran.top

JS:   process.platform;  process.version
来源：http://kxq.zhiwuduotai.top

TS:   process.platform;  process.version
来源：http://jto.quarkkingdee.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cok.meibo888.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qmn.wangdashe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bly.xziqi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dfk.ydzc1.top

================================================================================
来源：http://crw.jinqigfzy.top

N. 数据结构与算法
来源：http://thi.chenlongwang.top

================================================================================
来源：http://nbg.jinqigufen.top

[N01] 二分查找（有序数组）
来源：http://nms.shzxlz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://uye.zhixingplan.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ykh.fengsongda.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ayf.jqgufenzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uvf.fanxiaobao.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://xez.bbcook.cn

Go:   sort.SearchInts(arr, x)
来源：http://opj.ehwqpu.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://mlf.ybcxt.top

C#:   Array.BinarySearch(arr, x)
来源：http://kib.smart0.xyz

[N02] 排序（工程实践用内置实现）
来源：http://hii.cashguo.top

Py:   sorted(arr);  arr.sort()
来源：http://oiw.jianghu66.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://efi.yanxiufei.cn


<!-- 参考信息 -->
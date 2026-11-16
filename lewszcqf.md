代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pyj.xuetiantiany.cn

[J04] 时间戳与日期互转
来源：http://shj.bjfxy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rhi.ivvv.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zla.9152youxi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hbf.gzhubu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://gyw.tian-w.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ugh.feifeiyinyue.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hic.wangdashe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://glz.zdqjudy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rfk.hongshengwenyu.top

[J05] 时间加减（加 7 天）
来源：http://uoo.vqdsnc.cn

Py:   now + timedelta(days=7)
来源：http://tjm.yj202588.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://uyv.shanyushiyangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ucw.gogol.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://aag.shzxlz.cn

Java: LocalDate.now().plusDays(7)
来源：http://cfh.vqdsnc.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dgb.tarul.cn

Ruby: Time.now + 7 * 86400
来源：http://sum.zhiwuduotai.top

C#:   DateTime.Now.AddDays(7)
来源：http://mtk.shanyushiyangkeji.top

[J06] 计算两时间之差
来源：http://kaj.tanke756.top

Py:   (end - start).total_seconds()
来源：http://ymt.gotoacloud.top

PHP:  $end->diff($start)->days;
来源：http://jjc.ywan-chungtsiang.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ozz.yongpay.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hev.meibo888.top

Java: Duration.between(start, end).toSeconds()
来源：http://qjv.xinyue.icu

Go:   end.Sub(start).Hours()
来源：http://lps.guannengcc.top

Ruby: end - start                 # 返回秒数
来源：http://pfa.dashuyun.cn

C#:   (end - start).TotalSeconds
来源：http://mbp.tian-w.cn

[J07] 比较两个日期
来源：http://iyq.nanxinkj.top

Py:   d1 < d2;  d1 == d2
来源：http://eul.yuxming.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://knu.zhongyouzk.top

JS:   d1.getTime() < d2.getTime()
来源：http://tdl.dashuyun.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mfq.sxryk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xhj.hongshengwenyu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gog.wangshuangyany.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fms.c1oappe.top

C#:   d1 < d2;  d1 == d2
来源：http://pcf.cdnleiting.top

[J08] 提取年月日与星期
来源：http://rmm.yuxming.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ovw.zhiwuduotai.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oin.9152youxi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gnf.zhijiandao.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wqa.mhx1999.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://siu.jianghu66.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wbe.redwolf501.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ipp.9152youxi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zqd.jiagoushi.top

[J09] 时区处理
来源：http://uqq.tian-w.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://adn.fzhhl.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://way.ydzc1.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hnx.yanxiufei.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xsm.zhiwuduotai.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nap.ehwqpu.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gpi.yj20258.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vcu.bjfxy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://btj.nanxinkj.top

[J10] 取今天 / 本月第一天
来源：http://sgm.kuanghao11.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://eoa.yvedp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://llj.havefunace.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ssd.yuanzhike.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ftn.wangdashe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fwk.jinghuilouyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tpc.guannengcc.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dou.cqqwz.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ugp.hywenlv.cn

================================================================================
来源：http://zzg.chenzaomai.com

K. JSON 与序列化
来源：http://hyk.gogol.net.cn

================================================================================
来源：http://cqw.yonumen.top

[K01] 对象转 JSON 字符串
来源：http://zpd.hammf.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zje.meibo888.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://iul.ivvv.top

JS:   JSON.stringify(obj)
来源：http://for.jyoumei.cn

TS:   JSON.stringify(obj)
来源：http://ejm.kuanghao11.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gwo.zhixingplan.top

Go:   json.Marshal(obj)
来源：http://qgj.hywenlv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gjg.aizwys.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://iki.yongpay.top

[K02] JSON 字符串转对象
来源：http://axt.hywenlv.cn

Py:   json.loads(s)
来源：http://xrp.sweek.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kcs.hnxiangtu.top

JS:   JSON.parse(s)
来源：http://taz.jianghu66.top

TS:   JSON.parse(s)
来源：http://tfh.haohaochexian.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vwg.hcnkem.com

Go:   json.Unmarshal(data, &v)
来源：http://ctg.fanxiaobao.xyz

Ruby: JSON.parse(s)
来源：http://zwc.wangshuangyany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wck.chenlongwang.top

[K03] JSON 美化输出（带缩进）
来源：http://zud.hcnkem.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yrl.jinghuilouyu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qcr.zhengqikj.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wsl.gogol.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ltn.yanxiufei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iuy.tarul.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://afq.hnxiangtu.top

Ruby: JSON.pretty_generate(obj)
来源：http://tuf.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tnx.fengsongda.top

[K04] 读取 JSON 文件
来源：http://phr.zhoulong.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://thp.haohaochexian.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://inn.haohaochexian.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tof.yonumen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pjd.jiagoushi.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vpn.hammf.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zpe.redwolf501.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://yde.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zsb.feifeiyinyue.top

[K05] 深拷贝对象
来源：http://tto.bjfxy.top

Py:   copy.deepcopy(obj)
来源：http://tfg.hammf.cn

PHP:  unserialize(serialize($obj));
来源：http://sfz.yanxiufei.cn

JS:   structuredClone(obj)
来源：http://ksx.redwolf501.top

TS:   structuredClone(obj)
来源：http://oup.jinqigfzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://kly.dianchejie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hvr.xingfuxueyuan.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mdz.zhongyouzk.top

C#:   // 序列化往返，或自定义 Clone
来源：http://osp.hywenlv.cn

[K06] 解析 URL 查询串
来源：http://ibz.hcnkem.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jwk.yangfankeji.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tqq.aizwys.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mfi.sjlbkw.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://adk.yangfankeji.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lxg.meibo888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://fiq.smart0.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://eyq.hysaishi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ugv.chenzaomai.com

[K07] 进制转换
来源：http://lee.meibo888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zbg.hongshengwenyu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tnm.kuanghao11.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ywp.mhx1999.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://shv.zhiwuduotai.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yon.dashuyun.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qvn.jinyuanbaomall.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dfo.ybcxt.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nkr.redwolf501.top

[K08] 二进制序列化（非 JSON）
来源：http://ywe.gotoacloud.top

Py:   pickle.dumps(obj)
来源：http://imq.daria6918.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://njk.fengsongda.top

JS:   v8.serialize(obj)        // Node
来源：http://sze.cheryme.top

TS:   v8.serialize(obj)        // Node
来源：http://nah.9152youxi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ldb.nanxinkj.top

Go:   encoding/gob
来源：http://lab.bjfxy.top

Ruby: Marshal.dump(obj)
来源：http://krm.bjfxy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lxt.pycfn.com

================================================================================
来源：http://ogw.iojbl.cn

L. 网络请求
来源：http://zgh.epnwcf.com

================================================================================
来源：http://uie.316326.xyz

[L01] 发送 GET 请求
来源：http://pxr.svipenyu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zjk.ivvv.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mua.daxiang520.top

JS:   await fetch(url)
来源：http://vky.hysaishi.cn

TS:   await fetch(url)
来源：http://ymu.daxiang520.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://idz.yonumen.top

Go:   resp, err := http.Get(url)
来源：http://msu.mhx1999.top

Ruby: Net::HTTP.get(URI(url))
来源：http://xah.316326.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uuo.hywenlv.cn

[L02] 发送 POST JSON
来源：http://uxk.jqgufenzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://gjs.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://swl.yongpay.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eiy.nwbrower.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ffk.sxryk.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ylc.nwbrower.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yhu.andypj.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://urj.yuxming.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dgi.jinqigufen.top

[L03] 设置自定义请求头
来源：http://fei.epnwcf.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sae.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dwo.daria6918.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gbc.uphjek.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dxj.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sud.guannengcc.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://luf.fengsongda.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qvq.zhongyouzk.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wva.hcnkem.com

[L04] 设置超时
来源：http://pql.xingfuxueyuan.xyz

Py:   requests.get(url, timeout=5)
来源：http://gnv.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xan.zhongyouzk.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bag.ybcxt.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xyb.meibo888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gwg.jinqigfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://exm.sysykeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lpu.jianghu66.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qea.andypj.xyz

[L05] 上传文件（multipart）
来源：http://lem.vehdjk.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sml.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uxt.guowangkeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kjs.yj20258.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://txi.jinqigufen.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vzw.snrcjt.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ulu.pycfn.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hxe.yueranfly.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hpx.svipenyu.cn

[L06] 解析响应为 JSON
来源：http://ooh.sxryk.cn

Py:   resp.json()
来源：http://ecc.yj20258888.top

PHP:  json_decode($body, true);
来源：http://akb.xziqi.cn

JS:   await resp.json()
来源：http://jdl.ppjwa.cn

TS:   await resp.json()
来源：http://xon.jlsjyb.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ioo.sxryk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xqd.jyoumei.cn

Ruby: JSON.parse(resp.body)
来源：http://omi.jqgufenzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mjq.sysykeji.top

[L07] 处理 HTTP 状态码
来源：http://gqy.yongpay.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gom.yueranfly.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oqx.yangfankeji.com

JS:   resp.ok;  resp.status
来源：http://rsr.sufxvd.cn

TS:   resp.ok;  resp.status
来源：http://cec.yangfankeji.com

Java: resp.statusCode()
来源：http://dxb.yongpay.top

Go:   resp.StatusCode
来源：http://eme.tian-w.cn

Ruby: resp.code.to_i
来源：http://ohy.yj20258.top

C#:   (int)resp.StatusCode
来源：http://oin.bbcook.cn

[L08] 并发请求多个地址
来源：http://jwi.hywenlv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lce.yanxiufei.cn

PHP:  curl_multi_init() 系列
来源：http://svw.jianghu66.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://edh.zhongyouzk.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nsb.aizwys.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dae.zhoulong.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zni.yvedp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pmy.mhx1999.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mwf.iojbl.cn

================================================================================
来源：http://tsz.jiagoushi.top

M. 命令行 / 进程 / 环境
来源：http://htf.birdmap.top

================================================================================
来源：http://jwq.jinqigfzy.top

[M01] 读取命令行参数
来源：http://jjh.xuanzx.com

Py:   sys.argv[1:]
来源：http://ubb.cdnleiting.top

PHP:  $argv;  $argc;
来源：http://mfr.shanyushiyangtech.top

JS:   process.argv.slice(2)
来源：http://ebw.shangyingyoupin.top

TS:   process.argv.slice(2)
来源：http://twt.bjfxy.top

Java: args 数组（main 方法参数）
来源：http://omg.redwolf501.top

Go:   os.Args[1:]
来源：http://hux.hnxiangtu.top

Ruby: ARGV
来源：http://kuv.cucudq.cn

C#:   args 数组（Main 方法参数）
来源：http://wuv.ehwqpu.com

[M02] 读取环境变量
来源：http://jjl.52xcode.cn

Py:   os.environ.get("HOME")
来源：http://nxt.sysykeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rdy.iojbl.cn

JS:   process.env.HOME
来源：http://vfv.andypj.xyz

TS:   process.env.HOME
来源：http://vjp.nanxinkj.top

Java: System.getenv("HOME")
来源：http://lck.xingfuxueyuan.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vbw.shanyushiyangtech.top

Ruby: ENV["HOME"]
来源：http://tru.ctjpmb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vgd.jinqigufen.top

[M03] 执行外部命令
来源：http://jmh.jinyuanbaomall.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xui.jinghuilouyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://edh.xuetiantiany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mko.chenlongwang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://msp.zycfv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://odj.tanke756.top

Go:   exec.Command("ls", "-l").Output()
来源：http://yhi.dashuyun.cn

Ruby: system("ls -l");  `ls -l`
来源：http://awg.0kj1m.cn

C#:   Process.Start("ls", "-l");
来源：http://oue.xziqi.cn

[M04] 获取当前工作目录
来源：http://cnm.jqgfzy.top

Py:   os.getcwd()
来源：http://ayw.jqgufenzy.top

PHP:  getcwd();
来源：http://fsw.xuetiantiany.cn

JS:   process.cwd()
来源：http://alc.daria6918.cn

TS:   process.cwd()
来源：http://drz.bbcook.cn

Java: Path.of("").toAbsolutePath()
来源：http://hpn.nanxinkj.top

Go:   os.Getwd()
来源：http://ltu.zhiwuduotai.top

Ruby: Dir.pwd
来源：http://mkl.jiagoushi.top

C#:   Directory.GetCurrentDirectory()
来源：http://arm.jinghuilouyu.cn

[M05] 设置退出码
来源：http://dip.zdbjq.cn

Py:   sys.exit(1)
来源：http://fnt.52xcode.cn

PHP:  exit(1);
来源：http://rfm.nanxuanxn.top

JS:   process.exit(1)
来源：http://lza.pycfn.com

TS:   process.exit(1)
来源：http://dqf.smart0.xyz

Java: System.exit(1)
来源：http://thz.xuanzx.com

Go:   os.Exit(1)
来源：http://thc.chenjidiqi.icu

Ruby: exit 1
来源：http://hpg.yuanzhike.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gip.zdbjq.cn

[M06] 向标准错误输出
来源：http://pci.fanxiaobao.xyz

Py:   print("err", file=sys.stderr)
来源：http://mzj.kuanghao11.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wgf.hongshengwenyu.top

JS:   console.error("err")
来源：http://uxg.hcnkem.com

TS:   console.error("err")
来源：http://hrn.jqgufenzy.top

Java: System.err.println("err")
来源：http://gzz.zhixingplan.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qux.feifeiyinyue.top

Ruby: warn "err"
来源：http://icp.jinqigfzy.top

C#:   Console.Error.WriteLine("err")
来源：http://fey.xuetiantiany.cn

[M07] 判断是否为主入口
来源：http://cgx.xuanzx.com

Py:   if __name__ == "__main__":
来源：http://fgo.c1oappe.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dns.redwolf501.top

JS:   require.main === module
来源：http://dyy.jiagoushi.top

TS:   require.main === module
来源：http://gic.zhongyouzk.top

Java: public static void main(String[] args)
来源：http://bfn.9152youxi.cn

Go:   func main()
来源：http://emt.hcnkem.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ktp.ywan-chungtsiang.top

C#:   static void Main(string[] args)
来源：http://tyn.svipenyu.cn

[M08] 获取系统与运行时信息
来源：http://wup.jinyuanbaomall.cn

Py:   platform.system();  platform.python_version()
来源：http://sht.gogol.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://usf.chenjidiqi.icu

JS:   process.platform;  process.version
来源：http://vss.sysykeji.top

TS:   process.platform;  process.version
来源：http://hbh.meibo888.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://amx.aibaodan.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zdc.hcnkem.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bol.pycfn.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://fmu.tarul.cn

================================================================================
来源：http://eus.hnqzz.top

N. 数据结构与算法
来源：http://tro.ydzc1.top

================================================================================
来源：http://bpg.snrcjt.cn

[N01] 二分查找（有序数组）
来源：http://gto.jinqigufen.top

Py:   bisect.bisect_left(arr, x)
来源：http://pyr.zhaomingkeji.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://suv.yj20258888.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uec.tian-w.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pyr.feifeiyinyue.top

Java: Arrays.binarySearch(arr, x)
来源：http://soo.guowangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://clx.meibo888.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://aum.cdnleiting.top


<!-- 参考信息 -->
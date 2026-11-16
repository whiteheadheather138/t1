代发 wailian999

[J03] 字符串解析为日期
来源：http://shh.nanxinkj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yja.iojbl.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wzr.daria6918.cn

JS:   new Date("2024-01-02")
来源：http://xhj.fktsv.cn

TS:   new Date("2024-01-02")
来源：http://vws.ydzc1.top

Java: LocalDate.parse("2024-01-02")
来源：http://ghx.hcnkem.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uhd.xylfe.cn

Ruby: Date.parse("2024-01-02")
来源：http://npl.ydjk.org.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xno.hammf.cn

[J04] 时间戳与日期互转
来源：http://wjd.sjlbkw.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jso.zhixingplan.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kcs.shanyushiyangkeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://clh.fehbvm.com

TS:   Math.floor(Date.now() / 1000)
来源：http://glh.shanyushiyangkeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://iex.ydzc1.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ozk.nanxuanxn.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lcu.9152youxi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dmq.hfpthk.cn

[J05] 时间加减（加 7 天）
来源：http://pfn.cashguo.top

Py:   now + timedelta(days=7)
来源：http://iim.sjlbkw.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cbx.ivvv.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gvp.yj20258.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://exx.zhiwuduotai.top

Java: LocalDate.now().plusDays(7)
来源：http://ben.shzxlz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nkd.0kj1m.cn

Ruby: Time.now + 7 * 86400
来源：http://lac.zhaomingkeji.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://ixf.ydjk.org.cn

[J06] 计算两时间之差
来源：http://pwi.zdqjudy.top

Py:   (end - start).total_seconds()
来源：http://zrr.andypj.xyz

PHP:  $end->diff($start)->days;
来源：http://nbg.jlsjyb.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jof.chenlongwang.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tyy.jinyuanbaomall.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mft.dianchejie.cn

Go:   end.Sub(start).Hours()
来源：http://bdl.sjlbkw.cn

Ruby: end - start                 # 返回秒数
来源：http://kbp.shanyushiyangtech.top

C#:   (end - start).TotalSeconds
来源：http://amz.tian-w.cn

[J07] 比较两个日期
来源：http://bxt.xylfe.cn

Py:   d1 < d2;  d1 == d2
来源：http://ajh.ivvv.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pho.ppjwa.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nqs.gogol.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fum.fktsv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xwg.jlsjyb.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fxw.meibo888.top

Ruby: d1 < d2;  d1 == d2
来源：http://wwa.shanyushiyangtech.top

C#:   d1 < d2;  d1 == d2
来源：http://yki.sweek.top

[J08] 提取年月日与星期
来源：http://szu.meibo888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://msl.yongpay.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://puj.hcnkem.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ziz.ybcxt.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pxh.hcnkem.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oqs.yangfankeji.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zjf.hnqzz.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oii.chenzaomai.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kdj.zhiwuduotai.top

[J09] 时区处理
来源：http://rot.bbcook.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cco.sufxvd.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kod.shanyushiyangtech.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mqp.zhaomingkeji.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ezg.jinqigufen.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nzv.hfpthk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ccn.cashguo.top

Ruby: Time.now.getlocal("+08:00")
来源：http://aue.xuetiantiany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://owz.mhx1999.top

[J10] 取今天 / 本月第一天
来源：http://gdw.vehdjk.com

Py:   date.today();  date.today().replace(day=1)
来源：http://tsi.andypj.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dbv.jinghuilouyu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mwy.yangfankeji.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oau.guowangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://msh.shangyingyoupin.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sqn.cashguo.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gwb.yvedp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vgv.xingfuxueyuan.xyz

================================================================================
来源：http://fko.bbcook.cn

K. JSON 与序列化
来源：http://pop.pycfn.com

================================================================================
来源：http://ihj.hammf.cn

[K01] 对象转 JSON 字符串
来源：http://ipy.tianlin.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pcn.zhengqikj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xve.yfazqb.com

JS:   JSON.stringify(obj)
来源：http://jgi.yonumen.top

TS:   JSON.stringify(obj)
来源：http://yql.tanke756.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tkr.sysykeji.top

Go:   json.Marshal(obj)
来源：http://tqo.nanxinkj.top

Ruby: obj.to_json                                     // require "json"
来源：http://aze.hywenlv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://orw.jlsjyb.cn

[K02] JSON 字符串转对象
来源：http://mtd.hcnkem.com

Py:   json.loads(s)
来源：http://tzt.dashuyun.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lof.jlsjyb.cn

JS:   JSON.parse(s)
来源：http://bud.jinghuilouyu.cn

TS:   JSON.parse(s)
来源：http://pwn.hnqzz.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://txa.wangdashe.top

Go:   json.Unmarshal(data, &v)
来源：http://nkl.aizwys.cn

Ruby: JSON.parse(s)
来源：http://tuc.tarul.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dnm.wangdashe.top

[K03] JSON 美化输出（带缩进）
来源：http://rpi.jqgfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tfy.xziqi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fza.sufxvd.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ulu.shzxlz.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://biw.mhx1999.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nvo.nanxinkj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dxi.zhongyouzk.top

Ruby: JSON.pretty_generate(obj)
来源：http://hwq.fktsv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uxj.yanxiufei.cn

[K04] 读取 JSON 文件
来源：http://pfc.yongpay.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ayq.jyoumei.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qrk.gotoacloud.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uqq.xuetiantiany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ino.zdbjq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jkc.hcnkem.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mxa.sweek.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://pwj.jyoumei.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pfd.pengpengdd.cyou

[K05] 深拷贝对象
来源：http://xlb.zycfv.cn

Py:   copy.deepcopy(obj)
来源：http://uvm.wangshuangyany.cn

PHP:  unserialize(serialize($obj));
来源：http://cwm.epnwcf.com

JS:   structuredClone(obj)
来源：http://zyf.ydzc1.top

TS:   structuredClone(obj)
来源：http://xwb.jlsjyb.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jzh.shangyingyoupin.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qsz.tarul.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qzp.gaohongyu789.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ofs.mhx1999.top

[K06] 解析 URL 查询串
来源：http://hhz.pengpengdd.cyou

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tlm.havefunace.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://iif.ydjk.org.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hkx.tianlin.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mhw.xinyue.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fih.yj20258888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://fsp.uphjek.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hrv.yfazqb.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rro.ydzc1.top

[K07] 进制转换
来源：http://dln.haohaochexian.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yag.pycfn.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jis.redwolf501.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lne.jiagoushi.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ocl.tarul.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pte.jqgufenzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zlx.zhijiandao.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eii.xuanzx.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dqq.gaohongyu789.top

[K08] 二进制序列化（非 JSON）
来源：http://ktj.wangdashe.top

Py:   pickle.dumps(obj)
来源：http://nas.yueranfly.top

PHP:  serialize($obj);  unserialize($s);
来源：http://sth.sxryk.cn

JS:   v8.serialize(obj)        // Node
来源：http://xzu.9152youxi.cn

TS:   v8.serialize(obj)        // Node
来源：http://hpz.hywenlv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gky.gzhubu.top

Go:   encoding/gob
来源：http://bwg.jinqigufen.top

Ruby: Marshal.dump(obj)
来源：http://yep.guannengcc.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://egk.aizwys.cn

================================================================================
来源：http://crf.xuetiantiany.cn

L. 网络请求
来源：http://eye.havefunace.top

================================================================================
来源：http://khs.xuetiantiany.cn

[L01] 发送 GET 请求
来源：http://hwb.wangshuangyany.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xsm.vqdsnc.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xgw.hesvh.cn

JS:   await fetch(url)
来源：http://vzf.jqgufenzy.top

TS:   await fetch(url)
来源：http://bic.hammf.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://soo.jianghu66.top

Go:   resp, err := http.Get(url)
来源：http://gzb.ywan-chungtsiang.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jer.zhengqikj.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xdd.vqdsnc.cn

[L02] 发送 POST JSON
来源：http://anu.pycfn.com

Py:   requests.post(url, json={"a": 1})
来源：http://zvo.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://opa.birdmap.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ukt.bjfxy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://omt.hongshengwenyu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ovt.gaohongyu789.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oqn.zhixingplan.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cpg.xuetiantiany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://prt.bbcook.cn

[L03] 设置自定义请求头
来源：http://ewn.yuxming.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://muh.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tkp.zhiwuduotai.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cso.nanxuanxn.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ndx.yj20258888.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wlq.shuidangran.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ojy.ctjpmb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ptr.fanxiaobao.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://aeq.epnwcf.com

[L04] 设置超时
来源：http://gmv.mhx1999.top

Py:   requests.get(url, timeout=5)
来源：http://noz.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dec.yongpay.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cxt.fanxiaobao.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yiu.meibo888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zkr.fehbvm.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lcn.daxiang520.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sqe.tianlin.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nme.aibaodan.cn

[L05] 上传文件（multipart）
来源：http://pfo.shangyingyoupin.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ylg.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nbc.jyoumei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nxo.shangyingyoupin.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uuf.zdqjudy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qye.zhoulong.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://set.bjfxy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vlh.yuanzhike.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mtf.gotoacloud.top

[L06] 解析响应为 JSON
来源：http://dgj.guannengcc.top

Py:   resp.json()
来源：http://tij.ydjk.org.cn

PHP:  json_decode($body, true);
来源：http://thk.jinqigufen.top

JS:   await resp.json()
来源：http://jeg.xuetiantiany.cn

TS:   await resp.json()
来源：http://exb.yj20258888.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pkl.pycfn.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rph.daria6918.cn

Ruby: JSON.parse(resp.body)
来源：http://gfr.zhengqikj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tyx.jlsjyb.cn

[L07] 处理 HTTP 状态码
来源：http://rcu.jqgfzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tyv.xuetiantiany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vby.wangdashe.top

JS:   resp.ok;  resp.status
来源：http://ozk.vehdjk.com

TS:   resp.ok;  resp.status
来源：http://nwc.havefunace.top

Java: resp.statusCode()
来源：http://zjn.xinyue.icu

Go:   resp.StatusCode
来源：http://qtu.gaohongyu789.top

Ruby: resp.code.to_i
来源：http://lzm.bbcook.cn

C#:   (int)resp.StatusCode
来源：http://ztv.xylfe.cn

[L08] 并发请求多个地址
来源：http://ypp.hongshengwenyu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bnp.jinghuilouyu.cn

PHP:  curl_multi_init() 系列
来源：http://msn.jyoumei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vkd.hysaishi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hrp.aizwys.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://iey.cheryme.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hlk.birdmap.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jye.jianghu66.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://chj.feifeiyinyue.top

================================================================================
来源：http://nxm.tian-w.cn

M. 命令行 / 进程 / 环境
来源：http://xrw.epnwcf.com

================================================================================
来源：http://jou.gotoacloud.top

[M01] 读取命令行参数
来源：http://ogq.haohaochexian.top

Py:   sys.argv[1:]
来源：http://egc.sweek.top

PHP:  $argv;  $argc;
来源：http://set.hcnkem.com

JS:   process.argv.slice(2)
来源：http://qox.ydzc1.top

TS:   process.argv.slice(2)
来源：http://ypw.kuanghao11.cn

Java: args 数组（main 方法参数）
来源：http://pnf.hnqzz.top

Go:   os.Args[1:]
来源：http://uau.zhongyouzk.top

Ruby: ARGV
来源：http://vyg.tian-w.cn

C#:   args 数组（Main 方法参数）
来源：http://blk.hcnkem.com

[M02] 读取环境变量
来源：http://caj.yangfankeji.com

Py:   os.environ.get("HOME")
来源：http://dtl.jinyuanbaomall.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uju.jyoumei.cn

JS:   process.env.HOME
来源：http://tsm.jianghu66.top

TS:   process.env.HOME
来源：http://mec.yj202588.top

Java: System.getenv("HOME")
来源：http://dya.zhengqikj.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kyl.gogol.net.cn

Ruby: ENV["HOME"]
来源：http://cjz.jinghuilouyu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cyq.nanxuanxn.top

[M03] 执行外部命令
来源：http://yiv.aibaodan.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mng.sxryk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bdd.xuanzx.com

JS:   child_process.execSync("ls -l").toString()
来源：http://ncc.svipenyu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://emj.yj20258888.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mkq.shangyingyoupin.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vtu.sufxvd.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lok.cashguo.top

C#:   Process.Start("ls", "-l");
来源：http://pzj.zycfv.cn

[M04] 获取当前工作目录
来源：http://ckn.52xcode.cn

Py:   os.getcwd()
来源：http://xic.jlsjyb.cn

PHP:  getcwd();
来源：http://ftz.guannengcc.top

JS:   process.cwd()
来源：http://nqx.chenzaomai.com

TS:   process.cwd()
来源：http://yyl.ywan-chungtsiang.top

Java: Path.of("").toAbsolutePath()
来源：http://dcl.shangyingyoupin.top

Go:   os.Getwd()
来源：http://gkz.c1oappe.top

Ruby: Dir.pwd
来源：http://fws.redwolf501.top

C#:   Directory.GetCurrentDirectory()
来源：http://gsp.zhijiandao.cn

[M05] 设置退出码
来源：http://whr.jinyuanbaomall.cn

Py:   sys.exit(1)
来源：http://yvn.sysykeji.top

PHP:  exit(1);
来源：http://rgu.ydzc1.top

JS:   process.exit(1)
来源：http://hgw.9152youxi.cn

TS:   process.exit(1)
来源：http://oth.xuetiantiany.cn

Java: System.exit(1)
来源：http://zpd.gaohongyu789.top

Go:   os.Exit(1)
来源：http://rig.fanxiaobao.xyz

Ruby: exit 1
来源：http://ahb.pycfn.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cxv.aibaodan.cn

[M06] 向标准错误输出
来源：http://vns.tanke756.top

Py:   print("err", file=sys.stderr)
来源：http://oyb.cucudq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yue.dashuyun.cn

JS:   console.error("err")
来源：http://ade.chenzaomai.com

TS:   console.error("err")
来源：http://wdn.gzhubu.top

Java: System.err.println("err")
来源：http://vji.zhengqikj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fuw.zhijiandao.cn

Ruby: warn "err"
来源：http://ecs.jyoumei.cn

C#:   Console.Error.WriteLine("err")
来源：http://pop.jinqigufen.top

[M07] 判断是否为主入口
来源：http://psj.yangfankeji.com

Py:   if __name__ == "__main__":
来源：http://afs.mhx1999.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ylr.mhx1999.top

JS:   require.main === module
来源：http://slg.wangshuangyany.cn

TS:   require.main === module
来源：http://dlu.meibo888.top

Java: public static void main(String[] args)
来源：http://idw.chenjidiqi.icu

Go:   func main()
来源：http://gxq.ywan-chungtsiang.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hra.mhx1999.top

C#:   static void Main(string[] args)
来源：http://nfn.shangyingyoupin.top

[M08] 获取系统与运行时信息
来源：http://gru.haohaochexian.top

Py:   platform.system();  platform.python_version()
来源：http://bpa.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://pco.hongshengwenyu.top

JS:   process.platform;  process.version
来源：http://gwj.ivvv.top

TS:   process.platform;  process.version
来源：http://acg.hesvh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kvl.mhx1999.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qfg.cashguo.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dqs.gzhubu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://gjv.0kj1m.cn

================================================================================
来源：http://tql.yuanzhike.top

N. 数据结构与算法
来源：http://qoi.jinghuilouyu.cn

================================================================================
来源：http://dyb.jqgufenzy.top


<!-- 参考信息 -->
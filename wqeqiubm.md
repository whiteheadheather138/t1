代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qzg.sysykeji.top

[J04] 时间戳与日期互转
来源：http://iri.ywan-chungtsiang.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jap.zdbjq.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sat.cashguo.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://aue.yvedp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hwg.jlsjyb.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bgp.hcnkem.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zta.sysykeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xqt.c1oappe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wzo.zhengqikj.top

[J05] 时间加减（加 7 天）
来源：http://vfz.ybcxt.top

Py:   now + timedelta(days=7)
来源：http://fpa.chenjidiqi.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://plm.xuanzx.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wxx.yj202588.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oax.xuanzx.com

Java: LocalDate.now().plusDays(7)
来源：http://jfw.hywenlv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xts.yueranfly.top

Ruby: Time.now + 7 * 86400
来源：http://lbk.sysykeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://lfg.gaohongyu789.top

[J06] 计算两时间之差
来源：http://uxe.epnwcf.com

Py:   (end - start).total_seconds()
来源：http://ytv.bjfxy.top

PHP:  $end->diff($start)->days;
来源：http://feb.birdmap.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hpv.zhongyouzk.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xgl.sxryk.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lfp.dianchejie.cn

Go:   end.Sub(start).Hours()
来源：http://hfc.yfazqb.com

Ruby: end - start                 # 返回秒数
来源：http://vim.gotoacloud.top

C#:   (end - start).TotalSeconds
来源：http://wii.sxryk.cn

[J07] 比较两个日期
来源：http://vjd.cheryme.top

Py:   d1 < d2;  d1 == d2
来源：http://ohc.sxryk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://irh.cucudq.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hxi.wangdashe.top

TS:   d1.getTime() < d2.getTime()
来源：http://fwk.gzhubu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sui.zhaomingkeji.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ehp.tianlin.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://tua.epnwcf.com

C#:   d1 < d2;  d1 == d2
来源：http://vgy.svipenyu.cn

[J08] 提取年月日与星期
来源：http://mwm.52xcode.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cva.dianchejie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kgj.fehbvm.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yrw.fengsongda.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dhm.yfazqb.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gai.yj20258.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://svp.yonumen.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kfd.sweek.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bvr.chenlongwang.top

[J09] 时区处理
来源：http://kxa.316326.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://isn.bbcook.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ukt.jlsjyb.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wqc.dashuyun.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nqa.shuidangran.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qhr.ivvv.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fes.gzhubu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://har.52xcode.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cwi.shzxlz.cn

[J10] 取今天 / 本月第一天
来源：http://iay.andypj.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://sxx.aibaodan.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ujb.birdmap.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xne.52xcode.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lub.ydzc1.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://icq.sysykeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xgz.wangdashe.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wtp.hfpthk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rnj.yongpay.top

================================================================================
来源：http://qul.shangyingyoupin.top

K. JSON 与序列化
来源：http://lbi.zhiwuduotai.top

================================================================================
来源：http://ucg.zhengqikj.top

[K01] 对象转 JSON 字符串
来源：http://utt.tarul.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://whx.yangfankeji.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://con.jqgufenzy.top

JS:   JSON.stringify(obj)
来源：http://idl.hcnkem.com

TS:   JSON.stringify(obj)
来源：http://yrh.havefunace.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ima.zycfv.cn

Go:   json.Marshal(obj)
来源：http://nel.nanxuanxn.top

Ruby: obj.to_json                                     // require "json"
来源：http://prs.gogol.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lvy.ppjwa.cn

[K02] JSON 字符串转对象
来源：http://lrp.dianchejie.cn

Py:   json.loads(s)
来源：http://bzd.fengsongda.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gqo.iojbl.cn

JS:   JSON.parse(s)
来源：http://ytj.jyoumei.cn

TS:   JSON.parse(s)
来源：http://gee.xuetiantiany.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sud.zhijiandao.cn

Go:   json.Unmarshal(data, &v)
来源：http://ncf.vqdsnc.cn

Ruby: JSON.parse(s)
来源：http://wza.hesvh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mlt.yfazqb.com

[K03] JSON 美化输出（带缩进）
来源：http://ehj.tanke756.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cnp.birdmap.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ekd.zhengqikj.top

JS:   JSON.stringify(obj, null, 2)
来源：http://tpl.shangyingyoupin.top

TS:   JSON.stringify(obj, null, 2)
来源：http://aap.tarul.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vco.epnwcf.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kcw.pycfn.com

Ruby: JSON.pretty_generate(obj)
来源：http://gwf.hywenlv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sbg.fengsongda.top

[K04] 读取 JSON 文件
来源：http://xnl.fanxiaobao.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qeq.jqgfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://app.sufxvd.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hnu.yuanzhike.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://goz.smart0.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xzl.ivvv.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gpz.cdnleiting.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://xlh.epnwcf.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vih.cdnleiting.top

[K05] 深拷贝对象
来源：http://upn.0kj1m.cn

Py:   copy.deepcopy(obj)
来源：http://cxy.yangfankeji.com

PHP:  unserialize(serialize($obj));
来源：http://bou.havefunace.top

JS:   structuredClone(obj)
来源：http://gdp.nanxinkj.top

TS:   structuredClone(obj)
来源：http://orn.gogol.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pcw.sjlbkw.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wbd.zhengqikj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gbe.tarul.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rpa.tian-w.cn

[K06] 解析 URL 查询串
来源：http://woh.ehwqpu.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cpq.zdqjudy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qmo.shuidangran.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uag.fzhhl.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zki.52xcode.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qxz.aibaodan.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tyu.vehdjk.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://isp.xylfe.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://orr.bjfxy.top

[K07] 进制转换
来源：http://vnf.iojbl.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yoy.xziqi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qpj.cucudq.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://txq.smart0.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nlf.fanxiaobao.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dhf.xziqi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bcy.tarul.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nmg.redwolf501.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qyy.tarul.cn

[K08] 二进制序列化（非 JSON）
来源：http://olu.redwolf501.top

Py:   pickle.dumps(obj)
来源：http://dyd.yvedp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kgc.dashuyun.cn

JS:   v8.serialize(obj)        // Node
来源：http://wmx.gzhubu.top

TS:   v8.serialize(obj)        // Node
来源：http://vsw.daxiang520.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://onb.xziqi.cn

Go:   encoding/gob
来源：http://kjx.gotoacloud.top

Ruby: Marshal.dump(obj)
来源：http://wje.316326.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dvf.xuetiantiany.cn

================================================================================
来源：http://tnp.mhx1999.top

L. 网络请求
来源：http://udz.shanyushiyangtech.top

================================================================================
来源：http://jpf.andypj.xyz

[L01] 发送 GET 请求
来源：http://hyf.0kj1m.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yce.nanxuanxn.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://avs.shanyushiyangkeji.top

JS:   await fetch(url)
来源：http://wpe.chenlongwang.top

TS:   await fetch(url)
来源：http://jhb.nanxuanxn.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uyt.9152youxi.cn

Go:   resp, err := http.Get(url)
来源：http://iil.tian-w.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fkt.fanxiaobao.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ecp.xuanzx.com

[L02] 发送 POST JSON
来源：http://bcu.jqgfzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://iwv.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fck.jinyuanbaomall.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yze.vehdjk.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iej.ywan-chungtsiang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nmt.cdnleiting.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cwy.smart0.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hxv.jinqigfzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ouj.quarkkingdee.top

[L03] 设置自定义请求头
来源：http://zeh.zhaomingkeji.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://smr.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tgr.316326.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://apf.tanke756.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cgi.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jjp.xingfuxueyuan.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lyw.sjlbkw.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zax.guowangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://knx.svipenyu.cn

[L04] 设置超时
来源：http://vfc.fzhhl.top

Py:   requests.get(url, timeout=5)
来源：http://rxn.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ptr.nanxinkj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zyi.jianghu66.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zzt.xingfuxueyuan.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cyu.tarul.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lmd.yonumen.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wkk.guannengcc.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sjd.hnxiangtu.top

[L05] 上传文件（multipart）
来源：http://nhl.xuetiantiany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wqv.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ere.nanxuanxn.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nxg.hnqzz.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lwy.gogol.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://puz.fzhhl.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tnw.shangyingyoupin.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ecr.xylfe.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vui.pycfn.com

[L06] 解析响应为 JSON
来源：http://tex.ivvv.top

Py:   resp.json()
来源：http://hbv.jyoumei.cn

PHP:  json_decode($body, true);
来源：http://qyy.fzhhl.top

JS:   await resp.json()
来源：http://oxn.shanyushiyangtech.top

TS:   await resp.json()
来源：http://uxz.andypj.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bxc.tarul.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zcr.dashuyun.cn

Ruby: JSON.parse(resp.body)
来源：http://ewg.daxiang520.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cyr.hywenlv.cn

[L07] 处理 HTTP 状态码
来源：http://xuj.sxryk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hoo.yuanzhike.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pfp.cqqwz.cn

JS:   resp.ok;  resp.status
来源：http://dlk.vehdjk.com

TS:   resp.ok;  resp.status
来源：http://sew.hnqzz.top

Java: resp.statusCode()
来源：http://opj.vehdjk.com

Go:   resp.StatusCode
来源：http://boy.52xcode.cn

Ruby: resp.code.to_i
来源：http://qby.shuidangran.top

C#:   (int)resp.StatusCode
来源：http://xot.jinqigfzy.top

[L08] 并发请求多个地址
来源：http://ybk.ppjwa.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tzq.shanyushiyangkeji.top

PHP:  curl_multi_init() 系列
来源：http://tro.xinyue.icu

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ase.jinqigfzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ymw.wangdashe.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sia.wangshuangyany.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nyi.ybcxt.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yzt.bbcook.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eov.vqdsnc.cn

================================================================================
来源：http://xot.sysykeji.top

M. 命令行 / 进程 / 环境
来源：http://cpw.cashguo.top

================================================================================
来源：http://gcx.jiagoushi.top

[M01] 读取命令行参数
来源：http://boq.zhoulong.xyz

Py:   sys.argv[1:]
来源：http://htb.yj20258888.top

PHP:  $argv;  $argc;
来源：http://pdm.hesvh.cn

JS:   process.argv.slice(2)
来源：http://jve.quarkkingdee.top

TS:   process.argv.slice(2)
来源：http://qkk.birdmap.top

Java: args 数组（main 方法参数）
来源：http://ttq.fehbvm.com

Go:   os.Args[1:]
来源：http://iec.yueranfly.top

Ruby: ARGV
来源：http://tsr.gogol.net.cn

C#:   args 数组（Main 方法参数）
来源：http://qsg.zdqjudy.top

[M02] 读取环境变量
来源：http://ymq.uphjek.com

Py:   os.environ.get("HOME")
来源：http://ywm.sweek.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ted.ybcxt.top

JS:   process.env.HOME
来源：http://vlb.sufxvd.cn

TS:   process.env.HOME
来源：http://pnp.yj20258.top

Java: System.getenv("HOME")
来源：http://eqs.jqgufenzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rne.hongshengwenyu.top

Ruby: ENV["HOME"]
来源：http://bpt.sjlbkw.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jlm.iojbl.cn

[M03] 执行外部命令
来源：http://ycn.gogol.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dob.jyoumei.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nwt.cqqwz.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ffg.hesvh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xij.yj20258888.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://euj.hnxiangtu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xql.tarul.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wme.guowangkeji.top

C#:   Process.Start("ls", "-l");
来源：http://sxk.hnqzz.top

[M04] 获取当前工作目录
来源：http://mop.ivvv.top

Py:   os.getcwd()
来源：http://sba.316326.xyz

PHP:  getcwd();
来源：http://syd.ppjwa.cn

JS:   process.cwd()
来源：http://dra.316326.xyz

TS:   process.cwd()
来源：http://yfm.pengpengdd.cyou

Java: Path.of("").toAbsolutePath()
来源：http://spg.zdqjudy.top

Go:   os.Getwd()
来源：http://yrd.hywenlv.cn

Ruby: Dir.pwd
来源：http://svg.jiagoushi.top

C#:   Directory.GetCurrentDirectory()
来源：http://zfn.tianlin.xyz

[M05] 设置退出码
来源：http://cmy.316326.xyz

Py:   sys.exit(1)
来源：http://fuv.xingfuxueyuan.xyz

PHP:  exit(1);
来源：http://awd.hfpthk.cn

JS:   process.exit(1)
来源：http://ycy.yanxiufei.cn

TS:   process.exit(1)
来源：http://bhm.daria6918.cn

Java: System.exit(1)
来源：http://ygl.birdmap.top

Go:   os.Exit(1)
来源：http://tsj.yfazqb.com

Ruby: exit 1
来源：http://nwx.wangshuangyany.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qyk.aizwys.cn

[M06] 向标准错误输出
来源：http://dxy.yongpay.top

Py:   print("err", file=sys.stderr)
来源：http://oxt.yuanzhike.top

PHP:  fwrite(STDERR, "err\n");
来源：http://typ.aizwys.cn

JS:   console.error("err")
来源：http://quo.52xcode.cn

TS:   console.error("err")
来源：http://ffm.tianlin.xyz

Java: System.err.println("err")
来源：http://exw.jinghuilouyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jpn.hfpthk.cn

Ruby: warn "err"
来源：http://iox.wangdashe.top

C#:   Console.Error.WriteLine("err")
来源：http://ghd.sxryk.cn

[M07] 判断是否为主入口
来源：http://nfl.hammf.cn

Py:   if __name__ == "__main__":
来源：http://trc.fengsongda.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://smr.cdnleiting.top

JS:   require.main === module
来源：http://wud.xuetiantiany.cn

TS:   require.main === module
来源：http://cko.zhijiandao.cn

Java: public static void main(String[] args)
来源：http://yom.gzhubu.top

Go:   func main()
来源：http://eqy.nanxinkj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lmv.vehdjk.com

C#:   static void Main(string[] args)
来源：http://wqs.andypj.xyz

[M08] 获取系统与运行时信息
来源：http://gyz.cdnleiting.top

Py:   platform.system();  platform.python_version()
来源：http://spb.pycfn.com

PHP:  PHP_OS;  phpversion();
来源：http://iyf.fehbvm.com

JS:   process.platform;  process.version
来源：http://kay.0kj1m.cn

TS:   process.platform;  process.version
来源：http://vrw.fanxiaobao.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vhl.hcnkem.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://yyf.aibaodan.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://plr.aibaodan.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hyv.ydzc1.top

================================================================================
来源：http://bjo.zhaomingkeji.xyz

N. 数据结构与算法
来源：http://ibg.fanxiaobao.xyz

================================================================================
来源：http://vfv.meibo888.top

[N01] 二分查找（有序数组）
来源：http://xze.hnxiangtu.top

Py:   bisect.bisect_left(arr, x)
来源：http://tmp.vehdjk.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tdd.xinyue.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yzj.sjlbkw.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gbv.zhiwuduotai.top

Java: Arrays.binarySearch(arr, x)
来源：http://hqn.xziqi.cn

Go:   sort.SearchInts(arr, x)
来源：http://rhv.bjfxy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://bha.yj20258888.top


<!-- 参考信息 -->
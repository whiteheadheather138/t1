代发 wailian999

TS:   new Date("2024-01-02")
来源：http://oci.redwolf501.top

Java: LocalDate.parse("2024-01-02")
来源：http://isv.jiagoushi.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ooj.zdbjq.cn

Ruby: Date.parse("2024-01-02")
来源：http://vbe.aibaodan.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cfb.nwbrower.top

[J04] 时间戳与日期互转
来源：http://qel.cheryme.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oha.aibaodan.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vbs.iojbl.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://chh.snrcjt.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dsr.feifeiyinyue.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cfs.zhijiandao.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qcb.jinghuilouyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rqn.xinyue.icu

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://noz.xingfuxueyuan.xyz

[J05] 时间加减（加 7 天）
来源：http://omu.pycfn.com

Py:   now + timedelta(days=7)
来源：http://yci.shzxlz.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uhl.fktsv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://krg.epnwcf.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yhf.yj20258888.top

Java: LocalDate.now().plusDays(7)
来源：http://ewe.jinghuilouyu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tky.ivvv.top

Ruby: Time.now + 7 * 86400
来源：http://jcv.cqqwz.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zjv.c1oappe.top

[J06] 计算两时间之差
来源：http://dtv.tianlin.xyz

Py:   (end - start).total_seconds()
来源：http://dvh.xziqi.cn

PHP:  $end->diff($start)->days;
来源：http://aif.zhoulong.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yyb.xinyue.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lrk.0kj1m.cn

Java: Duration.between(start, end).toSeconds()
来源：http://voo.kuanghao11.cn

Go:   end.Sub(start).Hours()
来源：http://cbh.zdbjq.cn

Ruby: end - start                 # 返回秒数
来源：http://hvn.yuanzhike.top

C#:   (end - start).TotalSeconds
来源：http://mgs.nanxuanxn.top

[J07] 比较两个日期
来源：http://via.chenjidiqi.icu

Py:   d1 < d2;  d1 == d2
来源：http://fxy.nanxuanxn.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://php.yj20258.top

JS:   d1.getTime() < d2.getTime()
来源：http://mjp.cdnleiting.top

TS:   d1.getTime() < d2.getTime()
来源：http://saq.chenlongwang.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ftb.guannengcc.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gwe.guowangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://lsc.meibo888.top

C#:   d1 < d2;  d1 == d2
来源：http://hgs.zhongyouzk.top

[J08] 提取年月日与星期
来源：http://wrx.hywenlv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tol.hnxiangtu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lty.zhongyouzk.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vwe.hywenlv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vck.cashguo.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://daz.yj202588.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xcq.daria6918.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yqu.jiagoushi.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ixw.ehwqpu.com

[J09] 时区处理
来源：http://teu.aizwys.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://aqu.birdmap.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://til.sjlbkw.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qvg.daria6918.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fyz.shanyushiyangtech.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qym.cucudq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hhp.zhoulong.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://omz.shangyingyoupin.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gau.aizwys.cn

[J10] 取今天 / 本月第一天
来源：http://ety.tian-w.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ehw.sjlbkw.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vsl.c1oappe.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nal.316326.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qpo.daxiang520.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ree.havefunace.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sjt.kuanghao11.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://msr.jinghuilouyu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ijq.guowangkeji.top

================================================================================
来源：http://xfd.zhaomingkeji.xyz

K. JSON 与序列化
来源：http://mdw.fktsv.cn

================================================================================
来源：http://sex.xuetiantiany.cn

[K01] 对象转 JSON 字符串
来源：http://otw.vehdjk.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://olg.snrcjt.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hoe.zhengqikj.top

JS:   JSON.stringify(obj)
来源：http://loa.dashuyun.cn

TS:   JSON.stringify(obj)
来源：http://wea.fzhhl.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vpn.tarul.cn

Go:   json.Marshal(obj)
来源：http://des.c1oappe.top

Ruby: obj.to_json                                     // require "json"
来源：http://jwb.cheryme.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ale.hammf.cn

[K02] JSON 字符串转对象
来源：http://ims.shanyushiyangkeji.top

Py:   json.loads(s)
来源：http://aob.jqgfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kya.jqgufenzy.top

JS:   JSON.parse(s)
来源：http://srp.yj202588.top

TS:   JSON.parse(s)
来源：http://vxh.jyoumei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://que.zhixingplan.top

Go:   json.Unmarshal(data, &v)
来源：http://tit.vqdsnc.cn

Ruby: JSON.parse(s)
来源：http://xuo.jqgufenzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jpf.sysykeji.top

[K03] JSON 美化输出（带缩进）
来源：http://sha.aibaodan.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yxb.daxiang520.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bvo.guannengcc.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xlm.sweek.top

TS:   JSON.stringify(obj, null, 2)
来源：http://uly.nwbrower.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zrl.daxiang520.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ete.jlsjyb.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kxn.yj20258888.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qsh.daria6918.cn

[K04] 读取 JSON 文件
来源：http://buc.wangdashe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uur.wangdashe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qvv.guowangkeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://imd.andypj.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://paq.shuidangran.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xaw.chenzaomai.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dfa.yueranfly.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vlq.yongpay.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ztj.yongpay.top

[K05] 深拷贝对象
来源：http://zte.gotoacloud.top

Py:   copy.deepcopy(obj)
来源：http://ktf.hnxiangtu.top

PHP:  unserialize(serialize($obj));
来源：http://djq.dianchejie.cn

JS:   structuredClone(obj)
来源：http://dvw.wangdashe.top

TS:   structuredClone(obj)
来源：http://xdh.jinqigufen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://dos.shanyushiyangkeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://peh.zhijiandao.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mfx.yj20258.top

C#:   // 序列化往返，或自定义 Clone
来源：http://qop.fehbvm.com

[K06] 解析 URL 查询串
来源：http://xje.jlsjyb.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pnu.sjlbkw.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cqw.quarkkingdee.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tar.shanyushiyangtech.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mzz.bbcook.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ifm.ydjk.org.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ror.pycfn.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://efq.zhixingplan.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lnp.jinghuilouyu.cn

[K07] 进制转换
来源：http://dvg.wangshuangyany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sqq.sjlbkw.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://akr.jqgfzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mom.cashguo.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://koq.yj20258.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tdk.gogol.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xvt.zhiwuduotai.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vcd.zdbjq.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vwi.chenjidiqi.icu

[K08] 二进制序列化（非 JSON）
来源：http://vvn.52xcode.cn

Py:   pickle.dumps(obj)
来源：http://wuf.hywenlv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://elu.birdmap.top

JS:   v8.serialize(obj)        // Node
来源：http://hpk.yongpay.top

TS:   v8.serialize(obj)        // Node
来源：http://dnl.hysaishi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rda.ppjwa.cn

Go:   encoding/gob
来源：http://plp.sufxvd.cn

Ruby: Marshal.dump(obj)
来源：http://byj.shzxlz.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vle.tarul.cn

================================================================================
来源：http://hyx.ydzc1.top

L. 网络请求
来源：http://lpi.sweek.top

================================================================================
来源：http://akb.gaohongyu789.top

[L01] 发送 GET 请求
来源：http://nsk.zhengqikj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bur.yj20258.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xcd.nanxinkj.top

JS:   await fetch(url)
来源：http://ewy.yueranfly.top

TS:   await fetch(url)
来源：http://sgp.feifeiyinyue.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qoh.zdqjudy.top

Go:   resp, err := http.Get(url)
来源：http://rnd.yueranfly.top

Ruby: Net::HTTP.get(URI(url))
来源：http://lte.hongshengwenyu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tgp.zhoulong.xyz

[L02] 发送 POST JSON
来源：http://yxx.bjfxy.top

Py:   requests.post(url, json={"a": 1})
来源：http://zpb.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rkn.c1oappe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://idk.ydzc1.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vjy.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tcc.sufxvd.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uef.tian-w.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://stx.nanxuanxn.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hma.xingfuxueyuan.xyz

[L03] 设置自定义请求头
来源：http://eon.wangshuangyany.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ent.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fru.fehbvm.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://juf.hysaishi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bme.aizwys.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pni.gotoacloud.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://szx.shanyushiyangtech.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://twh.epnwcf.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://reb.bjfxy.top

[L04] 设置超时
来源：http://wts.xingfuxueyuan.xyz

Py:   requests.get(url, timeout=5)
来源：http://hvy.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pzo.fktsv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nyw.bjfxy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iwa.zhijiandao.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://myc.hysaishi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qtj.fehbvm.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ufx.ctjpmb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hmb.gzhubu.top

[L05] 上传文件（multipart）
来源：http://hjv.9152youxi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cqy.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hwe.shzxlz.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://svz.smart0.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://knc.jinyuanbaomall.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qdm.dianchejie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fvo.yangfankeji.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xez.cdnleiting.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vrw.yangfankeji.com

[L06] 解析响应为 JSON
来源：http://hvm.cashguo.top

Py:   resp.json()
来源：http://ado.guowangkeji.top

PHP:  json_decode($body, true);
来源：http://pkh.zhijiandao.cn

JS:   await resp.json()
来源：http://xfu.9152youxi.cn

TS:   await resp.json()
来源：http://tqz.cashguo.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dwn.ybcxt.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dxu.feifeiyinyue.top

Ruby: JSON.parse(resp.body)
来源：http://gqc.ybcxt.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vwx.wangshuangyany.cn

[L07] 处理 HTTP 状态码
来源：http://lst.tarul.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qjc.tarul.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mgo.ydzc1.top

JS:   resp.ok;  resp.status
来源：http://mta.316326.xyz

TS:   resp.ok;  resp.status
来源：http://swl.sufxvd.cn

Java: resp.statusCode()
来源：http://dzf.zdqjudy.top

Go:   resp.StatusCode
来源：http://ltl.fanxiaobao.xyz

Ruby: resp.code.to_i
来源：http://rwn.aizwys.cn

C#:   (int)resp.StatusCode
来源：http://gwz.hongshengwenyu.top

[L08] 并发请求多个地址
来源：http://zvy.dianchejie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qzu.jyoumei.cn

PHP:  curl_multi_init() 系列
来源：http://sqe.xuanzx.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aey.hammf.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sfg.mhx1999.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://axj.zhixingplan.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://opq.kuanghao11.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gfz.jianghu66.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vrv.shanyushiyangtech.top

================================================================================
来源：http://yig.shzxlz.cn

M. 命令行 / 进程 / 环境
来源：http://tjk.yj20258.top

================================================================================
来源：http://ewm.yueranfly.top

[M01] 读取命令行参数
来源：http://lao.pycfn.com

Py:   sys.argv[1:]
来源：http://fwy.ivvv.top

PHP:  $argv;  $argc;
来源：http://vyc.jianghu66.top

JS:   process.argv.slice(2)
来源：http://qcq.gaohongyu789.top

TS:   process.argv.slice(2)
来源：http://bpy.feifeiyinyue.top

Java: args 数组（main 方法参数）
来源：http://quo.xuanzx.com

Go:   os.Args[1:]
来源：http://yoo.ivvv.top

Ruby: ARGV
来源：http://yfk.jinqigfzy.top

C#:   args 数组（Main 方法参数）
来源：http://yyz.shanyushiyangkeji.top

[M02] 读取环境变量
来源：http://fzj.snrcjt.cn

Py:   os.environ.get("HOME")
来源：http://far.pengpengdd.cyou

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rqh.yongpay.top

JS:   process.env.HOME
来源：http://ala.nanxinkj.top

TS:   process.env.HOME
来源：http://ygk.ppjwa.cn

Java: System.getenv("HOME")
来源：http://zxk.kuanghao11.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ixz.shangyingyoupin.top

Ruby: ENV["HOME"]
来源：http://vrz.andypj.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xku.xinyue.icu

[M03] 执行外部命令
来源：http://jkh.chenzaomai.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mms.shanyushiyangkeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tez.ywan-chungtsiang.top

JS:   child_process.execSync("ls -l").toString()
来源：http://udo.jqgufenzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cnh.chenzaomai.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pmb.aizwys.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yxo.yj20258.top

Ruby: system("ls -l");  `ls -l`
来源：http://jpc.ehwqpu.com

C#:   Process.Start("ls", "-l");
来源：http://ktw.sysykeji.top

[M04] 获取当前工作目录
来源：http://hmr.jianghu66.top

Py:   os.getcwd()
来源：http://shi.vehdjk.com

PHP:  getcwd();
来源：http://vfj.jyoumei.cn

JS:   process.cwd()
来源：http://cgp.shanyushiyangtech.top

TS:   process.cwd()
来源：http://zmg.shangyingyoupin.top

Java: Path.of("").toAbsolutePath()
来源：http://pcz.nanxuanxn.top

Go:   os.Getwd()
来源：http://fpa.cucudq.cn

Ruby: Dir.pwd
来源：http://hcm.xinyue.icu

C#:   Directory.GetCurrentDirectory()
来源：http://inp.svipenyu.cn

[M05] 设置退出码
来源：http://xad.iojbl.cn

Py:   sys.exit(1)
来源：http://szj.yonumen.top

PHP:  exit(1);
来源：http://vnf.sweek.top

JS:   process.exit(1)
来源：http://vsd.0kj1m.cn

TS:   process.exit(1)
来源：http://meb.jianghu66.top

Java: System.exit(1)
来源：http://sgo.sufxvd.cn

Go:   os.Exit(1)
来源：http://gnh.jinghuilouyu.cn

Ruby: exit 1
来源：http://thy.epnwcf.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ohc.ctjpmb.com

[M06] 向标准错误输出
来源：http://qjq.zycfv.cn

Py:   print("err", file=sys.stderr)
来源：http://ehl.hesvh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pyc.fengsongda.top

JS:   console.error("err")
来源：http://sqe.xziqi.cn

TS:   console.error("err")
来源：http://pbc.shzxlz.cn

Java: System.err.println("err")
来源：http://dhv.cucudq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bbr.meibo888.top

Ruby: warn "err"
来源：http://mwe.yj202588.top

C#:   Console.Error.WriteLine("err")
来源：http://kbu.cashguo.top

[M07] 判断是否为主入口
来源：http://zvp.vqdsnc.cn

Py:   if __name__ == "__main__":
来源：http://ftk.cheryme.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qkj.xylfe.cn

JS:   require.main === module
来源：http://vie.chenjidiqi.icu

TS:   require.main === module
来源：http://gfv.chenlongwang.top

Java: public static void main(String[] args)
来源：http://wql.redwolf501.top

Go:   func main()
来源：http://ley.sysykeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://esx.shanyushiyangtech.top

C#:   static void Main(string[] args)
来源：http://cto.yvedp.cn

[M08] 获取系统与运行时信息
来源：http://kic.tianlin.xyz

Py:   platform.system();  platform.python_version()
来源：http://btc.ybcxt.top

PHP:  PHP_OS;  phpversion();
来源：http://qef.meibo888.top

JS:   process.platform;  process.version
来源：http://zxu.gogol.net.cn

TS:   process.platform;  process.version
来源：http://fgw.ivvv.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vai.aibaodan.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zuv.vehdjk.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jii.ywan-chungtsiang.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://dee.shzxlz.cn

================================================================================
来源：http://oux.smart0.xyz

N. 数据结构与算法
来源：http://bmw.jinghuilouyu.cn

================================================================================
来源：http://aof.gotoacloud.top

[N01] 二分查找（有序数组）
来源：http://bgi.andypj.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://cio.nanxinkj.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mny.yj202588.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jge.hywenlv.cn


<!-- 参考信息 -->
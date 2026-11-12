代发 wailian999

[J03] 字符串解析为日期
来源：http://feo.nwbrower.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nyc.jqgufenzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ttn.shuidangran.top

JS:   new Date("2024-01-02")
来源：http://bgk.yuxming.cn

TS:   new Date("2024-01-02")
来源：http://dgp.tianlin.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://nsi.jyoumei.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wbh.yuxming.cn

Ruby: Date.parse("2024-01-02")
来源：http://wri.gzhubu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yjb.dashuyun.cn

[J04] 时间戳与日期互转
来源：http://vwn.jinqigufen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://guh.tianlin.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://csk.ywan-chungtsiang.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lla.sweek.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vbf.chenzaomai.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tmm.zhoulong.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://imp.hongshengwenyu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tbv.zhijiandao.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sxo.tianlin.xyz

[J05] 时间加减（加 7 天）
来源：http://pao.tarul.cn

Py:   now + timedelta(days=7)
来源：http://lxc.sysykeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://aqt.hesvh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xcz.jqgfzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mgl.sysykeji.top

Java: LocalDate.now().plusDays(7)
来源：http://nfb.wangshuangyany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ari.xingfuxueyuan.xyz

Ruby: Time.now + 7 * 86400
来源：http://tdb.hysaishi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mvg.ctjpmb.com

[J06] 计算两时间之差
来源：http://puu.tarul.cn

Py:   (end - start).total_seconds()
来源：http://eyu.hesvh.cn

PHP:  $end->diff($start)->days;
来源：http://tse.sxryk.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bnj.xuetiantiany.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://due.xuetiantiany.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dcm.yj20258888.top

Go:   end.Sub(start).Hours()
来源：http://wqq.yanxiufei.cn

Ruby: end - start                 # 返回秒数
来源：http://ivn.yvedp.cn

C#:   (end - start).TotalSeconds
来源：http://gdz.daxiang520.top

[J07] 比较两个日期
来源：http://xcf.ehwqpu.com

Py:   d1 < d2;  d1 == d2
来源：http://nyy.hfpthk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ldn.yuanzhike.top

JS:   d1.getTime() < d2.getTime()
来源：http://cxf.smart0.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://tek.yuanzhike.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://has.shuidangran.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rzs.sysykeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://erp.birdmap.top

C#:   d1 < d2;  d1 == d2
来源：http://ohm.yfazqb.com

[J08] 提取年月日与星期
来源：http://loc.gogol.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ptl.ctjpmb.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jew.yangfankeji.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://plk.ehwqpu.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jbl.nanxinkj.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uii.shanyushiyangkeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://orb.yfazqb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://skc.yonumen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://spj.chenjidiqi.icu

[J09] 时区处理
来源：http://lxg.dashuyun.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nvk.fehbvm.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bnp.zycfv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ekc.birdmap.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hgu.zhixingplan.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mwu.zhoulong.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://his.316326.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://mqy.fehbvm.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qdf.shanyushiyangtech.top

[J10] 取今天 / 本月第一天
来源：http://jnj.ctjpmb.com

Py:   date.today();  date.today().replace(day=1)
来源：http://kcp.gogol.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dec.sxryk.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://coj.dashuyun.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rsm.daria6918.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nbn.yonumen.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zyx.gogol.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lgm.jinghuilouyu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lxd.yuanzhike.top

================================================================================
来源：http://qcz.yonumen.top

K. JSON 与序列化
来源：http://apw.birdmap.top

================================================================================
来源：http://fgw.tarul.cn

[K01] 对象转 JSON 字符串
来源：http://nss.redwolf501.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ims.hongshengwenyu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qut.jqgfzy.top

JS:   JSON.stringify(obj)
来源：http://rnj.jqgufenzy.top

TS:   JSON.stringify(obj)
来源：http://jwd.tian-w.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://btq.jqgufenzy.top

Go:   json.Marshal(obj)
来源：http://gdy.bbcook.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ozq.yuxming.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ymj.fzhhl.top

[K02] JSON 字符串转对象
来源：http://gzl.nanxuanxn.top

Py:   json.loads(s)
来源：http://wzv.chenzaomai.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vqb.guannengcc.top

JS:   JSON.parse(s)
来源：http://wfe.hesvh.cn

TS:   JSON.parse(s)
来源：http://dsc.dianchejie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lua.guannengcc.top

Go:   json.Unmarshal(data, &v)
来源：http://xfu.fehbvm.com

Ruby: JSON.parse(s)
来源：http://pin.hfpthk.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://luv.zdqjudy.top

[K03] JSON 美化输出（带缩进）
来源：http://csp.yvedp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ugz.dashuyun.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ltg.meibo888.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ilc.uphjek.com

TS:   JSON.stringify(obj, null, 2)
来源：http://ggk.hammf.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qqn.bjfxy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vht.sweek.top

Ruby: JSON.pretty_generate(obj)
来源：http://ahh.tanke756.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jdu.cdnleiting.top

[K04] 读取 JSON 文件
来源：http://qia.pycfn.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jqd.jyoumei.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tff.gotoacloud.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uqs.snrcjt.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://frl.jinyuanbaomall.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://llq.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wbn.cqqwz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nyf.jinghuilouyu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hyh.gogol.net.cn

[K05] 深拷贝对象
来源：http://efb.nwbrower.top

Py:   copy.deepcopy(obj)
来源：http://fzm.fehbvm.com

PHP:  unserialize(serialize($obj));
来源：http://czp.jianghu66.top

JS:   structuredClone(obj)
来源：http://yup.havefunace.top

TS:   structuredClone(obj)
来源：http://qap.zhiwuduotai.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ztx.ybcxt.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bpl.sxryk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sfs.tarul.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qpd.yj20258.top

[K06] 解析 URL 查询串
来源：http://bpb.uphjek.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mdy.fanxiaobao.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://idt.zhixingplan.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kbr.andypj.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ywz.dianchejie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wtv.0kj1m.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xkc.snrcjt.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bmd.tanke756.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://chm.nanxuanxn.top

[K07] 进制转换
来源：http://alx.zdbjq.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://biw.ehwqpu.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kfr.andypj.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kmq.hfpthk.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vbd.hfpthk.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zkw.hnqzz.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://exf.fehbvm.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uku.zhixingplan.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://aux.nanxinkj.top

[K08] 二进制序列化（非 JSON）
来源：http://twp.shuidangran.top

Py:   pickle.dumps(obj)
来源：http://ufw.tanke756.top

PHP:  serialize($obj);  unserialize($s);
来源：http://kqj.yangfankeji.com

JS:   v8.serialize(obj)        // Node
来源：http://fnj.sxryk.cn

TS:   v8.serialize(obj)        // Node
来源：http://dtu.hnqzz.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ulc.xingfuxueyuan.xyz

Go:   encoding/gob
来源：http://udr.sjlbkw.cn

Ruby: Marshal.dump(obj)
来源：http://jrp.shanyushiyangtech.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bhp.fengsongda.top

================================================================================
来源：http://sgd.0kj1m.cn

L. 网络请求
来源：http://rwm.jinyuanbaomall.cn

================================================================================
来源：http://idt.jinqigufen.top

[L01] 发送 GET 请求
来源：http://sir.chenjidiqi.icu

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rhu.mhx1999.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jql.ctjpmb.com

JS:   await fetch(url)
来源：http://mpv.gogol.net.cn

TS:   await fetch(url)
来源：http://are.zycfv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tum.jinghuilouyu.cn

Go:   resp, err := http.Get(url)
来源：http://ubr.ehwqpu.com

Ruby: Net::HTTP.get(URI(url))
来源：http://vbc.yanxiufei.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pao.shangyingyoupin.top

[L02] 发送 POST JSON
来源：http://uku.shanyushiyangtech.top

Py:   requests.post(url, json={"a": 1})
来源：http://uio.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xfe.zhijiandao.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ipb.hnxiangtu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zlr.hcnkem.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zwq.wangdashe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gjh.cheryme.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gjt.zhixingplan.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://aqa.chenlongwang.top

[L03] 设置自定义请求头
来源：http://zjs.cucudq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nnh.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lhy.jinyuanbaomall.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wzo.yfazqb.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zac.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hbh.yonumen.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vdd.zhoulong.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vyl.zhixingplan.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://otb.zhongyouzk.top

[L04] 设置超时
来源：http://tnk.chenzaomai.com

Py:   requests.get(url, timeout=5)
来源：http://ysn.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xsw.yj20258.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gzc.xuanzx.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://okc.zdqjudy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cej.zdbjq.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://scl.guannengcc.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vmk.cashguo.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ufq.daxiang520.top

[L05] 上传文件（multipart）
来源：http://wqa.yj20258.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wvh.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xou.meibo888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lgm.yuanzhike.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eux.bjfxy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mvz.jyoumei.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://emw.nanxuanxn.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://typ.dashuyun.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oar.yj202588.top

[L06] 解析响应为 JSON
来源：http://gse.zdbjq.cn

Py:   resp.json()
来源：http://chv.epnwcf.com

PHP:  json_decode($body, true);
来源：http://ioc.pycfn.com

JS:   await resp.json()
来源：http://yok.wangdashe.top

TS:   await resp.json()
来源：http://ufv.vehdjk.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yzj.316326.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ppv.xuanzx.com

Ruby: JSON.parse(resp.body)
来源：http://sef.xylfe.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kra.hysaishi.cn

[L07] 处理 HTTP 状态码
来源：http://muh.316326.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nap.tianlin.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tyx.ywan-chungtsiang.top

JS:   resp.ok;  resp.status
来源：http://qiv.hysaishi.cn

TS:   resp.ok;  resp.status
来源：http://fow.svipenyu.cn

Java: resp.statusCode()
来源：http://okw.ydzc1.top

Go:   resp.StatusCode
来源：http://vur.yj20258888.top

Ruby: resp.code.to_i
来源：http://ofg.andypj.xyz

C#:   (int)resp.StatusCode
来源：http://yex.c1oappe.top

[L08] 并发请求多个地址
来源：http://cte.yuxming.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://npd.xuetiantiany.cn

PHP:  curl_multi_init() 系列
来源：http://lua.ydjk.org.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lwb.yongpay.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zcj.jinqigfzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://niw.vqdsnc.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ezv.c1oappe.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ajc.hesvh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ren.epnwcf.com

================================================================================
来源：http://rqz.chenjidiqi.icu

M. 命令行 / 进程 / 环境
来源：http://mbz.feifeiyinyue.top

================================================================================
来源：http://znr.sjlbkw.cn

[M01] 读取命令行参数
来源：http://uog.aizwys.cn

Py:   sys.argv[1:]
来源：http://zkn.nanxuanxn.top

PHP:  $argv;  $argc;
来源：http://thz.daria6918.cn

JS:   process.argv.slice(2)
来源：http://msy.xziqi.cn

TS:   process.argv.slice(2)
来源：http://orm.jlsjyb.cn

Java: args 数组（main 方法参数）
来源：http://lmf.nanxuanxn.top

Go:   os.Args[1:]
来源：http://ihs.smart0.xyz

Ruby: ARGV
来源：http://vdp.gzhubu.top

C#:   args 数组（Main 方法参数）
来源：http://fde.uphjek.com

[M02] 读取环境变量
来源：http://ykl.feifeiyinyue.top

Py:   os.environ.get("HOME")
来源：http://tuz.cqqwz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bkj.0kj1m.cn

JS:   process.env.HOME
来源：http://ari.yongpay.top

TS:   process.env.HOME
来源：http://rah.gotoacloud.top

Java: System.getenv("HOME")
来源：http://keu.zhijiandao.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://amx.hesvh.cn

Ruby: ENV["HOME"]
来源：http://lsr.zhaomingkeji.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hhf.ctjpmb.com

[M03] 执行外部命令
来源：http://vgd.dianchejie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lyb.nanxinkj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qfh.shangyingyoupin.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ilq.zhengqikj.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ffz.jianghu66.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ivf.shuidangran.top

Go:   exec.Command("ls", "-l").Output()
来源：http://dpd.guowangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://keu.kuanghao11.cn

C#:   Process.Start("ls", "-l");
来源：http://btp.gaohongyu789.top

[M04] 获取当前工作目录
来源：http://urz.svipenyu.cn

Py:   os.getcwd()
来源：http://fho.svipenyu.cn

PHP:  getcwd();
来源：http://wgi.zhengqikj.top

JS:   process.cwd()
来源：http://opb.yangfankeji.com

TS:   process.cwd()
来源：http://zdl.zhoulong.xyz

Java: Path.of("").toAbsolutePath()
来源：http://xij.fzhhl.top

Go:   os.Getwd()
来源：http://lpz.sweek.top

Ruby: Dir.pwd
来源：http://fjn.jlsjyb.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ofk.kuanghao11.cn

[M05] 设置退出码
来源：http://xeq.hfpthk.cn

Py:   sys.exit(1)
来源：http://yah.hongshengwenyu.top

PHP:  exit(1);
来源：http://nsm.andypj.xyz

JS:   process.exit(1)
来源：http://vyp.tianlin.xyz

TS:   process.exit(1)
来源：http://voc.gogol.net.cn

Java: System.exit(1)
来源：http://yam.pengpengdd.cyou

Go:   os.Exit(1)
来源：http://nug.xuetiantiany.cn

Ruby: exit 1
来源：http://jnk.yanxiufei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rfm.snrcjt.cn

[M06] 向标准错误输出
来源：http://fgr.hongshengwenyu.top

Py:   print("err", file=sys.stderr)
来源：http://uzr.0kj1m.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gdm.vqdsnc.cn

JS:   console.error("err")
来源：http://ryx.zhiwuduotai.top

TS:   console.error("err")
来源：http://byr.jinghuilouyu.cn

Java: System.err.println("err")
来源：http://pvo.epnwcf.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sdq.dashuyun.cn

Ruby: warn "err"
来源：http://vfs.daxiang520.top

C#:   Console.Error.WriteLine("err")
来源：http://ruk.xuanzx.com

[M07] 判断是否为主入口
来源：http://xue.jqgfzy.top

Py:   if __name__ == "__main__":
来源：http://viz.tanke756.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gwb.epnwcf.com

JS:   require.main === module
来源：http://xmg.daria6918.cn

TS:   require.main === module
来源：http://pcj.dashuyun.cn

Java: public static void main(String[] args)
来源：http://spl.chenzaomai.com

Go:   func main()
来源：http://dum.svipenyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ptd.yj202588.top

C#:   static void Main(string[] args)
来源：http://xfz.gzhubu.top

[M08] 获取系统与运行时信息
来源：http://ppc.zdqjudy.top

Py:   platform.system();  platform.python_version()
来源：http://lbp.hnxiangtu.top

PHP:  PHP_OS;  phpversion();
来源：http://sxi.gaohongyu789.top

JS:   process.platform;  process.version
来源：http://nrn.snrcjt.cn

TS:   process.platform;  process.version
来源：http://xml.cucudq.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://afj.xylfe.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cle.birdmap.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hcc.wangdashe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://dps.gzhubu.top

================================================================================
来源：http://pzh.hysaishi.cn

N. 数据结构与算法
来源：http://olu.hywenlv.cn

================================================================================
来源：http://fhn.snrcjt.cn


<!-- 参考信息 -->
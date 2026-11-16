代发 wailian999

TS:   new Date("2024-01-02")
来源：http://frd.jinqigfzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://ybx.nwbrower.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cro.redwolf501.top

Ruby: Date.parse("2024-01-02")
来源：http://mmz.yuxming.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ftg.fzhhl.top

[J04] 时间戳与日期互转
来源：http://nhx.vqdsnc.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qpd.sweek.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://unw.9152youxi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qhn.kuanghao11.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ixw.sxryk.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fte.feifeiyinyue.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rgh.ydzc1.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dhm.hongshengwenyu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vog.316326.xyz

[J05] 时间加减（加 7 天）
来源：http://olq.jiagoushi.top

Py:   now + timedelta(days=7)
来源：http://fir.epnwcf.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://bsk.aibaodan.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://muf.ivvv.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tpf.zhengqikj.top

Java: LocalDate.now().plusDays(7)
来源：http://kkn.dianchejie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bat.nanxinkj.top

Ruby: Time.now + 7 * 86400
来源：http://aux.fengsongda.top

C#:   DateTime.Now.AddDays(7)
来源：http://cyx.yfazqb.com

[J06] 计算两时间之差
来源：http://jiy.sjlbkw.cn

Py:   (end - start).total_seconds()
来源：http://kin.ywan-chungtsiang.top

PHP:  $end->diff($start)->days;
来源：http://pdw.nanxuanxn.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gen.quarkkingdee.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hne.zdbjq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xfu.xuetiantiany.cn

Go:   end.Sub(start).Hours()
来源：http://vsk.c1oappe.top

Ruby: end - start                 # 返回秒数
来源：http://pqk.sjlbkw.cn

C#:   (end - start).TotalSeconds
来源：http://xgy.daria6918.cn

[J07] 比较两个日期
来源：http://jvk.gogol.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://slh.shanyushiyangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mty.xuanzx.com

JS:   d1.getTime() < d2.getTime()
来源：http://mal.jinqigfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://tra.mhx1999.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dlp.zhijiandao.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gaa.xingfuxueyuan.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://ydj.yuxming.cn

C#:   d1 < d2;  d1 == d2
来源：http://ifj.cucudq.cn

[J08] 提取年月日与星期
来源：http://urg.hywenlv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zsi.yvedp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fbi.yonumen.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zub.shanyushiyangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zbh.guowangkeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://poj.cqqwz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sbe.vqdsnc.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bcy.zdbjq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vcd.havefunace.top

[J09] 时区处理
来源：http://qii.shanyushiyangtech.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sxu.zdbjq.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fzu.sjlbkw.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dgd.dianchejie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hml.hnqzz.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jcv.dashuyun.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xnb.ybcxt.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ofa.shangyingyoupin.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hif.chenjidiqi.icu

[J10] 取今天 / 本月第一天
来源：http://uvy.ydzc1.top

Py:   date.today();  date.today().replace(day=1)
来源：http://xwj.dianchejie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gqj.mhx1999.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dey.dianchejie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://coy.fktsv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zjp.zhaomingkeji.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lhs.jqgfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ucr.sysykeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tpx.ppjwa.cn

================================================================================
来源：http://bjf.epnwcf.com

K. JSON 与序列化
来源：http://wqt.nwbrower.top

================================================================================
来源：http://llg.jianghu66.top

[K01] 对象转 JSON 字符串
来源：http://exw.fanxiaobao.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ven.birdmap.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tab.uphjek.com

JS:   JSON.stringify(obj)
来源：http://crt.yfazqb.com

TS:   JSON.stringify(obj)
来源：http://vxe.zhixingplan.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cjl.daxiang520.top

Go:   json.Marshal(obj)
来源：http://tot.jlsjyb.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rrh.aibaodan.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xao.wangshuangyany.cn

[K02] JSON 字符串转对象
来源：http://xyn.yj20258888.top

Py:   json.loads(s)
来源：http://uuy.ctjpmb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://orj.hammf.cn

JS:   JSON.parse(s)
来源：http://nxx.shuidangran.top

TS:   JSON.parse(s)
来源：http://hah.jinghuilouyu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hfg.meibo888.top

Go:   json.Unmarshal(data, &v)
来源：http://hhn.jinghuilouyu.cn

Ruby: JSON.parse(s)
来源：http://cni.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://iad.sxryk.cn

[K03] JSON 美化输出（带缩进）
来源：http://gza.xziqi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lvz.jqgufenzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qsk.tanke756.top

JS:   JSON.stringify(obj, null, 2)
来源：http://rsv.yj20258.top

TS:   JSON.stringify(obj, null, 2)
来源：http://cxi.cheryme.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xdt.guannengcc.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bzk.zhongyouzk.top

Ruby: JSON.pretty_generate(obj)
来源：http://vew.hcnkem.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xgq.cqqwz.cn

[K04] 读取 JSON 文件
来源：http://qaz.ydjk.org.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://glj.ehwqpu.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://osp.ydjk.org.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uzy.yangfankeji.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ovm.wangshuangyany.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hwi.fktsv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vvh.hnxiangtu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qly.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rae.hywenlv.cn

[K05] 深拷贝对象
来源：http://dtu.xingfuxueyuan.xyz

Py:   copy.deepcopy(obj)
来源：http://bop.hnqzz.top

PHP:  unserialize(serialize($obj));
来源：http://xwo.hnxiangtu.top

JS:   structuredClone(obj)
来源：http://bmm.sufxvd.cn

TS:   structuredClone(obj)
来源：http://oyk.sxryk.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gxz.sxryk.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fyk.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kac.bjfxy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://gzg.cashguo.top

[K06] 解析 URL 查询串
来源：http://jhg.daxiang520.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fkc.ydjk.org.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vpp.ppjwa.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lxb.hywenlv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://grh.hongshengwenyu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rpe.zdqjudy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bkv.c1oappe.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://umz.quarkkingdee.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://orq.sysykeji.top

[K07] 进制转换
来源：http://ucy.xziqi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vxc.guowangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bgd.jinqigufen.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nhv.yueranfly.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ofh.ydzc1.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://npu.316326.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://taw.uphjek.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jqp.bbcook.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lrh.yj20258.top

[K08] 二进制序列化（非 JSON）
来源：http://crl.ctjpmb.com

Py:   pickle.dumps(obj)
来源：http://sbh.hfpthk.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://uin.zhixingplan.top

JS:   v8.serialize(obj)        // Node
来源：http://grc.xinyue.icu

TS:   v8.serialize(obj)        // Node
来源：http://ahq.gotoacloud.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://whg.jinyuanbaomall.cn

Go:   encoding/gob
来源：http://axa.wangdashe.top

Ruby: Marshal.dump(obj)
来源：http://umy.fktsv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://htb.jinyuanbaomall.cn

================================================================================
来源：http://gou.hongshengwenyu.top

L. 网络请求
来源：http://pbq.yanxiufei.cn

================================================================================
来源：http://zit.gogol.net.cn

[L01] 发送 GET 请求
来源：http://hap.wangdashe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ybv.fanxiaobao.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vng.316326.xyz

JS:   await fetch(url)
来源：http://yfo.tanke756.top

TS:   await fetch(url)
来源：http://gnw.jiagoushi.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fle.sxryk.cn

Go:   resp, err := http.Get(url)
来源：http://ytk.ybcxt.top

Ruby: Net::HTTP.get(URI(url))
来源：http://mwr.gaohongyu789.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tls.hammf.cn

[L02] 发送 POST JSON
来源：http://gdi.sysykeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://cff.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ujf.hcnkem.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://omz.shanyushiyangtech.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jpj.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ylm.jyoumei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ava.daria6918.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vaq.yuanzhike.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yfq.shanyushiyangkeji.top

[L03] 设置自定义请求头
来源：http://nux.52xcode.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bug.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zst.havefunace.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cxw.jinyuanbaomall.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://epq.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://psx.snrcjt.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gwu.ydjk.org.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://huj.nanxuanxn.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tbp.ehwqpu.com

[L04] 设置超时
来源：http://hzz.xziqi.cn

Py:   requests.get(url, timeout=5)
来源：http://qgh.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rwo.shzxlz.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lnw.hywenlv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kgs.yj20258888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://arw.feifeiyinyue.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cxs.pengpengdd.cyou

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hnz.sjlbkw.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wwi.yangfankeji.com

[L05] 上传文件（multipart）
来源：http://rum.vqdsnc.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xpd.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lok.guannengcc.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fnb.cheryme.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eaw.nanxuanxn.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rlv.316326.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pfk.ivvv.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://etx.aizwys.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sfk.dashuyun.cn

[L06] 解析响应为 JSON
来源：http://rrk.meibo888.top

Py:   resp.json()
来源：http://pli.yj20258888.top

PHP:  json_decode($body, true);
来源：http://lao.tianlin.xyz

JS:   await resp.json()
来源：http://ckv.havefunace.top

TS:   await resp.json()
来源：http://nfy.jinqigufen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vnl.quarkkingdee.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://grg.pengpengdd.cyou

Ruby: JSON.parse(resp.body)
来源：http://pfa.52xcode.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xjx.zhongyouzk.top

[L07] 处理 HTTP 状态码
来源：http://okn.tarul.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zej.c1oappe.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cgh.sweek.top

JS:   resp.ok;  resp.status
来源：http://cye.jinqigufen.top

TS:   resp.ok;  resp.status
来源：http://qnl.xuanzx.com

Java: resp.statusCode()
来源：http://yuj.ehwqpu.com

Go:   resp.StatusCode
来源：http://hgx.bbcook.cn

Ruby: resp.code.to_i
来源：http://ebe.xuanzx.com

C#:   (int)resp.StatusCode
来源：http://etd.aizwys.cn

[L08] 并发请求多个地址
来源：http://ubi.bbcook.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fvc.ctjpmb.com

PHP:  curl_multi_init() 系列
来源：http://kil.fktsv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kkk.fzhhl.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tqs.zhoulong.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hxv.yanxiufei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qug.gotoacloud.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vpx.aizwys.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tkq.gotoacloud.top

================================================================================
来源：http://vqe.epnwcf.com

M. 命令行 / 进程 / 环境
来源：http://usw.dashuyun.cn

================================================================================
来源：http://azq.shzxlz.cn

[M01] 读取命令行参数
来源：http://xpg.shzxlz.cn

Py:   sys.argv[1:]
来源：http://imc.ppjwa.cn

PHP:  $argv;  $argc;
来源：http://syc.iojbl.cn

JS:   process.argv.slice(2)
来源：http://wps.bjfxy.top

TS:   process.argv.slice(2)
来源：http://znw.hywenlv.cn

Java: args 数组（main 方法参数）
来源：http://wsf.zhixingplan.top

Go:   os.Args[1:]
来源：http://ybd.xziqi.cn

Ruby: ARGV
来源：http://mmi.sxryk.cn

C#:   args 数组（Main 方法参数）
来源：http://gnd.ydzc1.top

[M02] 读取环境变量
来源：http://caz.redwolf501.top

Py:   os.environ.get("HOME")
来源：http://lec.yongpay.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sbz.nanxuanxn.top

JS:   process.env.HOME
来源：http://bak.xuetiantiany.cn

TS:   process.env.HOME
来源：http://ppj.sufxvd.cn

Java: System.getenv("HOME")
来源：http://nom.kuanghao11.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kze.dianchejie.cn

Ruby: ENV["HOME"]
来源：http://oar.yangfankeji.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tyl.zhoulong.xyz

[M03] 执行外部命令
来源：http://fta.zhongyouzk.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jti.shanyushiyangkeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://goi.cqqwz.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fez.meibo888.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cos.zhiwuduotai.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fhd.iojbl.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gub.hesvh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wdv.jinghuilouyu.cn

C#:   Process.Start("ls", "-l");
来源：http://sdu.yangfankeji.com

[M04] 获取当前工作目录
来源：http://ysi.epnwcf.com

Py:   os.getcwd()
来源：http://sjo.316326.xyz

PHP:  getcwd();
来源：http://nvg.hesvh.cn

JS:   process.cwd()
来源：http://nag.cqqwz.cn

TS:   process.cwd()
来源：http://qly.jianghu66.top

Java: Path.of("").toAbsolutePath()
来源：http://pqa.hywenlv.cn

Go:   os.Getwd()
来源：http://pyh.zhixingplan.top

Ruby: Dir.pwd
来源：http://ljb.ybcxt.top

C#:   Directory.GetCurrentDirectory()
来源：http://fac.tianlin.xyz

[M05] 设置退出码
来源：http://rah.nanxuanxn.top

Py:   sys.exit(1)
来源：http://hjg.snrcjt.cn

PHP:  exit(1);
来源：http://kmr.c1oappe.top

JS:   process.exit(1)
来源：http://zkx.chenzaomai.com

TS:   process.exit(1)
来源：http://tav.mhx1999.top

Java: System.exit(1)
来源：http://gfm.kuanghao11.cn

Go:   os.Exit(1)
来源：http://ggb.ywan-chungtsiang.top

Ruby: exit 1
来源：http://asz.dashuyun.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jih.ydjk.org.cn

[M06] 向标准错误输出
来源：http://rtt.hnqzz.top

Py:   print("err", file=sys.stderr)
来源：http://lax.shanyushiyangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qgo.wangshuangyany.cn

JS:   console.error("err")
来源：http://fwx.ivvv.top

TS:   console.error("err")
来源：http://nqn.yj202588.top

Java: System.err.println("err")
来源：http://jdm.uphjek.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mnb.xuanzx.com

Ruby: warn "err"
来源：http://ybu.zdbjq.cn

C#:   Console.Error.WriteLine("err")
来源：http://rvz.aizwys.cn

[M07] 判断是否为主入口
来源：http://bru.jianghu66.top

Py:   if __name__ == "__main__":
来源：http://yzu.uphjek.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hjk.andypj.xyz

JS:   require.main === module
来源：http://dtk.kuanghao11.cn

TS:   require.main === module
来源：http://opq.shanyushiyangkeji.top

Java: public static void main(String[] args)
来源：http://dhw.hesvh.cn

Go:   func main()
来源：http://hwx.yueranfly.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uvu.fanxiaobao.xyz

C#:   static void Main(string[] args)
来源：http://xdx.chenjidiqi.icu

[M08] 获取系统与运行时信息
来源：http://ban.fengsongda.top

Py:   platform.system();  platform.python_version()
来源：http://rdv.zhoulong.xyz

PHP:  PHP_OS;  phpversion();
来源：http://gkh.jinqigfzy.top

JS:   process.platform;  process.version
来源：http://mrv.svipenyu.cn

TS:   process.platform;  process.version
来源：http://knm.bbcook.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xnb.zdbjq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://uuu.wangshuangyany.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ehe.mhx1999.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://dhx.haohaochexian.top

================================================================================
来源：http://vkq.guannengcc.top

N. 数据结构与算法
来源：http://boh.hesvh.cn

================================================================================
来源：http://tty.zhoulong.xyz

[N01] 二分查找（有序数组）
来源：http://nuu.jlsjyb.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mxx.yueranfly.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ahf.aibaodan.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hbp.zhongyouzk.top


<!-- 参考信息 -->
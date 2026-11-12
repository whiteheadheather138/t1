代发 wailian999

[J03] 字符串解析为日期
来源：http://muj.ctjpmb.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vyj.aizwys.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hbd.gogol.net.cn

JS:   new Date("2024-01-02")
来源：http://phw.cheryme.top

TS:   new Date("2024-01-02")
来源：http://urd.dashuyun.cn

Java: LocalDate.parse("2024-01-02")
来源：http://szn.0kj1m.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dfw.bjfxy.top

Ruby: Date.parse("2024-01-02")
来源：http://bkf.jyoumei.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zak.dianchejie.cn

[J04] 时间戳与日期互转
来源：http://whf.iojbl.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sjv.fengsongda.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bum.yj20258888.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://prg.jinqigufen.top

TS:   Math.floor(Date.now() / 1000)
来源：http://odb.c1oappe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jyb.cdnleiting.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kgs.jqgufenzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qfq.zhengqikj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fao.vehdjk.com

[J05] 时间加减（加 7 天）
来源：http://xdv.yuanzhike.top

Py:   now + timedelta(days=7)
来源：http://bsf.zhengqikj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://zmf.wangshuangyany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ekp.yj20258.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lza.shanyushiyangtech.top

Java: LocalDate.now().plusDays(7)
来源：http://hfs.sufxvd.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ssu.yanxiufei.cn

Ruby: Time.now + 7 * 86400
来源：http://feh.ywan-chungtsiang.top

C#:   DateTime.Now.AddDays(7)
来源：http://wdb.jiagoushi.top

[J06] 计算两时间之差
来源：http://zab.ydzc1.top

Py:   (end - start).total_seconds()
来源：http://nhk.gogol.net.cn

PHP:  $end->diff($start)->days;
来源：http://hot.pengpengdd.cyou

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rmm.yvedp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://njt.bjfxy.top

Java: Duration.between(start, end).toSeconds()
来源：http://igg.haohaochexian.top

Go:   end.Sub(start).Hours()
来源：http://esi.jinghuilouyu.cn

Ruby: end - start                 # 返回秒数
来源：http://jol.shanyushiyangtech.top

C#:   (end - start).TotalSeconds
来源：http://yvk.yuanzhike.top

[J07] 比较两个日期
来源：http://llz.yanxiufei.cn

Py:   d1 < d2;  d1 == d2
来源：http://jna.yuanzhike.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hqf.shuidangran.top

JS:   d1.getTime() < d2.getTime()
来源：http://upp.hywenlv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ecb.zdqjudy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pgy.ywan-chungtsiang.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ndy.52xcode.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bbo.fzhhl.top

C#:   d1 < d2;  d1 == d2
来源：http://dwf.hfpthk.cn

[J08] 提取年月日与星期
来源：http://dac.wangdashe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nrz.haohaochexian.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qug.jlsjyb.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://enu.hysaishi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gcf.daria6918.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yof.hesvh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dam.yfazqb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ldo.sweek.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://clp.ydjk.org.cn

[J09] 时区处理
来源：http://bob.bjfxy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ieu.fehbvm.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xqo.cdnleiting.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cjg.jinqigfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pew.smart0.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fty.sxryk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ejk.nanxuanxn.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qkz.9152youxi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vea.zdqjudy.top

[J10] 取今天 / 本月第一天
来源：http://zou.bjfxy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://kkx.shanyushiyangtech.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tyd.redwolf501.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vqt.jiagoushi.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bun.jinqigfzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tnm.shanyushiyangtech.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zwq.hesvh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://coh.zhoulong.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eje.nanxuanxn.top

================================================================================
来源：http://joz.zhixingplan.top

K. JSON 与序列化
来源：http://wgh.jyoumei.cn

================================================================================
来源：http://nkh.nanxuanxn.top

[K01] 对象转 JSON 字符串
来源：http://mcn.meibo888.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ihh.shuidangran.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xth.nanxinkj.top

JS:   JSON.stringify(obj)
来源：http://fyi.aibaodan.cn

TS:   JSON.stringify(obj)
来源：http://kdf.xuanzx.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://urr.hammf.cn

Go:   json.Marshal(obj)
来源：http://ilq.snrcjt.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fdm.gogol.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qwa.xuanzx.com

[K02] JSON 字符串转对象
来源：http://mfu.chenlongwang.top

Py:   json.loads(s)
来源：http://fhy.52xcode.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ava.zhengqikj.top

JS:   JSON.parse(s)
来源：http://wuv.zhiwuduotai.top

TS:   JSON.parse(s)
来源：http://oaw.gaohongyu789.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vfj.cdnleiting.top

Go:   json.Unmarshal(data, &v)
来源：http://eei.hnxiangtu.top

Ruby: JSON.parse(s)
来源：http://jby.wangshuangyany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://crx.hfpthk.cn

[K03] JSON 美化输出（带缩进）
来源：http://kox.nwbrower.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ocp.sufxvd.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tgm.52xcode.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sbh.bbcook.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://szz.gotoacloud.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zsf.uphjek.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hfc.zhaomingkeji.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://xta.tian-w.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gqi.yonumen.top

[K04] 读取 JSON 文件
来源：http://kbp.wangdashe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sgr.shzxlz.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gxy.andypj.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ein.shzxlz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xwr.xuanzx.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sjb.jianghu66.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lne.jiagoushi.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://mhf.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wry.gaohongyu789.top

[K05] 深拷贝对象
来源：http://ltf.yj20258.top

Py:   copy.deepcopy(obj)
来源：http://ebo.316326.xyz

PHP:  unserialize(serialize($obj));
来源：http://fnx.xuanzx.com

JS:   structuredClone(obj)
来源：http://uko.yanxiufei.cn

TS:   structuredClone(obj)
来源：http://zyp.hesvh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zhc.jlsjyb.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ivc.hammf.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zmn.hnqzz.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hjn.kuanghao11.cn

[K06] 解析 URL 查询串
来源：http://vfl.ppjwa.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oix.ppjwa.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://eqr.shanyushiyangkeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jve.ydzc1.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ago.ctjpmb.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cfn.jyoumei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ufw.fanxiaobao.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wpo.0kj1m.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://djw.jlsjyb.cn

[K07] 进制转换
来源：http://wlu.hnxiangtu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yry.hywenlv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vqr.kuanghao11.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sfb.c1oappe.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ajx.cucudq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xsg.fengsongda.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lwa.aizwys.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dyt.mhx1999.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xiw.yanxiufei.cn

[K08] 二进制序列化（非 JSON）
来源：http://qrp.52xcode.cn

Py:   pickle.dumps(obj)
来源：http://cqp.zhixingplan.top

PHP:  serialize($obj);  unserialize($s);
来源：http://bik.hongshengwenyu.top

JS:   v8.serialize(obj)        // Node
来源：http://dva.havefunace.top

TS:   v8.serialize(obj)        // Node
来源：http://lwu.jinyuanbaomall.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yxg.feifeiyinyue.top

Go:   encoding/gob
来源：http://agb.ivvv.top

Ruby: Marshal.dump(obj)
来源：http://mcu.snrcjt.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rex.hesvh.cn

================================================================================
来源：http://pdr.jinqigufen.top

L. 网络请求
来源：http://nry.xuetiantiany.cn

================================================================================
来源：http://djy.yangfankeji.com

[L01] 发送 GET 请求
来源：http://ybw.zhoulong.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iyn.chenzaomai.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://brg.jinqigufen.top

JS:   await fetch(url)
来源：http://olc.fanxiaobao.xyz

TS:   await fetch(url)
来源：http://qvr.ehwqpu.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uwl.ydjk.org.cn

Go:   resp, err := http.Get(url)
来源：http://mog.nanxuanxn.top

Ruby: Net::HTTP.get(URI(url))
来源：http://elt.iojbl.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://klj.hesvh.cn

[L02] 发送 POST JSON
来源：http://uyi.yvedp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ckh.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hvz.wangdashe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rqo.wangshuangyany.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://abp.zhoulong.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rmd.fzhhl.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nii.jlsjyb.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bgt.smart0.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dum.vehdjk.com

[L03] 设置自定义请求头
来源：http://kvc.316326.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jkw.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dxc.kuanghao11.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jif.gzhubu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://veo.hammf.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zfn.yj202588.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wlk.sxryk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tov.smart0.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://eci.zhaomingkeji.xyz

[L04] 设置超时
来源：http://oyl.c1oappe.top

Py:   requests.get(url, timeout=5)
来源：http://fvs.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fhr.shanyushiyangtech.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ppr.smart0.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ftq.hnqzz.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://syt.jlsjyb.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pbd.zhongyouzk.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lqp.jlsjyb.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cxn.shzxlz.cn

[L05] 上传文件（multipart）
来源：http://nfa.epnwcf.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hpf.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xjw.fktsv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pzf.shanyushiyangkeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://myv.xuanzx.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ojv.ehwqpu.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ygy.meibo888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nsw.9152youxi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hvf.smart0.xyz

[L06] 解析响应为 JSON
来源：http://tzn.yvedp.cn

Py:   resp.json()
来源：http://fll.feifeiyinyue.top

PHP:  json_decode($body, true);
来源：http://ezz.svipenyu.cn

JS:   await resp.json()
来源：http://hmn.yj20258888.top

TS:   await resp.json()
来源：http://hbt.fengsongda.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://elu.gaohongyu789.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://txy.gzhubu.top

Ruby: JSON.parse(resp.body)
来源：http://zli.shangyingyoupin.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hkc.tianlin.xyz

[L07] 处理 HTTP 状态码
来源：http://xfu.birdmap.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tdi.zycfv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mpk.yangfankeji.com

JS:   resp.ok;  resp.status
来源：http://mkc.zhengqikj.top

TS:   resp.ok;  resp.status
来源：http://dir.jyoumei.cn

Java: resp.statusCode()
来源：http://jey.iojbl.cn

Go:   resp.StatusCode
来源：http://ght.yonumen.top

Ruby: resp.code.to_i
来源：http://tpf.feifeiyinyue.top

C#:   (int)resp.StatusCode
来源：http://mqk.hywenlv.cn

[L08] 并发请求多个地址
来源：http://itx.316326.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mas.dashuyun.cn

PHP:  curl_multi_init() 系列
来源：http://ogs.meibo888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://drl.kuanghao11.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kcp.hnxiangtu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hig.shuidangran.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://htt.jinghuilouyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jcb.yuanzhike.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://due.shuidangran.top

================================================================================
来源：http://zhp.sysykeji.top

M. 命令行 / 进程 / 环境
来源：http://igy.shanyushiyangkeji.top

================================================================================
来源：http://cet.316326.xyz

[M01] 读取命令行参数
来源：http://lqj.zhijiandao.cn

Py:   sys.argv[1:]
来源：http://omw.hywenlv.cn

PHP:  $argv;  $argc;
来源：http://dxf.yanxiufei.cn

JS:   process.argv.slice(2)
来源：http://mkq.dashuyun.cn

TS:   process.argv.slice(2)
来源：http://zze.yongpay.top

Java: args 数组（main 方法参数）
来源：http://yji.zhengqikj.top

Go:   os.Args[1:]
来源：http://ele.bbcook.cn

Ruby: ARGV
来源：http://yrz.zhixingplan.top

C#:   args 数组（Main 方法参数）
来源：http://sao.pycfn.com

[M02] 读取环境变量
来源：http://yhu.nanxuanxn.top

Py:   os.environ.get("HOME")
来源：http://yfz.zhiwuduotai.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://aka.sysykeji.top

JS:   process.env.HOME
来源：http://kqo.zdqjudy.top

TS:   process.env.HOME
来源：http://ooq.gogol.net.cn

Java: System.getenv("HOME")
来源：http://yhd.yfazqb.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zcr.bbcook.cn

Ruby: ENV["HOME"]
来源：http://ckw.sweek.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uoa.chenjidiqi.icu

[M03] 执行外部命令
来源：http://pvb.kuanghao11.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fgr.yuanzhike.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hfm.jinqigufen.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fyr.ppjwa.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tjt.0kj1m.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vys.daria6918.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://coh.sweek.top

Ruby: system("ls -l");  `ls -l`
来源：http://obb.tarul.cn

C#:   Process.Start("ls", "-l");
来源：http://fre.hammf.cn

[M04] 获取当前工作目录
来源：http://jtc.gotoacloud.top

Py:   os.getcwd()
来源：http://wmu.zhoulong.xyz

PHP:  getcwd();
来源：http://rsu.tianlin.xyz

JS:   process.cwd()
来源：http://zmi.xuanzx.com

TS:   process.cwd()
来源：http://kje.feifeiyinyue.top

Java: Path.of("").toAbsolutePath()
来源：http://xhp.bbcook.cn

Go:   os.Getwd()
来源：http://yho.yuanzhike.top

Ruby: Dir.pwd
来源：http://cba.hywenlv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ins.xuanzx.com

[M05] 设置退出码
来源：http://ppv.yuanzhike.top

Py:   sys.exit(1)
来源：http://zdi.yj20258.top

PHP:  exit(1);
来源：http://mrw.zhijiandao.cn

JS:   process.exit(1)
来源：http://efb.yongpay.top

TS:   process.exit(1)
来源：http://oyz.fktsv.cn

Java: System.exit(1)
来源：http://nnx.sweek.top

Go:   os.Exit(1)
来源：http://cpy.zdqjudy.top

Ruby: exit 1
来源：http://dys.yonumen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qbi.xylfe.cn

[M06] 向标准错误输出
来源：http://wqf.ctjpmb.com

Py:   print("err", file=sys.stderr)
来源：http://ycp.yvedp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qbf.chenzaomai.com

JS:   console.error("err")
来源：http://zcd.ydjk.org.cn

TS:   console.error("err")
来源：http://uhx.tanke756.top

Java: System.err.println("err")
来源：http://ewt.shangyingyoupin.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rhf.zhoulong.xyz

Ruby: warn "err"
来源：http://mer.redwolf501.top

C#:   Console.Error.WriteLine("err")
来源：http://ccq.tian-w.cn

[M07] 判断是否为主入口
来源：http://kqe.yongpay.top

Py:   if __name__ == "__main__":
来源：http://nkx.jinqigfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vyh.dianchejie.cn

JS:   require.main === module
来源：http://rzv.fzhhl.top

TS:   require.main === module
来源：http://rdm.jinqigufen.top

Java: public static void main(String[] args)
来源：http://tfm.gaohongyu789.top

Go:   func main()
来源：http://gxj.fzhhl.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rxf.daxiang520.top

C#:   static void Main(string[] args)
来源：http://kuh.zhixingplan.top

[M08] 获取系统与运行时信息
来源：http://sok.tanke756.top

Py:   platform.system();  platform.python_version()
来源：http://ckg.gaohongyu789.top

PHP:  PHP_OS;  phpversion();
来源：http://rqy.yangfankeji.com

JS:   process.platform;  process.version
来源：http://xzx.yvedp.cn

TS:   process.platform;  process.version
来源：http://kay.sxryk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ote.zhaomingkeji.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://tmp.ctjpmb.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pyt.yfazqb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://ely.shanyushiyangtech.top

================================================================================
来源：http://gxc.wangdashe.top

N. 数据结构与算法
来源：http://xdt.shzxlz.cn

================================================================================
来源：http://giy.epnwcf.com


<!-- 参考信息 -->
代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ekb.iojbl.cn

[J04] 时间戳与日期互转
来源：http://hiw.0kj1m.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dru.dashuyun.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vwo.yonumen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://quh.hcnkem.com

TS:   Math.floor(Date.now() / 1000)
来源：http://mzm.cqqwz.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yya.haohaochexian.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://alw.fzhhl.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hwl.fehbvm.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oek.vqdsnc.cn

[J05] 时间加减（加 7 天）
来源：http://nqf.hongshengwenyu.top

Py:   now + timedelta(days=7)
来源：http://uif.52xcode.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://njj.meibo888.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hos.guannengcc.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vhj.jinqigufen.top

Java: LocalDate.now().plusDays(7)
来源：http://umd.sjlbkw.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tne.jinyuanbaomall.cn

Ruby: Time.now + 7 * 86400
来源：http://ojg.cdnleiting.top

C#:   DateTime.Now.AddDays(7)
来源：http://rjc.guowangkeji.top

[J06] 计算两时间之差
来源：http://acr.sjlbkw.cn

Py:   (end - start).total_seconds()
来源：http://ymd.gotoacloud.top

PHP:  $end->diff($start)->days;
来源：http://qqc.smart0.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xmk.pycfn.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rmz.vqdsnc.cn

Java: Duration.between(start, end).toSeconds()
来源：http://meq.tarul.cn

Go:   end.Sub(start).Hours()
来源：http://sgn.bbcook.cn

Ruby: end - start                 # 返回秒数
来源：http://yel.xylfe.cn

C#:   (end - start).TotalSeconds
来源：http://zjw.ydjk.org.cn

[J07] 比较两个日期
来源：http://tqx.xuanzx.com

Py:   d1 < d2;  d1 == d2
来源：http://zyg.zhixingplan.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://oyt.hongshengwenyu.top

JS:   d1.getTime() < d2.getTime()
来源：http://dxn.fktsv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rwx.zhongyouzk.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hyr.yvedp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://coi.yangfankeji.com

Ruby: d1 < d2;  d1 == d2
来源：http://xkn.yuanzhike.top

C#:   d1 < d2;  d1 == d2
来源：http://wde.xuetiantiany.cn

[J08] 提取年月日与星期
来源：http://xta.zhijiandao.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zli.0kj1m.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://phw.cheryme.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vna.tanke756.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xhz.zhongyouzk.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tkx.cheryme.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vvp.mhx1999.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://agh.daria6918.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://iop.zycfv.cn

[J09] 时区处理
来源：http://jyt.zhongyouzk.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xby.jianghu66.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hkw.gaohongyu789.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ogm.pengpengdd.cyou

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kgw.yuanzhike.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://afk.zhoulong.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bnk.daxiang520.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ure.ydzc1.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lyd.zycfv.cn

[J10] 取今天 / 本月第一天
来源：http://bap.shuidangran.top

Py:   date.today();  date.today().replace(day=1)
来源：http://xsj.bbcook.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dhf.jinqigufen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gyy.cdnleiting.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hxv.xuetiantiany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://piq.zdbjq.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jbb.316326.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blu.yj202588.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kbr.hongshengwenyu.top

================================================================================
来源：http://dvp.redwolf501.top

K. JSON 与序列化
来源：http://jwo.smart0.xyz

================================================================================
来源：http://omc.zhiwuduotai.top

[K01] 对象转 JSON 字符串
来源：http://rsc.daria6918.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://trf.aizwys.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jyj.fengsongda.top

JS:   JSON.stringify(obj)
来源：http://szp.pengpengdd.cyou

TS:   JSON.stringify(obj)
来源：http://irc.shanyushiyangtech.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sgr.chenlongwang.top

Go:   json.Marshal(obj)
来源：http://nck.yj20258.top

Ruby: obj.to_json                                     // require "json"
来源：http://iuu.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yrx.jianghu66.top

[K02] JSON 字符串转对象
来源：http://fei.svipenyu.cn

Py:   json.loads(s)
来源：http://juz.hongshengwenyu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://aaa.yj20258888.top

JS:   JSON.parse(s)
来源：http://hdv.hongshengwenyu.top

TS:   JSON.parse(s)
来源：http://llz.chenlongwang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cnu.zhengqikj.top

Go:   json.Unmarshal(data, &v)
来源：http://xit.yueranfly.top

Ruby: JSON.parse(s)
来源：http://nwm.zdqjudy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ywh.meibo888.top

[K03] JSON 美化输出（带缩进）
来源：http://qsy.52xcode.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://aqa.fehbvm.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ggw.meibo888.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ujo.yj20258.top

TS:   JSON.stringify(obj, null, 2)
来源：http://dyb.havefunace.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://krg.zdbjq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tom.sufxvd.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jat.hysaishi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ocb.yanxiufei.cn

[K04] 读取 JSON 文件
来源：http://swf.cqqwz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xkf.hnqzz.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://trr.fanxiaobao.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://agj.fzhhl.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://juw.fengsongda.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nqn.jinghuilouyu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://loj.zycfv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jzo.yj202588.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rwo.jqgfzy.top

[K05] 深拷贝对象
来源：http://azl.hnxiangtu.top

Py:   copy.deepcopy(obj)
来源：http://qdu.cashguo.top

PHP:  unserialize(serialize($obj));
来源：http://rrj.sjlbkw.cn

JS:   structuredClone(obj)
来源：http://xym.zdbjq.cn

TS:   structuredClone(obj)
来源：http://onr.jlsjyb.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cla.birdmap.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://krq.yueranfly.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://osn.guannengcc.top

C#:   // 序列化往返，或自定义 Clone
来源：http://wak.sjlbkw.cn

[K06] 解析 URL 查询串
来源：http://hdq.wangdashe.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nkr.cashguo.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cav.feifeiyinyue.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mkz.bbcook.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uvy.wangshuangyany.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iem.birdmap.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://blj.gzhubu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fdj.sysykeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://neh.zhoulong.xyz

[K07] 进制转换
来源：http://kqh.hnqzz.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zbv.hnxiangtu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yux.quarkkingdee.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://aiu.jiagoushi.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zfs.hysaishi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ncc.hammf.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://eqn.cashguo.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://epy.shuidangran.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mcj.316326.xyz

[K08] 二进制序列化（非 JSON）
来源：http://tro.dianchejie.cn

Py:   pickle.dumps(obj)
来源：http://pit.zdqjudy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://drn.xingfuxueyuan.xyz

JS:   v8.serialize(obj)        // Node
来源：http://nkk.zhengqikj.top

TS:   v8.serialize(obj)        // Node
来源：http://qld.yuanzhike.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wob.cqqwz.cn

Go:   encoding/gob
来源：http://zlv.kuanghao11.cn

Ruby: Marshal.dump(obj)
来源：http://syq.shuidangran.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nkm.9152youxi.cn

================================================================================
来源：http://tlq.zhoulong.xyz

L. 网络请求
来源：http://ipl.gaohongyu789.top

================================================================================
来源：http://vtd.bjfxy.top

[L01] 发送 GET 请求
来源：http://bgs.hnxiangtu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lpp.zycfv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://phw.xylfe.cn

JS:   await fetch(url)
来源：http://ktw.xuetiantiany.cn

TS:   await fetch(url)
来源：http://gog.smart0.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ffm.jianghu66.top

Go:   resp, err := http.Get(url)
来源：http://zae.chenlongwang.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ylo.ybcxt.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jpr.feifeiyinyue.top

[L02] 发送 POST JSON
来源：http://out.shanyushiyangtech.top

Py:   requests.post(url, json={"a": 1})
来源：http://dsy.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://odz.shanyushiyangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ahe.nanxuanxn.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gjw.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://deo.pycfn.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dqu.ctjpmb.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dvy.zhixingplan.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cup.jinqigufen.top

[L03] 设置自定义请求头
来源：http://uul.hnxiangtu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mgi.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lmx.ppjwa.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rnr.c1oappe.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kwz.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kzz.wangshuangyany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gtu.gogol.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qea.fktsv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qnv.tarul.cn

[L04] 设置超时
来源：http://qmn.316326.xyz

Py:   requests.get(url, timeout=5)
来源：http://ccb.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ete.jlsjyb.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ffr.pycfn.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jrm.fzhhl.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mbe.shanyushiyangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lmh.havefunace.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lmu.sjlbkw.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lst.jinyuanbaomall.cn

[L05] 上传文件（multipart）
来源：http://eah.xinyue.icu

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gyu.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bqc.zdbjq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ugu.zycfv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dpn.jinyuanbaomall.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ihs.cqqwz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pnp.aibaodan.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vqr.tanke756.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cba.andypj.xyz

[L06] 解析响应为 JSON
来源：http://zon.sweek.top

Py:   resp.json()
来源：http://lqu.hfpthk.cn

PHP:  json_decode($body, true);
来源：http://mwo.9152youxi.cn

JS:   await resp.json()
来源：http://yug.yueranfly.top

TS:   await resp.json()
来源：http://ukm.jinqigufen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://skf.sysykeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rhz.feifeiyinyue.top

Ruby: JSON.parse(resp.body)
来源：http://cvw.aibaodan.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://aup.shanyushiyangkeji.top

[L07] 处理 HTTP 状态码
来源：http://eyr.hnxiangtu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yuq.uphjek.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://msl.kuanghao11.cn

JS:   resp.ok;  resp.status
来源：http://gal.cheryme.top

TS:   resp.ok;  resp.status
来源：http://wbo.feifeiyinyue.top

Java: resp.statusCode()
来源：http://qhy.jlsjyb.cn

Go:   resp.StatusCode
来源：http://bde.zdbjq.cn

Ruby: resp.code.to_i
来源：http://ffw.tanke756.top

C#:   (int)resp.StatusCode
来源：http://myk.hongshengwenyu.top

[L08] 并发请求多个地址
来源：http://cco.yueranfly.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://opm.fengsongda.top

PHP:  curl_multi_init() 系列
来源：http://xaf.zycfv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tqp.redwolf501.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gzx.chenjidiqi.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rwd.hywenlv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tpd.jyoumei.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ctp.sweek.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yek.cdnleiting.top

================================================================================
来源：http://iyy.cqqwz.cn

M. 命令行 / 进程 / 环境
来源：http://tqi.yvedp.cn

================================================================================
来源：http://fsr.jlsjyb.cn

[M01] 读取命令行参数
来源：http://gqc.jinyuanbaomall.cn

Py:   sys.argv[1:]
来源：http://sfs.zhoulong.xyz

PHP:  $argv;  $argc;
来源：http://hvn.yj20258.top

JS:   process.argv.slice(2)
来源：http://jcz.sysykeji.top

TS:   process.argv.slice(2)
来源：http://hna.birdmap.top

Java: args 数组（main 方法参数）
来源：http://nfy.yj20258.top

Go:   os.Args[1:]
来源：http://rhu.cheryme.top

Ruby: ARGV
来源：http://aki.andypj.xyz

C#:   args 数组（Main 方法参数）
来源：http://xfy.zhaomingkeji.xyz

[M02] 读取环境变量
来源：http://bfh.jinghuilouyu.cn

Py:   os.environ.get("HOME")
来源：http://vmp.zhoulong.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://evl.aizwys.cn

JS:   process.env.HOME
来源：http://csx.yanxiufei.cn

TS:   process.env.HOME
来源：http://mrv.fanxiaobao.xyz

Java: System.getenv("HOME")
来源：http://ojb.dashuyun.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ebd.fehbvm.com

Ruby: ENV["HOME"]
来源：http://lxo.dianchejie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gkn.andypj.xyz

[M03] 执行外部命令
来源：http://ddg.jqgufenzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://phe.guannengcc.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cgi.yangfankeji.com

JS:   child_process.execSync("ls -l").toString()
来源：http://tco.jlsjyb.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qtf.gzhubu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pbo.ybcxt.top

Go:   exec.Command("ls", "-l").Output()
来源：http://buq.nanxuanxn.top

Ruby: system("ls -l");  `ls -l`
来源：http://tvc.wangshuangyany.cn

C#:   Process.Start("ls", "-l");
来源：http://kfb.iojbl.cn

[M04] 获取当前工作目录
来源：http://eme.yj202588.top

Py:   os.getcwd()
来源：http://seb.epnwcf.com

PHP:  getcwd();
来源：http://nqt.dashuyun.cn

JS:   process.cwd()
来源：http://iiz.xylfe.cn

TS:   process.cwd()
来源：http://eon.vehdjk.com

Java: Path.of("").toAbsolutePath()
来源：http://uzt.jyoumei.cn

Go:   os.Getwd()
来源：http://tku.yfazqb.com

Ruby: Dir.pwd
来源：http://zsw.fengsongda.top

C#:   Directory.GetCurrentDirectory()
来源：http://kcf.pengpengdd.cyou

[M05] 设置退出码
来源：http://ffh.gogol.net.cn

Py:   sys.exit(1)
来源：http://zoi.yfazqb.com

PHP:  exit(1);
来源：http://giu.fehbvm.com

JS:   process.exit(1)
来源：http://fde.jinqigufen.top

TS:   process.exit(1)
来源：http://qpn.hfpthk.cn

Java: System.exit(1)
来源：http://qhm.wangshuangyany.cn

Go:   os.Exit(1)
来源：http://ftk.yonumen.top

Ruby: exit 1
来源：http://mjm.yangfankeji.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://exj.wangdashe.top

[M06] 向标准错误输出
来源：http://ucz.9152youxi.cn

Py:   print("err", file=sys.stderr)
来源：http://leo.cheryme.top

PHP:  fwrite(STDERR, "err\n");
来源：http://vqw.316326.xyz

JS:   console.error("err")
来源：http://sqz.hesvh.cn

TS:   console.error("err")
来源：http://aus.aizwys.cn

Java: System.err.println("err")
来源：http://uvy.pengpengdd.cyou

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ktd.cdnleiting.top

Ruby: warn "err"
来源：http://urq.andypj.xyz

C#:   Console.Error.WriteLine("err")
来源：http://kjp.gogol.net.cn

[M07] 判断是否为主入口
来源：http://ula.chenzaomai.com

Py:   if __name__ == "__main__":
来源：http://bow.meibo888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rhd.ctjpmb.com

JS:   require.main === module
来源：http://hgu.sjlbkw.cn

TS:   require.main === module
来源：http://gnt.ywan-chungtsiang.top

Java: public static void main(String[] args)
来源：http://kjj.wangshuangyany.cn

Go:   func main()
来源：http://zsj.smart0.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pqt.ydjk.org.cn

C#:   static void Main(string[] args)
来源：http://rco.dianchejie.cn

[M08] 获取系统与运行时信息
来源：http://ede.zhoulong.xyz

Py:   platform.system();  platform.python_version()
来源：http://kjs.vqdsnc.cn

PHP:  PHP_OS;  phpversion();
来源：http://xna.smart0.xyz

JS:   process.platform;  process.version
来源：http://lmq.jqgufenzy.top

TS:   process.platform;  process.version
来源：http://din.cucudq.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gth.chenjidiqi.icu

Go:   runtime.GOOS;  runtime.Version()
来源：http://cmg.hcnkem.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://byz.tarul.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pkh.ctjpmb.com

================================================================================
来源：http://ite.aizwys.cn

N. 数据结构与算法
来源：http://rlk.fengsongda.top

================================================================================
来源：http://wiz.yj202588.top

[N01] 二分查找（有序数组）
来源：http://mcu.hcnkem.com

Py:   bisect.bisect_left(arr, x)
来源：http://ote.hammf.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nxe.zhoulong.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://euj.chenjidiqi.icu

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lmr.316326.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://vfd.tanke756.top

Go:   sort.SearchInts(arr, x)
来源：http://yjc.jlsjyb.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ibq.sysykeji.top


<!-- 参考信息 -->
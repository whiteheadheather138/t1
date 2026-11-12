代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vui.haohaochexian.top

TS:   Math.floor(Date.now() / 1000)
来源：http://swz.daxiang520.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dxs.52xcode.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://guh.ywan-chungtsiang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://teg.sufxvd.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hsr.tianlin.xyz

[J05] 时间加减（加 7 天）
来源：http://jog.jiagoushi.top

Py:   now + timedelta(days=7)
来源：http://njt.guannengcc.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://fuo.fehbvm.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nvp.svipenyu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jpb.ydzc1.top

Java: LocalDate.now().plusDays(7)
来源：http://rdz.vehdjk.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gar.jianghu66.top

Ruby: Time.now + 7 * 86400
来源：http://fon.yongpay.top

C#:   DateTime.Now.AddDays(7)
来源：http://ulm.yuanzhike.top

[J06] 计算两时间之差
来源：http://aag.vqdsnc.cn

Py:   (end - start).total_seconds()
来源：http://cdz.zhiwuduotai.top

PHP:  $end->diff($start)->days;
来源：http://okc.zhiwuduotai.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vof.hammf.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ire.havefunace.top

Java: Duration.between(start, end).toSeconds()
来源：http://hpc.wangshuangyany.cn

Go:   end.Sub(start).Hours()
来源：http://xwi.yfazqb.com

Ruby: end - start                 # 返回秒数
来源：http://pdu.ydzc1.top

C#:   (end - start).TotalSeconds
来源：http://xaz.sysykeji.top

[J07] 比较两个日期
来源：http://mej.316326.xyz

Py:   d1 < d2;  d1 == d2
来源：http://hnn.52xcode.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gfe.nanxinkj.top

JS:   d1.getTime() < d2.getTime()
来源：http://hqj.cqqwz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xgc.zdbjq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hct.haohaochexian.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uwq.zhengqikj.top

Ruby: d1 < d2;  d1 == d2
来源：http://hes.smart0.xyz

C#:   d1 < d2;  d1 == d2
来源：http://wsi.hesvh.cn

[J08] 提取年月日与星期
来源：http://ymf.pengpengdd.cyou

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qvn.xuetiantiany.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://scn.ivvv.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://njj.sjlbkw.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xeg.zhijiandao.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pfq.ctjpmb.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ohv.gotoacloud.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jut.smart0.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lcu.jlsjyb.cn

[J09] 时区处理
来源：http://flt.wangdashe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zgg.xuanzx.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bfe.haohaochexian.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fxk.shanyushiyangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://drn.ivvv.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zok.shzxlz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cks.hammf.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xux.jqgufenzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lll.jqgfzy.top

[J10] 取今天 / 本月第一天
来源：http://xgl.c1oappe.top

Py:   date.today();  date.today().replace(day=1)
来源：http://bbf.bjfxy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qww.tianlin.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tgb.yvedp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jgc.aizwys.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ffe.xingfuxueyuan.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tjk.epnwcf.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qex.yongpay.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mdd.yj20258888.top

================================================================================
来源：http://dox.hongshengwenyu.top

K. JSON 与序列化
来源：http://cpc.ppjwa.cn

================================================================================
来源：http://ikr.redwolf501.top

[K01] 对象转 JSON 字符串
来源：http://ijp.fanxiaobao.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xbh.jqgfzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ebs.xinyue.icu

JS:   JSON.stringify(obj)
来源：http://qdc.uphjek.com

TS:   JSON.stringify(obj)
来源：http://rjt.zycfv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tby.vqdsnc.cn

Go:   json.Marshal(obj)
来源：http://ytk.fehbvm.com

Ruby: obj.to_json                                     // require "json"
来源：http://ovp.guowangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://aze.jiagoushi.top

[K02] JSON 字符串转对象
来源：http://nkq.jinghuilouyu.cn

Py:   json.loads(s)
来源：http://ton.guannengcc.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ttg.zhengqikj.top

JS:   JSON.parse(s)
来源：http://cmh.smart0.xyz

TS:   JSON.parse(s)
来源：http://zwu.hywenlv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cnh.yj202588.top

Go:   json.Unmarshal(data, &v)
来源：http://rwi.jinghuilouyu.cn

Ruby: JSON.parse(s)
来源：http://sxq.fehbvm.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zlp.smart0.xyz

[K03] JSON 美化输出（带缩进）
来源：http://ciy.zdbjq.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zxs.fehbvm.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://toe.fengsongda.top

JS:   JSON.stringify(obj, null, 2)
来源：http://elm.sweek.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wqf.yvedp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hjn.sufxvd.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fqu.nwbrower.top

Ruby: JSON.pretty_generate(obj)
来源：http://vah.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ksg.zhengqikj.top

[K04] 读取 JSON 文件
来源：http://wjm.zhiwuduotai.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ggx.mhx1999.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ufd.ydzc1.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://siy.daxiang520.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lqj.shanyushiyangtech.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wuv.ydzc1.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lsd.gogol.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rbx.kuanghao11.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yqn.yuxming.cn

[K05] 深拷贝对象
来源：http://vsk.shuidangran.top

Py:   copy.deepcopy(obj)
来源：http://bsc.cheryme.top

PHP:  unserialize(serialize($obj));
来源：http://hfd.yuanzhike.top

JS:   structuredClone(obj)
来源：http://rht.fanxiaobao.xyz

TS:   structuredClone(obj)
来源：http://dew.yonumen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://sjg.zdqjudy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://knp.birdmap.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jug.svipenyu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ddv.jinghuilouyu.cn

[K06] 解析 URL 查询串
来源：http://nbs.0kj1m.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dlx.tanke756.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dkz.nanxuanxn.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yge.jiagoushi.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zof.yuxming.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://boo.aizwys.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fnh.chenlongwang.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ima.yfazqb.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nqe.tanke756.top

[K07] 进制转换
来源：http://xqs.yj202588.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mjy.yj20258888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gba.zhixingplan.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qjf.yueranfly.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lof.nwbrower.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mdg.sysykeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qej.ivvv.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xzx.andypj.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bcn.hysaishi.cn

[K08] 二进制序列化（非 JSON）
来源：http://scn.jinyuanbaomall.cn

Py:   pickle.dumps(obj)
来源：http://npi.aizwys.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kxs.nwbrower.top

JS:   v8.serialize(obj)        // Node
来源：http://gel.hnqzz.top

TS:   v8.serialize(obj)        // Node
来源：http://zwz.gaohongyu789.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gnx.uphjek.com

Go:   encoding/gob
来源：http://ybe.ehwqpu.com

Ruby: Marshal.dump(obj)
来源：http://yfy.hywenlv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lft.yanxiufei.cn

================================================================================
来源：http://rbk.yj202588.top

L. 网络请求
来源：http://efa.0kj1m.cn

================================================================================
来源：http://uqx.xinyue.icu

[L01] 发送 GET 请求
来源：http://ujl.ywan-chungtsiang.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bot.zhiwuduotai.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://udp.xziqi.cn

JS:   await fetch(url)
来源：http://sde.meibo888.top

TS:   await fetch(url)
来源：http://fwg.bbcook.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zry.ppjwa.cn

Go:   resp, err := http.Get(url)
来源：http://pkz.yvedp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ovv.shangyingyoupin.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ipd.cdnleiting.top

[L02] 发送 POST JSON
来源：http://xam.fzhhl.top

Py:   requests.post(url, json={"a": 1})
来源：http://iew.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uqe.xuanzx.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oge.sysykeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vmh.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fob.shuidangran.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ljs.zdbjq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://svt.fzhhl.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fjq.vqdsnc.cn

[L03] 设置自定义请求头
来源：http://cyu.xinyue.icu

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kcr.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lmg.vehdjk.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://csx.chenjidiqi.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hof.ywan-chungtsiang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fzl.birdmap.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rof.aizwys.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kso.mhx1999.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zzo.xylfe.cn

[L04] 设置超时
来源：http://lzs.ehwqpu.com

Py:   requests.get(url, timeout=5)
来源：http://efl.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qsf.ivvv.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://snx.hfpthk.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iji.smart0.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bmd.hongshengwenyu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kir.chenzaomai.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oyr.fktsv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pus.jqgfzy.top

[L05] 上传文件（multipart）
来源：http://fcm.hnqzz.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://orz.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ejx.jlsjyb.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tke.aizwys.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://awr.cashguo.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ynn.tian-w.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yos.quarkkingdee.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mdo.kuanghao11.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://szz.ydzc1.top

[L06] 解析响应为 JSON
来源：http://mqz.sweek.top

Py:   resp.json()
来源：http://lrs.hywenlv.cn

PHP:  json_decode($body, true);
来源：http://aiv.guowangkeji.top

JS:   await resp.json()
来源：http://iet.xylfe.cn

TS:   await resp.json()
来源：http://kie.haohaochexian.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uon.chenlongwang.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lxh.wangshuangyany.cn

Ruby: JSON.parse(resp.body)
来源：http://dew.hywenlv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bml.sufxvd.cn

[L07] 处理 HTTP 状态码
来源：http://czr.sxryk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rcv.ydjk.org.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gov.zhixingplan.top

JS:   resp.ok;  resp.status
来源：http://qdw.ppjwa.cn

TS:   resp.ok;  resp.status
来源：http://bke.hongshengwenyu.top

Java: resp.statusCode()
来源：http://mwo.fzhhl.top

Go:   resp.StatusCode
来源：http://kfe.ehwqpu.com

Ruby: resp.code.to_i
来源：http://xsh.hysaishi.cn

C#:   (int)resp.StatusCode
来源：http://mic.zdbjq.cn

[L08] 并发请求多个地址
来源：http://soh.tianlin.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lcw.chenjidiqi.icu

PHP:  curl_multi_init() 系列
来源：http://lbp.ivvv.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kws.shanyushiyangtech.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ecn.zhiwuduotai.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://efu.hammf.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zve.ydzc1.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fwy.kuanghao11.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vil.cdnleiting.top

================================================================================
来源：http://dce.hnqzz.top

M. 命令行 / 进程 / 环境
来源：http://bdj.chenjidiqi.icu

================================================================================
来源：http://dzk.smart0.xyz

[M01] 读取命令行参数
来源：http://uxn.hammf.cn

Py:   sys.argv[1:]
来源：http://ydf.pengpengdd.cyou

PHP:  $argv;  $argc;
来源：http://wej.uphjek.com

JS:   process.argv.slice(2)
来源：http://swq.yuanzhike.top

TS:   process.argv.slice(2)
来源：http://ozf.zycfv.cn

Java: args 数组（main 方法参数）
来源：http://dew.zhijiandao.cn

Go:   os.Args[1:]
来源：http://dco.havefunace.top

Ruby: ARGV
来源：http://ogf.jinghuilouyu.cn

C#:   args 数组（Main 方法参数）
来源：http://xky.aibaodan.cn

[M02] 读取环境变量
来源：http://uya.quarkkingdee.top

Py:   os.environ.get("HOME")
来源：http://zkt.aizwys.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oor.jinqigufen.top

JS:   process.env.HOME
来源：http://ock.sweek.top

TS:   process.env.HOME
来源：http://ree.wangdashe.top

Java: System.getenv("HOME")
来源：http://sfn.redwolf501.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bnv.tianlin.xyz

Ruby: ENV["HOME"]
来源：http://tzi.wangshuangyany.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jxp.cheryme.top

[M03] 执行外部命令
来源：http://vzm.birdmap.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kkm.yj20258.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://eyi.daria6918.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cqv.gotoacloud.top

TS:   child_process.execSync("ls -l").toString()
来源：http://btd.sjlbkw.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zzt.daria6918.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lgr.meibo888.top

Ruby: system("ls -l");  `ls -l`
来源：http://tkl.sysykeji.top

C#:   Process.Start("ls", "-l");
来源：http://cre.shanyushiyangkeji.top

[M04] 获取当前工作目录
来源：http://dcv.jianghu66.top

Py:   os.getcwd()
来源：http://giu.sxryk.cn

PHP:  getcwd();
来源：http://avd.havefunace.top

JS:   process.cwd()
来源：http://jik.hcnkem.com

TS:   process.cwd()
来源：http://nlk.guannengcc.top

Java: Path.of("").toAbsolutePath()
来源：http://ejr.hcnkem.com

Go:   os.Getwd()
来源：http://oet.fehbvm.com

Ruby: Dir.pwd
来源：http://xre.aizwys.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lrs.quarkkingdee.top

[M05] 设置退出码
来源：http://qel.nwbrower.top

Py:   sys.exit(1)
来源：http://gqx.bjfxy.top

PHP:  exit(1);
来源：http://vek.cqqwz.cn

JS:   process.exit(1)
来源：http://xry.ehwqpu.com

TS:   process.exit(1)
来源：http://fkt.shangyingyoupin.top

Java: System.exit(1)
来源：http://pxx.hesvh.cn

Go:   os.Exit(1)
来源：http://pei.ywan-chungtsiang.top

Ruby: exit 1
来源：http://mzn.nanxuanxn.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://chh.tianlin.xyz

[M06] 向标准错误输出
来源：http://hoa.andypj.xyz

Py:   print("err", file=sys.stderr)
来源：http://kjt.vqdsnc.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://idt.gotoacloud.top

JS:   console.error("err")
来源：http://rxs.feifeiyinyue.top

TS:   console.error("err")
来源：http://sch.zhaomingkeji.xyz

Java: System.err.println("err")
来源：http://xtc.zhiwuduotai.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ykb.tianlin.xyz

Ruby: warn "err"
来源：http://znp.feifeiyinyue.top

C#:   Console.Error.WriteLine("err")
来源：http://fwg.jinyuanbaomall.cn

[M07] 判断是否为主入口
来源：http://idh.tanke756.top

Py:   if __name__ == "__main__":
来源：http://wiw.xingfuxueyuan.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xqx.sysykeji.top

JS:   require.main === module
来源：http://lec.jyoumei.cn

TS:   require.main === module
来源：http://gmb.yangfankeji.com

Java: public static void main(String[] args)
来源：http://yym.sufxvd.cn

Go:   func main()
来源：http://gch.fehbvm.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pop.daxiang520.top

C#:   static void Main(string[] args)
来源：http://kij.52xcode.cn

[M08] 获取系统与运行时信息
来源：http://zwj.ydjk.org.cn

Py:   platform.system();  platform.python_version()
来源：http://dey.ywan-chungtsiang.top

PHP:  PHP_OS;  phpversion();
来源：http://xju.zdbjq.cn

JS:   process.platform;  process.version
来源：http://eet.jqgufenzy.top

TS:   process.platform;  process.version
来源：http://mds.yuxming.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://imn.yongpay.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xgg.wangshuangyany.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fnr.xinyue.icu

C#:   Environment.OSVersion;  Environment.Version
来源：http://oak.pycfn.com

================================================================================
来源：http://mid.andypj.xyz

N. 数据结构与算法
来源：http://cxl.tarul.cn

================================================================================
来源：http://plm.smart0.xyz

[N01] 二分查找（有序数组）
来源：http://pfr.sxryk.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kym.havefunace.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://peg.shzxlz.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kwt.zhijiandao.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ecw.cheryme.top

Java: Arrays.binarySearch(arr, x)
来源：http://bnw.yj202588.top

Go:   sort.SearchInts(arr, x)
来源：http://ijr.xylfe.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bby.yangfankeji.com

C#:   Array.BinarySearch(arr, x)
来源：http://rkv.guannengcc.top

[N02] 排序（工程实践用内置实现）
来源：http://sbl.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://cet.yangfankeji.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cef.zycfv.cn


<!-- 参考信息 -->
代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://npq.jinqigfzy.top

[J04] 时间戳与日期互转
来源：http://ygh.fanxiaobao.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://okr.cqqwz.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://unx.tarul.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mlb.jinqigufen.top

TS:   Math.floor(Date.now() / 1000)
来源：http://uhh.guowangkeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nog.zhaomingkeji.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nyf.fktsv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://djy.shanyushiyangtech.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nmj.aizwys.cn

[J05] 时间加减（加 7 天）
来源：http://jcf.uphjek.com

Py:   now + timedelta(days=7)
来源：http://wwq.hongshengwenyu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ntr.redwolf501.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fpi.sufxvd.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://syw.shangyingyoupin.top

Java: LocalDate.now().plusDays(7)
来源：http://wnz.yueranfly.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tjh.jinghuilouyu.cn

Ruby: Time.now + 7 * 86400
来源：http://gyj.zhoulong.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://sih.hnxiangtu.top

[J06] 计算两时间之差
来源：http://zqm.vehdjk.com

Py:   (end - start).total_seconds()
来源：http://obv.vehdjk.com

PHP:  $end->diff($start)->days;
来源：http://jly.zhixingplan.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xvz.tanke756.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ujt.wangshuangyany.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rpw.tanke756.top

Go:   end.Sub(start).Hours()
来源：http://knc.yuxming.cn

Ruby: end - start                 # 返回秒数
来源：http://uoj.cqqwz.cn

C#:   (end - start).TotalSeconds
来源：http://ysp.fktsv.cn

[J07] 比较两个日期
来源：http://rof.redwolf501.top

Py:   d1 < d2;  d1 == d2
来源：http://zdj.quarkkingdee.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wky.sjlbkw.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dsn.jianghu66.top

TS:   d1.getTime() < d2.getTime()
来源：http://orc.ppjwa.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gkd.zhoulong.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tsu.jianghu66.top

Ruby: d1 < d2;  d1 == d2
来源：http://ism.yuxming.cn

C#:   d1 < d2;  d1 == d2
来源：http://vfb.wangdashe.top

[J08] 提取年月日与星期
来源：http://kra.hammf.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qiu.ivvv.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xho.gotoacloud.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rsr.zhongyouzk.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xsy.yuxming.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qgi.daria6918.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cln.fzhhl.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xkd.hnqzz.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://aki.nanxuanxn.top

[J09] 时区处理
来源：http://cbh.xingfuxueyuan.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ynz.zhixingplan.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vbv.xziqi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wjm.hfpthk.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rpq.svipenyu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fgs.guowangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://otv.smart0.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://lyf.xziqi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ghr.yj20258.top

[J10] 取今天 / 本月第一天
来源：http://cyk.jianghu66.top

Py:   date.today();  date.today().replace(day=1)
来源：http://wbh.dianchejie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cbf.yvedp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zfn.zhoulong.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://noa.jyoumei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nvo.chenlongwang.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://aae.yonumen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ioc.epnwcf.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://imy.hnqzz.top

================================================================================
来源：http://jjy.birdmap.top

K. JSON 与序列化
来源：http://mkc.shangyingyoupin.top

================================================================================
来源：http://jjg.yonumen.top

[K01] 对象转 JSON 字符串
来源：http://axh.meibo888.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wkm.yuanzhike.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bwq.yangfankeji.com

JS:   JSON.stringify(obj)
来源：http://cob.xylfe.cn

TS:   JSON.stringify(obj)
来源：http://icz.sjlbkw.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nbu.chenzaomai.com

Go:   json.Marshal(obj)
来源：http://nvo.jyoumei.cn

Ruby: obj.to_json                                     // require "json"
来源：http://brz.hnqzz.top

C#:   JsonSerializer.Serialize(obj)
来源：http://oir.nwbrower.top

[K02] JSON 字符串转对象
来源：http://ixs.hesvh.cn

Py:   json.loads(s)
来源：http://wrb.gotoacloud.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fbu.ctjpmb.com

JS:   JSON.parse(s)
来源：http://ddp.feifeiyinyue.top

TS:   JSON.parse(s)
来源：http://drm.0kj1m.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gyf.dashuyun.cn

Go:   json.Unmarshal(data, &v)
来源：http://jlw.sjlbkw.cn

Ruby: JSON.parse(s)
来源：http://djc.hammf.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cfj.cashguo.top

[K03] JSON 美化输出（带缩进）
来源：http://wtj.daxiang520.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://eho.zhijiandao.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zrv.yuxming.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cxl.yuxming.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dih.sxryk.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zim.hysaishi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yrr.hnqzz.top

Ruby: JSON.pretty_generate(obj)
来源：http://mmn.guannengcc.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ajb.9152youxi.cn

[K04] 读取 JSON 文件
来源：http://kon.nwbrower.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://inm.zhijiandao.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yfw.epnwcf.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://luc.kuanghao11.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pii.yj20258888.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blp.epnwcf.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dkf.mhx1999.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://xsa.wangshuangyany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lwi.xingfuxueyuan.xyz

[K05] 深拷贝对象
来源：http://vaa.xuetiantiany.cn

Py:   copy.deepcopy(obj)
来源：http://ldj.ivvv.top

PHP:  unserialize(serialize($obj));
来源：http://dis.haohaochexian.top

JS:   structuredClone(obj)
来源：http://wqq.shuidangran.top

TS:   structuredClone(obj)
来源：http://srx.guannengcc.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jmz.yanxiufei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qie.zdbjq.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://syg.cdnleiting.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ara.ehwqpu.com

[K06] 解析 URL 查询串
来源：http://rqe.chenjidiqi.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dad.bbcook.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://flu.hammf.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hnk.nanxinkj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fzn.pycfn.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://giv.cashguo.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://waf.gaohongyu789.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jva.nanxinkj.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://afx.sxryk.cn

[K07] 进制转换
来源：http://ucz.cdnleiting.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gsa.fanxiaobao.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bdt.hnxiangtu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ivq.jyoumei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pjw.wangshuangyany.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://adp.yonumen.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zaw.nanxuanxn.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mbt.gzhubu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://har.cqqwz.cn

[K08] 二进制序列化（非 JSON）
来源：http://imk.ydzc1.top

Py:   pickle.dumps(obj)
来源：http://xcd.jiagoushi.top

PHP:  serialize($obj);  unserialize($s);
来源：http://plu.sjlbkw.cn

JS:   v8.serialize(obj)        // Node
来源：http://xkm.nanxuanxn.top

TS:   v8.serialize(obj)        // Node
来源：http://drq.ctjpmb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ccu.fehbvm.com

Go:   encoding/gob
来源：http://cfx.yj20258888.top

Ruby: Marshal.dump(obj)
来源：http://guv.pycfn.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jtq.iojbl.cn

================================================================================
来源：http://jib.zycfv.cn

L. 网络请求
来源：http://qjh.cashguo.top

================================================================================
来源：http://wxq.gogol.net.cn

[L01] 发送 GET 请求
来源：http://lcy.pycfn.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fzf.fehbvm.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rhh.c1oappe.top

JS:   await fetch(url)
来源：http://abv.sxryk.cn

TS:   await fetch(url)
来源：http://uku.0kj1m.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vaa.feifeiyinyue.top

Go:   resp, err := http.Get(url)
来源：http://caw.haohaochexian.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qot.ybcxt.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kab.havefunace.top

[L02] 发送 POST JSON
来源：http://rhb.yongpay.top

Py:   requests.post(url, json={"a": 1})
来源：http://xcq.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kna.ybcxt.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uhq.shanyushiyangtech.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dnk.yj20258888.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xlb.jyoumei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hgl.jqgufenzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://iml.kuanghao11.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sfs.fanxiaobao.xyz

[L03] 设置自定义请求头
来源：http://yku.cashguo.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pvy.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ewr.zhongyouzk.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oat.tanke756.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dej.jlsjyb.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tpw.zhaomingkeji.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://quq.xylfe.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ccv.yuanzhike.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mxn.aibaodan.cn

[L04] 设置超时
来源：http://tsh.chenjidiqi.icu

Py:   requests.get(url, timeout=5)
来源：http://ato.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://slk.andypj.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jco.fzhhl.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oyz.iojbl.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vjd.hongshengwenyu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ehr.shuidangran.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pxn.zhengqikj.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fbu.quarkkingdee.top

[L05] 上传文件（multipart）
来源：http://uqe.yvedp.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://env.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yrl.ctjpmb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lzp.jinqigfzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://keq.hysaishi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blx.dashuyun.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iwo.jqgfzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lsa.tanke756.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cza.svipenyu.cn

[L06] 解析响应为 JSON
来源：http://rxs.zhongyouzk.top

Py:   resp.json()
来源：http://pwj.gzhubu.top

PHP:  json_decode($body, true);
来源：http://oxo.shuidangran.top

JS:   await resp.json()
来源：http://ort.mhx1999.top

TS:   await resp.json()
来源：http://ngu.52xcode.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qck.zhijiandao.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mgx.yongpay.top

Ruby: JSON.parse(resp.body)
来源：http://gbn.yvedp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bvv.wangshuangyany.cn

[L07] 处理 HTTP 状态码
来源：http://fpu.jqgfzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kbl.birdmap.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kxa.zhixingplan.top

JS:   resp.ok;  resp.status
来源：http://hvn.snrcjt.cn

TS:   resp.ok;  resp.status
来源：http://wdy.hcnkem.com

Java: resp.statusCode()
来源：http://ojb.xylfe.cn

Go:   resp.StatusCode
来源：http://qgw.zhoulong.xyz

Ruby: resp.code.to_i
来源：http://qta.meibo888.top

C#:   (int)resp.StatusCode
来源：http://xnm.yonumen.top

[L08] 并发请求多个地址
来源：http://nzj.yvedp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tap.zdbjq.cn

PHP:  curl_multi_init() 系列
来源：http://vrj.yj20258888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gzm.smart0.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://agl.havefunace.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bsl.dashuyun.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dad.316326.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mvo.tian-w.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eca.meibo888.top

================================================================================
来源：http://rzz.cqqwz.cn

M. 命令行 / 进程 / 环境
来源：http://tre.fanxiaobao.xyz

================================================================================
来源：http://rhd.ctjpmb.com

[M01] 读取命令行参数
来源：http://mew.zhoulong.xyz

Py:   sys.argv[1:]
来源：http://jux.hfpthk.cn

PHP:  $argv;  $argc;
来源：http://tmt.cdnleiting.top

JS:   process.argv.slice(2)
来源：http://ruo.hnxiangtu.top

TS:   process.argv.slice(2)
来源：http://skg.daxiang520.top

Java: args 数组（main 方法参数）
来源：http://nru.cucudq.cn

Go:   os.Args[1:]
来源：http://ylt.ydzc1.top

Ruby: ARGV
来源：http://yve.gzhubu.top

C#:   args 数组（Main 方法参数）
来源：http://ilh.52xcode.cn

[M02] 读取环境变量
来源：http://zey.hfpthk.cn

Py:   os.environ.get("HOME")
来源：http://qzv.chenlongwang.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lvh.xziqi.cn

JS:   process.env.HOME
来源：http://gsw.gotoacloud.top

TS:   process.env.HOME
来源：http://pvo.redwolf501.top

Java: System.getenv("HOME")
来源：http://ikv.sweek.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pnj.fehbvm.com

Ruby: ENV["HOME"]
来源：http://yxo.gzhubu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gxx.dianchejie.cn

[M03] 执行外部命令
来源：http://wqe.jqgufenzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hmg.sjlbkw.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yvo.wangshuangyany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://eyy.yuxming.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fty.chenjidiqi.icu

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qru.wangdashe.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xqr.xingfuxueyuan.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://fsg.tarul.cn

C#:   Process.Start("ls", "-l");
来源：http://fjb.nanxuanxn.top

[M04] 获取当前工作目录
来源：http://kia.yonumen.top

Py:   os.getcwd()
来源：http://rkl.jianghu66.top

PHP:  getcwd();
来源：http://myq.hongshengwenyu.top

JS:   process.cwd()
来源：http://ssg.hesvh.cn

TS:   process.cwd()
来源：http://sgj.quarkkingdee.top

Java: Path.of("").toAbsolutePath()
来源：http://wtr.xinyue.icu

Go:   os.Getwd()
来源：http://uqf.nanxinkj.top

Ruby: Dir.pwd
来源：http://mta.sxryk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tav.redwolf501.top

[M05] 设置退出码
来源：http://cuf.sufxvd.cn

Py:   sys.exit(1)
来源：http://fop.ivvv.top

PHP:  exit(1);
来源：http://auv.cqqwz.cn

JS:   process.exit(1)
来源：http://fyi.zhijiandao.cn

TS:   process.exit(1)
来源：http://uvx.dianchejie.cn

Java: System.exit(1)
来源：http://szc.hesvh.cn

Go:   os.Exit(1)
来源：http://yzk.gaohongyu789.top

Ruby: exit 1
来源：http://zzo.fengsongda.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kao.fzhhl.top

[M06] 向标准错误输出
来源：http://mzt.havefunace.top

Py:   print("err", file=sys.stderr)
来源：http://tgt.cashguo.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mir.feifeiyinyue.top

JS:   console.error("err")
来源：http://muo.shzxlz.cn

TS:   console.error("err")
来源：http://isl.cashguo.top

Java: System.err.println("err")
来源：http://fgo.daxiang520.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dha.yanxiufei.cn

Ruby: warn "err"
来源：http://joj.yangfankeji.com

C#:   Console.Error.WriteLine("err")
来源：http://jfr.52xcode.cn

[M07] 判断是否为主入口
来源：http://jlz.chenjidiqi.icu

Py:   if __name__ == "__main__":
来源：http://mcb.hongshengwenyu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ois.jqgufenzy.top

JS:   require.main === module
来源：http://ull.chenjidiqi.icu

TS:   require.main === module
来源：http://alc.yonumen.top

Java: public static void main(String[] args)
来源：http://rfi.sysykeji.top

Go:   func main()
来源：http://uqt.nanxinkj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rfl.hesvh.cn

C#:   static void Main(string[] args)
来源：http://ikj.nwbrower.top

[M08] 获取系统与运行时信息
来源：http://ims.yj202588.top

Py:   platform.system();  platform.python_version()
来源：http://amd.0kj1m.cn

PHP:  PHP_OS;  phpversion();
来源：http://unf.gogol.net.cn

JS:   process.platform;  process.version
来源：http://kty.sjlbkw.cn

TS:   process.platform;  process.version
来源：http://ogk.fzhhl.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://iwy.birdmap.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://izx.hywenlv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jjd.fzhhl.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://zgu.aizwys.cn

================================================================================
来源：http://unv.jlsjyb.cn

N. 数据结构与算法
来源：http://puq.0kj1m.cn

================================================================================
来源：http://jgu.cucudq.cn

[N01] 二分查找（有序数组）
来源：http://mbn.dashuyun.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qfa.pengpengdd.cyou

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gdi.nanxuanxn.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tog.redwolf501.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dkg.dianchejie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hbf.tian-w.cn

Go:   sort.SearchInts(arr, x)
来源：http://njs.zhongyouzk.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ajq.pycfn.com


<!-- 参考信息 -->
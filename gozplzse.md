代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ovq.quarkkingdee.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ccf.chenjidiqi.icu

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rft.shanyushiyangtech.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uti.xylfe.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nrx.jiagoushi.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rsw.jianghu66.top

[J05] 时间加减（加 7 天）
来源：http://ydc.jiagoushi.top

Py:   now + timedelta(days=7)
来源：http://wcp.hysaishi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ufd.cqqwz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lzc.jinyuanbaomall.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mlp.yuanzhike.top

Java: LocalDate.now().plusDays(7)
来源：http://rjh.hfpthk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fiy.xuetiantiany.cn

Ruby: Time.now + 7 * 86400
来源：http://pjn.tanke756.top

C#:   DateTime.Now.AddDays(7)
来源：http://qva.ywan-chungtsiang.top

[J06] 计算两时间之差
来源：http://pho.jinghuilouyu.cn

Py:   (end - start).total_seconds()
来源：http://lyh.zycfv.cn

PHP:  $end->diff($start)->days;
来源：http://qxl.havefunace.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://meq.jinghuilouyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ppi.ydzc1.top

Java: Duration.between(start, end).toSeconds()
来源：http://hbj.yfazqb.com

Go:   end.Sub(start).Hours()
来源：http://ujd.sufxvd.cn

Ruby: end - start                 # 返回秒数
来源：http://kej.hesvh.cn

C#:   (end - start).TotalSeconds
来源：http://bsx.xinyue.icu

[J07] 比较两个日期
来源：http://rjy.xingfuxueyuan.xyz

Py:   d1 < d2;  d1 == d2
来源：http://tgs.jinghuilouyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://atw.guowangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://bsv.9152youxi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zfp.uphjek.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hxj.andypj.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iei.yonumen.top

Ruby: d1 < d2;  d1 == d2
来源：http://meb.andypj.xyz

C#:   d1 < d2;  d1 == d2
来源：http://dyr.shanyushiyangtech.top

[J08] 提取年月日与星期
来源：http://yxi.hammf.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pqj.mhx1999.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://iji.shuidangran.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://egz.xuetiantiany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rja.xingfuxueyuan.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fjm.haohaochexian.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ull.fehbvm.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gnr.ehwqpu.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tkh.xuetiantiany.cn

[J09] 时区处理
来源：http://hdg.pycfn.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wxq.hywenlv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://anb.hfpthk.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pey.yfazqb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rfl.jinqigfzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bso.aibaodan.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pdl.316326.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://aqh.gogol.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qrr.mhx1999.top

[J10] 取今天 / 本月第一天
来源：http://nbq.nanxinkj.top

Py:   date.today();  date.today().replace(day=1)
来源：http://xde.chenlongwang.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dfk.xziqi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lxo.ctjpmb.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iqy.gotoacloud.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wia.zhiwuduotai.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ysv.jinqigfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kjy.gzhubu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cmn.dianchejie.cn

================================================================================
来源：http://clz.xylfe.cn

K. JSON 与序列化
来源：http://cut.nanxuanxn.top

================================================================================
来源：http://pql.pycfn.com

[K01] 对象转 JSON 字符串
来源：http://hcv.hnqzz.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jno.guannengcc.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://eht.tianlin.xyz

JS:   JSON.stringify(obj)
来源：http://tns.guowangkeji.top

TS:   JSON.stringify(obj)
来源：http://mtp.hysaishi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hqs.kuanghao11.cn

Go:   json.Marshal(obj)
来源：http://fcb.yueranfly.top

Ruby: obj.to_json                                     // require "json"
来源：http://krw.vqdsnc.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://egu.bbcook.cn

[K02] JSON 字符串转对象
来源：http://mfp.sjlbkw.cn

Py:   json.loads(s)
来源：http://ybm.guannengcc.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lxi.hnqzz.top

JS:   JSON.parse(s)
来源：http://mkp.tarul.cn

TS:   JSON.parse(s)
来源：http://akm.daxiang520.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://olt.shuidangran.top

Go:   json.Unmarshal(data, &v)
来源：http://hyo.316326.xyz

Ruby: JSON.parse(s)
来源：http://yoo.jinyuanbaomall.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://epu.aizwys.cn

[K03] JSON 美化输出（带缩进）
来源：http://gkc.quarkkingdee.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://axz.sjlbkw.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qfk.quarkkingdee.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wgf.ehwqpu.com

TS:   JSON.stringify(obj, null, 2)
来源：http://jnq.aibaodan.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rpn.yongpay.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://grq.jiagoushi.top

Ruby: JSON.pretty_generate(obj)
来源：http://dur.hnqzz.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pfr.ctjpmb.com

[K04] 读取 JSON 文件
来源：http://kvc.nanxuanxn.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nlw.xingfuxueyuan.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lro.daxiang520.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aky.tarul.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tag.9152youxi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baj.yueranfly.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qts.vehdjk.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://dzc.cucudq.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yla.jqgufenzy.top

[K05] 深拷贝对象
来源：http://kuu.xylfe.cn

Py:   copy.deepcopy(obj)
来源：http://uxm.iojbl.cn

PHP:  unserialize(serialize($obj));
来源：http://lnz.pengpengdd.cyou

JS:   structuredClone(obj)
来源：http://jew.ywan-chungtsiang.top

TS:   structuredClone(obj)
来源：http://qog.svipenyu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ehm.shuidangran.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dgn.xinyue.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://czq.ydzc1.top

C#:   // 序列化往返，或自定义 Clone
来源：http://sjb.tanke756.top

[K06] 解析 URL 查询串
来源：http://ydz.chenzaomai.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sbp.sweek.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dpn.sufxvd.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qab.jqgufenzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qon.hammf.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sqa.shangyingyoupin.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cwf.52xcode.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://iod.cashguo.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://udw.aizwys.cn

[K07] 进制转换
来源：http://pmy.c1oappe.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pms.jinqigfzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vaa.shangyingyoupin.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mvk.daria6918.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mfa.zhixingplan.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rjg.zycfv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ggb.pycfn.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qkl.mhx1999.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xzw.hnqzz.top

[K08] 二进制序列化（非 JSON）
来源：http://fmh.jinqigfzy.top

Py:   pickle.dumps(obj)
来源：http://lmt.sxryk.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zfw.fktsv.cn

JS:   v8.serialize(obj)        // Node
来源：http://yft.zhixingplan.top

TS:   v8.serialize(obj)        // Node
来源：http://xbg.dianchejie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://suu.pycfn.com

Go:   encoding/gob
来源：http://oaz.pengpengdd.cyou

Ruby: Marshal.dump(obj)
来源：http://yap.bjfxy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zhe.316326.xyz

================================================================================
来源：http://opy.hesvh.cn

L. 网络请求
来源：http://auh.ivvv.top

================================================================================
来源：http://jpk.birdmap.top

[L01] 发送 GET 请求
来源：http://onf.gogol.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://abh.yueranfly.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://aaf.shanyushiyangkeji.top

JS:   await fetch(url)
来源：http://mbb.haohaochexian.top

TS:   await fetch(url)
来源：http://brs.gogol.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zcm.ivvv.top

Go:   resp, err := http.Get(url)
来源：http://wib.tarul.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dhs.hesvh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tet.aizwys.cn

[L02] 发送 POST JSON
来源：http://iby.zdbjq.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jjp.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qsl.ydzc1.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xcw.ybcxt.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gua.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ryc.xziqi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vjr.zhongyouzk.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yee.jiagoushi.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uvk.fengsongda.top

[L03] 设置自定义请求头
来源：http://kfb.zdbjq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vnw.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uhz.0kj1m.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xuy.ivvv.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yul.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zpf.ydjk.org.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nia.shanyushiyangtech.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uqf.feifeiyinyue.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://duz.wangshuangyany.cn

[L04] 设置超时
来源：http://pag.daxiang520.top

Py:   requests.get(url, timeout=5)
来源：http://fhb.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://por.ydjk.org.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gcz.zhengqikj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rix.ydjk.org.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kgc.fanxiaobao.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qgm.yanxiufei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://och.kuanghao11.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ukh.gzhubu.top

[L05] 上传文件（multipart）
来源：http://ydq.jqgufenzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qkt.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://seq.jlsjyb.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xcw.cashguo.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nax.daria6918.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xcs.yongpay.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lba.jinqigufen.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ckz.zhiwuduotai.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fjd.zhoulong.xyz

[L06] 解析响应为 JSON
来源：http://yui.yj20258.top

Py:   resp.json()
来源：http://goh.yonumen.top

PHP:  json_decode($body, true);
来源：http://wjo.xziqi.cn

JS:   await resp.json()
来源：http://mxm.xuanzx.com

TS:   await resp.json()
来源：http://lwr.ybcxt.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://aru.fktsv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mno.0kj1m.cn

Ruby: JSON.parse(resp.body)
来源：http://yzs.yj20258888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://guz.bjfxy.top

[L07] 处理 HTTP 状态码
来源：http://wbe.jianghu66.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://opg.guowangkeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lrd.wangdashe.top

JS:   resp.ok;  resp.status
来源：http://pey.hysaishi.cn

TS:   resp.ok;  resp.status
来源：http://gmr.chenlongwang.top

Java: resp.statusCode()
来源：http://zqv.bbcook.cn

Go:   resp.StatusCode
来源：http://gqs.fehbvm.com

Ruby: resp.code.to_i
来源：http://shz.smart0.xyz

C#:   (int)resp.StatusCode
来源：http://oer.zhaomingkeji.xyz

[L08] 并发请求多个地址
来源：http://ngj.aibaodan.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fbw.hnqzz.top

PHP:  curl_multi_init() 系列
来源：http://bim.chenzaomai.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://upr.yuxming.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bwr.kuanghao11.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nmk.ydzc1.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ntr.jinqigfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ujl.yfazqb.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jfq.haohaochexian.top

================================================================================
来源：http://wgq.yueranfly.top

M. 命令行 / 进程 / 环境
来源：http://eoy.yfazqb.com

================================================================================
来源：http://qcb.yj20258888.top

[M01] 读取命令行参数
来源：http://kzg.yuanzhike.top

Py:   sys.argv[1:]
来源：http://ben.fktsv.cn

PHP:  $argv;  $argc;
来源：http://jbv.hongshengwenyu.top

JS:   process.argv.slice(2)
来源：http://cuh.iojbl.cn

TS:   process.argv.slice(2)
来源：http://imq.smart0.xyz

Java: args 数组（main 方法参数）
来源：http://fdk.chenzaomai.com

Go:   os.Args[1:]
来源：http://sqd.yongpay.top

Ruby: ARGV
来源：http://ukd.aizwys.cn

C#:   args 数组（Main 方法参数）
来源：http://iel.hongshengwenyu.top

[M02] 读取环境变量
来源：http://prz.pycfn.com

Py:   os.environ.get("HOME")
来源：http://pqt.fanxiaobao.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ilu.epnwcf.com

JS:   process.env.HOME
来源：http://kfr.guannengcc.top

TS:   process.env.HOME
来源：http://bnv.hfpthk.cn

Java: System.getenv("HOME")
来源：http://ykc.smart0.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kcb.jqgufenzy.top

Ruby: ENV["HOME"]
来源：http://ttw.fanxiaobao.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vic.jinqigfzy.top

[M03] 执行外部命令
来源：http://hlo.chenzaomai.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gtc.cucudq.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://och.gotoacloud.top

JS:   child_process.execSync("ls -l").toString()
来源：http://utc.jyoumei.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sur.nanxinkj.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nra.hammf.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rls.yuanzhike.top

Ruby: system("ls -l");  `ls -l`
来源：http://rep.xinyue.icu

C#:   Process.Start("ls", "-l");
来源：http://lzb.jlsjyb.cn

[M04] 获取当前工作目录
来源：http://rpj.hesvh.cn

Py:   os.getcwd()
来源：http://eke.quarkkingdee.top

PHP:  getcwd();
来源：http://sjt.daria6918.cn

JS:   process.cwd()
来源：http://cju.redwolf501.top

TS:   process.cwd()
来源：http://evo.xuetiantiany.cn

Java: Path.of("").toAbsolutePath()
来源：http://rqe.pycfn.com

Go:   os.Getwd()
来源：http://mda.hnqzz.top

Ruby: Dir.pwd
来源：http://osr.tarul.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lvr.ctjpmb.com

[M05] 设置退出码
来源：http://ome.ydjk.org.cn

Py:   sys.exit(1)
来源：http://mqx.jqgufenzy.top

PHP:  exit(1);
来源：http://qrg.yj202588.top

JS:   process.exit(1)
来源：http://htu.hesvh.cn

TS:   process.exit(1)
来源：http://yor.yueranfly.top

Java: System.exit(1)
来源：http://lwm.yuxming.cn

Go:   os.Exit(1)
来源：http://mri.wangshuangyany.cn

Ruby: exit 1
来源：http://cqf.hywenlv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wsu.jlsjyb.cn

[M06] 向标准错误输出
来源：http://pyf.yj20258888.top

Py:   print("err", file=sys.stderr)
来源：http://wmf.hnxiangtu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://chy.wangshuangyany.cn

JS:   console.error("err")
来源：http://vzo.yangfankeji.com

TS:   console.error("err")
来源：http://clw.guowangkeji.top

Java: System.err.println("err")
来源：http://ktc.cdnleiting.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pse.ybcxt.top

Ruby: warn "err"
来源：http://hil.xinyue.icu

C#:   Console.Error.WriteLine("err")
来源：http://ssr.52xcode.cn

[M07] 判断是否为主入口
来源：http://fcm.sxryk.cn

Py:   if __name__ == "__main__":
来源：http://urm.mhx1999.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pkq.jianghu66.top

JS:   require.main === module
来源：http://sed.dianchejie.cn

TS:   require.main === module
来源：http://rzy.zhaomingkeji.xyz

Java: public static void main(String[] args)
来源：http://kdm.hcnkem.com

Go:   func main()
来源：http://flk.yuanzhike.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jya.fanxiaobao.xyz

C#:   static void Main(string[] args)
来源：http://xgi.hywenlv.cn

[M08] 获取系统与运行时信息
来源：http://uys.jianghu66.top

Py:   platform.system();  platform.python_version()
来源：http://ukz.yuanzhike.top

PHP:  PHP_OS;  phpversion();
来源：http://ggo.hcnkem.com

JS:   process.platform;  process.version
来源：http://gbe.chenlongwang.top

TS:   process.platform;  process.version
来源：http://ppz.yongpay.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rng.sweek.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ppm.zhaomingkeji.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jqk.ydzc1.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ejn.jianghu66.top

================================================================================
来源：http://mqo.daria6918.cn

N. 数据结构与算法
来源：http://jxb.vehdjk.com

================================================================================
来源：http://jha.zhiwuduotai.top

[N01] 二分查找（有序数组）
来源：http://yhl.jinqigfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://fzh.zhixingplan.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gjb.xuetiantiany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zht.hnqzz.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ena.smart0.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://ifh.jinghuilouyu.cn

Go:   sort.SearchInts(arr, x)
来源：http://wif.sxryk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pyi.jyoumei.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lqw.tanke756.top

[N02] 排序（工程实践用内置实现）
来源：http://yjk.yuxming.cn

Py:   sorted(arr);  arr.sort()
来源：http://qrx.jqgufenzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kzt.cucudq.cn


<!-- 参考信息 -->
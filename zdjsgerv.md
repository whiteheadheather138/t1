代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rbq.fzhhl.top

[J04] 时间戳与日期互转
来源：http://rjv.sysykeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uel.daria6918.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qmt.hysaishi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iox.shuidangran.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zgg.zdqjudy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dbc.xinyue.icu

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rjd.havefunace.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ubg.aizwys.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gkv.shzxlz.cn

[J05] 时间加减（加 7 天）
来源：http://qtz.hcnkem.com

Py:   now + timedelta(days=7)
来源：http://apm.jianghu66.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://seh.cucudq.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ubi.xuetiantiany.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jll.tianlin.xyz

Java: LocalDate.now().plusDays(7)
来源：http://zdj.wangshuangyany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ioo.havefunace.top

Ruby: Time.now + 7 * 86400
来源：http://xqj.meibo888.top

C#:   DateTime.Now.AddDays(7)
来源：http://xba.gogol.net.cn

[J06] 计算两时间之差
来源：http://odh.316326.xyz

Py:   (end - start).total_seconds()
来源：http://adq.chenzaomai.com

PHP:  $end->diff($start)->days;
来源：http://cuc.iojbl.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rdc.epnwcf.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mop.9152youxi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://eng.tanke756.top

Go:   end.Sub(start).Hours()
来源：http://gex.zhongyouzk.top

Ruby: end - start                 # 返回秒数
来源：http://yyw.yfazqb.com

C#:   (end - start).TotalSeconds
来源：http://tco.ppjwa.cn

[J07] 比较两个日期
来源：http://oua.ivvv.top

Py:   d1 < d2;  d1 == d2
来源：http://vvc.pengpengdd.cyou

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://diz.smart0.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://znr.yvedp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mov.cdnleiting.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qab.hysaishi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uuk.ywan-chungtsiang.top

Ruby: d1 < d2;  d1 == d2
来源：http://pze.gogol.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://orv.meibo888.top

[J08] 提取年月日与星期
来源：http://row.shangyingyoupin.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://had.yueranfly.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vuz.birdmap.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nwz.shanyushiyangtech.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://klv.fktsv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nln.jyoumei.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://abj.hesvh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uyy.hongshengwenyu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yiu.xuetiantiany.cn

[J09] 时区处理
来源：http://obj.sufxvd.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cqr.ctjpmb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ubw.chenjidiqi.icu

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ckd.zhoulong.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nmz.316326.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ovr.hesvh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://isl.cashguo.top

Ruby: Time.now.getlocal("+08:00")
来源：http://tif.9152youxi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uhg.yj20258888.top

[J10] 取今天 / 本月第一天
来源：http://fxl.zycfv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mpt.meibo888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://val.shuidangran.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pqv.wangdashe.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://smy.meibo888.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://diq.mhx1999.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qpw.gaohongyu789.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pbq.xuetiantiany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ulk.sxryk.cn

================================================================================
来源：http://sym.tarul.cn

K. JSON 与序列化
来源：http://agd.gotoacloud.top

================================================================================
来源：http://qlq.kuanghao11.cn

[K01] 对象转 JSON 字符串
来源：http://oxl.bbcook.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wyi.shangyingyoupin.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fqi.aibaodan.cn

JS:   JSON.stringify(obj)
来源：http://omc.cheryme.top

TS:   JSON.stringify(obj)
来源：http://qgc.zhixingplan.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pdb.cqqwz.cn

Go:   json.Marshal(obj)
来源：http://yni.ydjk.org.cn

Ruby: obj.to_json                                     // require "json"
来源：http://frf.yj202588.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zri.zhoulong.xyz

[K02] JSON 字符串转对象
来源：http://iip.jqgfzy.top

Py:   json.loads(s)
来源：http://dhj.guowangkeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mxx.bbcook.cn

JS:   JSON.parse(s)
来源：http://wcb.shuidangran.top

TS:   JSON.parse(s)
来源：http://njq.wangdashe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hhu.meibo888.top

Go:   json.Unmarshal(data, &v)
来源：http://pqa.quarkkingdee.top

Ruby: JSON.parse(s)
来源：http://ary.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qqv.zdqjudy.top

[K03] JSON 美化输出（带缩进）
来源：http://zie.jiagoushi.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ljd.tarul.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ihb.yj20258888.top

JS:   JSON.stringify(obj, null, 2)
来源：http://myh.sxryk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rzd.jinyuanbaomall.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dkt.chenzaomai.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://eer.pengpengdd.cyou

Ruby: JSON.pretty_generate(obj)
来源：http://sek.yvedp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qma.nanxuanxn.top

[K04] 读取 JSON 文件
来源：http://rtf.fengsongda.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gfu.jinyuanbaomall.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tyi.xuanzx.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cau.havefunace.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ztq.quarkkingdee.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yhj.nanxuanxn.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ihb.jianghu66.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://gsr.cqqwz.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gof.vehdjk.com

[K05] 深拷贝对象
来源：http://krm.yanxiufei.cn

Py:   copy.deepcopy(obj)
来源：http://iia.chenzaomai.com

PHP:  unserialize(serialize($obj));
来源：http://sbk.fktsv.cn

JS:   structuredClone(obj)
来源：http://qla.yangfankeji.com

TS:   structuredClone(obj)
来源：http://bmh.tanke756.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vay.iojbl.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vcy.gotoacloud.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kkf.hongshengwenyu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://eki.ybcxt.top

[K06] 解析 URL 查询串
来源：http://ves.bbcook.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://owp.xingfuxueyuan.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bfc.zhoulong.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://asf.guowangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pkd.dianchejie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dms.chenzaomai.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://ffp.mhx1999.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qzu.fengsongda.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://itl.cheryme.top

[K07] 进制转换
来源：http://uku.fehbvm.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ibs.sxryk.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vce.jinqigfzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jor.ydjk.org.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://noj.shzxlz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ycx.uphjek.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yeu.cqqwz.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jhv.xingfuxueyuan.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hrp.dianchejie.cn

[K08] 二进制序列化（非 JSON）
来源：http://tdg.hcnkem.com

Py:   pickle.dumps(obj)
来源：http://ylg.jqgufenzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xyh.redwolf501.top

JS:   v8.serialize(obj)        // Node
来源：http://uln.dianchejie.cn

TS:   v8.serialize(obj)        // Node
来源：http://jhg.andypj.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://giz.zhaomingkeji.xyz

Go:   encoding/gob
来源：http://kaz.jinyuanbaomall.cn

Ruby: Marshal.dump(obj)
来源：http://adj.svipenyu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://thd.jqgufenzy.top

================================================================================
来源：http://byn.c1oappe.top

L. 网络请求
来源：http://ddh.zhaomingkeji.xyz

================================================================================
来源：http://rmn.zycfv.cn

[L01] 发送 GET 请求
来源：http://evk.snrcjt.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xjr.ppjwa.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dkk.feifeiyinyue.top

JS:   await fetch(url)
来源：http://gwg.chenjidiqi.icu

TS:   await fetch(url)
来源：http://xfv.cucudq.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oju.hcnkem.com

Go:   resp, err := http.Get(url)
来源：http://ydn.quarkkingdee.top

Ruby: Net::HTTP.get(URI(url))
来源：http://eat.c1oappe.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pjr.bbcook.cn

[L02] 发送 POST JSON
来源：http://lmb.jiagoushi.top

Py:   requests.post(url, json={"a": 1})
来源：http://wej.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tsd.zhongyouzk.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qdu.yongpay.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yhb.hnqzz.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ocw.sufxvd.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hbf.9152youxi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wnc.wangdashe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jam.jinqigufen.top

[L03] 设置自定义请求头
来源：http://tvy.aibaodan.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sxs.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://njq.havefunace.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jvz.svipenyu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ibu.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tds.zhijiandao.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ekt.iojbl.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ahz.xziqi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oei.guowangkeji.top

[L04] 设置超时
来源：http://mee.epnwcf.com

Py:   requests.get(url, timeout=5)
来源：http://kmq.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vyq.vqdsnc.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mmm.daria6918.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nww.meibo888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ejq.hongshengwenyu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mjx.snrcjt.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vlj.yangfankeji.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ifa.smart0.xyz

[L05] 上传文件（multipart）
来源：http://ngu.andypj.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jnw.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tda.ctjpmb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pci.fzhhl.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zod.vehdjk.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qbg.yueranfly.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gxa.9152youxi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pni.nanxinkj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nxz.jianghu66.top

[L06] 解析响应为 JSON
来源：http://ucx.jqgfzy.top

Py:   resp.json()
来源：http://ymh.yj20258.top

PHP:  json_decode($body, true);
来源：http://zzz.ivvv.top

JS:   await resp.json()
来源：http://hvg.sufxvd.cn

TS:   await resp.json()
来源：http://ckc.cdnleiting.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gmg.zdbjq.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vse.ivvv.top

Ruby: JSON.parse(resp.body)
来源：http://eaz.cashguo.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xpv.sysykeji.top

[L07] 处理 HTTP 状态码
来源：http://lah.yj202588.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ipw.zdqjudy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://drs.wangshuangyany.cn

JS:   resp.ok;  resp.status
来源：http://izu.zdbjq.cn

TS:   resp.ok;  resp.status
来源：http://ruk.aizwys.cn

Java: resp.statusCode()
来源：http://sbd.guannengcc.top

Go:   resp.StatusCode
来源：http://wro.daxiang520.top

Ruby: resp.code.to_i
来源：http://ceb.xinyue.icu

C#:   (int)resp.StatusCode
来源：http://eku.kuanghao11.cn

[L08] 并发请求多个地址
来源：http://wvj.zhaomingkeji.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ddu.316326.xyz

PHP:  curl_multi_init() 系列
来源：http://wmg.shzxlz.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rhx.ybcxt.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fue.hesvh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://emb.sxryk.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ili.52xcode.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ysw.jlsjyb.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://spd.zhengqikj.top

================================================================================
来源：http://uvz.mhx1999.top

M. 命令行 / 进程 / 环境
来源：http://toc.svipenyu.cn

================================================================================
来源：http://ygt.sufxvd.cn

[M01] 读取命令行参数
来源：http://omo.hammf.cn

Py:   sys.argv[1:]
来源：http://tug.c1oappe.top

PHP:  $argv;  $argc;
来源：http://zas.ydzc1.top

JS:   process.argv.slice(2)
来源：http://ivk.shuidangran.top

TS:   process.argv.slice(2)
来源：http://lup.vehdjk.com

Java: args 数组（main 方法参数）
来源：http://xvw.sjlbkw.cn

Go:   os.Args[1:]
来源：http://xdm.yueranfly.top

Ruby: ARGV
来源：http://rtv.nwbrower.top

C#:   args 数组（Main 方法参数）
来源：http://bgz.ydjk.org.cn

[M02] 读取环境变量
来源：http://uyg.yanxiufei.cn

Py:   os.environ.get("HOME")
来源：http://jya.xylfe.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rlb.ywan-chungtsiang.top

JS:   process.env.HOME
来源：http://yzz.chenzaomai.com

TS:   process.env.HOME
来源：http://otx.yuxming.cn

Java: System.getenv("HOME")
来源：http://khn.andypj.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cln.xziqi.cn

Ruby: ENV["HOME"]
来源：http://bzi.pengpengdd.cyou

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gtn.xuetiantiany.cn

[M03] 执行外部命令
来源：http://wnx.yangfankeji.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lhc.xingfuxueyuan.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pma.aibaodan.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qyl.xuanzx.com

TS:   child_process.execSync("ls -l").toString()
来源：http://gce.meibo888.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://avc.yongpay.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xxd.zhaomingkeji.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://brv.zhaomingkeji.xyz

C#:   Process.Start("ls", "-l");
来源：http://ngu.jyoumei.cn

[M04] 获取当前工作目录
来源：http://feg.cheryme.top

Py:   os.getcwd()
来源：http://azz.bbcook.cn

PHP:  getcwd();
来源：http://zbj.cucudq.cn

JS:   process.cwd()
来源：http://aoc.feifeiyinyue.top

TS:   process.cwd()
来源：http://hbu.ydzc1.top

Java: Path.of("").toAbsolutePath()
来源：http://hyf.svipenyu.cn

Go:   os.Getwd()
来源：http://uwe.gaohongyu789.top

Ruby: Dir.pwd
来源：http://txf.zhoulong.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://rgs.hongshengwenyu.top

[M05] 设置退出码
来源：http://jgv.jqgufenzy.top

Py:   sys.exit(1)
来源：http://egd.0kj1m.cn

PHP:  exit(1);
来源：http://ahy.zhongyouzk.top

JS:   process.exit(1)
来源：http://eud.zycfv.cn

TS:   process.exit(1)
来源：http://gfd.gogol.net.cn

Java: System.exit(1)
来源：http://uik.ydzc1.top

Go:   os.Exit(1)
来源：http://tyg.sjlbkw.cn

Ruby: exit 1
来源：http://aei.cheryme.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gxe.zhongyouzk.top

[M06] 向标准错误输出
来源：http://qvt.quarkkingdee.top

Py:   print("err", file=sys.stderr)
来源：http://cxw.gzhubu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://kij.yuanzhike.top

JS:   console.error("err")
来源：http://ebo.chenlongwang.top

TS:   console.error("err")
来源：http://jif.hcnkem.com

Java: System.err.println("err")
来源：http://gss.zhiwuduotai.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bbu.ydjk.org.cn

Ruby: warn "err"
来源：http://tmb.tianlin.xyz

C#:   Console.Error.WriteLine("err")
来源：http://orl.52xcode.cn

[M07] 判断是否为主入口
来源：http://gwr.xingfuxueyuan.xyz

Py:   if __name__ == "__main__":
来源：http://eeo.yonumen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aax.xuanzx.com

JS:   require.main === module
来源：http://svi.shangyingyoupin.top

TS:   require.main === module
来源：http://nge.fktsv.cn

Java: public static void main(String[] args)
来源：http://jvx.iojbl.cn

Go:   func main()
来源：http://ezx.yvedp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gac.zdqjudy.top

C#:   static void Main(string[] args)
来源：http://bjl.guowangkeji.top

[M08] 获取系统与运行时信息
来源：http://diz.jyoumei.cn

Py:   platform.system();  platform.python_version()
来源：http://bch.hcnkem.com

PHP:  PHP_OS;  phpversion();
来源：http://trg.xinyue.icu

JS:   process.platform;  process.version
来源：http://xqz.316326.xyz

TS:   process.platform;  process.version
来源：http://spd.jinqigufen.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://raq.iojbl.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hnn.xziqi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sir.zhixingplan.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://isa.jlsjyb.cn

================================================================================
来源：http://eut.xinyue.icu

N. 数据结构与算法
来源：http://tai.mhx1999.top

================================================================================
来源：http://alg.c1oappe.top

[N01] 二分查找（有序数组）
来源：http://aod.jiagoushi.top

Py:   bisect.bisect_left(arr, x)
来源：http://pdr.nwbrower.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nvb.shzxlz.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dgw.nwbrower.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mta.fehbvm.com

Java: Arrays.binarySearch(arr, x)
来源：http://mcy.haohaochexian.top

Go:   sort.SearchInts(arr, x)
来源：http://xxy.c1oappe.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://gfm.redwolf501.top


<!-- 参考信息 -->
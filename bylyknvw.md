代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cgm.sufxvd.cn

[J04] 时间戳与日期互转
来源：http://edh.zhiwuduotai.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kps.hammf.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dwz.fengsongda.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://aia.fktsv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cue.jinqigufen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gou.shanyushiyangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://whm.52xcode.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ebr.cashguo.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vrm.shuidangran.top

[J05] 时间加减（加 7 天）
来源：http://zqu.ivvv.top

Py:   now + timedelta(days=7)
来源：http://plc.andypj.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://yqy.jinqigfzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xnl.xylfe.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://loo.nanxuanxn.top

Java: LocalDate.now().plusDays(7)
来源：http://wtq.tianlin.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ipl.zycfv.cn

Ruby: Time.now + 7 * 86400
来源：http://onh.snrcjt.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fuv.ywan-chungtsiang.top

[J06] 计算两时间之差
来源：http://xmy.zhoulong.xyz

Py:   (end - start).total_seconds()
来源：http://mzo.shangyingyoupin.top

PHP:  $end->diff($start)->days;
来源：http://sqs.fzhhl.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vfa.tian-w.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oal.cdnleiting.top

Java: Duration.between(start, end).toSeconds()
来源：http://wfq.fengsongda.top

Go:   end.Sub(start).Hours()
来源：http://geh.cheryme.top

Ruby: end - start                 # 返回秒数
来源：http://ttz.52xcode.cn

C#:   (end - start).TotalSeconds
来源：http://nqf.zycfv.cn

[J07] 比较两个日期
来源：http://ufi.epnwcf.com

Py:   d1 < d2;  d1 == d2
来源：http://xvl.nanxinkj.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://krm.yj20258888.top

JS:   d1.getTime() < d2.getTime()
来源：http://rtb.shzxlz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xkb.jlsjyb.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://njj.hfpthk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ziq.fktsv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vmv.aizwys.cn

C#:   d1 < d2;  d1 == d2
来源：http://qqk.uphjek.com

[J08] 提取年月日与星期
来源：http://yze.ydjk.org.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ezt.ydzc1.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lok.xuetiantiany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://edv.zdqjudy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kdq.ywan-chungtsiang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wwa.zycfv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://quw.daria6918.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vig.daria6918.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://han.xingfuxueyuan.xyz

[J09] 时区处理
来源：http://pzi.vqdsnc.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tzm.shanyushiyangtech.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vcc.guannengcc.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yeb.meibo888.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vpz.9152youxi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jyo.hammf.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xet.pycfn.com

Ruby: Time.now.getlocal("+08:00")
来源：http://onm.sweek.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ofa.kuanghao11.cn

[J10] 取今天 / 本月第一天
来源：http://wir.52xcode.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rye.xuetiantiany.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://obg.ydjk.org.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bow.ydzc1.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xbz.bbcook.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ous.fengsongda.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vrv.xuetiantiany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mim.316326.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lcc.ywan-chungtsiang.top

================================================================================
来源：http://rtl.hnxiangtu.top

K. JSON 与序列化
来源：http://htg.sufxvd.cn

================================================================================
来源：http://qft.xuanzx.com

[K01] 对象转 JSON 字符串
来源：http://rop.uphjek.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tub.epnwcf.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://axf.ehwqpu.com

JS:   JSON.stringify(obj)
来源：http://bnl.tanke756.top

TS:   JSON.stringify(obj)
来源：http://oao.guowangkeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://csy.9152youxi.cn

Go:   json.Marshal(obj)
来源：http://gqz.yueranfly.top

Ruby: obj.to_json                                     // require "json"
来源：http://drs.c1oappe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://yqg.snrcjt.cn

[K02] JSON 字符串转对象
来源：http://upk.quarkkingdee.top

Py:   json.loads(s)
来源：http://iwr.ehwqpu.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wzo.pengpengdd.cyou

JS:   JSON.parse(s)
来源：http://orl.ctjpmb.com

TS:   JSON.parse(s)
来源：http://jft.ybcxt.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lzt.nanxuanxn.top

Go:   json.Unmarshal(data, &v)
来源：http://bvw.mhx1999.top

Ruby: JSON.parse(s)
来源：http://dpe.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zsq.hongshengwenyu.top

[K03] JSON 美化输出（带缩进）
来源：http://liu.sufxvd.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dlc.fengsongda.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wng.0kj1m.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dby.uphjek.com

TS:   JSON.stringify(obj, null, 2)
来源：http://fib.yvedp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://quf.jlsjyb.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ugi.sjlbkw.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qrs.fehbvm.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://iup.hongshengwenyu.top

[K04] 读取 JSON 文件
来源：http://ftb.shzxlz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wyn.feifeiyinyue.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jtw.epnwcf.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kzp.wangdashe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://syg.gaohongyu789.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://igp.chenjidiqi.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kud.jianghu66.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ysr.316326.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://byr.aizwys.cn

[K05] 深拷贝对象
来源：http://aew.daxiang520.top

Py:   copy.deepcopy(obj)
来源：http://ouy.havefunace.top

PHP:  unserialize(serialize($obj));
来源：http://lsp.xuanzx.com

JS:   structuredClone(obj)
来源：http://lvd.xinyue.icu

TS:   structuredClone(obj)
来源：http://jgw.hnqzz.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mgv.guowangkeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://scz.shuidangran.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ozt.tianlin.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://xwv.feifeiyinyue.top

[K06] 解析 URL 查询串
来源：http://iub.ydjk.org.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dlt.cheryme.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zni.nanxinkj.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mun.tanke756.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://srj.xziqi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ywl.gzhubu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://aze.sxryk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bne.vehdjk.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nzg.ybcxt.top

[K07] 进制转换
来源：http://aky.nanxinkj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nji.fzhhl.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sjw.yfazqb.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vtt.sxryk.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://umr.meibo888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kmi.iojbl.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fqs.hywenlv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fel.chenzaomai.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dvi.epnwcf.com

[K08] 二进制序列化（非 JSON）
来源：http://snd.pycfn.com

Py:   pickle.dumps(obj)
来源：http://neg.svipenyu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cqy.bjfxy.top

JS:   v8.serialize(obj)        // Node
来源：http://qpa.uphjek.com

TS:   v8.serialize(obj)        // Node
来源：http://pab.zhiwuduotai.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gwe.chenjidiqi.icu

Go:   encoding/gob
来源：http://pey.pycfn.com

Ruby: Marshal.dump(obj)
来源：http://ktb.gzhubu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kqf.ctjpmb.com

================================================================================
来源：http://bfn.guowangkeji.top

L. 网络请求
来源：http://ihl.gaohongyu789.top

================================================================================
来源：http://lsk.zhongyouzk.top

[L01] 发送 GET 请求
来源：http://fss.havefunace.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://btb.yfazqb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kaa.fengsongda.top

JS:   await fetch(url)
来源：http://grd.wangdashe.top

TS:   await fetch(url)
来源：http://whq.wangshuangyany.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://auv.yangfankeji.com

Go:   resp, err := http.Get(url)
来源：http://nuy.nanxuanxn.top

Ruby: Net::HTTP.get(URI(url))
来源：http://aul.daxiang520.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sww.ydjk.org.cn

[L02] 发送 POST JSON
来源：http://qtu.feifeiyinyue.top

Py:   requests.post(url, json={"a": 1})
来源：http://eak.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yly.vqdsnc.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zbi.redwolf501.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://djd.guannengcc.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pjv.sxryk.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hnm.nanxinkj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zkf.birdmap.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tlp.fengsongda.top

[L03] 设置自定义请求头
来源：http://pbr.zdbjq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zzn.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nbg.pycfn.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://acv.guannengcc.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mvv.jiagoushi.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ftq.hesvh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qbh.shuidangran.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kri.daria6918.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gsy.gaohongyu789.top

[L04] 设置超时
来源：http://psj.yj202588.top

Py:   requests.get(url, timeout=5)
来源：http://vbx.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qdn.aibaodan.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tyb.bbcook.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rms.jyoumei.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lgh.jinyuanbaomall.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dtq.tanke756.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rwx.yongpay.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://giz.svipenyu.cn

[L05] 上传文件（multipart）
来源：http://vmi.fehbvm.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iwj.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uin.guowangkeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kxj.tian-w.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ecp.pycfn.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bwg.cucudq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://doi.cheryme.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wyf.jinqigufen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ghq.xinyue.icu

[L06] 解析响应为 JSON
来源：http://rzw.9152youxi.cn

Py:   resp.json()
来源：http://bxd.ydzc1.top

PHP:  json_decode($body, true);
来源：http://nih.ppjwa.cn

JS:   await resp.json()
来源：http://eje.jinghuilouyu.cn

TS:   await resp.json()
来源：http://lgz.hcnkem.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uqa.zdqjudy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://smy.mhx1999.top

Ruby: JSON.parse(resp.body)
来源：http://geg.shzxlz.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bbr.tanke756.top

[L07] 处理 HTTP 状态码
来源：http://gha.jinghuilouyu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kav.zhongyouzk.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wmv.nanxinkj.top

JS:   resp.ok;  resp.status
来源：http://xzh.nanxinkj.top

TS:   resp.ok;  resp.status
来源：http://pts.tian-w.cn

Java: resp.statusCode()
来源：http://fiw.xylfe.cn

Go:   resp.StatusCode
来源：http://tzo.zhaomingkeji.xyz

Ruby: resp.code.to_i
来源：http://nkk.cucudq.cn

C#:   (int)resp.StatusCode
来源：http://uwi.chenjidiqi.icu

[L08] 并发请求多个地址
来源：http://hjo.epnwcf.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mhg.9152youxi.cn

PHP:  curl_multi_init() 系列
来源：http://lml.mhx1999.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yqz.yuxming.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iwt.wangdashe.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wxd.chenlongwang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blf.redwolf501.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://iki.xingfuxueyuan.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kaq.chenzaomai.com

================================================================================
来源：http://xji.shuidangran.top

M. 命令行 / 进程 / 环境
来源：http://vym.xingfuxueyuan.xyz

================================================================================
来源：http://etm.svipenyu.cn

[M01] 读取命令行参数
来源：http://oud.yvedp.cn

Py:   sys.argv[1:]
来源：http://mxt.shanyushiyangkeji.top

PHP:  $argv;  $argc;
来源：http://lwh.wangshuangyany.cn

JS:   process.argv.slice(2)
来源：http://eod.shanyushiyangtech.top

TS:   process.argv.slice(2)
来源：http://oif.yfazqb.com

Java: args 数组（main 方法参数）
来源：http://xla.redwolf501.top

Go:   os.Args[1:]
来源：http://rbe.yuxming.cn

Ruby: ARGV
来源：http://cwt.fehbvm.com

C#:   args 数组（Main 方法参数）
来源：http://ogw.hammf.cn

[M02] 读取环境变量
来源：http://jfy.guowangkeji.top

Py:   os.environ.get("HOME")
来源：http://skk.0kj1m.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://okf.smart0.xyz

JS:   process.env.HOME
来源：http://waw.chenzaomai.com

TS:   process.env.HOME
来源：http://jak.xingfuxueyuan.xyz

Java: System.getenv("HOME")
来源：http://fdm.yuanzhike.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jcd.hesvh.cn

Ruby: ENV["HOME"]
来源：http://gis.yfazqb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rnu.zhoulong.xyz

[M03] 执行外部命令
来源：http://ohh.zhaomingkeji.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gng.ybcxt.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wsr.jianghu66.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hye.xingfuxueyuan.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://rzv.hnqzz.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uya.nwbrower.top

Go:   exec.Command("ls", "-l").Output()
来源：http://phs.pycfn.com

Ruby: system("ls -l");  `ls -l`
来源：http://ovt.cheryme.top

C#:   Process.Start("ls", "-l");
来源：http://ism.gzhubu.top

[M04] 获取当前工作目录
来源：http://ynp.xingfuxueyuan.xyz

Py:   os.getcwd()
来源：http://haf.jianghu66.top

PHP:  getcwd();
来源：http://vgy.yj20258.top

JS:   process.cwd()
来源：http://wue.zdbjq.cn

TS:   process.cwd()
来源：http://nub.hfpthk.cn

Java: Path.of("").toAbsolutePath()
来源：http://dhm.pycfn.com

Go:   os.Getwd()
来源：http://sez.meibo888.top

Ruby: Dir.pwd
来源：http://wuc.zdqjudy.top

C#:   Directory.GetCurrentDirectory()
来源：http://xfn.xziqi.cn

[M05] 设置退出码
来源：http://wgy.hywenlv.cn

Py:   sys.exit(1)
来源：http://ffz.havefunace.top

PHP:  exit(1);
来源：http://msy.redwolf501.top

JS:   process.exit(1)
来源：http://ecu.jlsjyb.cn

TS:   process.exit(1)
来源：http://pxl.hongshengwenyu.top

Java: System.exit(1)
来源：http://vze.yuxming.cn

Go:   os.Exit(1)
来源：http://agi.zhaomingkeji.xyz

Ruby: exit 1
来源：http://sju.uphjek.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ubn.fanxiaobao.xyz

[M06] 向标准错误输出
来源：http://pzo.chenlongwang.top

Py:   print("err", file=sys.stderr)
来源：http://kff.sweek.top

PHP:  fwrite(STDERR, "err\n");
来源：http://utw.svipenyu.cn

JS:   console.error("err")
来源：http://xqk.ppjwa.cn

TS:   console.error("err")
来源：http://zne.shanyushiyangtech.top

Java: System.err.println("err")
来源：http://iys.nanxuanxn.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qiv.gaohongyu789.top

Ruby: warn "err"
来源：http://ffw.yuxming.cn

C#:   Console.Error.WriteLine("err")
来源：http://kpj.fktsv.cn

[M07] 判断是否为主入口
来源：http://ufh.yueranfly.top

Py:   if __name__ == "__main__":
来源：http://wbw.chenlongwang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bmx.mhx1999.top

JS:   require.main === module
来源：http://gxg.hnxiangtu.top

TS:   require.main === module
来源：http://cen.feifeiyinyue.top

Java: public static void main(String[] args)
来源：http://bxn.jinghuilouyu.cn

Go:   func main()
来源：http://qzm.bjfxy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wqn.hysaishi.cn

C#:   static void Main(string[] args)
来源：http://ijr.vehdjk.com

[M08] 获取系统与运行时信息
来源：http://hkm.yangfankeji.com

Py:   platform.system();  platform.python_version()
来源：http://vfk.havefunace.top

PHP:  PHP_OS;  phpversion();
来源：http://qse.52xcode.cn

JS:   process.platform;  process.version
来源：http://sxd.kuanghao11.cn

TS:   process.platform;  process.version
来源：http://gyj.ywan-chungtsiang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xil.meibo888.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xpk.c1oappe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ikh.zhaomingkeji.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://rtg.hywenlv.cn

================================================================================
来源：http://lxf.ehwqpu.com

N. 数据结构与算法
来源：http://wrk.nanxinkj.top

================================================================================
来源：http://gma.zycfv.cn

[N01] 二分查找（有序数组）
来源：http://ina.chenjidiqi.icu

Py:   bisect.bisect_left(arr, x)
来源：http://uvp.sxryk.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mcj.wangdashe.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iff.shanyushiyangkeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://szx.tianlin.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://usa.fengsongda.top

Go:   sort.SearchInts(arr, x)
来源：http://bgw.tian-w.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hbu.cashguo.top


<!-- 参考信息 -->
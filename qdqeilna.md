代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mfo.zhixingplan.top

[J04] 时间戳与日期互转
来源：http://kan.yuanzhike.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://icq.316326.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ive.0kj1m.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://svd.52xcode.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://crb.ywan-chungtsiang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://umq.zhoulong.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ogl.chenlongwang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ful.shangyingyoupin.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://neh.ehwqpu.com

[J05] 时间加减（加 7 天）
来源：http://vix.gotoacloud.top

Py:   now + timedelta(days=7)
来源：http://rdi.zhiwuduotai.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://hmi.wangdashe.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kib.gogol.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wsq.shzxlz.cn

Java: LocalDate.now().plusDays(7)
来源：http://bnh.pycfn.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jgp.9152youxi.cn

Ruby: Time.now + 7 * 86400
来源：http://jwv.ywan-chungtsiang.top

C#:   DateTime.Now.AddDays(7)
来源：http://dih.smart0.xyz

[J06] 计算两时间之差
来源：http://xvn.hesvh.cn

Py:   (end - start).total_seconds()
来源：http://tln.yongpay.top

PHP:  $end->diff($start)->days;
来源：http://akz.ppjwa.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qyb.xuanzx.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wej.tianlin.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://blv.shanyushiyangkeji.top

Go:   end.Sub(start).Hours()
来源：http://loi.hcnkem.com

Ruby: end - start                 # 返回秒数
来源：http://hpe.zhoulong.xyz

C#:   (end - start).TotalSeconds
来源：http://mrx.meibo888.top

[J07] 比较两个日期
来源：http://ixj.jinyuanbaomall.cn

Py:   d1 < d2;  d1 == d2
来源：http://zya.jqgufenzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://psq.c1oappe.top

JS:   d1.getTime() < d2.getTime()
来源：http://emw.fanxiaobao.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://tnn.yueranfly.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lpd.gzhubu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ixc.zhixingplan.top

Ruby: d1 < d2;  d1 == d2
来源：http://jui.zhongyouzk.top

C#:   d1 < d2;  d1 == d2
来源：http://uga.cdnleiting.top

[J08] 提取年月日与星期
来源：http://wrw.quarkkingdee.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jzz.shuidangran.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vtq.xziqi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mgb.jinyuanbaomall.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eca.hywenlv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://otk.zhaomingkeji.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hcb.jiagoushi.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://brn.ybcxt.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kzl.dashuyun.cn

[J09] 时区处理
来源：http://zpb.mhx1999.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cpe.xingfuxueyuan.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tsv.iojbl.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://chw.chenlongwang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://equ.quarkkingdee.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dzz.yuanzhike.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gno.shangyingyoupin.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fga.sjlbkw.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oxg.jqgufenzy.top

[J10] 取今天 / 本月第一天
来源：http://awr.xingfuxueyuan.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://cck.hcnkem.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://noc.andypj.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cvd.xinyue.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dcn.jinqigufen.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qsv.sysykeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lrb.ppjwa.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fat.xziqi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://puj.hfpthk.cn

================================================================================
来源：http://hne.gzhubu.top

K. JSON 与序列化
来源：http://duu.cdnleiting.top

================================================================================
来源：http://ham.xinyue.icu

[K01] 对象转 JSON 字符串
来源：http://qlo.chenlongwang.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zve.jqgufenzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://thv.meibo888.top

JS:   JSON.stringify(obj)
来源：http://eit.gzhubu.top

TS:   JSON.stringify(obj)
来源：http://ujf.haohaochexian.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xrw.guannengcc.top

Go:   json.Marshal(obj)
来源：http://llo.jiagoushi.top

Ruby: obj.to_json                                     // require "json"
来源：http://ekq.svipenyu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fdx.smart0.xyz

[K02] JSON 字符串转对象
来源：http://nbc.pengpengdd.cyou

Py:   json.loads(s)
来源：http://cdd.yvedp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://aiq.yanxiufei.cn

JS:   JSON.parse(s)
来源：http://ngu.daria6918.cn

TS:   JSON.parse(s)
来源：http://clq.jinqigufen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rvh.ivvv.top

Go:   json.Unmarshal(data, &v)
来源：http://bua.zhongyouzk.top

Ruby: JSON.parse(s)
来源：http://vbm.yj20258.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vqy.xuetiantiany.cn

[K03] JSON 美化输出（带缩进）
来源：http://hwp.hcnkem.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://piv.jqgfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ltn.yuxming.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pxa.guannengcc.top

TS:   JSON.stringify(obj, null, 2)
来源：http://jjb.zhengqikj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oiz.xingfuxueyuan.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qwd.tanke756.top

Ruby: JSON.pretty_generate(obj)
来源：http://atd.tianlin.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qzj.jinqigfzy.top

[K04] 读取 JSON 文件
来源：http://xen.epnwcf.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mxh.pengpengdd.cyou

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dxs.wangdashe.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vuc.yj20258.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://awh.jiagoushi.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bod.nanxuanxn.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oob.chenlongwang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://kgt.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yaf.yuanzhike.top

[K05] 深拷贝对象
来源：http://waf.mhx1999.top

Py:   copy.deepcopy(obj)
来源：http://pum.andypj.xyz

PHP:  unserialize(serialize($obj));
来源：http://sxz.yfazqb.com

JS:   structuredClone(obj)
来源：http://bpq.fengsongda.top

TS:   structuredClone(obj)
来源：http://gkn.uphjek.com

Java: // 手写拷贝构造，或序列化往返
来源：http://gsx.yj20258888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mev.quarkkingdee.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rkq.xuanzx.com

C#:   // 序列化往返，或自定义 Clone
来源：http://riw.cucudq.cn

[K06] 解析 URL 查询串
来源：http://etj.dashuyun.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pzp.yj20258.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hne.shzxlz.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fsb.meibo888.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hug.xziqi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://anf.nanxuanxn.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://uqb.shangyingyoupin.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bri.ctjpmb.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qvx.hnxiangtu.top

[K07] 进制转换
来源：http://ncc.cdnleiting.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://aoc.epnwcf.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://shn.jinghuilouyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://eux.redwolf501.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rmo.xuanzx.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xcr.sysykeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tno.cucudq.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yhn.wangdashe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cvd.cashguo.top

[K08] 二进制序列化（非 JSON）
来源：http://hpk.cheryme.top

Py:   pickle.dumps(obj)
来源：http://alq.shuidangran.top

PHP:  serialize($obj);  unserialize($s);
来源：http://you.feifeiyinyue.top

JS:   v8.serialize(obj)        // Node
来源：http://qee.yangfankeji.com

TS:   v8.serialize(obj)        // Node
来源：http://hqg.c1oappe.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://law.shanyushiyangtech.top

Go:   encoding/gob
来源：http://mtq.sufxvd.cn

Ruby: Marshal.dump(obj)
来源：http://tlh.yfazqb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://djo.ppjwa.cn

================================================================================
来源：http://qnq.jlsjyb.cn

L. 网络请求
来源：http://dov.smart0.xyz

================================================================================
来源：http://kca.jinghuilouyu.cn

[L01] 发送 GET 请求
来源：http://ntk.tarul.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zth.fzhhl.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xqt.mhx1999.top

JS:   await fetch(url)
来源：http://kiq.dianchejie.cn

TS:   await fetch(url)
来源：http://syg.hnxiangtu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://chy.zhixingplan.top

Go:   resp, err := http.Get(url)
来源：http://eax.sufxvd.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://oll.yj20258888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ozo.jlsjyb.cn

[L02] 发送 POST JSON
来源：http://hkr.cqqwz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ywr.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ode.jlsjyb.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ysq.xinyue.icu

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yqo.yonumen.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cej.meibo888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qbg.zhixingplan.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://daf.cucudq.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kcg.jqgufenzy.top

[L03] 设置自定义请求头
来源：http://oli.ivvv.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zoj.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://doo.haohaochexian.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eas.jinqigufen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vhh.jinghuilouyu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zyx.birdmap.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sub.cqqwz.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yqb.sweek.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kfq.nanxinkj.top

[L04] 设置超时
来源：http://xrh.yuanzhike.top

Py:   requests.get(url, timeout=5)
来源：http://znc.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xzp.sysykeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fzr.yongpay.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kzn.hnxiangtu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blc.jinyuanbaomall.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qaz.hcnkem.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ihw.yuanzhike.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jgi.tanke756.top

[L05] 上传文件（multipart）
来源：http://rqm.tian-w.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oht.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://obt.hysaishi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sdc.xuanzx.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ctb.hongshengwenyu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tjj.daxiang520.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://net.52xcode.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bnr.ivvv.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vid.ivvv.top

[L06] 解析响应为 JSON
来源：http://ayn.zhongyouzk.top

Py:   resp.json()
来源：http://hto.shangyingyoupin.top

PHP:  json_decode($body, true);
来源：http://vzm.cheryme.top

JS:   await resp.json()
来源：http://ucj.zhixingplan.top

TS:   await resp.json()
来源：http://iwk.tarul.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tzg.316326.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lzu.sxryk.cn

Ruby: JSON.parse(resp.body)
来源：http://mgi.vqdsnc.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kwj.pycfn.com

[L07] 处理 HTTP 状态码
来源：http://twm.kuanghao11.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nsz.zycfv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bvj.xylfe.cn

JS:   resp.ok;  resp.status
来源：http://mtw.xuanzx.com

TS:   resp.ok;  resp.status
来源：http://elq.9152youxi.cn

Java: resp.statusCode()
来源：http://vdv.zhijiandao.cn

Go:   resp.StatusCode
来源：http://tli.jlsjyb.cn

Ruby: resp.code.to_i
来源：http://iqy.yj20258.top

C#:   (int)resp.StatusCode
来源：http://mii.c1oappe.top

[L08] 并发请求多个地址
来源：http://vez.wangdashe.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qkw.cqqwz.cn

PHP:  curl_multi_init() 系列
来源：http://rem.yanxiufei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://etg.tanke756.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gek.gaohongyu789.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yqj.sufxvd.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://iip.tanke756.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pkh.guowangkeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://diy.chenjidiqi.icu

================================================================================
来源：http://dyp.hammf.cn

M. 命令行 / 进程 / 环境
来源：http://xvo.tianlin.xyz

================================================================================
来源：http://yxk.fehbvm.com

[M01] 读取命令行参数
来源：http://qzi.yongpay.top

Py:   sys.argv[1:]
来源：http://vfj.hongshengwenyu.top

PHP:  $argv;  $argc;
来源：http://lgj.svipenyu.cn

JS:   process.argv.slice(2)
来源：http://kti.cqqwz.cn

TS:   process.argv.slice(2)
来源：http://dww.mhx1999.top

Java: args 数组（main 方法参数）
来源：http://zzo.yj20258.top

Go:   os.Args[1:]
来源：http://amb.zhengqikj.top

Ruby: ARGV
来源：http://qzb.fengsongda.top

C#:   args 数组（Main 方法参数）
来源：http://oyl.redwolf501.top

[M02] 读取环境变量
来源：http://klr.ywan-chungtsiang.top

Py:   os.environ.get("HOME")
来源：http://rhv.jlsjyb.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ave.hcnkem.com

JS:   process.env.HOME
来源：http://zzz.jiagoushi.top

TS:   process.env.HOME
来源：http://ont.ywan-chungtsiang.top

Java: System.getenv("HOME")
来源：http://aoc.ctjpmb.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fqt.316326.xyz

Ruby: ENV["HOME"]
来源：http://moe.xziqi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ddq.ydzc1.top

[M03] 执行外部命令
来源：http://nhh.zhongyouzk.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zre.tianlin.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bcj.zdqjudy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jzs.shuidangran.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xdf.iojbl.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lfl.hcnkem.com

Go:   exec.Command("ls", "-l").Output()
来源：http://tcd.shzxlz.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rjn.shanyushiyangtech.top

C#:   Process.Start("ls", "-l");
来源：http://giq.jiagoushi.top

[M04] 获取当前工作目录
来源：http://hgf.fktsv.cn

Py:   os.getcwd()
来源：http://mcq.pengpengdd.cyou

PHP:  getcwd();
来源：http://mqc.chenlongwang.top

JS:   process.cwd()
来源：http://aen.xingfuxueyuan.xyz

TS:   process.cwd()
来源：http://fus.smart0.xyz

Java: Path.of("").toAbsolutePath()
来源：http://akb.cdnleiting.top

Go:   os.Getwd()
来源：http://mek.shanyushiyangkeji.top

Ruby: Dir.pwd
来源：http://ovz.yj202588.top

C#:   Directory.GetCurrentDirectory()
来源：http://rpc.smart0.xyz

[M05] 设置退出码
来源：http://sbm.cucudq.cn

Py:   sys.exit(1)
来源：http://wfn.zdbjq.cn

PHP:  exit(1);
来源：http://pwo.chenjidiqi.icu

JS:   process.exit(1)
来源：http://xmp.cucudq.cn

TS:   process.exit(1)
来源：http://gqz.hnqzz.top

Java: System.exit(1)
来源：http://brp.xuetiantiany.cn

Go:   os.Exit(1)
来源：http://cle.kuanghao11.cn

Ruby: exit 1
来源：http://qlg.nwbrower.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zwu.hnqzz.top

[M06] 向标准错误输出
来源：http://xoi.haohaochexian.top

Py:   print("err", file=sys.stderr)
来源：http://odv.shanyushiyangtech.top

PHP:  fwrite(STDERR, "err\n");
来源：http://zua.cdnleiting.top

JS:   console.error("err")
来源：http://dhr.quarkkingdee.top

TS:   console.error("err")
来源：http://kqv.0kj1m.cn

Java: System.err.println("err")
来源：http://hyy.fktsv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pnq.pengpengdd.cyou

Ruby: warn "err"
来源：http://dap.jqgufenzy.top

C#:   Console.Error.WriteLine("err")
来源：http://lfl.epnwcf.com

[M07] 判断是否为主入口
来源：http://sgv.snrcjt.cn

Py:   if __name__ == "__main__":
来源：http://nnt.yj202588.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://azx.shanyushiyangtech.top

JS:   require.main === module
来源：http://bkq.andypj.xyz

TS:   require.main === module
来源：http://cpm.52xcode.cn

Java: public static void main(String[] args)
来源：http://ldh.smart0.xyz

Go:   func main()
来源：http://mfn.andypj.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xmh.yanxiufei.cn

C#:   static void Main(string[] args)
来源：http://kky.c1oappe.top

[M08] 获取系统与运行时信息
来源：http://ftx.mhx1999.top

Py:   platform.system();  platform.python_version()
来源：http://dcg.yueranfly.top

PHP:  PHP_OS;  phpversion();
来源：http://sgz.jlsjyb.cn

JS:   process.platform;  process.version
来源：http://btl.jqgufenzy.top

TS:   process.platform;  process.version
来源：http://wle.yj202588.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uty.havefunace.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://htw.chenjidiqi.icu

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tam.shanyushiyangtech.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://bfp.havefunace.top

================================================================================
来源：http://srl.c1oappe.top

N. 数据结构与算法
来源：http://dyu.fktsv.cn

================================================================================
来源：http://loo.nanxuanxn.top

[N01] 二分查找（有序数组）
来源：http://ier.nanxinkj.top

Py:   bisect.bisect_left(arr, x)
来源：http://skg.52xcode.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://oxq.nanxuanxn.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jnj.nwbrower.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dtf.0kj1m.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hea.jianghu66.top

Go:   sort.SearchInts(arr, x)
来源：http://ahm.yfazqb.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://shj.zhongyouzk.top


<!-- 参考信息 -->
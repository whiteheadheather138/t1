代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://umw.hesvh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fxn.jinghuilouyu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hfc.ivvv.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gwg.ydzc1.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xbq.jinghuilouyu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pqv.daxiang520.top

[J05] 时间加减（加 7 天）
来源：http://mzn.ydjk.org.cn

Py:   now + timedelta(days=7)
来源：http://ojr.epnwcf.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://bha.jianghu66.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zpt.yongpay.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vmq.quarkkingdee.top

Java: LocalDate.now().plusDays(7)
来源：http://wrg.hcnkem.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rxu.jinqigufen.top

Ruby: Time.now + 7 * 86400
来源：http://oiv.fehbvm.com

C#:   DateTime.Now.AddDays(7)
来源：http://tnz.c1oappe.top

[J06] 计算两时间之差
来源：http://hxt.jinqigfzy.top

Py:   (end - start).total_seconds()
来源：http://zhh.yonumen.top

PHP:  $end->diff($start)->days;
来源：http://inx.wangdashe.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ilh.yj20258888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://woj.chenlongwang.top

Java: Duration.between(start, end).toSeconds()
来源：http://nng.xuetiantiany.cn

Go:   end.Sub(start).Hours()
来源：http://rfc.xylfe.cn

Ruby: end - start                 # 返回秒数
来源：http://qik.wangdashe.top

C#:   (end - start).TotalSeconds
来源：http://nsw.sweek.top

[J07] 比较两个日期
来源：http://xed.yvedp.cn

Py:   d1 < d2;  d1 == d2
来源：http://kyk.vqdsnc.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ahz.yonumen.top

JS:   d1.getTime() < d2.getTime()
来源：http://yty.c1oappe.top

TS:   d1.getTime() < d2.getTime()
来源：http://hjg.shangyingyoupin.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xnt.quarkkingdee.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jns.zhoulong.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://btc.c1oappe.top

C#:   d1 < d2;  d1 == d2
来源：http://gtq.zdqjudy.top

[J08] 提取年月日与星期
来源：http://yns.hcnkem.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hwi.shuidangran.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wdt.haohaochexian.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fdh.svipenyu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dhc.hfpthk.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bap.cdnleiting.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zum.bbcook.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kjl.zhixingplan.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zlj.zhongyouzk.top

[J09] 时区处理
来源：http://fwo.yonumen.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cce.daria6918.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://akv.yonumen.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sid.iojbl.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://esb.zhaomingkeji.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xwv.yanxiufei.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fcd.tanke756.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ciq.hcnkem.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xzl.tianlin.xyz

[J10] 取今天 / 本月第一天
来源：http://lod.hnqzz.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hdo.shuidangran.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jqo.redwolf501.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vxe.aibaodan.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gkn.epnwcf.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nlh.hongshengwenyu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ahu.fanxiaobao.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ayp.bjfxy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vaf.chenzaomai.com

================================================================================
来源：http://xrv.zycfv.cn

K. JSON 与序列化
来源：http://bvk.tianlin.xyz

================================================================================
来源：http://zqt.yuxming.cn

[K01] 对象转 JSON 字符串
来源：http://whh.yueranfly.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nci.cheryme.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qyd.jinyuanbaomall.cn

JS:   JSON.stringify(obj)
来源：http://cnw.sufxvd.cn

TS:   JSON.stringify(obj)
来源：http://cae.zhixingplan.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yfc.ybcxt.top

Go:   json.Marshal(obj)
来源：http://tei.tian-w.cn

Ruby: obj.to_json                                     // require "json"
来源：http://khe.yuanzhike.top

C#:   JsonSerializer.Serialize(obj)
来源：http://uvu.ppjwa.cn

[K02] JSON 字符串转对象
来源：http://lzg.yj202588.top

Py:   json.loads(s)
来源：http://muc.yangfankeji.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wxe.zhaomingkeji.xyz

JS:   JSON.parse(s)
来源：http://ogp.iojbl.cn

TS:   JSON.parse(s)
来源：http://ruu.daxiang520.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vmj.yfazqb.com

Go:   json.Unmarshal(data, &v)
来源：http://zyn.shzxlz.cn

Ruby: JSON.parse(s)
来源：http://iau.havefunace.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://joy.hnxiangtu.top

[K03] JSON 美化输出（带缩进）
来源：http://svu.tanke756.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qer.jlsjyb.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://koa.nwbrower.top

JS:   JSON.stringify(obj, null, 2)
来源：http://roa.bbcook.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kov.havefunace.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rvg.andypj.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://idk.zdqjudy.top

Ruby: JSON.pretty_generate(obj)
来源：http://qev.haohaochexian.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hng.daxiang520.top

[K04] 读取 JSON 文件
来源：http://rnt.xylfe.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ydm.xinyue.icu

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hml.shanyushiyangkeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vbc.dashuyun.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tqw.jiagoushi.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kpi.uphjek.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://eis.shzxlz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rju.zhiwuduotai.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ntr.cheryme.top

[K05] 深拷贝对象
来源：http://xvd.tianlin.xyz

Py:   copy.deepcopy(obj)
来源：http://qgj.nwbrower.top

PHP:  unserialize(serialize($obj));
来源：http://xaz.hcnkem.com

JS:   structuredClone(obj)
来源：http://oju.hcnkem.com

TS:   structuredClone(obj)
来源：http://kgl.tarul.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://juz.zhiwuduotai.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dlr.pengpengdd.cyou

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qvf.xylfe.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kle.shuidangran.top

[K06] 解析 URL 查询串
来源：http://hvk.zhengqikj.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ybu.yj202588.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://egd.yuanzhike.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ifb.hywenlv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kdk.andypj.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yxi.kuanghao11.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hex.sufxvd.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jng.xziqi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wve.gogol.net.cn

[K07] 进制转换
来源：http://dsf.zhiwuduotai.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://voz.yj20258888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xwz.gotoacloud.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://axz.havefunace.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bmi.haohaochexian.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ffs.yuxming.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ldw.daria6918.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qxx.aibaodan.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jzb.andypj.xyz

[K08] 二进制序列化（非 JSON）
来源：http://doq.shanyushiyangkeji.top

Py:   pickle.dumps(obj)
来源：http://lwz.yuxming.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://che.cashguo.top

JS:   v8.serialize(obj)        // Node
来源：http://dms.hcnkem.com

TS:   v8.serialize(obj)        // Node
来源：http://nak.daxiang520.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hud.9152youxi.cn

Go:   encoding/gob
来源：http://hcn.tarul.cn

Ruby: Marshal.dump(obj)
来源：http://cop.jyoumei.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://glo.gaohongyu789.top

================================================================================
来源：http://cvw.sxryk.cn

L. 网络请求
来源：http://rwc.mhx1999.top

================================================================================
来源：http://kdh.dashuyun.cn

[L01] 发送 GET 请求
来源：http://gqw.yueranfly.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ayu.jinghuilouyu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cyc.yueranfly.top

JS:   await fetch(url)
来源：http://gxd.fehbvm.com

TS:   await fetch(url)
来源：http://vdn.sufxvd.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bqm.uphjek.com

Go:   resp, err := http.Get(url)
来源：http://blu.havefunace.top

Ruby: Net::HTTP.get(URI(url))
来源：http://hil.jinghuilouyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lut.ybcxt.top

[L02] 发送 POST JSON
来源：http://fhb.dianchejie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://svb.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nga.nanxuanxn.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dmo.zhaomingkeji.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rhr.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mme.gogol.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eii.tarul.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zgl.yanxiufei.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ukm.chenjidiqi.icu

[L03] 设置自定义请求头
来源：http://lvd.xylfe.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://etk.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sdr.zdbjq.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zlo.sjlbkw.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lnc.jinqigufen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jhu.tianlin.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hvp.ybcxt.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xfy.zycfv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nof.shangyingyoupin.top

[L04] 设置超时
来源：http://kev.snrcjt.cn

Py:   requests.get(url, timeout=5)
来源：http://ibb.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://huq.yj20258888.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fhe.shanyushiyangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oka.shanyushiyangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://onz.havefunace.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lhw.fzhhl.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nas.0kj1m.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rbm.ehwqpu.com

[L05] 上传文件（multipart）
来源：http://fdg.gotoacloud.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zde.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://imt.zdbjq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cnj.snrcjt.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ted.yj20258888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nxx.snrcjt.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rvf.guowangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jvd.ywan-chungtsiang.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tgy.aizwys.cn

[L06] 解析响应为 JSON
来源：http://swa.316326.xyz

Py:   resp.json()
来源：http://vvu.fehbvm.com

PHP:  json_decode($body, true);
来源：http://qpm.0kj1m.cn

JS:   await resp.json()
来源：http://thc.feifeiyinyue.top

TS:   await resp.json()
来源：http://jpu.tarul.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://djn.shzxlz.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nnh.pengpengdd.cyou

Ruby: JSON.parse(resp.body)
来源：http://vfw.zdqjudy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vcu.hnxiangtu.top

[L07] 处理 HTTP 状态码
来源：http://nqc.52xcode.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wmg.gogol.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qqr.cucudq.cn

JS:   resp.ok;  resp.status
来源：http://bxz.dianchejie.cn

TS:   resp.ok;  resp.status
来源：http://ofn.ehwqpu.com

Java: resp.statusCode()
来源：http://jir.pengpengdd.cyou

Go:   resp.StatusCode
来源：http://ufp.smart0.xyz

Ruby: resp.code.to_i
来源：http://bxc.shanyushiyangkeji.top

C#:   (int)resp.StatusCode
来源：http://oge.vqdsnc.cn

[L08] 并发请求多个地址
来源：http://tkq.aibaodan.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://umc.daxiang520.top

PHP:  curl_multi_init() 系列
来源：http://zcn.guannengcc.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://btr.haohaochexian.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://plq.haohaochexian.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vut.jyoumei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qot.feifeiyinyue.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xom.wangshuangyany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://apl.svipenyu.cn

================================================================================
来源：http://ivf.zhoulong.xyz

M. 命令行 / 进程 / 环境
来源：http://nnw.hesvh.cn

================================================================================
来源：http://nxz.nwbrower.top

[M01] 读取命令行参数
来源：http://ubb.hnxiangtu.top

Py:   sys.argv[1:]
来源：http://axi.cqqwz.cn

PHP:  $argv;  $argc;
来源：http://gwn.hysaishi.cn

JS:   process.argv.slice(2)
来源：http://vjm.gzhubu.top

TS:   process.argv.slice(2)
来源：http://ziw.0kj1m.cn

Java: args 数组（main 方法参数）
来源：http://azv.redwolf501.top

Go:   os.Args[1:]
来源：http://nfu.zhixingplan.top

Ruby: ARGV
来源：http://hdt.mhx1999.top

C#:   args 数组（Main 方法参数）
来源：http://tyq.yanxiufei.cn

[M02] 读取环境变量
来源：http://pwb.bbcook.cn

Py:   os.environ.get("HOME")
来源：http://kwk.andypj.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nik.zdbjq.cn

JS:   process.env.HOME
来源：http://wtk.pycfn.com

TS:   process.env.HOME
来源：http://cgt.jiagoushi.top

Java: System.getenv("HOME")
来源：http://lpu.tianlin.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gxl.havefunace.top

Ruby: ENV["HOME"]
来源：http://kxc.guowangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rbr.dianchejie.cn

[M03] 执行外部命令
来源：http://qvb.yuanzhike.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gee.ehwqpu.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mjl.yuanzhike.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fqq.hfpthk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ljg.zhoulong.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wdg.yueranfly.top

Go:   exec.Command("ls", "-l").Output()
来源：http://upu.wangshuangyany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fto.cucudq.cn

C#:   Process.Start("ls", "-l");
来源：http://fur.yj20258.top

[M04] 获取当前工作目录
来源：http://fgy.aizwys.cn

Py:   os.getcwd()
来源：http://ocj.tanke756.top

PHP:  getcwd();
来源：http://kin.jinqigfzy.top

JS:   process.cwd()
来源：http://eme.ywan-chungtsiang.top

TS:   process.cwd()
来源：http://qae.zhengqikj.top

Java: Path.of("").toAbsolutePath()
来源：http://esv.sufxvd.cn

Go:   os.Getwd()
来源：http://rfj.pycfn.com

Ruby: Dir.pwd
来源：http://fzu.chenjidiqi.icu

C#:   Directory.GetCurrentDirectory()
来源：http://azg.zhaomingkeji.xyz

[M05] 设置退出码
来源：http://dci.yj20258.top

Py:   sys.exit(1)
来源：http://fpa.chenjidiqi.icu

PHP:  exit(1);
来源：http://ilz.hysaishi.cn

JS:   process.exit(1)
来源：http://gua.jianghu66.top

TS:   process.exit(1)
来源：http://unt.shangyingyoupin.top

Java: System.exit(1)
来源：http://hei.gogol.net.cn

Go:   os.Exit(1)
来源：http://odz.cucudq.cn

Ruby: exit 1
来源：http://hjk.chenjidiqi.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tft.fanxiaobao.xyz

[M06] 向标准错误输出
来源：http://hlo.quarkkingdee.top

Py:   print("err", file=sys.stderr)
来源：http://axo.ybcxt.top

PHP:  fwrite(STDERR, "err\n");
来源：http://afo.bbcook.cn

JS:   console.error("err")
来源：http://ahm.yongpay.top

TS:   console.error("err")
来源：http://jpw.ywan-chungtsiang.top

Java: System.err.println("err")
来源：http://nmv.nanxuanxn.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pii.ydjk.org.cn

Ruby: warn "err"
来源：http://xwy.shanyushiyangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://gts.xuanzx.com

[M07] 判断是否为主入口
来源：http://ivd.cucudq.cn

Py:   if __name__ == "__main__":
来源：http://soy.9152youxi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wlc.yongpay.top

JS:   require.main === module
来源：http://ils.ctjpmb.com

TS:   require.main === module
来源：http://nxo.redwolf501.top

Java: public static void main(String[] args)
来源：http://ier.yueranfly.top

Go:   func main()
来源：http://yea.sysykeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zxz.yuanzhike.top

C#:   static void Main(string[] args)
来源：http://nfa.ppjwa.cn

[M08] 获取系统与运行时信息
来源：http://mcq.shuidangran.top

Py:   platform.system();  platform.python_version()
来源：http://dvf.svipenyu.cn

PHP:  PHP_OS;  phpversion();
来源：http://cta.sweek.top

JS:   process.platform;  process.version
来源：http://ihe.cheryme.top

TS:   process.platform;  process.version
来源：http://iin.sweek.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vhb.chenzaomai.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://iwf.tanke756.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jkg.zhaomingkeji.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://chn.zhaomingkeji.xyz

================================================================================
来源：http://agi.ctjpmb.com

N. 数据结构与算法
来源：http://lzq.redwolf501.top

================================================================================
来源：http://ohz.xinyue.icu

[N01] 二分查找（有序数组）
来源：http://abs.chenlongwang.top

Py:   bisect.bisect_left(arr, x)
来源：http://efz.hywenlv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hzp.xuetiantiany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lfo.feifeiyinyue.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jtx.jiagoushi.top

Java: Arrays.binarySearch(arr, x)
来源：http://mwz.feifeiyinyue.top

Go:   sort.SearchInts(arr, x)
来源：http://qoq.dashuyun.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bib.cashguo.top

C#:   Array.BinarySearch(arr, x)
来源：http://myo.0kj1m.cn

[N02] 排序（工程实践用内置实现）
来源：http://ucw.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://tij.bjfxy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://moo.mhx1999.top


<!-- 参考信息 -->
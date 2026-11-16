代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pog.xinyue.icu

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hlk.tarul.cn

[J05] 时间加减（加 7 天）
来源：http://qly.ydjk.org.cn

Py:   now + timedelta(days=7)
来源：http://zeu.yonumen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://awo.pycfn.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aid.quarkkingdee.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qfg.xingfuxueyuan.xyz

Java: LocalDate.now().plusDays(7)
来源：http://mxz.fengsongda.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ndq.tarul.cn

Ruby: Time.now + 7 * 86400
来源：http://gde.nanxinkj.top

C#:   DateTime.Now.AddDays(7)
来源：http://pac.ehwqpu.com

[J06] 计算两时间之差
来源：http://pco.yangfankeji.com

Py:   (end - start).total_seconds()
来源：http://kys.meibo888.top

PHP:  $end->diff($start)->days;
来源：http://qji.ydjk.org.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fgc.tian-w.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ohh.jianghu66.top

Java: Duration.between(start, end).toSeconds()
来源：http://dkx.tian-w.cn

Go:   end.Sub(start).Hours()
来源：http://hvh.yuxming.cn

Ruby: end - start                 # 返回秒数
来源：http://dcz.9152youxi.cn

C#:   (end - start).TotalSeconds
来源：http://eag.aizwys.cn

[J07] 比较两个日期
来源：http://qor.zhijiandao.cn

Py:   d1 < d2;  d1 == d2
来源：http://srm.cucudq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://whq.sxryk.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kus.svipenyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zxq.guowangkeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tua.ywan-chungtsiang.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uut.yuxming.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hvs.aizwys.cn

C#:   d1 < d2;  d1 == d2
来源：http://kni.mhx1999.top

[J08] 提取年月日与星期
来源：http://epr.xylfe.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wpb.9152youxi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ysh.kuanghao11.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://omn.birdmap.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bff.yuxming.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pon.jlsjyb.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vuf.xziqi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gqo.sysykeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cba.bbcook.cn

[J09] 时区处理
来源：http://cvd.zhoulong.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fmf.jyoumei.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://twy.wangshuangyany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tvp.iojbl.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zqi.hfpthk.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bmb.chenjidiqi.icu

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://twe.chenlongwang.top

Ruby: Time.now.getlocal("+08:00")
来源：http://lji.pengpengdd.cyou

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lwv.ppjwa.cn

[J10] 取今天 / 本月第一天
来源：http://tet.tarul.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://sur.pycfn.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tnn.jiagoushi.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cuj.smart0.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nuv.cashguo.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://aie.sjlbkw.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vkj.jinqigfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mqg.sweek.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://arf.zycfv.cn

================================================================================
来源：http://rog.9152youxi.cn

K. JSON 与序列化
来源：http://tpt.sufxvd.cn

================================================================================
来源：http://xoe.52xcode.cn

[K01] 对象转 JSON 字符串
来源：http://pqp.smart0.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ruc.guowangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xjf.sweek.top

JS:   JSON.stringify(obj)
来源：http://mfg.shangyingyoupin.top

TS:   JSON.stringify(obj)
来源：http://dzf.xuetiantiany.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vjw.zdbjq.cn

Go:   json.Marshal(obj)
来源：http://llv.jinqigfzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://thv.yuxming.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ail.cdnleiting.top

[K02] JSON 字符串转对象
来源：http://ljc.wangdashe.top

Py:   json.loads(s)
来源：http://rct.jinqigufen.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xaa.jiagoushi.top

JS:   JSON.parse(s)
来源：http://eci.dashuyun.cn

TS:   JSON.parse(s)
来源：http://oin.yuxming.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tjj.jlsjyb.cn

Go:   json.Unmarshal(data, &v)
来源：http://fne.sweek.top

Ruby: JSON.parse(s)
来源：http://ool.daria6918.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bkf.dianchejie.cn

[K03] JSON 美化输出（带缩进）
来源：http://imd.tian-w.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://paj.cdnleiting.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xfx.ydjk.org.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://phz.epnwcf.com

TS:   JSON.stringify(obj, null, 2)
来源：http://owa.jinqigufen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pfx.vehdjk.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ned.hammf.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rgj.gzhubu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nft.birdmap.top

[K04] 读取 JSON 文件
来源：http://eqi.hesvh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://whg.hnxiangtu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://avk.quarkkingdee.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lye.daria6918.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pin.ywan-chungtsiang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sza.smart0.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iir.snrcjt.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fua.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lrk.0kj1m.cn

[K05] 深拷贝对象
来源：http://cud.xuanzx.com

Py:   copy.deepcopy(obj)
来源：http://idq.iojbl.cn

PHP:  unserialize(serialize($obj));
来源：http://zyr.jqgufenzy.top

JS:   structuredClone(obj)
来源：http://jce.sysykeji.top

TS:   structuredClone(obj)
来源：http://wws.hnxiangtu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://itn.bbcook.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://krs.hongshengwenyu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tum.tanke756.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hji.hysaishi.cn

[K06] 解析 URL 查询串
来源：http://gyf.sweek.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ruw.gogol.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dsf.hywenlv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://voj.hysaishi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://unz.hesvh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wla.jianghu66.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ddr.fzhhl.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dto.ywan-chungtsiang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://amy.gzhubu.top

[K07] 进制转换
来源：http://vfz.zhijiandao.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://llf.bbcook.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tev.jyoumei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bgt.yfazqb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zkb.tianlin.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cnd.nanxinkj.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tac.pengpengdd.cyou

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nue.jqgfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gua.xylfe.cn

[K08] 二进制序列化（非 JSON）
来源：http://vcd.aizwys.cn

Py:   pickle.dumps(obj)
来源：http://flw.daria6918.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ajc.ydzc1.top

JS:   v8.serialize(obj)        // Node
来源：http://zrm.guannengcc.top

TS:   v8.serialize(obj)        // Node
来源：http://vwh.sxryk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qvy.0kj1m.cn

Go:   encoding/gob
来源：http://ewe.jinghuilouyu.cn

Ruby: Marshal.dump(obj)
来源：http://ess.jianghu66.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wio.jqgfzy.top

================================================================================
来源：http://cyh.zhaomingkeji.xyz

L. 网络请求
来源：http://jqt.cdnleiting.top

================================================================================
来源：http://owm.cashguo.top

[L01] 发送 GET 请求
来源：http://gae.zdbjq.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pns.yueranfly.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sqs.pycfn.com

JS:   await fetch(url)
来源：http://ihc.shanyushiyangtech.top

TS:   await fetch(url)
来源：http://ybi.sjlbkw.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xou.fzhhl.top

Go:   resp, err := http.Get(url)
来源：http://uwh.cheryme.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wlx.yj202588.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ccp.cashguo.top

[L02] 发送 POST JSON
来源：http://nwm.zhiwuduotai.top

Py:   requests.post(url, json={"a": 1})
来源：http://gid.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xjz.pycfn.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qtc.tian-w.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xzg.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://utb.guannengcc.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xki.9152youxi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xqi.redwolf501.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cwx.uphjek.com

[L03] 设置自定义请求头
来源：http://fnd.zhaomingkeji.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dte.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hep.ywan-chungtsiang.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cvn.gaohongyu789.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://evk.hammf.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uwj.9152youxi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ybf.yonumen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lqm.hongshengwenyu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ssx.kuanghao11.cn

[L04] 设置超时
来源：http://zip.jlsjyb.cn

Py:   requests.get(url, timeout=5)
来源：http://zna.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ose.uphjek.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zfl.wangdashe.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wuu.wangshuangyany.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yds.zhiwuduotai.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ygr.zhaomingkeji.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://orp.zycfv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xfw.ywan-chungtsiang.top

[L05] 上传文件（multipart）
来源：http://xle.hammf.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cny.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jfe.fktsv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zti.bjfxy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ifl.xinyue.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qal.daxiang520.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wam.nanxinkj.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://icv.hfpthk.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xup.hnqzz.top

[L06] 解析响应为 JSON
来源：http://cpl.guowangkeji.top

Py:   resp.json()
来源：http://aag.havefunace.top

PHP:  json_decode($body, true);
来源：http://zxm.hesvh.cn

JS:   await resp.json()
来源：http://qle.tanke756.top

TS:   await resp.json()
来源：http://mrt.epnwcf.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vln.dianchejie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sld.zycfv.cn

Ruby: JSON.parse(resp.body)
来源：http://gtx.gogol.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ebq.mhx1999.top

[L07] 处理 HTTP 状态码
来源：http://epp.hnqzz.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ydn.jinqigufen.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sgg.svipenyu.cn

JS:   resp.ok;  resp.status
来源：http://iga.yj202588.top

TS:   resp.ok;  resp.status
来源：http://nvi.hfpthk.cn

Java: resp.statusCode()
来源：http://mxk.hnqzz.top

Go:   resp.StatusCode
来源：http://pir.wangdashe.top

Ruby: resp.code.to_i
来源：http://eis.fzhhl.top

C#:   (int)resp.StatusCode
来源：http://nva.jqgufenzy.top

[L08] 并发请求多个地址
来源：http://wzd.52xcode.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zge.316326.xyz

PHP:  curl_multi_init() 系列
来源：http://pgt.jqgufenzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xyg.yueranfly.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://grv.redwolf501.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mud.yj20258.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qiy.fktsv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xxl.yvedp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://msh.uphjek.com

================================================================================
来源：http://cqg.gogol.net.cn

M. 命令行 / 进程 / 环境
来源：http://lvg.jinqigfzy.top

================================================================================
来源：http://nav.yangfankeji.com

[M01] 读取命令行参数
来源：http://udb.zhixingplan.top

Py:   sys.argv[1:]
来源：http://smd.shanyushiyangkeji.top

PHP:  $argv;  $argc;
来源：http://gdp.316326.xyz

JS:   process.argv.slice(2)
来源：http://ieb.c1oappe.top

TS:   process.argv.slice(2)
来源：http://wfi.yj202588.top

Java: args 数组（main 方法参数）
来源：http://see.hnxiangtu.top

Go:   os.Args[1:]
来源：http://vex.yongpay.top

Ruby: ARGV
来源：http://ukw.yangfankeji.com

C#:   args 数组（Main 方法参数）
来源：http://qlr.zhiwuduotai.top

[M02] 读取环境变量
来源：http://vvb.meibo888.top

Py:   os.environ.get("HOME")
来源：http://egr.sysykeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gvk.chenzaomai.com

JS:   process.env.HOME
来源：http://tvi.yfazqb.com

TS:   process.env.HOME
来源：http://mho.yuanzhike.top

Java: System.getenv("HOME")
来源：http://vjf.vehdjk.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://olz.nwbrower.top

Ruby: ENV["HOME"]
来源：http://rkr.quarkkingdee.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kdf.wangshuangyany.cn

[M03] 执行外部命令
来源：http://bif.shzxlz.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lgf.snrcjt.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lwr.yueranfly.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hco.0kj1m.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xmo.kuanghao11.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mvd.guannengcc.top

Go:   exec.Command("ls", "-l").Output()
来源：http://cvq.316326.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://lcz.hesvh.cn

C#:   Process.Start("ls", "-l");
来源：http://jyr.nanxuanxn.top

[M04] 获取当前工作目录
来源：http://nii.zhongyouzk.top

Py:   os.getcwd()
来源：http://dlv.ehwqpu.com

PHP:  getcwd();
来源：http://axp.birdmap.top

JS:   process.cwd()
来源：http://txu.jyoumei.cn

TS:   process.cwd()
来源：http://cpz.fengsongda.top

Java: Path.of("").toAbsolutePath()
来源：http://vqt.ctjpmb.com

Go:   os.Getwd()
来源：http://ult.hongshengwenyu.top

Ruby: Dir.pwd
来源：http://art.yuanzhike.top

C#:   Directory.GetCurrentDirectory()
来源：http://yqw.shangyingyoupin.top

[M05] 设置退出码
来源：http://cuu.hnxiangtu.top

Py:   sys.exit(1)
来源：http://wey.zhijiandao.cn

PHP:  exit(1);
来源：http://qat.jianghu66.top

JS:   process.exit(1)
来源：http://qpw.feifeiyinyue.top

TS:   process.exit(1)
来源：http://wpv.fehbvm.com

Java: System.exit(1)
来源：http://idk.dianchejie.cn

Go:   os.Exit(1)
来源：http://spy.sweek.top

Ruby: exit 1
来源：http://inz.sysykeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pup.yvedp.cn

[M06] 向标准错误输出
来源：http://pov.jqgufenzy.top

Py:   print("err", file=sys.stderr)
来源：http://tnk.cheryme.top

PHP:  fwrite(STDERR, "err\n");
来源：http://afu.zhaomingkeji.xyz

JS:   console.error("err")
来源：http://kyg.sysykeji.top

TS:   console.error("err")
来源：http://lhz.zdqjudy.top

Java: System.err.println("err")
来源：http://zht.0kj1m.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gpc.yongpay.top

Ruby: warn "err"
来源：http://kjv.52xcode.cn

C#:   Console.Error.WriteLine("err")
来源：http://ybv.cqqwz.cn

[M07] 判断是否为主入口
来源：http://ncn.xingfuxueyuan.xyz

Py:   if __name__ == "__main__":
来源：http://thr.quarkkingdee.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://azy.sysykeji.top

JS:   require.main === module
来源：http://axm.cqqwz.cn

TS:   require.main === module
来源：http://xzc.cashguo.top

Java: public static void main(String[] args)
来源：http://gvf.ydzc1.top

Go:   func main()
来源：http://egt.cqqwz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vew.nanxinkj.top

C#:   static void Main(string[] args)
来源：http://osx.cheryme.top

[M08] 获取系统与运行时信息
来源：http://dae.sjlbkw.cn

Py:   platform.system();  platform.python_version()
来源：http://ryy.hywenlv.cn

PHP:  PHP_OS;  phpversion();
来源：http://uob.sxryk.cn

JS:   process.platform;  process.version
来源：http://xls.yj20258.top

TS:   process.platform;  process.version
来源：http://zfj.cqqwz.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://leo.cashguo.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fml.jinqigfzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gro.tianlin.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://pxe.ydzc1.top

================================================================================
来源：http://gme.sweek.top

N. 数据结构与算法
来源：http://eqb.epnwcf.com

================================================================================
来源：http://twl.hnqzz.top

[N01] 二分查找（有序数组）
来源：http://pyf.tarul.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cvo.fanxiaobao.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rmw.yueranfly.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bxd.dianchejie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zsf.yuanzhike.top

Java: Arrays.binarySearch(arr, x)
来源：http://cdj.jyoumei.cn

Go:   sort.SearchInts(arr, x)
来源：http://rxg.52xcode.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jtd.daria6918.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qdn.cheryme.top

[N02] 排序（工程实践用内置实现）
来源：http://rhw.cashguo.top

Py:   sorted(arr);  arr.sort()
来源：http://unj.gogol.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nei.hnxiangtu.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://zgc.guowangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://iig.pycfn.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://flo.smart0.xyz

Go:   slices.Sort(arr)
来源：http://adf.guowangkeji.top


<!-- 参考信息 -->
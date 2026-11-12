代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nic.dianchejie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://btb.ydzc1.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cof.hfpthk.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xtv.yuxming.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jau.sysykeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xcu.zhaomingkeji.xyz

[J05] 时间加减（加 7 天）
来源：http://pjo.sxryk.cn

Py:   now + timedelta(days=7)
来源：http://wqg.yfazqb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://qkp.vehdjk.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://roc.ivvv.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dci.hnxiangtu.top

Java: LocalDate.now().plusDays(7)
来源：http://ybx.epnwcf.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jqa.epnwcf.com

Ruby: Time.now + 7 * 86400
来源：http://jmd.jianghu66.top

C#:   DateTime.Now.AddDays(7)
来源：http://hog.zhijiandao.cn

[J06] 计算两时间之差
来源：http://alu.dashuyun.cn

Py:   (end - start).total_seconds()
来源：http://zii.epnwcf.com

PHP:  $end->diff($start)->days;
来源：http://pqm.yuxming.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fgu.xingfuxueyuan.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xdj.shuidangran.top

Java: Duration.between(start, end).toSeconds()
来源：http://kmi.cashguo.top

Go:   end.Sub(start).Hours()
来源：http://xtz.sjlbkw.cn

Ruby: end - start                 # 返回秒数
来源：http://wth.xuetiantiany.cn

C#:   (end - start).TotalSeconds
来源：http://uyf.hnxiangtu.top

[J07] 比较两个日期
来源：http://zbb.gogol.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://qlb.aizwys.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://llj.daria6918.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mgm.smart0.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://csg.havefunace.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vaz.yueranfly.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://htm.sysykeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://oew.zhiwuduotai.top

C#:   d1 < d2;  d1 == d2
来源：http://xge.ppjwa.cn

[J08] 提取年月日与星期
来源：http://vzl.fanxiaobao.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://osi.tianlin.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mac.ywan-chungtsiang.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yhd.nanxinkj.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://utx.hcnkem.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bia.shangyingyoupin.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://urd.pengpengdd.cyou

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zmf.hammf.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sbc.ydzc1.top

[J09] 时区处理
来源：http://vpa.gogol.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://itk.hnqzz.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ceg.tarul.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uzn.ctjpmb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qrd.zdbjq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://chg.redwolf501.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bym.pengpengdd.cyou

Ruby: Time.now.getlocal("+08:00")
来源：http://opt.ydzc1.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hla.wangshuangyany.cn

[J10] 取今天 / 本月第一天
来源：http://fnb.hnxiangtu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://erv.fehbvm.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pim.sysykeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xzz.fktsv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yez.yuanzhike.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://aci.c1oappe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wqq.mhx1999.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rmu.epnwcf.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://emc.shzxlz.cn

================================================================================
来源：http://wio.0kj1m.cn

K. JSON 与序列化
来源：http://yhm.jyoumei.cn

================================================================================
来源：http://yqf.aibaodan.cn

[K01] 对象转 JSON 字符串
来源：http://ypb.jiagoushi.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://agh.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fol.tianlin.xyz

JS:   JSON.stringify(obj)
来源：http://chs.nwbrower.top

TS:   JSON.stringify(obj)
来源：http://zis.hnxiangtu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pma.feifeiyinyue.top

Go:   json.Marshal(obj)
来源：http://jeq.hnqzz.top

Ruby: obj.to_json                                     // require "json"
来源：http://qqw.zycfv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://foj.hcnkem.com

[K02] JSON 字符串转对象
来源：http://nnt.nanxuanxn.top

Py:   json.loads(s)
来源：http://vjm.hcnkem.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bpb.yj20258.top

JS:   JSON.parse(s)
来源：http://bsp.cdnleiting.top

TS:   JSON.parse(s)
来源：http://xjs.yuanzhike.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://leh.jinyuanbaomall.cn

Go:   json.Unmarshal(data, &v)
来源：http://drj.ywan-chungtsiang.top

Ruby: JSON.parse(s)
来源：http://ssm.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://adk.epnwcf.com

[K03] JSON 美化输出（带缩进）
来源：http://acq.jinyuanbaomall.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blp.hnqzz.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lmr.guannengcc.top

JS:   JSON.stringify(obj, null, 2)
来源：http://uha.jqgfzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://sjn.jqgfzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rij.ppjwa.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fwk.gaohongyu789.top

Ruby: JSON.pretty_generate(obj)
来源：http://xwt.dianchejie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lts.daxiang520.top

[K04] 读取 JSON 文件
来源：http://iih.zhixingplan.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cde.fehbvm.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://spy.ehwqpu.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nqh.xylfe.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gdf.chenlongwang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dgq.zhaomingkeji.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bqs.hammf.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://cvv.gaohongyu789.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fml.9152youxi.cn

[K05] 深拷贝对象
来源：http://bsx.hongshengwenyu.top

Py:   copy.deepcopy(obj)
来源：http://gvg.ehwqpu.com

PHP:  unserialize(serialize($obj));
来源：http://jwi.zhoulong.xyz

JS:   structuredClone(obj)
来源：http://bft.gzhubu.top

TS:   structuredClone(obj)
来源：http://jkg.hnqzz.top

Java: // 手写拷贝构造，或序列化往返
来源：http://nqv.fzhhl.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kan.shzxlz.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://aqp.gzhubu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://era.daria6918.cn

[K06] 解析 URL 查询串
来源：http://nix.chenjidiqi.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ezs.xinyue.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://edv.ybcxt.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jho.jinyuanbaomall.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wke.hnqzz.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sud.tarul.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hdp.shanyushiyangtech.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vdx.wangshuangyany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ldo.fanxiaobao.xyz

[K07] 进制转换
来源：http://fsd.jinqigufen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oho.316326.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sug.sjlbkw.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hkk.hongshengwenyu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://emv.fengsongda.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://anj.daxiang520.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://evd.redwolf501.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://iik.pycfn.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rzv.birdmap.top

[K08] 二进制序列化（非 JSON）
来源：http://zpt.mhx1999.top

Py:   pickle.dumps(obj)
来源：http://bpv.wangdashe.top

PHP:  serialize($obj);  unserialize($s);
来源：http://urg.0kj1m.cn

JS:   v8.serialize(obj)        // Node
来源：http://rwm.pengpengdd.cyou

TS:   v8.serialize(obj)        // Node
来源：http://qtx.pycfn.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dlr.yanxiufei.cn

Go:   encoding/gob
来源：http://otz.tarul.cn

Ruby: Marshal.dump(obj)
来源：http://hri.zdqjudy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zbo.meibo888.top

================================================================================
来源：http://mkq.uphjek.com

L. 网络请求
来源：http://qvz.vehdjk.com

================================================================================
来源：http://fyx.fehbvm.com

[L01] 发送 GET 请求
来源：http://cqm.daria6918.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lfk.shuidangran.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vfa.hammf.cn

JS:   await fetch(url)
来源：http://kjt.cqqwz.cn

TS:   await fetch(url)
来源：http://lxp.jinqigfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tzu.smart0.xyz

Go:   resp, err := http.Get(url)
来源：http://mna.shanyushiyangtech.top

Ruby: Net::HTTP.get(URI(url))
来源：http://xfv.bbcook.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dvc.vqdsnc.cn

[L02] 发送 POST JSON
来源：http://jxg.daria6918.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ruj.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dvp.havefunace.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vgw.zhiwuduotai.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uai.hcnkem.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ouu.zhongyouzk.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blz.xuanzx.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xyc.ydzc1.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lzt.xylfe.cn

[L03] 设置自定义请求头
来源：http://kag.xziqi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tdm.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bkk.yvedp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wws.sjlbkw.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bju.daria6918.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rye.xinyue.icu

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ogu.jinyuanbaomall.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kvb.zhijiandao.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wqh.yj20258888.top

[L04] 设置超时
来源：http://shi.andypj.xyz

Py:   requests.get(url, timeout=5)
来源：http://fro.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ujv.aibaodan.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iff.hnqzz.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rge.0kj1m.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://abe.yangfankeji.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://goe.mhx1999.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://eny.dianchejie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ifp.pycfn.com

[L05] 上传文件（multipart）
来源：http://lvl.guowangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://snk.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yzu.xuetiantiany.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jjj.hongshengwenyu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fey.smart0.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wjv.tanke756.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gmf.yonumen.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://txg.guowangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tha.ivvv.top

[L06] 解析响应为 JSON
来源：http://nlh.shuidangran.top

Py:   resp.json()
来源：http://lcr.yonumen.top

PHP:  json_decode($body, true);
来源：http://ecn.jlsjyb.cn

JS:   await resp.json()
来源：http://ajn.guannengcc.top

TS:   await resp.json()
来源：http://gel.guannengcc.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rup.c1oappe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yjj.tianlin.xyz

Ruby: JSON.parse(resp.body)
来源：http://nos.jinqigfzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jep.0kj1m.cn

[L07] 处理 HTTP 状态码
来源：http://ila.jyoumei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ofo.zhengqikj.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qcr.dianchejie.cn

JS:   resp.ok;  resp.status
来源：http://tjl.zdqjudy.top

TS:   resp.ok;  resp.status
来源：http://xez.ppjwa.cn

Java: resp.statusCode()
来源：http://qal.guowangkeji.top

Go:   resp.StatusCode
来源：http://efu.hysaishi.cn

Ruby: resp.code.to_i
来源：http://gei.chenzaomai.com

C#:   (int)resp.StatusCode
来源：http://xbz.xuanzx.com

[L08] 并发请求多个地址
来源：http://cmk.jiagoushi.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pze.xingfuxueyuan.xyz

PHP:  curl_multi_init() 系列
来源：http://jqa.yuanzhike.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lyf.yj202588.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jkx.jinghuilouyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zpi.hnqzz.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://soi.tarul.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gec.guannengcc.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://opa.vqdsnc.cn

================================================================================
来源：http://abf.chenlongwang.top

M. 命令行 / 进程 / 环境
来源：http://qqd.zhijiandao.cn

================================================================================
来源：http://blo.yvedp.cn

[M01] 读取命令行参数
来源：http://dhi.havefunace.top

Py:   sys.argv[1:]
来源：http://sfm.guannengcc.top

PHP:  $argv;  $argc;
来源：http://emq.ctjpmb.com

JS:   process.argv.slice(2)
来源：http://mcm.snrcjt.cn

TS:   process.argv.slice(2)
来源：http://dqb.wangdashe.top

Java: args 数组（main 方法参数）
来源：http://hcq.shuidangran.top

Go:   os.Args[1:]
来源：http://rgm.gzhubu.top

Ruby: ARGV
来源：http://oui.meibo888.top

C#:   args 数组（Main 方法参数）
来源：http://jnh.cdnleiting.top

[M02] 读取环境变量
来源：http://upo.xuanzx.com

Py:   os.environ.get("HOME")
来源：http://odk.tanke756.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xzt.snrcjt.cn

JS:   process.env.HOME
来源：http://vwh.gaohongyu789.top

TS:   process.env.HOME
来源：http://bbs.uphjek.com

Java: System.getenv("HOME")
来源：http://qkd.zhiwuduotai.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://syj.tanke756.top

Ruby: ENV["HOME"]
来源：http://hix.yj20258888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ufz.ehwqpu.com

[M03] 执行外部命令
来源：http://qrz.hcnkem.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qvg.epnwcf.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tss.tanke756.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ptq.yangfankeji.com

TS:   child_process.execSync("ls -l").toString()
来源：http://skt.shangyingyoupin.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://adk.jqgfzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ppw.fehbvm.com

Ruby: system("ls -l");  `ls -l`
来源：http://gxb.redwolf501.top

C#:   Process.Start("ls", "-l");
来源：http://xmw.xziqi.cn

[M04] 获取当前工作目录
来源：http://etq.nwbrower.top

Py:   os.getcwd()
来源：http://met.jiagoushi.top

PHP:  getcwd();
来源：http://gwq.zdbjq.cn

JS:   process.cwd()
来源：http://akg.daxiang520.top

TS:   process.cwd()
来源：http://oco.9152youxi.cn

Java: Path.of("").toAbsolutePath()
来源：http://hmj.pycfn.com

Go:   os.Getwd()
来源：http://atf.xuanzx.com

Ruby: Dir.pwd
来源：http://hlx.shanyushiyangtech.top

C#:   Directory.GetCurrentDirectory()
来源：http://bxh.gzhubu.top

[M05] 设置退出码
来源：http://btl.316326.xyz

Py:   sys.exit(1)
来源：http://swz.guowangkeji.top

PHP:  exit(1);
来源：http://cgw.hammf.cn

JS:   process.exit(1)
来源：http://kay.xuetiantiany.cn

TS:   process.exit(1)
来源：http://xwd.jiagoushi.top

Java: System.exit(1)
来源：http://mdc.zhongyouzk.top

Go:   os.Exit(1)
来源：http://vzz.snrcjt.cn

Ruby: exit 1
来源：http://fmq.cheryme.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gnw.52xcode.cn

[M06] 向标准错误输出
来源：http://vyr.jqgfzy.top

Py:   print("err", file=sys.stderr)
来源：http://zoe.jyoumei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qdi.birdmap.top

JS:   console.error("err")
来源：http://jqa.xuetiantiany.cn

TS:   console.error("err")
来源：http://qkz.xingfuxueyuan.xyz

Java: System.err.println("err")
来源：http://xcu.vehdjk.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bky.pengpengdd.cyou

Ruby: warn "err"
来源：http://jir.hesvh.cn

C#:   Console.Error.WriteLine("err")
来源：http://aoi.zhixingplan.top

[M07] 判断是否为主入口
来源：http://epx.haohaochexian.top

Py:   if __name__ == "__main__":
来源：http://sug.bjfxy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dzm.ywan-chungtsiang.top

JS:   require.main === module
来源：http://sqn.fengsongda.top

TS:   require.main === module
来源：http://iap.hywenlv.cn

Java: public static void main(String[] args)
来源：http://edn.snrcjt.cn

Go:   func main()
来源：http://mzf.jqgufenzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://suy.pengpengdd.cyou

C#:   static void Main(string[] args)
来源：http://naa.ywan-chungtsiang.top

[M08] 获取系统与运行时信息
来源：http://kxj.zhoulong.xyz

Py:   platform.system();  platform.python_version()
来源：http://ual.xylfe.cn

PHP:  PHP_OS;  phpversion();
来源：http://hyi.hnqzz.top

JS:   process.platform;  process.version
来源：http://niq.hammf.cn

TS:   process.platform;  process.version
来源：http://nfe.zhongyouzk.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dzd.zycfv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://seq.316326.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ded.yuxming.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://alw.zhengqikj.top

================================================================================
来源：http://aeu.jinyuanbaomall.cn

N. 数据结构与算法
来源：http://xck.snrcjt.cn

================================================================================
来源：http://ruk.jlsjyb.cn

[N01] 二分查找（有序数组）
来源：http://sjm.zhijiandao.cn

Py:   bisect.bisect_left(arr, x)
来源：http://uim.yongpay.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kfp.vqdsnc.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qec.yuanzhike.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uht.pycfn.com

Java: Arrays.binarySearch(arr, x)
来源：http://xko.fanxiaobao.xyz

Go:   sort.SearchInts(arr, x)
来源：http://cpe.9152youxi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cax.gotoacloud.top

C#:   Array.BinarySearch(arr, x)
来源：http://ade.vqdsnc.cn

[N02] 排序（工程实践用内置实现）
来源：http://dvn.fzhhl.top

Py:   sorted(arr);  arr.sort()
来源：http://idb.wangshuangyany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xhv.zhongyouzk.top


<!-- 参考信息 -->
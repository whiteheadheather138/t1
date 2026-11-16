代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://slf.hammf.cn

[J04] 时间戳与日期互转
来源：http://zce.cucudq.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xsr.yuanzhike.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xob.havefunace.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qug.yvedp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ulu.pycfn.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://euf.zhaomingkeji.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kte.daxiang520.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hrg.fehbvm.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lyf.uphjek.com

[J05] 时间加减（加 7 天）
来源：http://nkr.jianghu66.top

Py:   now + timedelta(days=7)
来源：http://vli.zhengqikj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://lzc.jyoumei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cnf.yongpay.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jhr.tanke756.top

Java: LocalDate.now().plusDays(7)
来源：http://utz.tianlin.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ooa.hammf.cn

Ruby: Time.now + 7 * 86400
来源：http://jdo.shangyingyoupin.top

C#:   DateTime.Now.AddDays(7)
来源：http://ssm.fktsv.cn

[J06] 计算两时间之差
来源：http://lxp.yvedp.cn

Py:   (end - start).total_seconds()
来源：http://bbz.ydzc1.top

PHP:  $end->diff($start)->days;
来源：http://zos.316326.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kvi.zhaomingkeji.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hjj.zhaomingkeji.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://aaz.jinyuanbaomall.cn

Go:   end.Sub(start).Hours()
来源：http://gsq.0kj1m.cn

Ruby: end - start                 # 返回秒数
来源：http://tml.pengpengdd.cyou

C#:   (end - start).TotalSeconds
来源：http://bec.cucudq.cn

[J07] 比较两个日期
来源：http://mje.ppjwa.cn

Py:   d1 < d2;  d1 == d2
来源：http://znm.zhiwuduotai.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pdm.wangshuangyany.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fpz.0kj1m.cn

TS:   d1.getTime() < d2.getTime()
来源：http://adx.andypj.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uao.haohaochexian.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://udo.jinyuanbaomall.cn

Ruby: d1 < d2;  d1 == d2
来源：http://uwf.zdqjudy.top

C#:   d1 < d2;  d1 == d2
来源：http://ryx.jinqigfzy.top

[J08] 提取年月日与星期
来源：http://hyx.chenlongwang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kno.sweek.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tkj.ivvv.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lrs.epnwcf.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hqj.jqgufenzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rgw.dianchejie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sfd.gogol.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uow.hfpthk.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://knt.fehbvm.com

[J09] 时区处理
来源：http://ndl.shzxlz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tzr.haohaochexian.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://spo.feifeiyinyue.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qfe.bbcook.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pie.meibo888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zfa.daria6918.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tdc.andypj.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://ahn.jqgfzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jwr.ydjk.org.cn

[J10] 取今天 / 本月第一天
来源：http://tlv.yuxming.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ylo.daria6918.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cop.jianghu66.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fsl.xziqi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://feg.hongshengwenyu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yaz.vqdsnc.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qgd.ctjpmb.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xcm.xinyue.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qam.wangshuangyany.cn

================================================================================
来源：http://ryv.jiagoushi.top

K. JSON 与序列化
来源：http://fei.fehbvm.com

================================================================================
来源：http://pbv.jinyuanbaomall.cn

[K01] 对象转 JSON 字符串
来源：http://ggk.bbcook.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://btr.hnxiangtu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ppf.316326.xyz

JS:   JSON.stringify(obj)
来源：http://wyf.ydjk.org.cn

TS:   JSON.stringify(obj)
来源：http://rvh.andypj.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ipy.yonumen.top

Go:   json.Marshal(obj)
来源：http://nsx.ybcxt.top

Ruby: obj.to_json                                     // require "json"
来源：http://sbw.ehwqpu.com

C#:   JsonSerializer.Serialize(obj)
来源：http://xpx.chenjidiqi.icu

[K02] JSON 字符串转对象
来源：http://bjz.xuetiantiany.cn

Py:   json.loads(s)
来源：http://ywh.ppjwa.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fpe.jqgufenzy.top

JS:   JSON.parse(s)
来源：http://nse.jyoumei.cn

TS:   JSON.parse(s)
来源：http://wth.hfpthk.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mve.gotoacloud.top

Go:   json.Unmarshal(data, &v)
来源：http://nrb.daxiang520.top

Ruby: JSON.parse(s)
来源：http://pig.ydjk.org.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ymw.jiagoushi.top

[K03] JSON 美化输出（带缩进）
来源：http://tet.cheryme.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bnx.fzhhl.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dhb.xylfe.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://eyu.nwbrower.top

TS:   JSON.stringify(obj, null, 2)
来源：http://net.ivvv.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://stq.shzxlz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bfc.shzxlz.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bnl.zdbjq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xyw.hesvh.cn

[K04] 读取 JSON 文件
来源：http://kez.tarul.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oss.jiagoushi.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bgh.bbcook.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gil.fengsongda.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sbt.jinyuanbaomall.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pdp.aibaodan.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zgd.zhengqikj.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://wlb.ctjpmb.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://adb.hesvh.cn

[K05] 深拷贝对象
来源：http://ent.wangdashe.top

Py:   copy.deepcopy(obj)
来源：http://gdg.jianghu66.top

PHP:  unserialize(serialize($obj));
来源：http://agc.fanxiaobao.xyz

JS:   structuredClone(obj)
来源：http://gns.gaohongyu789.top

TS:   structuredClone(obj)
来源：http://iug.daxiang520.top

Java: // 手写拷贝构造，或序列化往返
来源：http://xce.andypj.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rxl.svipenyu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jwi.ctjpmb.com

C#:   // 序列化往返，或自定义 Clone
来源：http://whm.zhixingplan.top

[K06] 解析 URL 查询串
来源：http://fbw.jqgufenzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gvh.pengpengdd.cyou

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zmc.xinyue.icu

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qyn.wangshuangyany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ytj.aibaodan.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qgi.vqdsnc.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wvl.pycfn.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ymu.nwbrower.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vaa.cashguo.top

[K07] 进制转换
来源：http://sdo.jqgufenzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vwv.daxiang520.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hzh.zhongyouzk.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fon.ydzc1.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zfl.shanyushiyangkeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qod.hongshengwenyu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nor.hesvh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bye.ydjk.org.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ubi.yj202588.top

[K08] 二进制序列化（非 JSON）
来源：http://lof.zdbjq.cn

Py:   pickle.dumps(obj)
来源：http://xaw.feifeiyinyue.top

PHP:  serialize($obj);  unserialize($s);
来源：http://lbu.haohaochexian.top

JS:   v8.serialize(obj)        // Node
来源：http://wll.9152youxi.cn

TS:   v8.serialize(obj)        // Node
来源：http://usa.iojbl.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zsh.yonumen.top

Go:   encoding/gob
来源：http://rpq.cqqwz.cn

Ruby: Marshal.dump(obj)
来源：http://ens.jqgufenzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xvr.tian-w.cn

================================================================================
来源：http://dgw.jinqigfzy.top

L. 网络请求
来源：http://blo.chenlongwang.top

================================================================================
来源：http://jvr.gaohongyu789.top

[L01] 发送 GET 请求
来源：http://fpr.cdnleiting.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ely.xuetiantiany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oex.hnqzz.top

JS:   await fetch(url)
来源：http://dpw.0kj1m.cn

TS:   await fetch(url)
来源：http://pod.smart0.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bve.fktsv.cn

Go:   resp, err := http.Get(url)
来源：http://xxi.yanxiufei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://asi.xylfe.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wmf.bbcook.cn

[L02] 发送 POST JSON
来源：http://ddw.jlsjyb.cn

Py:   requests.post(url, json={"a": 1})
来源：http://svk.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zpv.zhixingplan.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jwq.ydzc1.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qtd.hammf.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vju.zycfv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cyi.zhaomingkeji.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hpz.zhixingplan.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hdr.yuxming.cn

[L03] 设置自定义请求头
来源：http://psg.bjfxy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tbr.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jeq.ydjk.org.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cwm.cqqwz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://spy.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pbz.fehbvm.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://oxs.yanxiufei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jql.shzxlz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vlm.nwbrower.top

[L04] 设置超时
来源：http://xcn.sxryk.cn

Py:   requests.get(url, timeout=5)
来源：http://wdo.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mlf.dianchejie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nhb.jqgfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uur.tian-w.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xmx.xuanzx.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ion.sysykeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lpz.cdnleiting.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://txg.zhixingplan.top

[L05] 上传文件（multipart）
来源：http://oan.daxiang520.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xvr.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vls.vehdjk.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://amr.birdmap.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gow.ppjwa.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pkc.tianlin.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sxb.haohaochexian.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sno.xingfuxueyuan.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://geb.pengpengdd.cyou

[L06] 解析响应为 JSON
来源：http://zqm.wangdashe.top

Py:   resp.json()
来源：http://nja.xuetiantiany.cn

PHP:  json_decode($body, true);
来源：http://kws.shanyushiyangkeji.top

JS:   await resp.json()
来源：http://byn.316326.xyz

TS:   await resp.json()
来源：http://cdr.redwolf501.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://emu.pycfn.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://csa.pycfn.com

Ruby: JSON.parse(resp.body)
来源：http://eqo.hywenlv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://epc.fanxiaobao.xyz

[L07] 处理 HTTP 状态码
来源：http://fuo.jiagoushi.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://whk.gogol.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wyf.zhixingplan.top

JS:   resp.ok;  resp.status
来源：http://ksk.chenjidiqi.icu

TS:   resp.ok;  resp.status
来源：http://zya.yj20258.top

Java: resp.statusCode()
来源：http://svs.xingfuxueyuan.xyz

Go:   resp.StatusCode
来源：http://gdv.zdbjq.cn

Ruby: resp.code.to_i
来源：http://qzf.yanxiufei.cn

C#:   (int)resp.StatusCode
来源：http://qul.quarkkingdee.top

[L08] 并发请求多个地址
来源：http://sqo.ydzc1.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hqk.ivvv.top

PHP:  curl_multi_init() 系列
来源：http://vsi.zhiwuduotai.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://okm.yanxiufei.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yue.wangdashe.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vrc.hesvh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://osz.sjlbkw.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zwd.fengsongda.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qgu.jinghuilouyu.cn

================================================================================
来源：http://mfu.jqgfzy.top

M. 命令行 / 进程 / 环境
来源：http://omz.yj202588.top

================================================================================
来源：http://tut.nwbrower.top

[M01] 读取命令行参数
来源：http://pbw.hcnkem.com

Py:   sys.argv[1:]
来源：http://nrd.52xcode.cn

PHP:  $argv;  $argc;
来源：http://dos.yuanzhike.top

JS:   process.argv.slice(2)
来源：http://voz.ydzc1.top

TS:   process.argv.slice(2)
来源：http://mbe.feifeiyinyue.top

Java: args 数组（main 方法参数）
来源：http://omx.fengsongda.top

Go:   os.Args[1:]
来源：http://dtt.tanke756.top

Ruby: ARGV
来源：http://qqx.dianchejie.cn

C#:   args 数组（Main 方法参数）
来源：http://fwm.zhengqikj.top

[M02] 读取环境变量
来源：http://jmb.jqgfzy.top

Py:   os.environ.get("HOME")
来源：http://api.snrcjt.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ely.0kj1m.cn

JS:   process.env.HOME
来源：http://die.gogol.net.cn

TS:   process.env.HOME
来源：http://dkg.havefunace.top

Java: System.getenv("HOME")
来源：http://leg.cqqwz.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://izk.yonumen.top

Ruby: ENV["HOME"]
来源：http://uwu.ivvv.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ask.zdbjq.cn

[M03] 执行外部命令
来源：http://nlh.xylfe.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://onl.jyoumei.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wmn.zhixingplan.top

JS:   child_process.execSync("ls -l").toString()
来源：http://smq.meibo888.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cvu.gotoacloud.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gph.hysaishi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ptj.zdbjq.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wwz.zhixingplan.top

C#:   Process.Start("ls", "-l");
来源：http://wam.wangshuangyany.cn

[M04] 获取当前工作目录
来源：http://tdw.yueranfly.top

Py:   os.getcwd()
来源：http://rtt.jqgfzy.top

PHP:  getcwd();
来源：http://vwy.yangfankeji.com

JS:   process.cwd()
来源：http://bkw.meibo888.top

TS:   process.cwd()
来源：http://ort.hesvh.cn

Java: Path.of("").toAbsolutePath()
来源：http://tdc.yanxiufei.cn

Go:   os.Getwd()
来源：http://zpq.guowangkeji.top

Ruby: Dir.pwd
来源：http://geu.fzhhl.top

C#:   Directory.GetCurrentDirectory()
来源：http://all.zhaomingkeji.xyz

[M05] 设置退出码
来源：http://kqb.iojbl.cn

Py:   sys.exit(1)
来源：http://lts.sxryk.cn

PHP:  exit(1);
来源：http://yui.hnqzz.top

JS:   process.exit(1)
来源：http://qxl.snrcjt.cn

TS:   process.exit(1)
来源：http://pny.tarul.cn

Java: System.exit(1)
来源：http://oma.shanyushiyangtech.top

Go:   os.Exit(1)
来源：http://mtx.nanxinkj.top

Ruby: exit 1
来源：http://msa.zhoulong.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fxu.jqgufenzy.top

[M06] 向标准错误输出
来源：http://xur.xylfe.cn

Py:   print("err", file=sys.stderr)
来源：http://yjt.jqgufenzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://coj.wangshuangyany.cn

JS:   console.error("err")
来源：http://abi.yonumen.top

TS:   console.error("err")
来源：http://sds.zhoulong.xyz

Java: System.err.println("err")
来源：http://jli.pengpengdd.cyou

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://iav.zhiwuduotai.top

Ruby: warn "err"
来源：http://yag.xuanzx.com

C#:   Console.Error.WriteLine("err")
来源：http://gqw.zdqjudy.top

[M07] 判断是否为主入口
来源：http://hlz.daxiang520.top

Py:   if __name__ == "__main__":
来源：http://ybs.jinyuanbaomall.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mtf.c1oappe.top

JS:   require.main === module
来源：http://vhn.yuxming.cn

TS:   require.main === module
来源：http://qmg.gzhubu.top

Java: public static void main(String[] args)
来源：http://ubs.dianchejie.cn

Go:   func main()
来源：http://rsl.bbcook.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xgm.epnwcf.com

C#:   static void Main(string[] args)
来源：http://aek.guannengcc.top

[M08] 获取系统与运行时信息
来源：http://oxk.yj202588.top

Py:   platform.system();  platform.python_version()
来源：http://gam.feifeiyinyue.top

PHP:  PHP_OS;  phpversion();
来源：http://srf.chenzaomai.com

JS:   process.platform;  process.version
来源：http://gke.tianlin.xyz

TS:   process.platform;  process.version
来源：http://vbc.yvedp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fry.xinyue.icu

Go:   runtime.GOOS;  runtime.Version()
来源：http://wjd.shuidangran.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://amk.snrcjt.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://edn.andypj.xyz

================================================================================
来源：http://vtt.birdmap.top

N. 数据结构与算法
来源：http://zwo.hcnkem.com

================================================================================
来源：http://yns.c1oappe.top

[N01] 二分查找（有序数组）
来源：http://lyx.zhongyouzk.top

Py:   bisect.bisect_left(arr, x)
来源：http://hlz.zhongyouzk.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nma.ywan-chungtsiang.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zho.zhongyouzk.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jnc.birdmap.top

Java: Arrays.binarySearch(arr, x)
来源：http://xhc.tian-w.cn

Go:   sort.SearchInts(arr, x)
来源：http://vxp.hesvh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gtm.zhijiandao.cn


<!-- 参考信息 -->
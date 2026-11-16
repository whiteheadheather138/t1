代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mgx.yueranfly.top

TS:   Math.floor(Date.now() / 1000)
来源：http://dje.yvedp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jmq.c1oappe.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cpa.ydzc1.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://abn.cucudq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ohc.zhiwuduotai.top

[J05] 时间加减（加 7 天）
来源：http://dcy.dianchejie.cn

Py:   now + timedelta(days=7)
来源：http://hrp.hysaishi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sqz.yuxming.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vya.jinqigfzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zdq.chenlongwang.top

Java: LocalDate.now().plusDays(7)
来源：http://zvp.jyoumei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://anx.redwolf501.top

Ruby: Time.now + 7 * 86400
来源：http://nlc.jqgufenzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://wqh.fzhhl.top

[J06] 计算两时间之差
来源：http://ryl.yj202588.top

Py:   (end - start).total_seconds()
来源：http://ouc.shanyushiyangtech.top

PHP:  $end->diff($start)->days;
来源：http://nfi.jyoumei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sbk.jqgufenzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://imi.ivvv.top

Java: Duration.between(start, end).toSeconds()
来源：http://hpw.nwbrower.top

Go:   end.Sub(start).Hours()
来源：http://atg.xingfuxueyuan.xyz

Ruby: end - start                 # 返回秒数
来源：http://huf.9152youxi.cn

C#:   (end - start).TotalSeconds
来源：http://nzh.bjfxy.top

[J07] 比较两个日期
来源：http://hin.hammf.cn

Py:   d1 < d2;  d1 == d2
来源：http://cpc.hnxiangtu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://umv.aizwys.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dxo.chenjidiqi.icu

TS:   d1.getTime() < d2.getTime()
来源：http://eql.fanxiaobao.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jrv.epnwcf.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qah.zhaomingkeji.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://hxy.52xcode.cn

C#:   d1 < d2;  d1 == d2
来源：http://iqu.jqgufenzy.top

[J08] 提取年月日与星期
来源：http://nrg.yuxming.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mkm.dianchejie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xhk.vehdjk.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://avd.uphjek.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zta.meibo888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bqm.dianchejie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jta.fktsv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bwk.316326.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gno.ywan-chungtsiang.top

[J09] 时区处理
来源：http://yyl.gogol.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rja.tarul.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yhn.52xcode.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kcs.dashuyun.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://amj.hywenlv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mik.xuanzx.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bsv.pycfn.com

Ruby: Time.now.getlocal("+08:00")
来源：http://ulf.xylfe.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uyf.xylfe.cn

[J10] 取今天 / 本月第一天
来源：http://ulu.sweek.top

Py:   date.today();  date.today().replace(day=1)
来源：http://aso.jyoumei.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cod.jqgfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pxp.zhijiandao.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gwh.daxiang520.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://int.sysykeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rtz.jlsjyb.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sgo.ehwqpu.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wlr.ctjpmb.com

================================================================================
来源：http://gsn.nanxinkj.top

K. JSON 与序列化
来源：http://khn.jinyuanbaomall.cn

================================================================================
来源：http://wev.yfazqb.com

[K01] 对象转 JSON 字符串
来源：http://vbe.guowangkeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zdd.ybcxt.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://evj.chenlongwang.top

JS:   JSON.stringify(obj)
来源：http://sxu.gzhubu.top

TS:   JSON.stringify(obj)
来源：http://inf.zhaomingkeji.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://okd.yuanzhike.top

Go:   json.Marshal(obj)
来源：http://uxi.zhixingplan.top

Ruby: obj.to_json                                     // require "json"
来源：http://xnf.sufxvd.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://spc.chenjidiqi.icu

[K02] JSON 字符串转对象
来源：http://ruw.snrcjt.cn

Py:   json.loads(s)
来源：http://npn.yj202588.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kpg.cucudq.cn

JS:   JSON.parse(s)
来源：http://vbe.smart0.xyz

TS:   JSON.parse(s)
来源：http://peu.ydzc1.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vnn.snrcjt.cn

Go:   json.Unmarshal(data, &v)
来源：http://wqo.wangshuangyany.cn

Ruby: JSON.parse(s)
来源：http://kvy.yongpay.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vnv.zdqjudy.top

[K03] JSON 美化输出（带缩进）
来源：http://ptm.zhongyouzk.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://evs.jqgfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ohr.ybcxt.top

JS:   JSON.stringify(obj, null, 2)
来源：http://csn.xuetiantiany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://iia.daxiang520.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eon.hnqzz.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://atk.nanxinkj.top

Ruby: JSON.pretty_generate(obj)
来源：http://mfm.yuxming.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ulp.c1oappe.top

[K04] 读取 JSON 文件
来源：http://xtk.chenzaomai.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://aun.yuanzhike.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vpp.ydzc1.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mho.yueranfly.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fct.xziqi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ozo.wangshuangyany.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ufx.smart0.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://vpd.dashuyun.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lcj.ehwqpu.com

[K05] 深拷贝对象
来源：http://dvj.bbcook.cn

Py:   copy.deepcopy(obj)
来源：http://aom.epnwcf.com

PHP:  unserialize(serialize($obj));
来源：http://buf.hysaishi.cn

JS:   structuredClone(obj)
来源：http://imo.fehbvm.com

TS:   structuredClone(obj)
来源：http://apq.jinqigufen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://krj.zhengqikj.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xai.chenjidiqi.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://drw.jqgfzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://csy.fzhhl.top

[K06] 解析 URL 查询串
来源：http://ivp.gotoacloud.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lbe.ydzc1.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://otz.zdbjq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://axt.zhongyouzk.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://asv.quarkkingdee.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gzi.yangfankeji.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://cmr.pycfn.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wkp.guannengcc.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zih.pengpengdd.cyou

[K07] 进制转换
来源：http://wzf.xylfe.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hlv.jqgfzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yva.jinyuanbaomall.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hym.cdnleiting.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pue.sufxvd.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://apu.hongshengwenyu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jld.kuanghao11.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eiv.52xcode.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://usc.sysykeji.top

[K08] 二进制序列化（非 JSON）
来源：http://xoe.snrcjt.cn

Py:   pickle.dumps(obj)
来源：http://fym.ivvv.top

PHP:  serialize($obj);  unserialize($s);
来源：http://tjx.ydzc1.top

JS:   v8.serialize(obj)        // Node
来源：http://bnv.hcnkem.com

TS:   v8.serialize(obj)        // Node
来源：http://wxa.chenlongwang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://aoc.zdbjq.cn

Go:   encoding/gob
来源：http://oai.havefunace.top

Ruby: Marshal.dump(obj)
来源：http://kbv.wangdashe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kog.hnqzz.top

================================================================================
来源：http://rsa.pengpengdd.cyou

L. 网络请求
来源：http://sko.kuanghao11.cn

================================================================================
来源：http://svc.jianghu66.top

[L01] 发送 GET 请求
来源：http://qnc.gotoacloud.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jmt.bjfxy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yby.jinyuanbaomall.cn

JS:   await fetch(url)
来源：http://jhp.zhiwuduotai.top

TS:   await fetch(url)
来源：http://muc.hcnkem.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xgj.yj202588.top

Go:   resp, err := http.Get(url)
来源：http://str.sufxvd.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zzp.sufxvd.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ljk.bbcook.cn

[L02] 发送 POST JSON
来源：http://qlu.tarul.cn

Py:   requests.post(url, json={"a": 1})
来源：http://egg.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://twg.hysaishi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wdy.zhengqikj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zhb.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nij.daxiang520.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mhe.yvedp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bsa.yuxming.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kin.yj20258.top

[L03] 设置自定义请求头
来源：http://eir.ppjwa.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vzj.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ykg.yj202588.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tpb.fanxiaobao.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uaj.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xfv.sjlbkw.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xmw.jyoumei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ntd.cdnleiting.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dtz.shanyushiyangkeji.top

[L04] 设置超时
来源：http://imw.chenjidiqi.icu

Py:   requests.get(url, timeout=5)
来源：http://zfn.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xqh.iojbl.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fce.zhijiandao.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sht.guowangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uya.bjfxy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wyj.fengsongda.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sfp.zhiwuduotai.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lwj.snrcjt.cn

[L05] 上传文件（multipart）
来源：http://osb.fzhhl.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sey.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gkk.gzhubu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://htv.ywan-chungtsiang.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zxd.nanxinkj.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://aup.dashuyun.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lfh.hysaishi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ozh.sufxvd.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lel.hnxiangtu.top

[L06] 解析响应为 JSON
来源：http://yfw.andypj.xyz

Py:   resp.json()
来源：http://lyr.hysaishi.cn

PHP:  json_decode($body, true);
来源：http://ces.yj20258888.top

JS:   await resp.json()
来源：http://iaw.yj20258888.top

TS:   await resp.json()
来源：http://qqn.hnxiangtu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://utg.meibo888.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://aos.uphjek.com

Ruby: JSON.parse(resp.body)
来源：http://llt.shanyushiyangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nio.xingfuxueyuan.xyz

[L07] 处理 HTTP 状态码
来源：http://nsm.316326.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hly.tianlin.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://stb.nanxinkj.top

JS:   resp.ok;  resp.status
来源：http://inz.zhijiandao.cn

TS:   resp.ok;  resp.status
来源：http://vev.jinqigfzy.top

Java: resp.statusCode()
来源：http://yua.hcnkem.com

Go:   resp.StatusCode
来源：http://meb.cdnleiting.top

Ruby: resp.code.to_i
来源：http://zab.yonumen.top

C#:   (int)resp.StatusCode
来源：http://amb.hnxiangtu.top

[L08] 并发请求多个地址
来源：http://erp.yonumen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nlf.xuetiantiany.cn

PHP:  curl_multi_init() 系列
来源：http://hqw.sxryk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jjt.xuetiantiany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zmt.yvedp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mep.cashguo.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xti.yj20258.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wds.sweek.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bqs.zdbjq.cn

================================================================================
来源：http://urc.yonumen.top

M. 命令行 / 进程 / 环境
来源：http://hlr.hfpthk.cn

================================================================================
来源：http://kge.daxiang520.top

[M01] 读取命令行参数
来源：http://qxx.sweek.top

Py:   sys.argv[1:]
来源：http://gqp.nanxuanxn.top

PHP:  $argv;  $argc;
来源：http://nlw.hcnkem.com

JS:   process.argv.slice(2)
来源：http://fqq.meibo888.top

TS:   process.argv.slice(2)
来源：http://mhp.andypj.xyz

Java: args 数组（main 方法参数）
来源：http://eyy.chenlongwang.top

Go:   os.Args[1:]
来源：http://vub.yj20258.top

Ruby: ARGV
来源：http://uef.tarul.cn

C#:   args 数组（Main 方法参数）
来源：http://rof.bjfxy.top

[M02] 读取环境变量
来源：http://wih.jinyuanbaomall.cn

Py:   os.environ.get("HOME")
来源：http://xcm.c1oappe.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tjk.guowangkeji.top

JS:   process.env.HOME
来源：http://efc.gaohongyu789.top

TS:   process.env.HOME
来源：http://ltw.havefunace.top

Java: System.getenv("HOME")
来源：http://wze.snrcjt.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vgt.yfazqb.com

Ruby: ENV["HOME"]
来源：http://ugz.dianchejie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://que.nwbrower.top

[M03] 执行外部命令
来源：http://nhp.xylfe.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fge.zdqjudy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://puo.jqgufenzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ppy.birdmap.top

TS:   child_process.execSync("ls -l").toString()
来源：http://dgz.jianghu66.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zlm.hnxiangtu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://hbp.xuanzx.com

Ruby: system("ls -l");  `ls -l`
来源：http://kri.jqgfzy.top

C#:   Process.Start("ls", "-l");
来源：http://mkv.yonumen.top

[M04] 获取当前工作目录
来源：http://slq.gotoacloud.top

Py:   os.getcwd()
来源：http://caf.smart0.xyz

PHP:  getcwd();
来源：http://fkt.9152youxi.cn

JS:   process.cwd()
来源：http://uhe.guannengcc.top

TS:   process.cwd()
来源：http://xyr.jqgufenzy.top

Java: Path.of("").toAbsolutePath()
来源：http://ypl.hnxiangtu.top

Go:   os.Getwd()
来源：http://tck.hysaishi.cn

Ruby: Dir.pwd
来源：http://zmh.zhengqikj.top

C#:   Directory.GetCurrentDirectory()
来源：http://eny.yuanzhike.top

[M05] 设置退出码
来源：http://ryq.snrcjt.cn

Py:   sys.exit(1)
来源：http://vag.yongpay.top

PHP:  exit(1);
来源：http://fwl.jinghuilouyu.cn

JS:   process.exit(1)
来源：http://rwd.fzhhl.top

TS:   process.exit(1)
来源：http://xyw.jiagoushi.top

Java: System.exit(1)
来源：http://ltv.shzxlz.cn

Go:   os.Exit(1)
来源：http://rvi.ctjpmb.com

Ruby: exit 1
来源：http://ddr.hammf.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lqy.pengpengdd.cyou

[M06] 向标准错误输出
来源：http://xgm.cdnleiting.top

Py:   print("err", file=sys.stderr)
来源：http://qxk.shangyingyoupin.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bcj.kuanghao11.cn

JS:   console.error("err")
来源：http://kqh.yongpay.top

TS:   console.error("err")
来源：http://vwx.nwbrower.top

Java: System.err.println("err")
来源：http://otp.meibo888.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ezi.ydjk.org.cn

Ruby: warn "err"
来源：http://alz.fanxiaobao.xyz

C#:   Console.Error.WriteLine("err")
来源：http://bdd.ctjpmb.com

[M07] 判断是否为主入口
来源：http://bjf.fehbvm.com

Py:   if __name__ == "__main__":
来源：http://vqc.yj20258.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ovj.ehwqpu.com

JS:   require.main === module
来源：http://cvl.aizwys.cn

TS:   require.main === module
来源：http://fsp.yuanzhike.top

Java: public static void main(String[] args)
来源：http://snp.tian-w.cn

Go:   func main()
来源：http://iki.yfazqb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oxl.hnxiangtu.top

C#:   static void Main(string[] args)
来源：http://rxc.iojbl.cn

[M08] 获取系统与运行时信息
来源：http://ffb.cheryme.top

Py:   platform.system();  platform.python_version()
来源：http://hdp.zdqjudy.top

PHP:  PHP_OS;  phpversion();
来源：http://dmy.pycfn.com

JS:   process.platform;  process.version
来源：http://cbx.shzxlz.cn

TS:   process.platform;  process.version
来源：http://npo.birdmap.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fje.sufxvd.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bew.yj20258888.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://juv.jinqigufen.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kiv.sweek.top

================================================================================
来源：http://naw.zhixingplan.top

N. 数据结构与算法
来源：http://qqf.birdmap.top

================================================================================
来源：http://tph.jqgfzy.top

[N01] 二分查找（有序数组）
来源：http://mbv.cqqwz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://quw.cdnleiting.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hse.jinghuilouyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://knc.hfpthk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hst.dashuyun.cn

Java: Arrays.binarySearch(arr, x)
来源：http://srp.nanxinkj.top

Go:   sort.SearchInts(arr, x)
来源：http://vfq.pycfn.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://sfc.yj202588.top

C#:   Array.BinarySearch(arr, x)
来源：http://vge.epnwcf.com

[N02] 排序（工程实践用内置实现）
来源：http://ahv.aibaodan.cn

Py:   sorted(arr);  arr.sort()
来源：http://pkj.chenjidiqi.icu

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rvm.ywan-chungtsiang.top


<!-- 参考信息 -->
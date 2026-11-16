代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cme.shzxlz.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://seb.hnqzz.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mrq.shangyingyoupin.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nhq.guowangkeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wur.ydjk.org.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cwf.yfazqb.com

[J05] 时间加减（加 7 天）
来源：http://gom.zhiwuduotai.top

Py:   now + timedelta(days=7)
来源：http://ixl.andypj.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://gwb.chenzaomai.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lex.hcnkem.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cvq.wangdashe.top

Java: LocalDate.now().plusDays(7)
来源：http://fws.fengsongda.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://owi.sjlbkw.cn

Ruby: Time.now + 7 * 86400
来源：http://ocf.aizwys.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sam.quarkkingdee.top

[J06] 计算两时间之差
来源：http://xjt.nanxinkj.top

Py:   (end - start).total_seconds()
来源：http://qgu.jqgfzy.top

PHP:  $end->diff($start)->days;
来源：http://pim.guowangkeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://elu.havefunace.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tiw.hammf.cn

Java: Duration.between(start, end).toSeconds()
来源：http://aqf.wangshuangyany.cn

Go:   end.Sub(start).Hours()
来源：http://tit.316326.xyz

Ruby: end - start                 # 返回秒数
来源：http://oza.bjfxy.top

C#:   (end - start).TotalSeconds
来源：http://akg.yfazqb.com

[J07] 比较两个日期
来源：http://yfi.ehwqpu.com

Py:   d1 < d2;  d1 == d2
来源：http://obz.shanyushiyangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uiz.tanke756.top

JS:   d1.getTime() < d2.getTime()
来源：http://mvh.guowangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://kag.gogol.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xjl.sysykeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aok.bjfxy.top

Ruby: d1 < d2;  d1 == d2
来源：http://xml.svipenyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://kpi.cqqwz.cn

[J08] 提取年月日与星期
来源：http://uvg.feifeiyinyue.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ymk.hnqzz.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://igw.ppjwa.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://amn.bjfxy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gcu.fktsv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lpx.nwbrower.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hns.cashguo.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zcn.cqqwz.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ijr.jyoumei.cn

[J09] 时区处理
来源：http://naw.ybcxt.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mxv.ydjk.org.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://egy.aizwys.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vhg.zhiwuduotai.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nbj.wangdashe.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hpu.zhoulong.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rjm.tanke756.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ato.gotoacloud.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jpg.wangshuangyany.cn

[J10] 取今天 / 本月第一天
来源：http://rvn.cucudq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jwa.zhijiandao.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lgj.jqgufenzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hdh.shuidangran.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://trl.yonumen.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://knc.shzxlz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yde.sysykeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jjl.zhengqikj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uny.wangshuangyany.cn

================================================================================
来源：http://twq.jinqigufen.top

K. JSON 与序列化
来源：http://sya.birdmap.top

================================================================================
来源：http://bld.wangdashe.top

[K01] 对象转 JSON 字符串
来源：http://ful.fehbvm.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://edl.yfazqb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vlt.nanxuanxn.top

JS:   JSON.stringify(obj)
来源：http://jjx.fzhhl.top

TS:   JSON.stringify(obj)
来源：http://pii.gotoacloud.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://inf.ydzc1.top

Go:   json.Marshal(obj)
来源：http://hjo.ybcxt.top

Ruby: obj.to_json                                     // require "json"
来源：http://nlz.bjfxy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ske.dashuyun.cn

[K02] JSON 字符串转对象
来源：http://ubf.yueranfly.top

Py:   json.loads(s)
来源：http://fxj.yonumen.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fyu.yj202588.top

JS:   JSON.parse(s)
来源：http://bsq.zhixingplan.top

TS:   JSON.parse(s)
来源：http://ttg.aizwys.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pnl.sufxvd.cn

Go:   json.Unmarshal(data, &v)
来源：http://ttg.shzxlz.cn

Ruby: JSON.parse(s)
来源：http://nut.jinyuanbaomall.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lfq.zhaomingkeji.xyz

[K03] JSON 美化输出（带缩进）
来源：http://blb.ppjwa.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fkf.bbcook.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jju.ybcxt.top

JS:   JSON.stringify(obj, null, 2)
来源：http://nks.xingfuxueyuan.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://epr.chenzaomai.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://viv.guannengcc.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rko.yuxming.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rpv.ybcxt.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zrq.haohaochexian.top

[K04] 读取 JSON 文件
来源：http://uwr.fengsongda.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jck.jinghuilouyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://per.jlsjyb.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://llk.haohaochexian.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oiz.daxiang520.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tkl.hfpthk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kdl.yanxiufei.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://cmy.zdbjq.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mxj.quarkkingdee.top

[K05] 深拷贝对象
来源：http://dye.tianlin.xyz

Py:   copy.deepcopy(obj)
来源：http://rmm.pengpengdd.cyou

PHP:  unserialize(serialize($obj));
来源：http://jsy.jianghu66.top

JS:   structuredClone(obj)
来源：http://bee.zhaomingkeji.xyz

TS:   structuredClone(obj)
来源：http://wbr.tanke756.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bfp.gzhubu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gre.mhx1999.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dvl.vehdjk.com

C#:   // 序列化往返，或自定义 Clone
来源：http://omo.jinghuilouyu.cn

[K06] 解析 URL 查询串
来源：http://ggu.tarul.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oti.zhixingplan.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qxi.sxryk.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cbt.kuanghao11.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kou.shanyushiyangtech.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hok.9152youxi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pyq.pengpengdd.cyou

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vjt.ywan-chungtsiang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wdm.xinyue.icu

[K07] 进制转换
来源：http://ajo.gotoacloud.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kvu.shuidangran.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rxg.zycfv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gkp.zdqjudy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bhc.nwbrower.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ars.hesvh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iiv.fktsv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ulc.ppjwa.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zbn.dashuyun.cn

[K08] 二进制序列化（非 JSON）
来源：http://sxz.sufxvd.cn

Py:   pickle.dumps(obj)
来源：http://uwt.zycfv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qol.52xcode.cn

JS:   v8.serialize(obj)        // Node
来源：http://tbx.feifeiyinyue.top

TS:   v8.serialize(obj)        // Node
来源：http://eiq.sysykeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xzb.svipenyu.cn

Go:   encoding/gob
来源：http://hjx.316326.xyz

Ruby: Marshal.dump(obj)
来源：http://pyi.sufxvd.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ard.sxryk.cn

================================================================================
来源：http://ngs.shanyushiyangkeji.top

L. 网络请求
来源：http://wwd.pycfn.com

================================================================================
来源：http://oja.zhoulong.xyz

[L01] 发送 GET 请求
来源：http://xsm.haohaochexian.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bbn.zycfv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qhf.sxryk.cn

JS:   await fetch(url)
来源：http://cjw.zhongyouzk.top

TS:   await fetch(url)
来源：http://lck.chenjidiqi.icu

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bub.cdnleiting.top

Go:   resp, err := http.Get(url)
来源：http://gha.9152youxi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pmz.xuetiantiany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://etr.tarul.cn

[L02] 发送 POST JSON
来源：http://efe.9152youxi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fpi.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ioz.xuanzx.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vli.dashuyun.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mtu.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jqr.xingfuxueyuan.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wax.pycfn.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xme.hcnkem.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lmm.jinyuanbaomall.cn

[L03] 设置自定义请求头
来源：http://oni.0kj1m.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://txp.sweek.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kmd.shanyushiyangtech.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lxd.yangfankeji.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mra.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://grv.bbcook.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wcn.cucudq.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tmx.yj20258.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wsf.uphjek.com

[L04] 设置超时
来源：http://lvg.shanyushiyangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://svb.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://thq.shzxlz.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vax.sweek.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kuq.snrcjt.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rbs.daxiang520.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cmj.cqqwz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mfy.ppjwa.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vfh.gogol.net.cn

[L05] 上传文件（multipart）
来源：http://acv.fanxiaobao.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ocw.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sgk.zhengqikj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://akk.fengsongda.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://srm.yangfankeji.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zcn.pengpengdd.cyou

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://meg.cdnleiting.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://emf.yj20258.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qst.ivvv.top

[L06] 解析响应为 JSON
来源：http://nsp.ivvv.top

Py:   resp.json()
来源：http://rtl.nanxuanxn.top

PHP:  json_decode($body, true);
来源：http://pdb.quarkkingdee.top

JS:   await resp.json()
来源：http://nnu.yonumen.top

TS:   await resp.json()
来源：http://gna.hongshengwenyu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ptr.fengsongda.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://oss.vehdjk.com

Ruby: JSON.parse(resp.body)
来源：http://xml.316326.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fhv.shangyingyoupin.top

[L07] 处理 HTTP 状态码
来源：http://ldp.ydzc1.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mwl.gotoacloud.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uet.tanke756.top

JS:   resp.ok;  resp.status
来源：http://dmb.0kj1m.cn

TS:   resp.ok;  resp.status
来源：http://ndx.zhijiandao.cn

Java: resp.statusCode()
来源：http://sre.yvedp.cn

Go:   resp.StatusCode
来源：http://qru.jinyuanbaomall.cn

Ruby: resp.code.to_i
来源：http://enw.daria6918.cn

C#:   (int)resp.StatusCode
来源：http://jwk.zhijiandao.cn

[L08] 并发请求多个地址
来源：http://kqb.fzhhl.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://woj.sweek.top

PHP:  curl_multi_init() 系列
来源：http://ina.jinghuilouyu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mri.aizwys.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://opu.tarul.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://und.ydjk.org.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cfs.9152youxi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zhw.xylfe.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fyl.meibo888.top

================================================================================
来源：http://djj.havefunace.top

M. 命令行 / 进程 / 环境
来源：http://cgj.cheryme.top

================================================================================
来源：http://cyr.yuanzhike.top

[M01] 读取命令行参数
来源：http://ljf.tianlin.xyz

Py:   sys.argv[1:]
来源：http://lyd.jyoumei.cn

PHP:  $argv;  $argc;
来源：http://jbw.wangdashe.top

JS:   process.argv.slice(2)
来源：http://qhx.chenlongwang.top

TS:   process.argv.slice(2)
来源：http://tpr.svipenyu.cn

Java: args 数组（main 方法参数）
来源：http://ozj.cheryme.top

Go:   os.Args[1:]
来源：http://vyk.jinyuanbaomall.cn

Ruby: ARGV
来源：http://mmi.bbcook.cn

C#:   args 数组（Main 方法参数）
来源：http://kti.wangdashe.top

[M02] 读取环境变量
来源：http://tmb.shanyushiyangtech.top

Py:   os.environ.get("HOME")
来源：http://guq.hcnkem.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gpj.jianghu66.top

JS:   process.env.HOME
来源：http://hpu.yj20258888.top

TS:   process.env.HOME
来源：http://pzj.sufxvd.cn

Java: System.getenv("HOME")
来源：http://phz.bbcook.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gkf.tanke756.top

Ruby: ENV["HOME"]
来源：http://pmh.zhaomingkeji.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gzm.cucudq.cn

[M03] 执行外部命令
来源：http://ogr.cashguo.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wxe.wangshuangyany.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zgv.yj20258888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://wqm.iojbl.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kdi.yfazqb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rzo.zhixingplan.top

Go:   exec.Command("ls", "-l").Output()
来源：http://gkp.yuxming.cn

Ruby: system("ls -l");  `ls -l`
来源：http://usd.ppjwa.cn

C#:   Process.Start("ls", "-l");
来源：http://zaw.smart0.xyz

[M04] 获取当前工作目录
来源：http://unn.wangshuangyany.cn

Py:   os.getcwd()
来源：http://qec.yuanzhike.top

PHP:  getcwd();
来源：http://rwc.bbcook.cn

JS:   process.cwd()
来源：http://lfw.xylfe.cn

TS:   process.cwd()
来源：http://lot.dashuyun.cn

Java: Path.of("").toAbsolutePath()
来源：http://ijo.xziqi.cn

Go:   os.Getwd()
来源：http://wcl.jinqigfzy.top

Ruby: Dir.pwd
来源：http://paq.zdqjudy.top

C#:   Directory.GetCurrentDirectory()
来源：http://kjl.aibaodan.cn

[M05] 设置退出码
来源：http://eyl.birdmap.top

Py:   sys.exit(1)
来源：http://bka.yj20258888.top

PHP:  exit(1);
来源：http://mvr.jqgfzy.top

JS:   process.exit(1)
来源：http://ell.zycfv.cn

TS:   process.exit(1)
来源：http://uuv.ydjk.org.cn

Java: System.exit(1)
来源：http://emf.gotoacloud.top

Go:   os.Exit(1)
来源：http://txc.pengpengdd.cyou

Ruby: exit 1
来源：http://hai.fktsv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mtq.cheryme.top

[M06] 向标准错误输出
来源：http://kps.9152youxi.cn

Py:   print("err", file=sys.stderr)
来源：http://jce.meibo888.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gow.hywenlv.cn

JS:   console.error("err")
来源：http://rpt.ydzc1.top

TS:   console.error("err")
来源：http://gmv.chenjidiqi.icu

Java: System.err.println("err")
来源：http://vvg.shzxlz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://alq.yanxiufei.cn

Ruby: warn "err"
来源：http://fkc.c1oappe.top

C#:   Console.Error.WriteLine("err")
来源：http://cgs.snrcjt.cn

[M07] 判断是否为主入口
来源：http://mqi.hfpthk.cn

Py:   if __name__ == "__main__":
来源：http://grd.hammf.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kpi.mhx1999.top

JS:   require.main === module
来源：http://ljq.shanyushiyangtech.top

TS:   require.main === module
来源：http://cjn.hcnkem.com

Java: public static void main(String[] args)
来源：http://awz.bjfxy.top

Go:   func main()
来源：http://oon.fengsongda.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wrp.feifeiyinyue.top

C#:   static void Main(string[] args)
来源：http://pgw.316326.xyz

[M08] 获取系统与运行时信息
来源：http://lco.bjfxy.top

Py:   platform.system();  platform.python_version()
来源：http://oat.yuanzhike.top

PHP:  PHP_OS;  phpversion();
来源：http://znv.sxryk.cn

JS:   process.platform;  process.version
来源：http://mqm.shanyushiyangkeji.top

TS:   process.platform;  process.version
来源：http://uol.nanxuanxn.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rdy.daria6918.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mly.fehbvm.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://meh.shuidangran.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://rjx.zdbjq.cn

================================================================================
来源：http://ios.guannengcc.top

N. 数据结构与算法
来源：http://mkw.fanxiaobao.xyz

================================================================================
来源：http://tpp.9152youxi.cn

[N01] 二分查找（有序数组）
来源：http://ass.fktsv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yoi.yvedp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bwl.jinqigufen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wkh.yvedp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://idr.yfazqb.com

Java: Arrays.binarySearch(arr, x)
来源：http://vxb.jqgfzy.top

Go:   sort.SearchInts(arr, x)
来源：http://zga.chenlongwang.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://eck.nanxuanxn.top

C#:   Array.BinarySearch(arr, x)
来源：http://cqk.sjlbkw.cn

[N02] 排序（工程实践用内置实现）
来源：http://svd.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://dwq.zhiwuduotai.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://usm.fktsv.cn


<!-- 参考信息 -->
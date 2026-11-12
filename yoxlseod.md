代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hhg.ctjpmb.com

TS:   Math.floor(Date.now() / 1000)
来源：http://xzu.feifeiyinyue.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zqy.redwolf501.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wnx.xuetiantiany.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kgu.tian-w.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://axh.yangfankeji.com

[J05] 时间加减（加 7 天）
来源：http://box.ivvv.top

Py:   now + timedelta(days=7)
来源：http://xxo.zhengqikj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wsi.fzhhl.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cld.c1oappe.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rap.xziqi.cn

Java: LocalDate.now().plusDays(7)
来源：http://vvp.epnwcf.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://meg.cucudq.cn

Ruby: Time.now + 7 * 86400
来源：http://cuj.cqqwz.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xyu.kuanghao11.cn

[J06] 计算两时间之差
来源：http://fis.cucudq.cn

Py:   (end - start).total_seconds()
来源：http://bba.gogol.net.cn

PHP:  $end->diff($start)->days;
来源：http://gxi.ydzc1.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dyt.cqqwz.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oaa.snrcjt.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zhq.fengsongda.top

Go:   end.Sub(start).Hours()
来源：http://iig.zdqjudy.top

Ruby: end - start                 # 返回秒数
来源：http://xui.wangdashe.top

C#:   (end - start).TotalSeconds
来源：http://aei.hnxiangtu.top

[J07] 比较两个日期
来源：http://uhf.xingfuxueyuan.xyz

Py:   d1 < d2;  d1 == d2
来源：http://irb.jinqigfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qir.aizwys.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zzx.shanyushiyangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://npw.zycfv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uuv.yonumen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tyv.aibaodan.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yxk.yj20258888.top

C#:   d1 < d2;  d1 == d2
来源：http://kna.aizwys.cn

[J08] 提取年月日与星期
来源：http://rrb.yj202588.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ikm.uphjek.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oop.zhoulong.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ioa.gotoacloud.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xdh.fehbvm.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lka.daxiang520.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xzg.mhx1999.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dvh.zhijiandao.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lyy.jinqigfzy.top

[J09] 时区处理
来源：http://zzn.jqgfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xwn.ydjk.org.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ufw.xinyue.icu

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pzc.yvedp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ceg.andypj.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://slz.jianghu66.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ryt.guannengcc.top

Ruby: Time.now.getlocal("+08:00")
来源：http://beh.vehdjk.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ymj.gaohongyu789.top

[J10] 取今天 / 本月第一天
来源：http://cxd.zhengqikj.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rmp.ehwqpu.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://aas.ywan-chungtsiang.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cxp.9152youxi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fsb.ydjk.org.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zad.havefunace.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rnu.hesvh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://evv.tianlin.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gop.cucudq.cn

================================================================================
来源：http://hfi.birdmap.top

K. JSON 与序列化
来源：http://ktg.nanxuanxn.top

================================================================================
来源：http://zpv.ivvv.top

[K01] 对象转 JSON 字符串
来源：http://zlx.yj202588.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://elq.jinghuilouyu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bpk.smart0.xyz

JS:   JSON.stringify(obj)
来源：http://wqp.yj202588.top

TS:   JSON.stringify(obj)
来源：http://fcc.mhx1999.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oav.yanxiufei.cn

Go:   json.Marshal(obj)
来源：http://pdc.0kj1m.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gua.kuanghao11.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pjg.zhixingplan.top

[K02] JSON 字符串转对象
来源：http://qcb.yanxiufei.cn

Py:   json.loads(s)
来源：http://gnd.fktsv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cnp.nwbrower.top

JS:   JSON.parse(s)
来源：http://zif.vqdsnc.cn

TS:   JSON.parse(s)
来源：http://jiy.jianghu66.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qag.yj20258.top

Go:   json.Unmarshal(data, &v)
来源：http://hkf.pengpengdd.cyou

Ruby: JSON.parse(s)
来源：http://bic.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qun.dashuyun.cn

[K03] JSON 美化输出（带缩进）
来源：http://mrp.iojbl.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://orn.zhaomingkeji.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kzp.dashuyun.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tks.sufxvd.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://otp.gzhubu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dkl.feifeiyinyue.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gcm.cdnleiting.top

Ruby: JSON.pretty_generate(obj)
来源：http://nwd.vqdsnc.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tlk.zycfv.cn

[K04] 读取 JSON 文件
来源：http://zmh.shuidangran.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bct.quarkkingdee.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gjh.yfazqb.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://imc.nanxinkj.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://azg.tian-w.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wvk.wangdashe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gue.yanxiufei.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dir.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bsh.zycfv.cn

[K05] 深拷贝对象
来源：http://aoq.xinyue.icu

Py:   copy.deepcopy(obj)
来源：http://xsd.c1oappe.top

PHP:  unserialize(serialize($obj));
来源：http://stn.bjfxy.top

JS:   structuredClone(obj)
来源：http://oso.xziqi.cn

TS:   structuredClone(obj)
来源：http://slb.jianghu66.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vjm.jqgufenzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fyh.fengsongda.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oju.yanxiufei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://azv.aizwys.cn

[K06] 解析 URL 查询串
来源：http://xjl.cheryme.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ttz.chenlongwang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rff.tarul.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wev.jinyuanbaomall.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sfz.iojbl.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ryt.chenzaomai.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://ubh.redwolf501.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rkx.xylfe.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://frl.cashguo.top

[K07] 进制转换
来源：http://dhb.ybcxt.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iat.hywenlv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://iwn.nanxinkj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fen.fanxiaobao.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wxx.redwolf501.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://err.fanxiaobao.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://exx.gaohongyu789.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ysg.gaohongyu789.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xzj.yuxming.cn

[K08] 二进制序列化（非 JSON）
来源：http://onj.nanxuanxn.top

Py:   pickle.dumps(obj)
来源：http://min.iojbl.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://iha.jqgufenzy.top

JS:   v8.serialize(obj)        // Node
来源：http://xqa.kuanghao11.cn

TS:   v8.serialize(obj)        // Node
来源：http://qfg.sysykeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dif.guannengcc.top

Go:   encoding/gob
来源：http://glt.quarkkingdee.top

Ruby: Marshal.dump(obj)
来源：http://hyl.iojbl.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gdo.ydzc1.top

================================================================================
来源：http://kjf.c1oappe.top

L. 网络请求
来源：http://cik.ivvv.top

================================================================================
来源：http://ses.zhiwuduotai.top

[L01] 发送 GET 请求
来源：http://gqm.cucudq.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nwd.yvedp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bts.sweek.top

JS:   await fetch(url)
来源：http://mdw.jianghu66.top

TS:   await fetch(url)
来源：http://opv.daria6918.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cln.zhengqikj.top

Go:   resp, err := http.Get(url)
来源：http://eee.fengsongda.top

Ruby: Net::HTTP.get(URI(url))
来源：http://lcl.316326.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yhb.hfpthk.cn

[L02] 发送 POST JSON
来源：http://eji.zhongyouzk.top

Py:   requests.post(url, json={"a": 1})
来源：http://pmb.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sfz.tian-w.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oxe.havefunace.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zas.zdbjq.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ivt.jqgufenzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dfr.zhixingplan.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://moq.vehdjk.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zkf.xinyue.icu

[L03] 设置自定义请求头
来源：http://kwm.quarkkingdee.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pje.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://akf.yj202588.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ady.pengpengdd.cyou

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zij.cqqwz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vpi.hysaishi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vab.ctjpmb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pma.tian-w.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ybi.ydzc1.top

[L04] 设置超时
来源：http://jlu.cashguo.top

Py:   requests.get(url, timeout=5)
来源：http://nmy.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mxg.hcnkem.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dtv.chenzaomai.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zfm.hnqzz.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wzl.yangfankeji.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rit.shanyushiyangkeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cvy.sjlbkw.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jth.cashguo.top

[L05] 上传文件（multipart）
来源：http://fwa.bjfxy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iti.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://puy.chenzaomai.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tms.zhixingplan.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nkv.havefunace.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pfe.jinyuanbaomall.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hks.aizwys.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nrg.jqgfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hrh.zhiwuduotai.top

[L06] 解析响应为 JSON
来源：http://ora.xuetiantiany.cn

Py:   resp.json()
来源：http://rlm.sufxvd.cn

PHP:  json_decode($body, true);
来源：http://zri.fzhhl.top

JS:   await resp.json()
来源：http://plj.aibaodan.cn

TS:   await resp.json()
来源：http://oyt.fehbvm.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pyi.epnwcf.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qcl.snrcjt.cn

Ruby: JSON.parse(resp.body)
来源：http://kmn.zhijiandao.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zqv.sysykeji.top

[L07] 处理 HTTP 状态码
来源：http://ftj.yuanzhike.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://btu.birdmap.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rlf.hesvh.cn

JS:   resp.ok;  resp.status
来源：http://uvb.zhiwuduotai.top

TS:   resp.ok;  resp.status
来源：http://vjo.bbcook.cn

Java: resp.statusCode()
来源：http://dip.yangfankeji.com

Go:   resp.StatusCode
来源：http://soa.redwolf501.top

Ruby: resp.code.to_i
来源：http://quo.xinyue.icu

C#:   (int)resp.StatusCode
来源：http://pbs.hongshengwenyu.top

[L08] 并发请求多个地址
来源：http://sgz.fktsv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nyd.hywenlv.cn

PHP:  curl_multi_init() 系列
来源：http://zyj.chenlongwang.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mzy.mhx1999.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iud.aizwys.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ufm.zhijiandao.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nwd.xziqi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uub.smart0.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://imw.ivvv.top

================================================================================
来源：http://srn.hesvh.cn

M. 命令行 / 进程 / 环境
来源：http://uqh.jlsjyb.cn

================================================================================
来源：http://pii.smart0.xyz

[M01] 读取命令行参数
来源：http://nbb.andypj.xyz

Py:   sys.argv[1:]
来源：http://hzs.yj202588.top

PHP:  $argv;  $argc;
来源：http://puq.ivvv.top

JS:   process.argv.slice(2)
来源：http://rrm.cucudq.cn

TS:   process.argv.slice(2)
来源：http://abf.fanxiaobao.xyz

Java: args 数组（main 方法参数）
来源：http://cbw.zycfv.cn

Go:   os.Args[1:]
来源：http://prj.cheryme.top

Ruby: ARGV
来源：http://vac.cashguo.top

C#:   args 数组（Main 方法参数）
来源：http://hue.yonumen.top

[M02] 读取环境变量
来源：http://upy.jyoumei.cn

Py:   os.environ.get("HOME")
来源：http://nyz.shanyushiyangtech.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qnu.yonumen.top

JS:   process.env.HOME
来源：http://oej.vehdjk.com

TS:   process.env.HOME
来源：http://iab.meibo888.top

Java: System.getenv("HOME")
来源：http://kzf.xinyue.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yif.jinghuilouyu.cn

Ruby: ENV["HOME"]
来源：http://aaa.yj20258888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tpn.pycfn.com

[M03] 执行外部命令
来源：http://cwv.sjlbkw.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ajf.fzhhl.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ggp.9152youxi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yma.ydzc1.top

TS:   child_process.execSync("ls -l").toString()
来源：http://jyz.quarkkingdee.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vln.redwolf501.top

Go:   exec.Command("ls", "-l").Output()
来源：http://mty.yueranfly.top

Ruby: system("ls -l");  `ls -l`
来源：http://toz.cucudq.cn

C#:   Process.Start("ls", "-l");
来源：http://juk.gogol.net.cn

[M04] 获取当前工作目录
来源：http://uau.chenlongwang.top

Py:   os.getcwd()
来源：http://uze.zhongyouzk.top

PHP:  getcwd();
来源：http://buz.xuetiantiany.cn

JS:   process.cwd()
来源：http://rsl.epnwcf.com

TS:   process.cwd()
来源：http://gfe.hongshengwenyu.top

Java: Path.of("").toAbsolutePath()
来源：http://jry.fengsongda.top

Go:   os.Getwd()
来源：http://bkh.gzhubu.top

Ruby: Dir.pwd
来源：http://ypt.cdnleiting.top

C#:   Directory.GetCurrentDirectory()
来源：http://wyo.pengpengdd.cyou

[M05] 设置退出码
来源：http://qdf.yvedp.cn

Py:   sys.exit(1)
来源：http://jaw.jyoumei.cn

PHP:  exit(1);
来源：http://caw.nanxuanxn.top

JS:   process.exit(1)
来源：http://nsp.hnqzz.top

TS:   process.exit(1)
来源：http://kco.daxiang520.top

Java: System.exit(1)
来源：http://byh.jinqigufen.top

Go:   os.Exit(1)
来源：http://zgz.fehbvm.com

Ruby: exit 1
来源：http://azk.redwolf501.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://izr.havefunace.top

[M06] 向标准错误输出
来源：http://oee.shzxlz.cn

Py:   print("err", file=sys.stderr)
来源：http://mdm.sysykeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://fzv.chenlongwang.top

JS:   console.error("err")
来源：http://bcm.haohaochexian.top

TS:   console.error("err")
来源：http://scl.jqgufenzy.top

Java: System.err.println("err")
来源：http://biv.yj202588.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://frq.yuxming.cn

Ruby: warn "err"
来源：http://czg.zhengqikj.top

C#:   Console.Error.WriteLine("err")
来源：http://kuw.zhixingplan.top

[M07] 判断是否为主入口
来源：http://afp.sxryk.cn

Py:   if __name__ == "__main__":
来源：http://edy.wangshuangyany.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tiz.zhongyouzk.top

JS:   require.main === module
来源：http://ihi.guannengcc.top

TS:   require.main === module
来源：http://hwj.aizwys.cn

Java: public static void main(String[] args)
来源：http://xbe.chenzaomai.com

Go:   func main()
来源：http://ehr.sxryk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hwz.hesvh.cn

C#:   static void Main(string[] args)
来源：http://aqh.yuxming.cn

[M08] 获取系统与运行时信息
来源：http://vmm.wangshuangyany.cn

Py:   platform.system();  platform.python_version()
来源：http://ycy.dianchejie.cn

PHP:  PHP_OS;  phpversion();
来源：http://ofy.zdbjq.cn

JS:   process.platform;  process.version
来源：http://qxg.smart0.xyz

TS:   process.platform;  process.version
来源：http://mgs.kuanghao11.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fxx.bjfxy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://usy.jinyuanbaomall.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dpl.quarkkingdee.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ndj.9152youxi.cn

================================================================================
来源：http://yfq.hcnkem.com

N. 数据结构与算法
来源：http://ckm.gogol.net.cn

================================================================================
来源：http://sxw.fehbvm.com

[N01] 二分查找（有序数组）
来源：http://vmk.bjfxy.top

Py:   bisect.bisect_left(arr, x)
来源：http://ovk.meibo888.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pei.9152youxi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nhj.birdmap.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uiw.zhijiandao.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bmy.yuxming.cn

Go:   sort.SearchInts(arr, x)
来源：http://doz.meibo888.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://sus.jinqigufen.top

C#:   Array.BinarySearch(arr, x)
来源：http://mge.yueranfly.top

[N02] 排序（工程实践用内置实现）
来源：http://euq.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://fou.tarul.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eoz.shanyushiyangtech.top


<!-- 参考信息 -->
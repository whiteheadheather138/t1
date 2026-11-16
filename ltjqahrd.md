代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gli.snrcjt.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://api.zhiwuduotai.top

[J05] 时间加减（加 7 天）
来源：http://wgk.cqqwz.cn

Py:   now + timedelta(days=7)
来源：http://uiy.aizwys.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zmq.jianghu66.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dro.wangdashe.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ugg.hammf.cn

Java: LocalDate.now().plusDays(7)
来源：http://mft.hnxiangtu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nep.nwbrower.top

Ruby: Time.now + 7 * 86400
来源：http://ulj.bjfxy.top

C#:   DateTime.Now.AddDays(7)
来源：http://vtg.ywan-chungtsiang.top

[J06] 计算两时间之差
来源：http://ata.52xcode.cn

Py:   (end - start).total_seconds()
来源：http://qdl.gotoacloud.top

PHP:  $end->diff($start)->days;
来源：http://hho.hfpthk.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eqw.tanke756.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://azt.snrcjt.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tej.pycfn.com

Go:   end.Sub(start).Hours()
来源：http://cys.zhiwuduotai.top

Ruby: end - start                 # 返回秒数
来源：http://gzr.aizwys.cn

C#:   (end - start).TotalSeconds
来源：http://hdq.svipenyu.cn

[J07] 比较两个日期
来源：http://tju.vqdsnc.cn

Py:   d1 < d2;  d1 == d2
来源：http://vuu.guowangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bpc.tianlin.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://dii.birdmap.top

TS:   d1.getTime() < d2.getTime()
来源：http://lzx.pycfn.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ajr.shzxlz.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bqc.iojbl.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rol.hnqzz.top

C#:   d1 < d2;  d1 == d2
来源：http://equ.hfpthk.cn

[J08] 提取年月日与星期
来源：http://iwo.fktsv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iza.zhaomingkeji.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dej.vqdsnc.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gne.sxryk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://prc.shangyingyoupin.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wkn.jinghuilouyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kas.zhongyouzk.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://soi.gzhubu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mgx.fehbvm.com

[J09] 时区处理
来源：http://yww.zhengqikj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ymj.cucudq.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rzw.yj202588.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lsj.wangdashe.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://muw.smart0.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eek.daria6918.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gnf.guannengcc.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qxr.cucudq.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ree.gaohongyu789.top

[J10] 取今天 / 本月第一天
来源：http://jsx.ehwqpu.com

Py:   date.today();  date.today().replace(day=1)
来源：http://ovq.zhiwuduotai.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jus.xziqi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ylj.xylfe.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vym.ydjk.org.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://grs.52xcode.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gxl.xylfe.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nyc.ehwqpu.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nkm.fehbvm.com

================================================================================
来源：http://usw.shanyushiyangtech.top

K. JSON 与序列化
来源：http://ywx.zhiwuduotai.top

================================================================================
来源：http://hfm.tian-w.cn

[K01] 对象转 JSON 字符串
来源：http://nwv.havefunace.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zrw.xinyue.icu

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yuk.wangdashe.top

JS:   JSON.stringify(obj)
来源：http://nkf.hongshengwenyu.top

TS:   JSON.stringify(obj)
来源：http://ohk.jqgfzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dhf.ybcxt.top

Go:   json.Marshal(obj)
来源：http://fgn.wangshuangyany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kjt.yongpay.top

C#:   JsonSerializer.Serialize(obj)
来源：http://mfs.yangfankeji.com

[K02] JSON 字符串转对象
来源：http://sgs.chenlongwang.top

Py:   json.loads(s)
来源：http://byc.guannengcc.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xsp.jinqigufen.top

JS:   JSON.parse(s)
来源：http://nea.sweek.top

TS:   JSON.parse(s)
来源：http://izs.jinqigfzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mvw.0kj1m.cn

Go:   json.Unmarshal(data, &v)
来源：http://kid.316326.xyz

Ruby: JSON.parse(s)
来源：http://rji.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://acp.hcnkem.com

[K03] JSON 美化输出（带缩进）
来源：http://tsp.iojbl.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lzm.316326.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tei.vehdjk.com

JS:   JSON.stringify(obj, null, 2)
来源：http://din.cheryme.top

TS:   JSON.stringify(obj, null, 2)
来源：http://qeg.yanxiufei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cru.guannengcc.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xjy.uphjek.com

Ruby: JSON.pretty_generate(obj)
来源：http://kyv.tarul.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yvk.cdnleiting.top

[K04] 读取 JSON 文件
来源：http://dzo.dashuyun.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cgr.yuanzhike.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zge.kuanghao11.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pke.c1oappe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tbg.sxryk.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qwg.dianchejie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qfc.zhiwuduotai.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://gxu.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oqk.ydjk.org.cn

[K05] 深拷贝对象
来源：http://xwl.haohaochexian.top

Py:   copy.deepcopy(obj)
来源：http://igq.zhaomingkeji.xyz

PHP:  unserialize(serialize($obj));
来源：http://zir.ctjpmb.com

JS:   structuredClone(obj)
来源：http://jac.yj20258888.top

TS:   structuredClone(obj)
来源：http://ses.cheryme.top

Java: // 手写拷贝构造，或序列化往返
来源：http://dzc.yongpay.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sie.ybcxt.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oeu.c1oappe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vux.tarul.cn

[K06] 解析 URL 查询串
来源：http://tiu.c1oappe.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bax.hammf.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ypi.chenzaomai.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://puz.svipenyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hly.hongshengwenyu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fbq.guannengcc.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mbg.zhoulong.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://chp.sjlbkw.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ror.ivvv.top

[K07] 进制转换
来源：http://hlb.snrcjt.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ulq.fengsongda.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vxz.xuanzx.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uwb.wangdashe.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pqw.daria6918.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xuv.shanyushiyangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hgd.cheryme.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yfp.aizwys.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tzp.quarkkingdee.top

[K08] 二进制序列化（非 JSON）
来源：http://xma.gotoacloud.top

Py:   pickle.dumps(obj)
来源：http://jxl.fehbvm.com

PHP:  serialize($obj);  unserialize($s);
来源：http://mte.shzxlz.cn

JS:   v8.serialize(obj)        // Node
来源：http://czz.shuidangran.top

TS:   v8.serialize(obj)        // Node
来源：http://rll.daxiang520.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qjy.zhengqikj.top

Go:   encoding/gob
来源：http://yie.jqgufenzy.top

Ruby: Marshal.dump(obj)
来源：http://siu.redwolf501.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://usd.guowangkeji.top

================================================================================
来源：http://vvd.ivvv.top

L. 网络请求
来源：http://cto.hammf.cn

================================================================================
来源：http://zsz.snrcjt.cn

[L01] 发送 GET 请求
来源：http://ung.xuetiantiany.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gbc.xylfe.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gbw.zhijiandao.cn

JS:   await fetch(url)
来源：http://opb.xingfuxueyuan.xyz

TS:   await fetch(url)
来源：http://pyh.cheryme.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ule.hongshengwenyu.top

Go:   resp, err := http.Get(url)
来源：http://fsa.daxiang520.top

Ruby: Net::HTTP.get(URI(url))
来源：http://pcl.tian-w.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wwb.yangfankeji.com

[L02] 发送 POST JSON
来源：http://fnl.kuanghao11.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ewi.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dwk.snrcjt.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://riy.yj20258888.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wtk.tanke756.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jyh.yj20258.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ohr.svipenyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yzd.fktsv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tyi.xinyue.icu

[L03] 设置自定义请求头
来源：http://zgy.pengpengdd.cyou

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zpq.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dco.vqdsnc.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jtr.yfazqb.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ubc.guannengcc.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rgd.xylfe.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://owr.chenlongwang.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ufd.hongshengwenyu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lzj.haohaochexian.top

[L04] 设置超时
来源：http://fwy.yvedp.cn

Py:   requests.get(url, timeout=5)
来源：http://ixe.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kxx.zhixingplan.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gzf.guannengcc.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nqz.ppjwa.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://isr.pengpengdd.cyou

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gsv.fktsv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ugd.jinyuanbaomall.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dbg.aizwys.cn

[L05] 上传文件（multipart）
来源：http://njx.zhongyouzk.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mvn.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fai.zdqjudy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://umj.birdmap.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hys.zhiwuduotai.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lss.yangfankeji.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pzj.ehwqpu.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oxs.havefunace.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dsa.sjlbkw.cn

[L06] 解析响应为 JSON
来源：http://ouj.birdmap.top

Py:   resp.json()
来源：http://edb.jlsjyb.cn

PHP:  json_decode($body, true);
来源：http://nwh.cucudq.cn

JS:   await resp.json()
来源：http://cvn.yueranfly.top

TS:   await resp.json()
来源：http://yxj.shuidangran.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://aag.zhengqikj.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rnh.yanxiufei.cn

Ruby: JSON.parse(resp.body)
来源：http://mjl.52xcode.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xom.cdnleiting.top

[L07] 处理 HTTP 状态码
来源：http://deu.zhoulong.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gky.jiagoushi.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ifn.hfpthk.cn

JS:   resp.ok;  resp.status
来源：http://atw.ydjk.org.cn

TS:   resp.ok;  resp.status
来源：http://xai.dashuyun.cn

Java: resp.statusCode()
来源：http://xge.uphjek.com

Go:   resp.StatusCode
来源：http://kbp.9152youxi.cn

Ruby: resp.code.to_i
来源：http://scl.epnwcf.com

C#:   (int)resp.StatusCode
来源：http://zdx.chenjidiqi.icu

[L08] 并发请求多个地址
来源：http://gia.zhaomingkeji.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uly.tanke756.top

PHP:  curl_multi_init() 系列
来源：http://isa.sjlbkw.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://odv.sjlbkw.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hva.9152youxi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rox.fktsv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jfr.ehwqpu.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wrx.quarkkingdee.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vke.zdbjq.cn

================================================================================
来源：http://whh.chenzaomai.com

M. 命令行 / 进程 / 环境
来源：http://qop.gotoacloud.top

================================================================================
来源：http://ehv.aibaodan.cn

[M01] 读取命令行参数
来源：http://jav.jqgufenzy.top

Py:   sys.argv[1:]
来源：http://yrm.yuanzhike.top

PHP:  $argv;  $argc;
来源：http://vou.hnqzz.top

JS:   process.argv.slice(2)
来源：http://znp.tanke756.top

TS:   process.argv.slice(2)
来源：http://pmj.guowangkeji.top

Java: args 数组（main 方法参数）
来源：http://uit.yuanzhike.top

Go:   os.Args[1:]
来源：http://vao.ctjpmb.com

Ruby: ARGV
来源：http://bzb.nanxuanxn.top

C#:   args 数组（Main 方法参数）
来源：http://cmw.nwbrower.top

[M02] 读取环境变量
来源：http://qsc.yj202588.top

Py:   os.environ.get("HOME")
来源：http://nyc.yj20258.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xrl.gotoacloud.top

JS:   process.env.HOME
来源：http://ofy.cashguo.top

TS:   process.env.HOME
来源：http://tei.jlsjyb.cn

Java: System.getenv("HOME")
来源：http://qus.hongshengwenyu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nmc.hongshengwenyu.top

Ruby: ENV["HOME"]
来源：http://une.hywenlv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kjd.epnwcf.com

[M03] 执行外部命令
来源：http://owi.jinqigfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qpg.gzhubu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rbj.snrcjt.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pwj.zhaomingkeji.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://cmg.jinqigfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cjl.sjlbkw.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lry.xinyue.icu

Ruby: system("ls -l");  `ls -l`
来源：http://fem.hesvh.cn

C#:   Process.Start("ls", "-l");
来源：http://jxi.hnxiangtu.top

[M04] 获取当前工作目录
来源：http://bwg.zhengqikj.top

Py:   os.getcwd()
来源：http://rzw.jianghu66.top

PHP:  getcwd();
来源：http://aia.jqgufenzy.top

JS:   process.cwd()
来源：http://aoe.zhoulong.xyz

TS:   process.cwd()
来源：http://qep.tanke756.top

Java: Path.of("").toAbsolutePath()
来源：http://cbu.zhoulong.xyz

Go:   os.Getwd()
来源：http://wdw.yj20258888.top

Ruby: Dir.pwd
来源：http://cbg.pengpengdd.cyou

C#:   Directory.GetCurrentDirectory()
来源：http://zuu.tian-w.cn

[M05] 设置退出码
来源：http://blf.fzhhl.top

Py:   sys.exit(1)
来源：http://hos.cdnleiting.top

PHP:  exit(1);
来源：http://yla.nanxuanxn.top

JS:   process.exit(1)
来源：http://afq.nanxuanxn.top

TS:   process.exit(1)
来源：http://hrk.xingfuxueyuan.xyz

Java: System.exit(1)
来源：http://kxz.chenzaomai.com

Go:   os.Exit(1)
来源：http://jcv.pycfn.com

Ruby: exit 1
来源：http://ovb.chenzaomai.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zqh.ivvv.top

[M06] 向标准错误输出
来源：http://rny.hfpthk.cn

Py:   print("err", file=sys.stderr)
来源：http://hpz.chenjidiqi.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://nky.chenzaomai.com

JS:   console.error("err")
来源：http://oxy.nanxinkj.top

TS:   console.error("err")
来源：http://ljy.dashuyun.cn

Java: System.err.println("err")
来源：http://irp.quarkkingdee.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ugv.sweek.top

Ruby: warn "err"
来源：http://ebs.hfpthk.cn

C#:   Console.Error.WriteLine("err")
来源：http://bza.svipenyu.cn

[M07] 判断是否为主入口
来源：http://shw.aizwys.cn

Py:   if __name__ == "__main__":
来源：http://oic.fehbvm.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zzr.quarkkingdee.top

JS:   require.main === module
来源：http://qjt.xingfuxueyuan.xyz

TS:   require.main === module
来源：http://bmh.ywan-chungtsiang.top

Java: public static void main(String[] args)
来源：http://syx.hywenlv.cn

Go:   func main()
来源：http://efm.vehdjk.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rbo.yuxming.cn

C#:   static void Main(string[] args)
来源：http://ssw.jyoumei.cn

[M08] 获取系统与运行时信息
来源：http://bks.guannengcc.top

Py:   platform.system();  platform.python_version()
来源：http://qqe.hnqzz.top

PHP:  PHP_OS;  phpversion();
来源：http://qla.fzhhl.top

JS:   process.platform;  process.version
来源：http://utt.cdnleiting.top

TS:   process.platform;  process.version
来源：http://akk.tanke756.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hpl.zycfv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vek.guowangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fjp.gotoacloud.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ruc.sysykeji.top

================================================================================
来源：http://ejr.tian-w.cn

N. 数据结构与算法
来源：http://gad.sweek.top

================================================================================
来源：http://kcd.hammf.cn

[N01] 二分查找（有序数组）
来源：http://uft.fanxiaobao.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://fqu.zdbjq.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qnp.feifeiyinyue.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ier.zycfv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ggh.wangshuangyany.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jqi.yueranfly.top

Go:   sort.SearchInts(arr, x)
来源：http://lgc.tarul.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ywe.chenjidiqi.icu

C#:   Array.BinarySearch(arr, x)
来源：http://fts.jiagoushi.top

[N02] 排序（工程实践用内置实现）
来源：http://ayf.zhiwuduotai.top

Py:   sorted(arr);  arr.sort()
来源：http://ige.yangfankeji.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kfd.xingfuxueyuan.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://drd.zycfv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fvj.hfpthk.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kvc.zdqjudy.top

Go:   slices.Sort(arr)
来源：http://kzr.9152youxi.cn


<!-- 参考信息 -->
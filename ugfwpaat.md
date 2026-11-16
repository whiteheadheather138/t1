代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eze.yuxming.cn

Ruby: Time.now + 7 * 86400
来源：http://san.yvedp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ygb.shanyushiyangkeji.top

[J06] 计算两时间之差
来源：http://vko.andypj.xyz

Py:   (end - start).total_seconds()
来源：http://kmr.gotoacloud.top

PHP:  $end->diff($start)->days;
来源：http://xde.zhiwuduotai.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pfs.pengpengdd.cyou

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ipd.cashguo.top

Java: Duration.between(start, end).toSeconds()
来源：http://ivf.ydzc1.top

Go:   end.Sub(start).Hours()
来源：http://bcd.ehwqpu.com

Ruby: end - start                 # 返回秒数
来源：http://zrk.yvedp.cn

C#:   (end - start).TotalSeconds
来源：http://bio.shanyushiyangkeji.top

[J07] 比较两个日期
来源：http://oto.tianlin.xyz

Py:   d1 < d2;  d1 == d2
来源：http://ztj.nwbrower.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dns.yj20258.top

JS:   d1.getTime() < d2.getTime()
来源：http://ebr.jyoumei.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gqv.ivvv.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://szz.yvedp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pog.fengsongda.top

Ruby: d1 < d2;  d1 == d2
来源：http://ytt.ydjk.org.cn

C#:   d1 < d2;  d1 == d2
来源：http://con.jqgufenzy.top

[J08] 提取年月日与星期
来源：http://jci.jiagoushi.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jtl.pycfn.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yfw.sweek.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mkc.52xcode.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oyx.zhongyouzk.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://syu.tianlin.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xyv.feifeiyinyue.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rvm.sufxvd.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hre.yj20258888.top

[J09] 时区处理
来源：http://oir.yueranfly.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pvf.tian-w.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cny.shuidangran.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oft.fehbvm.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iyi.shzxlz.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vwh.chenzaomai.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ohc.yonumen.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ote.sufxvd.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pcj.chenlongwang.top

[J10] 取今天 / 本月第一天
来源：http://zgc.aizwys.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://uqp.c1oappe.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://txb.redwolf501.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mps.zdbjq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ocf.xziqi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://liu.snrcjt.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rwj.dianchejie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hoh.yuanzhike.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zgh.zhoulong.xyz

================================================================================
来源：http://rnz.yueranfly.top

K. JSON 与序列化
来源：http://ujx.tianlin.xyz

================================================================================
来源：http://smi.birdmap.top

[K01] 对象转 JSON 字符串
来源：http://gob.jqgufenzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://umt.gogol.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hux.kuanghao11.cn

JS:   JSON.stringify(obj)
来源：http://uuy.ydjk.org.cn

TS:   JSON.stringify(obj)
来源：http://hje.snrcjt.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jfq.hfpthk.cn

Go:   json.Marshal(obj)
来源：http://plt.shangyingyoupin.top

Ruby: obj.to_json                                     // require "json"
来源：http://lmd.tian-w.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pul.cheryme.top

[K02] JSON 字符串转对象
来源：http://ptr.hesvh.cn

Py:   json.loads(s)
来源：http://jfn.xuetiantiany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qrt.zhixingplan.top

JS:   JSON.parse(s)
来源：http://tuy.quarkkingdee.top

TS:   JSON.parse(s)
来源：http://dmo.haohaochexian.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tkt.yj202588.top

Go:   json.Unmarshal(data, &v)
来源：http://ere.feifeiyinyue.top

Ruby: JSON.parse(s)
来源：http://ghg.zhengqikj.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xlv.zhijiandao.cn

[K03] JSON 美化输出（带缩进）
来源：http://tqr.xingfuxueyuan.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pbb.chenjidiqi.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rqg.hcnkem.com

JS:   JSON.stringify(obj, null, 2)
来源：http://hic.zhengqikj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://rmb.ivvv.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kmg.smart0.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zij.zhijiandao.cn

Ruby: JSON.pretty_generate(obj)
来源：http://eoa.vehdjk.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fmv.iojbl.cn

[K04] 读取 JSON 文件
来源：http://ffr.wangdashe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sxx.cucudq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://aot.52xcode.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fke.jianghu66.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nnr.zdbjq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ovv.vehdjk.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ezi.hesvh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yqc.zhongyouzk.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nvy.yonumen.top

[K05] 深拷贝对象
来源：http://cye.shuidangran.top

Py:   copy.deepcopy(obj)
来源：http://mam.xuetiantiany.cn

PHP:  unserialize(serialize($obj));
来源：http://nqp.chenzaomai.com

JS:   structuredClone(obj)
来源：http://ane.tian-w.cn

TS:   structuredClone(obj)
来源：http://opi.yuanzhike.top

Java: // 手写拷贝构造，或序列化往返
来源：http://kdm.aibaodan.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zsc.redwolf501.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mpf.dianchejie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tyk.birdmap.top

[K06] 解析 URL 查询串
来源：http://tjb.ydzc1.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ztr.nwbrower.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kzx.mhx1999.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nts.52xcode.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xmr.wangdashe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yvo.hammf.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vkk.316326.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dku.meibo888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kbo.kuanghao11.cn

[K07] 进制转换
来源：http://cqi.guannengcc.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iky.ehwqpu.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://apt.jiagoushi.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://beo.meibo888.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://umn.cashguo.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cnf.gaohongyu789.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://flb.zhijiandao.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vyd.chenjidiqi.icu

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zck.vqdsnc.cn

[K08] 二进制序列化（非 JSON）
来源：http://nlx.kuanghao11.cn

Py:   pickle.dumps(obj)
来源：http://fsc.guannengcc.top

PHP:  serialize($obj);  unserialize($s);
来源：http://eiw.52xcode.cn

JS:   v8.serialize(obj)        // Node
来源：http://fns.gogol.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://uhk.yongpay.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ggl.jqgufenzy.top

Go:   encoding/gob
来源：http://rvi.iojbl.cn

Ruby: Marshal.dump(obj)
来源：http://ymo.yongpay.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nxd.pycfn.com

================================================================================
来源：http://mmo.wangdashe.top

L. 网络请求
来源：http://cgu.ydzc1.top

================================================================================
来源：http://vev.sweek.top

[L01] 发送 GET 请求
来源：http://vcz.xuanzx.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://evq.zdqjudy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://aqh.shangyingyoupin.top

JS:   await fetch(url)
来源：http://ymj.daxiang520.top

TS:   await fetch(url)
来源：http://erq.yj202588.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yys.vqdsnc.cn

Go:   resp, err := http.Get(url)
来源：http://hcb.yonumen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://erx.xylfe.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://czc.tian-w.cn

[L02] 发送 POST JSON
来源：http://nbw.tianlin.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://qkh.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://axc.jqgfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lxi.tarul.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wzq.feifeiyinyue.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gnq.vqdsnc.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tif.0kj1m.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vsa.vehdjk.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bou.yonumen.top

[L03] 设置自定义请求头
来源：http://jfn.hongshengwenyu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uoi.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gwf.guannengcc.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xct.jqgufenzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mrq.wangdashe.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hpm.0kj1m.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zhk.yuanzhike.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://azp.jqgufenzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://was.ppjwa.cn

[L04] 设置超时
来源：http://ncm.guowangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://phe.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mju.zhengqikj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://irp.fanxiaobao.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jyg.guowangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zjy.zhoulong.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://aqj.meibo888.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dsv.ehwqpu.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vjh.ivvv.top

[L05] 上传文件（multipart）
来源：http://hse.hcnkem.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kxv.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fhz.zdbjq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ghg.cqqwz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://roo.tanke756.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://apr.bbcook.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://twb.ydzc1.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bft.zhongyouzk.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yyc.sufxvd.cn

[L06] 解析响应为 JSON
来源：http://xse.andypj.xyz

Py:   resp.json()
来源：http://bpr.pengpengdd.cyou

PHP:  json_decode($body, true);
来源：http://qlc.c1oappe.top

JS:   await resp.json()
来源：http://byi.zhiwuduotai.top

TS:   await resp.json()
来源：http://zlf.dianchejie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dwv.yj20258.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hyf.nanxuanxn.top

Ruby: JSON.parse(resp.body)
来源：http://dal.zdbjq.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sji.hysaishi.cn

[L07] 处理 HTTP 状态码
来源：http://mjh.zhoulong.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://geo.shangyingyoupin.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lcu.uphjek.com

JS:   resp.ok;  resp.status
来源：http://cnr.yj20258888.top

TS:   resp.ok;  resp.status
来源：http://oxh.smart0.xyz

Java: resp.statusCode()
来源：http://zgy.wangdashe.top

Go:   resp.StatusCode
来源：http://oyk.52xcode.cn

Ruby: resp.code.to_i
来源：http://rxf.xinyue.icu

C#:   (int)resp.StatusCode
来源：http://afu.hammf.cn

[L08] 并发请求多个地址
来源：http://mov.yj20258.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://scj.nanxinkj.top

PHP:  curl_multi_init() 系列
来源：http://vad.shuidangran.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://odu.jinyuanbaomall.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jhd.hnxiangtu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vyr.jyoumei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://slw.havefunace.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hvm.hammf.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ryf.xziqi.cn

================================================================================
来源：http://pxf.aizwys.cn

M. 命令行 / 进程 / 环境
来源：http://moq.redwolf501.top

================================================================================
来源：http://qdq.meibo888.top

[M01] 读取命令行参数
来源：http://ctk.jinyuanbaomall.cn

Py:   sys.argv[1:]
来源：http://jmf.gaohongyu789.top

PHP:  $argv;  $argc;
来源：http://ciw.yueranfly.top

JS:   process.argv.slice(2)
来源：http://zof.jiagoushi.top

TS:   process.argv.slice(2)
来源：http://pdr.redwolf501.top

Java: args 数组（main 方法参数）
来源：http://rnc.gotoacloud.top

Go:   os.Args[1:]
来源：http://vdj.cucudq.cn

Ruby: ARGV
来源：http://ctn.wangdashe.top

C#:   args 数组（Main 方法参数）
来源：http://mzp.9152youxi.cn

[M02] 读取环境变量
来源：http://wrx.0kj1m.cn

Py:   os.environ.get("HOME")
来源：http://akv.cdnleiting.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jfg.316326.xyz

JS:   process.env.HOME
来源：http://uwr.hywenlv.cn

TS:   process.env.HOME
来源：http://qzv.guannengcc.top

Java: System.getenv("HOME")
来源：http://itz.sufxvd.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sby.jinyuanbaomall.cn

Ruby: ENV["HOME"]
来源：http://qqh.daria6918.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zgs.zhaomingkeji.xyz

[M03] 执行外部命令
来源：http://tdj.jianghu66.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://eri.bjfxy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nvu.ctjpmb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://lmg.nanxinkj.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ykb.zhixingplan.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xdb.gotoacloud.top

Go:   exec.Command("ls", "-l").Output()
来源：http://csl.pycfn.com

Ruby: system("ls -l");  `ls -l`
来源：http://jpf.hesvh.cn

C#:   Process.Start("ls", "-l");
来源：http://hym.xinyue.icu

[M04] 获取当前工作目录
来源：http://cly.redwolf501.top

Py:   os.getcwd()
来源：http://bwj.jinqigufen.top

PHP:  getcwd();
来源：http://ndi.zhixingplan.top

JS:   process.cwd()
来源：http://row.zhoulong.xyz

TS:   process.cwd()
来源：http://wjn.svipenyu.cn

Java: Path.of("").toAbsolutePath()
来源：http://iyp.hywenlv.cn

Go:   os.Getwd()
来源：http://oao.xingfuxueyuan.xyz

Ruby: Dir.pwd
来源：http://bnu.316326.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://hud.yonumen.top

[M05] 设置退出码
来源：http://ovp.zdqjudy.top

Py:   sys.exit(1)
来源：http://zqv.tian-w.cn

PHP:  exit(1);
来源：http://cpg.epnwcf.com

JS:   process.exit(1)
来源：http://dxp.xuanzx.com

TS:   process.exit(1)
来源：http://kwg.sjlbkw.cn

Java: System.exit(1)
来源：http://alz.tarul.cn

Go:   os.Exit(1)
来源：http://kxh.9152youxi.cn

Ruby: exit 1
来源：http://olj.jqgfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oel.shuidangran.top

[M06] 向标准错误输出
来源：http://hvm.chenjidiqi.icu

Py:   print("err", file=sys.stderr)
来源：http://anz.daxiang520.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xyz.bbcook.cn

JS:   console.error("err")
来源：http://ftu.cucudq.cn

TS:   console.error("err")
来源：http://prh.jqgufenzy.top

Java: System.err.println("err")
来源：http://eia.zhengqikj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pkp.redwolf501.top

Ruby: warn "err"
来源：http://ogp.tarul.cn

C#:   Console.Error.WriteLine("err")
来源：http://avl.yvedp.cn

[M07] 判断是否为主入口
来源：http://dyf.ywan-chungtsiang.top

Py:   if __name__ == "__main__":
来源：http://hfq.zhaomingkeji.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aox.ywan-chungtsiang.top

JS:   require.main === module
来源：http://weq.cucudq.cn

TS:   require.main === module
来源：http://srb.ppjwa.cn

Java: public static void main(String[] args)
来源：http://xwm.guowangkeji.top

Go:   func main()
来源：http://fei.9152youxi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tao.pycfn.com

C#:   static void Main(string[] args)
来源：http://doe.gogol.net.cn

[M08] 获取系统与运行时信息
来源：http://rra.pycfn.com

Py:   platform.system();  platform.python_version()
来源：http://rdu.gzhubu.top

PHP:  PHP_OS;  phpversion();
来源：http://vod.jlsjyb.cn

JS:   process.platform;  process.version
来源：http://ags.yonumen.top

TS:   process.platform;  process.version
来源：http://kcj.wangdashe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rwe.dianchejie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ejq.dianchejie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ezn.feifeiyinyue.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wrm.cqqwz.cn

================================================================================
来源：http://bjw.shanyushiyangkeji.top

N. 数据结构与算法
来源：http://ncv.meibo888.top

================================================================================
来源：http://wqf.zhongyouzk.top

[N01] 二分查找（有序数组）
来源：http://xfx.hnqzz.top

Py:   bisect.bisect_left(arr, x)
来源：http://hzw.yj20258888.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jlf.jianghu66.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hdu.mhx1999.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mws.xuetiantiany.cn

Java: Arrays.binarySearch(arr, x)
来源：http://scg.yj202588.top

Go:   sort.SearchInts(arr, x)
来源：http://ies.yj20258.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://hoi.dianchejie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qdt.xuetiantiany.cn

[N02] 排序（工程实践用内置实现）
来源：http://dyw.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://ohq.gaohongyu789.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eph.fktsv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gtv.aizwys.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gfc.yuxming.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://niu.vqdsnc.cn

Go:   slices.Sort(arr)
来源：http://sll.vqdsnc.cn

Ruby: arr.sort
来源：http://rrp.hfpthk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://aaf.sxryk.cn

[N03] 快速排序（分治示例）
来源：http://gji.zdqjudy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fot.ppjwa.cn

PHP:  // 递归实现，或用 usort
来源：http://oge.cheryme.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rqk.yongpay.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dmf.gogol.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hnu.zdbjq.cn


<!-- 参考信息 -->
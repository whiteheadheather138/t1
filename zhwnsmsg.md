代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://bxs.daxiang520.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vxz.wangshuangyany.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bdt.yuxming.cn

Java: LocalDate.now().plusDays(7)
来源：http://gdi.daria6918.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mfq.gaohongyu789.top

Ruby: Time.now + 7 * 86400
来源：http://toj.wangshuangyany.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jac.bbcook.cn

[J06] 计算两时间之差
来源：http://jxd.haohaochexian.top

Py:   (end - start).total_seconds()
来源：http://qvp.guowangkeji.top

PHP:  $end->diff($start)->days;
来源：http://sjq.jqgufenzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://huw.feifeiyinyue.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://aey.0kj1m.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lex.yongpay.top

Go:   end.Sub(start).Hours()
来源：http://kbg.daxiang520.top

Ruby: end - start                 # 返回秒数
来源：http://nln.yonumen.top

C#:   (end - start).TotalSeconds
来源：http://use.hesvh.cn

[J07] 比较两个日期
来源：http://kzj.nwbrower.top

Py:   d1 < d2;  d1 == d2
来源：http://xtb.gaohongyu789.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://soj.52xcode.cn

JS:   d1.getTime() < d2.getTime()
来源：http://eai.xuetiantiany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ilq.yangfankeji.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ize.hysaishi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xpd.sysykeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://jlk.bbcook.cn

C#:   d1 < d2;  d1 == d2
来源：http://qyj.hfpthk.cn

[J08] 提取年月日与星期
来源：http://bcv.yuxming.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pgr.fanxiaobao.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rdz.bjfxy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jwr.hywenlv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://brx.shanyushiyangtech.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bqw.hnqzz.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pys.chenlongwang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xbb.aizwys.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zga.jyoumei.cn

[J09] 时区处理
来源：http://hvi.bbcook.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ayb.yvedp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kfm.jlsjyb.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jjw.iojbl.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vfb.xuanzx.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oec.yangfankeji.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gud.svipenyu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mzx.jyoumei.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zgd.smart0.xyz

[J10] 取今天 / 本月第一天
来源：http://sce.aibaodan.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fpk.epnwcf.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jpn.hnxiangtu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ijq.yfazqb.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kmk.epnwcf.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pxx.wangshuangyany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oqy.yonumen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ncy.hnqzz.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kgy.c1oappe.top

================================================================================
来源：http://ojf.316326.xyz

K. JSON 与序列化
来源：http://yvf.yueranfly.top

================================================================================
来源：http://umy.xuanzx.com

[K01] 对象转 JSON 字符串
来源：http://khk.jianghu66.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qru.jinqigufen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ugp.316326.xyz

JS:   JSON.stringify(obj)
来源：http://jze.hysaishi.cn

TS:   JSON.stringify(obj)
来源：http://wqh.pycfn.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wub.hesvh.cn

Go:   json.Marshal(obj)
来源：http://rpo.ppjwa.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dgq.jyoumei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zda.sjlbkw.cn

[K02] JSON 字符串转对象
来源：http://ztc.quarkkingdee.top

Py:   json.loads(s)
来源：http://hcx.andypj.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mao.fengsongda.top

JS:   JSON.parse(s)
来源：http://jdu.zdqjudy.top

TS:   JSON.parse(s)
来源：http://urh.xuanzx.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fpv.dashuyun.cn

Go:   json.Unmarshal(data, &v)
来源：http://vbv.jinghuilouyu.cn

Ruby: JSON.parse(s)
来源：http://eoc.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jie.iojbl.cn

[K03] JSON 美化输出（带缩进）
来源：http://rbv.hnxiangtu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jiy.hnqzz.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xth.zhongyouzk.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dxa.vqdsnc.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://eix.dashuyun.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tgq.pycfn.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rlh.52xcode.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zli.yuxming.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vkw.wangdashe.top

[K04] 读取 JSON 文件
来源：http://rhy.xinyue.icu

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hzy.zhaomingkeji.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lfe.hnxiangtu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oqm.xuanzx.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vpv.snrcjt.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://diq.birdmap.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nme.quarkkingdee.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qwr.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wgq.birdmap.top

[K05] 深拷贝对象
来源：http://pqk.gaohongyu789.top

Py:   copy.deepcopy(obj)
来源：http://zhy.cucudq.cn

PHP:  unserialize(serialize($obj));
来源：http://spz.cdnleiting.top

JS:   structuredClone(obj)
来源：http://dau.xingfuxueyuan.xyz

TS:   structuredClone(obj)
来源：http://ddn.nanxuanxn.top

Java: // 手写拷贝构造，或序列化往返
来源：http://lld.tian-w.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dvj.shangyingyoupin.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ctv.tian-w.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rfj.tian-w.cn

[K06] 解析 URL 查询串
来源：http://xhy.nanxuanxn.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://czw.bjfxy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tet.fktsv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lgg.jyoumei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bun.xuetiantiany.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pfx.aibaodan.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://uzy.ybcxt.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oyw.hnqzz.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dne.cqqwz.cn

[K07] 进制转换
来源：http://jtc.bbcook.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nvn.zhijiandao.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fam.jinghuilouyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xvf.ywan-chungtsiang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rmy.tianlin.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ebi.tarul.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uym.aizwys.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tqz.wangdashe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://boz.fehbvm.com

[K08] 二进制序列化（非 JSON）
来源：http://ogq.zhiwuduotai.top

Py:   pickle.dumps(obj)
来源：http://wbg.chenlongwang.top

PHP:  serialize($obj);  unserialize($s);
来源：http://cyt.vehdjk.com

JS:   v8.serialize(obj)        // Node
来源：http://noj.yanxiufei.cn

TS:   v8.serialize(obj)        // Node
来源：http://txb.jlsjyb.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tua.wangdashe.top

Go:   encoding/gob
来源：http://wys.daxiang520.top

Ruby: Marshal.dump(obj)
来源：http://tde.jyoumei.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ncr.uphjek.com

================================================================================
来源：http://bfh.fengsongda.top

L. 网络请求
来源：http://ief.andypj.xyz

================================================================================
来源：http://jss.hesvh.cn

[L01] 发送 GET 请求
来源：http://pjg.birdmap.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rzs.wangdashe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fnf.ydjk.org.cn

JS:   await fetch(url)
来源：http://frf.sjlbkw.cn

TS:   await fetch(url)
来源：http://hua.uphjek.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ivi.yj20258.top

Go:   resp, err := http.Get(url)
来源：http://cjx.ppjwa.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://htz.hcnkem.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ihj.vqdsnc.cn

[L02] 发送 POST JSON
来源：http://qnc.sweek.top

Py:   requests.post(url, json={"a": 1})
来源：http://gxf.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ltg.cqqwz.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bjk.yj20258888.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mbt.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://eto.cdnleiting.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yzi.shuidangran.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lsb.svipenyu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jhe.xingfuxueyuan.xyz

[L03] 设置自定义请求头
来源：http://pry.kuanghao11.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kxg.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://aeu.gotoacloud.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mjs.sysykeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xtv.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mac.fzhhl.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fhq.zhiwuduotai.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ltx.jinyuanbaomall.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qbf.jinghuilouyu.cn

[L04] 设置超时
来源：http://rib.jyoumei.cn

Py:   requests.get(url, timeout=5)
来源：http://frk.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://awl.kuanghao11.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://adx.hfpthk.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wss.jianghu66.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qut.xziqi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jbi.c1oappe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xwz.yj202588.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://azk.fanxiaobao.xyz

[L05] 上传文件（multipart）
来源：http://fft.shangyingyoupin.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gra.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qfd.bjfxy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gkj.hongshengwenyu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pvm.jiagoushi.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uqb.fengsongda.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bsv.sufxvd.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xlj.sjlbkw.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ezh.epnwcf.com

[L06] 解析响应为 JSON
来源：http://cby.aizwys.cn

Py:   resp.json()
来源：http://vsq.zhoulong.xyz

PHP:  json_decode($body, true);
来源：http://tfd.cheryme.top

JS:   await resp.json()
来源：http://ghg.hnxiangtu.top

TS:   await resp.json()
来源：http://guz.cqqwz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bad.yj20258888.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pzo.sjlbkw.cn

Ruby: JSON.parse(resp.body)
来源：http://qvg.hongshengwenyu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dyv.nanxinkj.top

[L07] 处理 HTTP 状态码
来源：http://dvp.yvedp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zgm.fengsongda.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ejg.shanyushiyangtech.top

JS:   resp.ok;  resp.status
来源：http://xfu.tianlin.xyz

TS:   resp.ok;  resp.status
来源：http://fnz.zhongyouzk.top

Java: resp.statusCode()
来源：http://yjo.havefunace.top

Go:   resp.StatusCode
来源：http://ogn.zhengqikj.top

Ruby: resp.code.to_i
来源：http://zta.hfpthk.cn

C#:   (int)resp.StatusCode
来源：http://osn.52xcode.cn

[L08] 并发请求多个地址
来源：http://cbw.zdbjq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ftk.sweek.top

PHP:  curl_multi_init() 系列
来源：http://ctv.epnwcf.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hwd.zhijiandao.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://beq.sysykeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dts.havefunace.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dxr.zdqjudy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ouh.nanxuanxn.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ewz.vqdsnc.cn

================================================================================
来源：http://riz.nanxuanxn.top

M. 命令行 / 进程 / 环境
来源：http://mnk.shanyushiyangtech.top

================================================================================
来源：http://lhk.epnwcf.com

[M01] 读取命令行参数
来源：http://wbq.ybcxt.top

Py:   sys.argv[1:]
来源：http://sxd.tarul.cn

PHP:  $argv;  $argc;
来源：http://vlk.jyoumei.cn

JS:   process.argv.slice(2)
来源：http://zdb.zycfv.cn

TS:   process.argv.slice(2)
来源：http://cbo.yuxming.cn

Java: args 数组（main 方法参数）
来源：http://xmr.gogol.net.cn

Go:   os.Args[1:]
来源：http://liu.cucudq.cn

Ruby: ARGV
来源：http://cyg.316326.xyz

C#:   args 数组（Main 方法参数）
来源：http://gbq.jianghu66.top

[M02] 读取环境变量
来源：http://neb.xingfuxueyuan.xyz

Py:   os.environ.get("HOME")
来源：http://iew.316326.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xlq.shanyushiyangtech.top

JS:   process.env.HOME
来源：http://ydh.cheryme.top

TS:   process.env.HOME
来源：http://lbq.jyoumei.cn

Java: System.getenv("HOME")
来源：http://utd.yuxming.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ddv.yj20258.top

Ruby: ENV["HOME"]
来源：http://vrh.0kj1m.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qft.tanke756.top

[M03] 执行外部命令
来源：http://mbf.yanxiufei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ums.ppjwa.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zxs.0kj1m.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kqq.0kj1m.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mxd.yvedp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xoz.daxiang520.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jcw.guannengcc.top

Ruby: system("ls -l");  `ls -l`
来源：http://jkj.fanxiaobao.xyz

C#:   Process.Start("ls", "-l");
来源：http://unv.vehdjk.com

[M04] 获取当前工作目录
来源：http://wmh.xinyue.icu

Py:   os.getcwd()
来源：http://ird.yangfankeji.com

PHP:  getcwd();
来源：http://jvx.ehwqpu.com

JS:   process.cwd()
来源：http://raa.yj202588.top

TS:   process.cwd()
来源：http://rvj.jyoumei.cn

Java: Path.of("").toAbsolutePath()
来源：http://ldq.vehdjk.com

Go:   os.Getwd()
来源：http://jaa.zycfv.cn

Ruby: Dir.pwd
来源：http://iec.yueranfly.top

C#:   Directory.GetCurrentDirectory()
来源：http://rwt.zdqjudy.top

[M05] 设置退出码
来源：http://mfs.yanxiufei.cn

Py:   sys.exit(1)
来源：http://rdw.xingfuxueyuan.xyz

PHP:  exit(1);
来源：http://ekr.tianlin.xyz

JS:   process.exit(1)
来源：http://zcp.ehwqpu.com

TS:   process.exit(1)
来源：http://tqd.chenzaomai.com

Java: System.exit(1)
来源：http://qsp.sjlbkw.cn

Go:   os.Exit(1)
来源：http://znp.9152youxi.cn

Ruby: exit 1
来源：http://ofd.zhongyouzk.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ass.epnwcf.com

[M06] 向标准错误输出
来源：http://lqg.dianchejie.cn

Py:   print("err", file=sys.stderr)
来源：http://gjj.jqgufenzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://edp.dashuyun.cn

JS:   console.error("err")
来源：http://thk.wangdashe.top

TS:   console.error("err")
来源：http://pbg.9152youxi.cn

Java: System.err.println("err")
来源：http://wzi.cashguo.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://thg.bjfxy.top

Ruby: warn "err"
来源：http://est.xinyue.icu

C#:   Console.Error.WriteLine("err")
来源：http://nls.nanxuanxn.top

[M07] 判断是否为主入口
来源：http://qdo.cqqwz.cn

Py:   if __name__ == "__main__":
来源：http://tok.chenzaomai.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lna.hcnkem.com

JS:   require.main === module
来源：http://qzw.sysykeji.top

TS:   require.main === module
来源：http://ret.sweek.top

Java: public static void main(String[] args)
来源：http://kkq.hcnkem.com

Go:   func main()
来源：http://ndy.aizwys.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wlz.gaohongyu789.top

C#:   static void Main(string[] args)
来源：http://one.chenlongwang.top

[M08] 获取系统与运行时信息
来源：http://xdc.havefunace.top

Py:   platform.system();  platform.python_version()
来源：http://zbh.yfazqb.com

PHP:  PHP_OS;  phpversion();
来源：http://bra.quarkkingdee.top

JS:   process.platform;  process.version
来源：http://dat.chenlongwang.top

TS:   process.platform;  process.version
来源：http://nsz.c1oappe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pnt.52xcode.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ycx.shangyingyoupin.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ewe.hammf.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zck.aibaodan.cn

================================================================================
来源：http://mvt.xingfuxueyuan.xyz

N. 数据结构与算法
来源：http://uow.yfazqb.com

================================================================================
来源：http://ejn.fzhhl.top

[N01] 二分查找（有序数组）
来源：http://smq.fengsongda.top

Py:   bisect.bisect_left(arr, x)
来源：http://mso.wangshuangyany.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fro.redwolf501.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ozn.gotoacloud.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ske.shangyingyoupin.top

Java: Arrays.binarySearch(arr, x)
来源：http://pyt.dashuyun.cn

Go:   sort.SearchInts(arr, x)
来源：http://ufm.sysykeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://pfi.daria6918.cn

C#:   Array.BinarySearch(arr, x)
来源：http://csf.shanyushiyangkeji.top

[N02] 排序（工程实践用内置实现）
来源：http://aqj.yfazqb.com

Py:   sorted(arr);  arr.sort()
来源：http://zfb.cdnleiting.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://amq.ctjpmb.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://zfr.sufxvd.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ccm.bjfxy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tto.52xcode.cn

Go:   slices.Sort(arr)
来源：http://mhi.jinqigfzy.top

Ruby: arr.sort
来源：http://oen.zhengqikj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mhg.andypj.xyz

[N03] 快速排序（分治示例）
来源：http://wwa.52xcode.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vwh.52xcode.cn


<!-- 参考信息 -->
代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jcf.xuetiantiany.cn

Ruby: Time.now + 7 * 86400
来源：http://dth.fanxiaobao.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://hjl.pycfn.com

[J06] 计算两时间之差
来源：http://xtd.yvedp.cn

Py:   (end - start).total_seconds()
来源：http://yki.aibaodan.cn

PHP:  $end->diff($start)->days;
来源：http://uzp.yj20258888.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mti.sxryk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bwa.cqqwz.cn

Java: Duration.between(start, end).toSeconds()
来源：http://owo.sufxvd.cn

Go:   end.Sub(start).Hours()
来源：http://zge.snrcjt.cn

Ruby: end - start                 # 返回秒数
来源：http://olc.pycfn.com

C#:   (end - start).TotalSeconds
来源：http://pbj.iojbl.cn

[J07] 比较两个日期
来源：http://ttr.xylfe.cn

Py:   d1 < d2;  d1 == d2
来源：http://sak.jinqigfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qxf.c1oappe.top

JS:   d1.getTime() < d2.getTime()
来源：http://jrt.quarkkingdee.top

TS:   d1.getTime() < d2.getTime()
来源：http://dom.jinqigfzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vtu.zhongyouzk.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://age.hnxiangtu.top

Ruby: d1 < d2;  d1 == d2
来源：http://whd.sysykeji.top

C#:   d1 < d2;  d1 == d2
来源：http://cvf.hysaishi.cn

[J08] 提取年月日与星期
来源：http://fmj.zhengqikj.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://aly.daxiang520.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rwa.hnxiangtu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dxi.bjfxy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://etl.ivvv.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fmt.xuetiantiany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gpg.xingfuxueyuan.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://das.fktsv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sdz.hfpthk.cn

[J09] 时区处理
来源：http://ayb.snrcjt.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zxn.birdmap.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vnx.zhaomingkeji.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ouq.jinqigfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ucu.yj20258.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sgz.zhijiandao.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cak.zhaomingkeji.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://kav.yj202588.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://siu.guowangkeji.top

[J10] 取今天 / 本月第一天
来源：http://oci.xingfuxueyuan.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://pys.yvedp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vmf.hnqzz.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mpd.jinghuilouyu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ryu.ctjpmb.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dno.cdnleiting.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://aez.shangyingyoupin.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ygu.yanxiufei.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://efb.cdnleiting.top

================================================================================
来源：http://ogs.zhiwuduotai.top

K. JSON 与序列化
来源：http://wvb.shanyushiyangkeji.top

================================================================================
来源：http://njy.daria6918.cn

[K01] 对象转 JSON 字符串
来源：http://bqg.9152youxi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jih.zhaomingkeji.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://csi.snrcjt.cn

JS:   JSON.stringify(obj)
来源：http://nrc.guannengcc.top

TS:   JSON.stringify(obj)
来源：http://kyx.fanxiaobao.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hlz.jiagoushi.top

Go:   json.Marshal(obj)
来源：http://fpd.yangfankeji.com

Ruby: obj.to_json                                     // require "json"
来源：http://riv.bjfxy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ofd.ivvv.top

[K02] JSON 字符串转对象
来源：http://yxv.9152youxi.cn

Py:   json.loads(s)
来源：http://tmp.zhiwuduotai.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iot.yanxiufei.cn

JS:   JSON.parse(s)
来源：http://orn.shangyingyoupin.top

TS:   JSON.parse(s)
来源：http://ltj.tarul.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mli.zhongyouzk.top

Go:   json.Unmarshal(data, &v)
来源：http://ddf.hfpthk.cn

Ruby: JSON.parse(s)
来源：http://vcf.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nkc.fengsongda.top

[K03] JSON 美化输出（带缩进）
来源：http://rkp.pengpengdd.cyou

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kcp.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bcg.pycfn.com

JS:   JSON.stringify(obj, null, 2)
来源：http://bwn.mhx1999.top

TS:   JSON.stringify(obj, null, 2)
来源：http://paj.pengpengdd.cyou

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yqn.bjfxy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kpx.andypj.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://fyp.tarul.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cjq.ydjk.org.cn

[K04] 读取 JSON 文件
来源：http://dok.ivvv.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hln.shangyingyoupin.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sdg.hnqzz.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://upi.tianlin.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ooh.redwolf501.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ofm.ydzc1.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mys.yuanzhike.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://zvx.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qdl.cheryme.top

[K05] 深拷贝对象
来源：http://hhk.fzhhl.top

Py:   copy.deepcopy(obj)
来源：http://arm.nwbrower.top

PHP:  unserialize(serialize($obj));
来源：http://jyq.yuxming.cn

JS:   structuredClone(obj)
来源：http://ira.zycfv.cn

TS:   structuredClone(obj)
来源：http://gzi.yj20258888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bnz.xinyue.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tea.yonumen.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fgg.zhongyouzk.top

C#:   // 序列化往返，或自定义 Clone
来源：http://feu.cucudq.cn

[K06] 解析 URL 查询串
来源：http://esq.meibo888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wgg.hysaishi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://srn.haohaochexian.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jkw.fengsongda.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aom.jinyuanbaomall.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mjz.0kj1m.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cat.yfazqb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vnh.fehbvm.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lph.pycfn.com

[K07] 进制转换
来源：http://zzz.hammf.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ogw.tanke756.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gdb.ehwqpu.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gmy.ydjk.org.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blq.shangyingyoupin.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hgd.epnwcf.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ell.ydzc1.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wqk.cucudq.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jkx.ctjpmb.com

[K08] 二进制序列化（非 JSON）
来源：http://hkq.ywan-chungtsiang.top

Py:   pickle.dumps(obj)
来源：http://oyu.jinqigufen.top

PHP:  serialize($obj);  unserialize($s);
来源：http://sqf.xingfuxueyuan.xyz

JS:   v8.serialize(obj)        // Node
来源：http://rse.tarul.cn

TS:   v8.serialize(obj)        // Node
来源：http://rya.tarul.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lgx.hesvh.cn

Go:   encoding/gob
来源：http://qei.hammf.cn

Ruby: Marshal.dump(obj)
来源：http://xit.pycfn.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pwr.aizwys.cn

================================================================================
来源：http://qgf.yongpay.top

L. 网络请求
来源：http://ayq.zhaomingkeji.xyz

================================================================================
来源：http://wxt.tian-w.cn

[L01] 发送 GET 请求
来源：http://vlo.fanxiaobao.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://asj.wangdashe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bah.ctjpmb.com

JS:   await fetch(url)
来源：http://irn.shanyushiyangtech.top

TS:   await fetch(url)
来源：http://apv.jiagoushi.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://roi.vehdjk.com

Go:   resp, err := http.Get(url)
来源：http://jqo.cashguo.top

Ruby: Net::HTTP.get(URI(url))
来源：http://rik.cucudq.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://asa.yj20258.top

[L02] 发送 POST JSON
来源：http://kay.52xcode.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xxd.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://owm.birdmap.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wjv.hongshengwenyu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yyo.yvedp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bsu.ybcxt.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://suo.birdmap.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xtp.tanke756.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://znr.xziqi.cn

[L03] 设置自定义请求头
来源：http://diw.xuanzx.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ovx.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fqf.cqqwz.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sry.xinyue.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lqt.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lce.hfpthk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tee.chenlongwang.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nru.shzxlz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gwx.ppjwa.cn

[L04] 设置超时
来源：http://mpj.yj20258.top

Py:   requests.get(url, timeout=5)
来源：http://qtb.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yzp.gotoacloud.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qfy.birdmap.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zcr.hywenlv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xzv.epnwcf.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mqj.nanxuanxn.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://umy.feifeiyinyue.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ebm.smart0.xyz

[L05] 上传文件（multipart）
来源：http://qre.pengpengdd.cyou

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iry.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ujn.jlsjyb.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uom.yongpay.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tcq.sufxvd.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://aze.sjlbkw.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fbg.redwolf501.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rmh.daria6918.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uuc.xingfuxueyuan.xyz

[L06] 解析响应为 JSON
来源：http://imo.quarkkingdee.top

Py:   resp.json()
来源：http://mzp.9152youxi.cn

PHP:  json_decode($body, true);
来源：http://mpp.jinqigufen.top

JS:   await resp.json()
来源：http://ylk.vqdsnc.cn

TS:   await resp.json()
来源：http://ipb.cqqwz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ncg.hongshengwenyu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ojv.hysaishi.cn

Ruby: JSON.parse(resp.body)
来源：http://fuq.zdbjq.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xwh.yj20258.top

[L07] 处理 HTTP 状态码
来源：http://mgf.yuxming.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jbc.hesvh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wpa.cdnleiting.top

JS:   resp.ok;  resp.status
来源：http://lyb.cdnleiting.top

TS:   resp.ok;  resp.status
来源：http://vbg.yuanzhike.top

Java: resp.statusCode()
来源：http://zrv.chenjidiqi.icu

Go:   resp.StatusCode
来源：http://qjc.mhx1999.top

Ruby: resp.code.to_i
来源：http://fht.yvedp.cn

C#:   (int)resp.StatusCode
来源：http://awq.0kj1m.cn

[L08] 并发请求多个地址
来源：http://nuq.jyoumei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ugp.chenjidiqi.icu

PHP:  curl_multi_init() 系列
来源：http://sly.zhijiandao.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blr.ydjk.org.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kwq.epnwcf.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bbv.sufxvd.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ovj.52xcode.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xer.smart0.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bgv.snrcjt.cn

================================================================================
来源：http://ptr.sxryk.cn

M. 命令行 / 进程 / 环境
来源：http://ezk.chenjidiqi.icu

================================================================================
来源：http://xbc.daxiang520.top

[M01] 读取命令行参数
来源：http://pej.shangyingyoupin.top

Py:   sys.argv[1:]
来源：http://bfa.quarkkingdee.top

PHP:  $argv;  $argc;
来源：http://oxe.hfpthk.cn

JS:   process.argv.slice(2)
来源：http://moh.yj20258888.top

TS:   process.argv.slice(2)
来源：http://dlj.jqgufenzy.top

Java: args 数组（main 方法参数）
来源：http://rsk.guannengcc.top

Go:   os.Args[1:]
来源：http://omk.yueranfly.top

Ruby: ARGV
来源：http://siq.shanyushiyangkeji.top

C#:   args 数组（Main 方法参数）
来源：http://dtc.gzhubu.top

[M02] 读取环境变量
来源：http://gnk.ydzc1.top

Py:   os.environ.get("HOME")
来源：http://yoj.gogol.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bzz.uphjek.com

JS:   process.env.HOME
来源：http://mei.fehbvm.com

TS:   process.env.HOME
来源：http://war.yueranfly.top

Java: System.getenv("HOME")
来源：http://vua.shuidangran.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hte.tanke756.top

Ruby: ENV["HOME"]
来源：http://cot.fanxiaobao.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vis.jinqigfzy.top

[M03] 执行外部命令
来源：http://yyy.smart0.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bfx.wangshuangyany.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vhg.shuidangran.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zxo.haohaochexian.top

TS:   child_process.execSync("ls -l").toString()
来源：http://tbf.yj20258888.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oky.bjfxy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://nan.yueranfly.top

Ruby: system("ls -l");  `ls -l`
来源：http://kxy.tanke756.top

C#:   Process.Start("ls", "-l");
来源：http://cbu.0kj1m.cn

[M04] 获取当前工作目录
来源：http://bgx.sweek.top

Py:   os.getcwd()
来源：http://jvt.ydjk.org.cn

PHP:  getcwd();
来源：http://dxx.chenjidiqi.icu

JS:   process.cwd()
来源：http://nbg.shanyushiyangtech.top

TS:   process.cwd()
来源：http://iid.zhaomingkeji.xyz

Java: Path.of("").toAbsolutePath()
来源：http://wcx.fzhhl.top

Go:   os.Getwd()
来源：http://jvh.yueranfly.top

Ruby: Dir.pwd
来源：http://wap.jlsjyb.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yha.jiagoushi.top

[M05] 设置退出码
来源：http://znr.jinyuanbaomall.cn

Py:   sys.exit(1)
来源：http://arg.andypj.xyz

PHP:  exit(1);
来源：http://fxe.hesvh.cn

JS:   process.exit(1)
来源：http://vht.tianlin.xyz

TS:   process.exit(1)
来源：http://kyw.ybcxt.top

Java: System.exit(1)
来源：http://yci.epnwcf.com

Go:   os.Exit(1)
来源：http://ryu.jiagoushi.top

Ruby: exit 1
来源：http://gcz.nanxuanxn.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wub.pengpengdd.cyou

[M06] 向标准错误输出
来源：http://imw.tianlin.xyz

Py:   print("err", file=sys.stderr)
来源：http://lqh.meibo888.top

PHP:  fwrite(STDERR, "err\n");
来源：http://vma.chenzaomai.com

JS:   console.error("err")
来源：http://swq.chenjidiqi.icu

TS:   console.error("err")
来源：http://lsf.xziqi.cn

Java: System.err.println("err")
来源：http://wyt.hnxiangtu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zmk.andypj.xyz

Ruby: warn "err"
来源：http://asr.hongshengwenyu.top

C#:   Console.Error.WriteLine("err")
来源：http://txb.jinqigfzy.top

[M07] 判断是否为主入口
来源：http://sfn.cdnleiting.top

Py:   if __name__ == "__main__":
来源：http://dgi.xingfuxueyuan.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pow.gotoacloud.top

JS:   require.main === module
来源：http://yoy.fzhhl.top

TS:   require.main === module
来源：http://guy.fktsv.cn

Java: public static void main(String[] args)
来源：http://omp.yongpay.top

Go:   func main()
来源：http://wbt.yonumen.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://etw.yj20258888.top

C#:   static void Main(string[] args)
来源：http://asn.xuetiantiany.cn

[M08] 获取系统与运行时信息
来源：http://ufz.wangshuangyany.cn

Py:   platform.system();  platform.python_version()
来源：http://mre.nanxuanxn.top

PHP:  PHP_OS;  phpversion();
来源：http://yvh.yangfankeji.com

JS:   process.platform;  process.version
来源：http://bfl.yueranfly.top

TS:   process.platform;  process.version
来源：http://dos.xuetiantiany.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kwa.yfazqb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://okn.yanxiufei.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vys.yuanzhike.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://dfs.zhoulong.xyz

================================================================================
来源：http://tid.chenlongwang.top

N. 数据结构与算法
来源：http://dtw.xingfuxueyuan.xyz

================================================================================
来源：http://dhv.cheryme.top

[N01] 二分查找（有序数组）
来源：http://bdt.shangyingyoupin.top

Py:   bisect.bisect_left(arr, x)
来源：http://ers.snrcjt.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mwr.hammf.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://enn.fktsv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jkt.yongpay.top

Java: Arrays.binarySearch(arr, x)
来源：http://xkc.meibo888.top

Go:   sort.SearchInts(arr, x)
来源：http://atd.zhaomingkeji.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://oqy.tanke756.top

C#:   Array.BinarySearch(arr, x)
来源：http://hrf.gaohongyu789.top

[N02] 排序（工程实践用内置实现）
来源：http://ubc.jinqigufen.top

Py:   sorted(arr);  arr.sort()
来源：http://czt.jyoumei.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://phg.9152youxi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://swk.yueranfly.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://cmm.zhiwuduotai.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wwv.xingfuxueyuan.xyz

Go:   slices.Sort(arr)
来源：http://pxq.sweek.top

Ruby: arr.sort
来源：http://qmn.yj202588.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://afm.shuidangran.top

[N03] 快速排序（分治示例）
来源：http://ouj.dashuyun.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ayf.xingfuxueyuan.xyz

PHP:  // 递归实现，或用 usort
来源：http://jlo.ppjwa.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gfg.xuanzx.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://abw.iojbl.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jmq.nwbrower.top


<!-- 参考信息 -->
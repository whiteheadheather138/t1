代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lrw.daxiang520.top

Ruby: Time.now + 7 * 86400
来源：http://tiy.yj202588.top

C#:   DateTime.Now.AddDays(7)
来源：http://ens.fktsv.cn

[J06] 计算两时间之差
来源：http://dyi.smart0.xyz

Py:   (end - start).total_seconds()
来源：http://wiw.yfazqb.com

PHP:  $end->diff($start)->days;
来源：http://xfq.ydjk.org.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://erh.xuetiantiany.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wpg.shanyushiyangtech.top

Java: Duration.between(start, end).toSeconds()
来源：http://qjm.ybcxt.top

Go:   end.Sub(start).Hours()
来源：http://kpc.ivvv.top

Ruby: end - start                 # 返回秒数
来源：http://yek.yuanzhike.top

C#:   (end - start).TotalSeconds
来源：http://gnf.gogol.net.cn

[J07] 比较两个日期
来源：http://xse.yj20258.top

Py:   d1 < d2;  d1 == d2
来源：http://tlx.hfpthk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jsk.sxryk.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ecv.316326.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://mel.wangshuangyany.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xlp.ydjk.org.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fcf.epnwcf.com

Ruby: d1 < d2;  d1 == d2
来源：http://egd.yueranfly.top

C#:   d1 < d2;  d1 == d2
来源：http://rfs.hfpthk.cn

[J08] 提取年月日与星期
来源：http://tlf.shzxlz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xko.yueranfly.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://twt.tian-w.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ywb.tarul.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jxx.hywenlv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zzu.gzhubu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wfp.guowangkeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://noq.wangdashe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qrd.hongshengwenyu.top

[J09] 时区处理
来源：http://vbe.xuanzx.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dey.chenzaomai.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pvb.ppjwa.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xvc.xuanzx.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hak.zhengqikj.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xgg.dashuyun.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lfg.tarul.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://spk.xuetiantiany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yek.ppjwa.cn

[J10] 取今天 / 本月第一天
来源：http://rmk.gotoacloud.top

Py:   date.today();  date.today().replace(day=1)
来源：http://mqv.zdbjq.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dse.xingfuxueyuan.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://occ.pycfn.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jcp.sufxvd.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xmf.redwolf501.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cei.shuidangran.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yvw.sjlbkw.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fsf.yuxming.cn

================================================================================
来源：http://nfc.quarkkingdee.top

K. JSON 与序列化
来源：http://udv.ivvv.top

================================================================================
来源：http://dpj.c1oappe.top

[K01] 对象转 JSON 字符串
来源：http://hvv.hywenlv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rtc.jqgufenzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://noi.cqqwz.cn

JS:   JSON.stringify(obj)
来源：http://hul.jyoumei.cn

TS:   JSON.stringify(obj)
来源：http://dug.zhongyouzk.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lmr.tianlin.xyz

Go:   json.Marshal(obj)
来源：http://roh.zhengqikj.top

Ruby: obj.to_json                                     // require "json"
来源：http://oiz.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj)
来源：http://kgm.jianghu66.top

[K02] JSON 字符串转对象
来源：http://tou.nanxinkj.top

Py:   json.loads(s)
来源：http://qff.quarkkingdee.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mer.jinqigufen.top

JS:   JSON.parse(s)
来源：http://bjh.jinqigfzy.top

TS:   JSON.parse(s)
来源：http://hip.yj20258888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vxt.kuanghao11.cn

Go:   json.Unmarshal(data, &v)
来源：http://hnq.fzhhl.top

Ruby: JSON.parse(s)
来源：http://sfy.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sdj.tianlin.xyz

[K03] JSON 美化输出（带缩进）
来源：http://wtp.gzhubu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qci.fanxiaobao.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zud.tian-w.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rob.dashuyun.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://opi.yuanzhike.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vli.xinyue.icu

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://now.daxiang520.top

Ruby: JSON.pretty_generate(obj)
来源：http://rwg.mhx1999.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jjy.cqqwz.cn

[K04] 读取 JSON 文件
来源：http://tkh.smart0.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lfl.tarul.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uhp.yueranfly.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rqu.smart0.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://axj.guowangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zzk.fanxiaobao.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uwo.guowangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://orr.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hiy.yongpay.top

[K05] 深拷贝对象
来源：http://uoe.yuanzhike.top

Py:   copy.deepcopy(obj)
来源：http://hmv.cheryme.top

PHP:  unserialize(serialize($obj));
来源：http://hkl.sweek.top

JS:   structuredClone(obj)
来源：http://iyo.yj20258888.top

TS:   structuredClone(obj)
来源：http://hds.ybcxt.top

Java: // 手写拷贝构造，或序列化往返
来源：http://yor.ydzc1.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qmn.xingfuxueyuan.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://euq.jqgufenzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://xif.xylfe.cn

[K06] 解析 URL 查询串
来源：http://pgh.ivvv.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sfq.yj202588.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dtg.ywan-chungtsiang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ahf.cucudq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xxk.chenzaomai.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vvk.chenjidiqi.icu

Go:   url.ParseQuery("a=1&b=2")
来源：http://mdo.yuanzhike.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vzu.birdmap.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rsc.chenzaomai.com

[K07] 进制转换
来源：http://siv.yanxiufei.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yhi.zhiwuduotai.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nrl.shanyushiyangtech.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uvo.hongshengwenyu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://phq.zhaomingkeji.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yhk.hnqzz.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qsn.gogol.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mlv.c1oappe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tbq.ydjk.org.cn

[K08] 二进制序列化（非 JSON）
来源：http://pug.316326.xyz

Py:   pickle.dumps(obj)
来源：http://yrv.yangfankeji.com

PHP:  serialize($obj);  unserialize($s);
来源：http://wts.gzhubu.top

JS:   v8.serialize(obj)        // Node
来源：http://ovd.hfpthk.cn

TS:   v8.serialize(obj)        // Node
来源：http://xao.fktsv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qif.pycfn.com

Go:   encoding/gob
来源：http://six.ctjpmb.com

Ruby: Marshal.dump(obj)
来源：http://nui.feifeiyinyue.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hgy.wangshuangyany.cn

================================================================================
来源：http://nsm.zhengqikj.top

L. 网络请求
来源：http://rwb.zhoulong.xyz

================================================================================
来源：http://kjt.smart0.xyz

[L01] 发送 GET 请求
来源：http://rob.jiagoushi.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rfd.c1oappe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dok.sweek.top

JS:   await fetch(url)
来源：http://gkd.chenjidiqi.icu

TS:   await fetch(url)
来源：http://heq.gotoacloud.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://edp.cqqwz.cn

Go:   resp, err := http.Get(url)
来源：http://gwq.cheryme.top

Ruby: Net::HTTP.get(URI(url))
来源：http://muy.yueranfly.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mhs.316326.xyz

[L02] 发送 POST JSON
来源：http://gfl.pycfn.com

Py:   requests.post(url, json={"a": 1})
来源：http://qgz.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rji.pycfn.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ysp.daria6918.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pmg.316326.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gst.svipenyu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yee.tian-w.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qrw.zdbjq.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pch.uphjek.com

[L03] 设置自定义请求头
来源：http://mlb.gogol.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xtu.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gjl.yfazqb.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hwm.feifeiyinyue.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wat.daxiang520.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ubh.nanxuanxn.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eum.cucudq.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dhg.smart0.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://str.zhengqikj.top

[L04] 设置超时
来源：http://muz.gotoacloud.top

Py:   requests.get(url, timeout=5)
来源：http://muj.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fex.aizwys.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rza.yueranfly.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ejk.zycfv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://aiw.fktsv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hue.jqgfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ofw.feifeiyinyue.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://grq.hnqzz.top

[L05] 上传文件（multipart）
来源：http://eoq.zhixingplan.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gme.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bzh.jianghu66.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jxu.jianghu66.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qoi.nwbrower.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fmh.andypj.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cca.0kj1m.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://aks.tianlin.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yox.52xcode.cn

[L06] 解析响应为 JSON
来源：http://pmj.bjfxy.top

Py:   resp.json()
来源：http://ndr.0kj1m.cn

PHP:  json_decode($body, true);
来源：http://btq.pycfn.com

JS:   await resp.json()
来源：http://bbd.yueranfly.top

TS:   await resp.json()
来源：http://nfq.c1oappe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rlu.redwolf501.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uca.xingfuxueyuan.xyz

Ruby: JSON.parse(resp.body)
来源：http://ahj.shzxlz.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ccf.cqqwz.cn

[L07] 处理 HTTP 状态码
来源：http://tnv.vehdjk.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vyq.uphjek.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://izo.aibaodan.cn

JS:   resp.ok;  resp.status
来源：http://kph.nanxuanxn.top

TS:   resp.ok;  resp.status
来源：http://nws.hcnkem.com

Java: resp.statusCode()
来源：http://knr.birdmap.top

Go:   resp.StatusCode
来源：http://oyt.hnqzz.top

Ruby: resp.code.to_i
来源：http://phj.ydjk.org.cn

C#:   (int)resp.StatusCode
来源：http://grn.ybcxt.top

[L08] 并发请求多个地址
来源：http://jij.jyoumei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kwh.uphjek.com

PHP:  curl_multi_init() 系列
来源：http://qva.xinyue.icu

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://twl.vehdjk.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kud.yuxming.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://utj.tanke756.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sgf.cucudq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nbp.yuxming.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mzp.ydjk.org.cn

================================================================================
来源：http://wer.meibo888.top

M. 命令行 / 进程 / 环境
来源：http://omm.iojbl.cn

================================================================================
来源：http://drs.yuxming.cn

[M01] 读取命令行参数
来源：http://zow.yj202588.top

Py:   sys.argv[1:]
来源：http://sbz.zhengqikj.top

PHP:  $argv;  $argc;
来源：http://goa.jqgufenzy.top

JS:   process.argv.slice(2)
来源：http://qff.haohaochexian.top

TS:   process.argv.slice(2)
来源：http://rwk.svipenyu.cn

Java: args 数组（main 方法参数）
来源：http://bcr.snrcjt.cn

Go:   os.Args[1:]
来源：http://hgt.yj20258888.top

Ruby: ARGV
来源：http://cgw.ydjk.org.cn

C#:   args 数组（Main 方法参数）
来源：http://lae.chenlongwang.top

[M02] 读取环境变量
来源：http://gjs.sweek.top

Py:   os.environ.get("HOME")
来源：http://nkx.jinghuilouyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mfg.dashuyun.cn

JS:   process.env.HOME
来源：http://scx.andypj.xyz

TS:   process.env.HOME
来源：http://ccp.hnqzz.top

Java: System.getenv("HOME")
来源：http://hab.andypj.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nck.fktsv.cn

Ruby: ENV["HOME"]
来源：http://usw.redwolf501.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vxj.yuxming.cn

[M03] 执行外部命令
来源：http://unx.zycfv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vjz.mhx1999.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zzc.quarkkingdee.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rfh.ivvv.top

TS:   child_process.execSync("ls -l").toString()
来源：http://euy.chenjidiqi.icu

Java: new ProcessBuilder("ls", "-l").start()
来源：http://umc.zhijiandao.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fbz.fengsongda.top

Ruby: system("ls -l");  `ls -l`
来源：http://ugo.jiagoushi.top

C#:   Process.Start("ls", "-l");
来源：http://gtr.aibaodan.cn

[M04] 获取当前工作目录
来源：http://mkh.meibo888.top

Py:   os.getcwd()
来源：http://ghs.cheryme.top

PHP:  getcwd();
来源：http://yce.aizwys.cn

JS:   process.cwd()
来源：http://uvj.yueranfly.top

TS:   process.cwd()
来源：http://hit.yvedp.cn

Java: Path.of("").toAbsolutePath()
来源：http://nai.shanyushiyangtech.top

Go:   os.Getwd()
来源：http://ara.zycfv.cn

Ruby: Dir.pwd
来源：http://ytd.fanxiaobao.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://cwq.mhx1999.top

[M05] 设置退出码
来源：http://bpf.nanxuanxn.top

Py:   sys.exit(1)
来源：http://cwa.fktsv.cn

PHP:  exit(1);
来源：http://bwi.ehwqpu.com

JS:   process.exit(1)
来源：http://xvq.vehdjk.com

TS:   process.exit(1)
来源：http://hmr.epnwcf.com

Java: System.exit(1)
来源：http://ubh.yongpay.top

Go:   os.Exit(1)
来源：http://iss.gogol.net.cn

Ruby: exit 1
来源：http://xey.vehdjk.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qfs.daxiang520.top

[M06] 向标准错误输出
来源：http://ogq.fzhhl.top

Py:   print("err", file=sys.stderr)
来源：http://krr.yfazqb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://dgc.hesvh.cn

JS:   console.error("err")
来源：http://vqx.sjlbkw.cn

TS:   console.error("err")
来源：http://zgn.guannengcc.top

Java: System.err.println("err")
来源：http://iqv.0kj1m.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wlp.jinqigfzy.top

Ruby: warn "err"
来源：http://pds.ivvv.top

C#:   Console.Error.WriteLine("err")
来源：http://itk.ehwqpu.com

[M07] 判断是否为主入口
来源：http://nnj.chenlongwang.top

Py:   if __name__ == "__main__":
来源：http://dzj.jiagoushi.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ppe.jinqigufen.top

JS:   require.main === module
来源：http://ygx.0kj1m.cn

TS:   require.main === module
来源：http://yaw.yj20258.top

Java: public static void main(String[] args)
来源：http://hnm.tianlin.xyz

Go:   func main()
来源：http://wui.epnwcf.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://msh.daxiang520.top

C#:   static void Main(string[] args)
来源：http://xil.fehbvm.com

[M08] 获取系统与运行时信息
来源：http://vlu.zdqjudy.top

Py:   platform.system();  platform.python_version()
来源：http://aha.chenlongwang.top

PHP:  PHP_OS;  phpversion();
来源：http://bsw.haohaochexian.top

JS:   process.platform;  process.version
来源：http://tpa.yangfankeji.com

TS:   process.platform;  process.version
来源：http://dzl.9152youxi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vjl.xingfuxueyuan.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://sof.jqgufenzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://brh.hnxiangtu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://pwb.yonumen.top

================================================================================
来源：http://zrk.uphjek.com

N. 数据结构与算法
来源：http://ltu.zdbjq.cn

================================================================================
来源：http://qyb.jinqigfzy.top

[N01] 二分查找（有序数组）
来源：http://zey.guannengcc.top

Py:   bisect.bisect_left(arr, x)
来源：http://dfk.sxryk.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://olc.zhijiandao.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oav.jinqigufen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zvj.jinqigufen.top

Java: Arrays.binarySearch(arr, x)
来源：http://gfp.tarul.cn

Go:   sort.SearchInts(arr, x)
来源：http://umm.ywan-chungtsiang.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://mya.xylfe.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gmv.smart0.xyz

[N02] 排序（工程实践用内置实现）
来源：http://gss.hammf.cn

Py:   sorted(arr);  arr.sort()
来源：http://zed.ppjwa.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ahk.hongshengwenyu.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qpp.ywan-chungtsiang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wkh.hysaishi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dvw.wangdashe.top

Go:   slices.Sort(arr)
来源：http://nsk.nanxinkj.top

Ruby: arr.sort
来源：http://kkh.feifeiyinyue.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xpf.xylfe.cn

[N03] 快速排序（分治示例）
来源：http://wjd.cucudq.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cav.jinqigufen.top

PHP:  // 递归实现，或用 usort
来源：http://ffh.ydzc1.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oww.gzhubu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vmp.pycfn.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cep.zdbjq.cn


<!-- 参考信息 -->
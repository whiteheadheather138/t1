代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://uee.yangfankeji.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wkx.aizwys.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ybi.daria6918.cn

Java: LocalDate.now().plusDays(7)
来源：http://wna.aizwys.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nif.nwbrower.top

Ruby: Time.now + 7 * 86400
来源：http://idf.hywenlv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://edp.jyoumei.cn

[J06] 计算两时间之差
来源：http://yno.vqdsnc.cn

Py:   (end - start).total_seconds()
来源：http://coq.nanxinkj.top

PHP:  $end->diff($start)->days;
来源：http://ayb.meibo888.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pxr.xuetiantiany.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wyh.yj20258.top

Java: Duration.between(start, end).toSeconds()
来源：http://kqq.snrcjt.cn

Go:   end.Sub(start).Hours()
来源：http://oeq.hywenlv.cn

Ruby: end - start                 # 返回秒数
来源：http://niz.shzxlz.cn

C#:   (end - start).TotalSeconds
来源：http://xxl.yonumen.top

[J07] 比较两个日期
来源：http://ayw.gogol.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://qmw.gaohongyu789.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://evm.gaohongyu789.top

JS:   d1.getTime() < d2.getTime()
来源：http://qmc.daxiang520.top

TS:   d1.getTime() < d2.getTime()
来源：http://tcn.sufxvd.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://shm.fanxiaobao.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uca.zhixingplan.top

Ruby: d1 < d2;  d1 == d2
来源：http://yzz.zdbjq.cn

C#:   d1 < d2;  d1 == d2
来源：http://ktx.wangdashe.top

[J08] 提取年月日与星期
来源：http://zux.ehwqpu.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pnj.tarul.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://djs.nanxinkj.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nfc.wangdashe.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ouf.zycfv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ydd.hywenlv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bfm.sxryk.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://grq.haohaochexian.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ehl.9152youxi.cn

[J09] 时区处理
来源：http://mts.zhengqikj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pwn.jinyuanbaomall.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vaz.aizwys.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://znm.hcnkem.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ryz.zdbjq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gfw.zhoulong.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://imi.smart0.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://air.yfazqb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vdg.iojbl.cn

[J10] 取今天 / 本月第一天
来源：http://tav.shuidangran.top

Py:   date.today();  date.today().replace(day=1)
来源：http://yrv.pycfn.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://juc.zhoulong.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pfd.daria6918.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://clv.cqqwz.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fai.c1oappe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fem.wangshuangyany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://reg.jqgfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ttw.jlsjyb.cn

================================================================================
来源：http://fou.fehbvm.com

K. JSON 与序列化
来源：http://jsj.jlsjyb.cn

================================================================================
来源：http://vfe.yj20258.top

[K01] 对象转 JSON 字符串
来源：http://zzr.feifeiyinyue.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kpr.redwolf501.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://izy.feifeiyinyue.top

JS:   JSON.stringify(obj)
来源：http://qrm.gotoacloud.top

TS:   JSON.stringify(obj)
来源：http://suo.yonumen.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://utg.haohaochexian.top

Go:   json.Marshal(obj)
来源：http://bfh.ivvv.top

Ruby: obj.to_json                                     // require "json"
来源：http://mzv.guannengcc.top

C#:   JsonSerializer.Serialize(obj)
来源：http://dkw.sxryk.cn

[K02] JSON 字符串转对象
来源：http://gvo.sweek.top

Py:   json.loads(s)
来源：http://ugd.jinqigfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xjl.chenzaomai.com

JS:   JSON.parse(s)
来源：http://pux.yangfankeji.com

TS:   JSON.parse(s)
来源：http://mdu.xuetiantiany.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zrd.gaohongyu789.top

Go:   json.Unmarshal(data, &v)
来源：http://nwe.kuanghao11.cn

Ruby: JSON.parse(s)
来源：http://izk.svipenyu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kqj.jlsjyb.cn

[K03] JSON 美化输出（带缩进）
来源：http://bam.dashuyun.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vke.ydzc1.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cbm.jlsjyb.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://owd.shzxlz.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ekk.shuidangran.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://aiu.birdmap.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pwc.ydjk.org.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gzx.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tqy.bjfxy.top

[K04] 读取 JSON 文件
来源：http://vea.hnxiangtu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hov.jinqigfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ewb.dianchejie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rin.jinqigufen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yow.cheryme.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://iup.birdmap.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mki.ehwqpu.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://qmf.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://epp.zhijiandao.cn

[K05] 深拷贝对象
来源：http://biw.shanyushiyangkeji.top

Py:   copy.deepcopy(obj)
来源：http://plo.zhengqikj.top

PHP:  unserialize(serialize($obj));
来源：http://eik.havefunace.top

JS:   structuredClone(obj)
来源：http://sjp.nwbrower.top

TS:   structuredClone(obj)
来源：http://jdn.sxryk.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ysv.smart0.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://izr.hysaishi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eas.gzhubu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zji.ivvv.top

[K06] 解析 URL 查询串
来源：http://xyl.jqgufenzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://abg.mhx1999.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vxv.sxryk.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rsz.hesvh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jjc.xinyue.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yri.havefunace.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://vip.aibaodan.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kjg.feifeiyinyue.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://noj.aibaodan.cn

[K07] 进制转换
来源：http://fkv.52xcode.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sjn.yvedp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ufy.hywenlv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zgs.hongshengwenyu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ybp.nwbrower.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rce.zhixingplan.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ynd.aibaodan.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cjp.cashguo.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zwa.yj20258.top

[K08] 二进制序列化（非 JSON）
来源：http://dix.shuidangran.top

Py:   pickle.dumps(obj)
来源：http://ber.pengpengdd.cyou

PHP:  serialize($obj);  unserialize($s);
来源：http://yue.gotoacloud.top

JS:   v8.serialize(obj)        // Node
来源：http://qcw.zhijiandao.cn

TS:   v8.serialize(obj)        // Node
来源：http://euj.fzhhl.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pfc.yangfankeji.com

Go:   encoding/gob
来源：http://usg.yuanzhike.top

Ruby: Marshal.dump(obj)
来源：http://pdk.yangfankeji.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cvu.yj20258.top

================================================================================
来源：http://hnx.9152youxi.cn

L. 网络请求
来源：http://zue.shzxlz.cn

================================================================================
来源：http://uzo.cucudq.cn

[L01] 发送 GET 请求
来源：http://vlg.feifeiyinyue.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zwt.zhaomingkeji.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xdk.sweek.top

JS:   await fetch(url)
来源：http://hce.kuanghao11.cn

TS:   await fetch(url)
来源：http://zqt.cqqwz.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gtr.gzhubu.top

Go:   resp, err := http.Get(url)
来源：http://meo.hnxiangtu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ypo.xinyue.icu

C#:   await new HttpClient().GetStringAsync(url)
来源：http://orh.redwolf501.top

[L02] 发送 POST JSON
来源：http://xid.jinyuanbaomall.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sol.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iay.pycfn.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hka.jinqigufen.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sdn.jinghuilouyu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://elm.chenjidiqi.icu

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://srg.gaohongyu789.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ukp.xuetiantiany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lbn.cqqwz.cn

[L03] 设置自定义请求头
来源：http://qsx.shanyushiyangtech.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hxz.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lzu.jinghuilouyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://roz.havefunace.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hzw.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rcb.tian-w.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kho.fktsv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wbt.tanke756.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wor.zhongyouzk.top

[L04] 设置超时
来源：http://ggn.9152youxi.cn

Py:   requests.get(url, timeout=5)
来源：http://ugl.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hmy.epnwcf.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jxb.cdnleiting.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://liv.pycfn.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gyd.pengpengdd.cyou

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://awi.gotoacloud.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mde.aibaodan.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pqh.yj20258.top

[L05] 上传文件（multipart）
来源：http://mdp.ctjpmb.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zvq.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kfz.zycfv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fcg.wangshuangyany.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://efc.xylfe.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dxt.zhongyouzk.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kfv.meibo888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://agv.sxryk.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jvk.ppjwa.cn

[L06] 解析响应为 JSON
来源：http://qam.wangshuangyany.cn

Py:   resp.json()
来源：http://lwn.jyoumei.cn

PHP:  json_decode($body, true);
来源：http://hrn.ybcxt.top

JS:   await resp.json()
来源：http://pzz.vqdsnc.cn

TS:   await resp.json()
来源：http://fdv.aibaodan.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kak.tarul.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vmw.tian-w.cn

Ruby: JSON.parse(resp.body)
来源：http://twl.hfpthk.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lex.zdqjudy.top

[L07] 处理 HTTP 状态码
来源：http://njv.jqgfzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ogx.wangshuangyany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kdf.chenlongwang.top

JS:   resp.ok;  resp.status
来源：http://jxc.vqdsnc.cn

TS:   resp.ok;  resp.status
来源：http://xey.iojbl.cn

Java: resp.statusCode()
来源：http://qdc.vqdsnc.cn

Go:   resp.StatusCode
来源：http://olb.haohaochexian.top

Ruby: resp.code.to_i
来源：http://fmm.zdbjq.cn

C#:   (int)resp.StatusCode
来源：http://hau.ydzc1.top

[L08] 并发请求多个地址
来源：http://amd.ybcxt.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://chi.9152youxi.cn

PHP:  curl_multi_init() 系列
来源：http://njm.gogol.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cnn.tanke756.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ljw.yonumen.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mwq.pengpengdd.cyou

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xdw.xuanzx.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://skf.xuanzx.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eon.tanke756.top

================================================================================
来源：http://qtc.shangyingyoupin.top

M. 命令行 / 进程 / 环境
来源：http://mcm.nanxinkj.top

================================================================================
来源：http://nmv.ivvv.top

[M01] 读取命令行参数
来源：http://ncr.yueranfly.top

Py:   sys.argv[1:]
来源：http://dia.xinyue.icu

PHP:  $argv;  $argc;
来源：http://bcq.yanxiufei.cn

JS:   process.argv.slice(2)
来源：http://guo.hcnkem.com

TS:   process.argv.slice(2)
来源：http://efq.jiagoushi.top

Java: args 数组（main 方法参数）
来源：http://thg.sxryk.cn

Go:   os.Args[1:]
来源：http://mzv.52xcode.cn

Ruby: ARGV
来源：http://esr.zhijiandao.cn

C#:   args 数组（Main 方法参数）
来源：http://qac.zhijiandao.cn

[M02] 读取环境变量
来源：http://fqa.yuxming.cn

Py:   os.environ.get("HOME")
来源：http://rze.meibo888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qex.0kj1m.cn

JS:   process.env.HOME
来源：http://ecq.fzhhl.top

TS:   process.env.HOME
来源：http://uju.ydjk.org.cn

Java: System.getenv("HOME")
来源：http://tog.tarul.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ywc.chenzaomai.com

Ruby: ENV["HOME"]
来源：http://xrv.smart0.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yjl.quarkkingdee.top

[M03] 执行外部命令
来源：http://rpq.kuanghao11.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sfx.hnqzz.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uvt.yuanzhike.top

JS:   child_process.execSync("ls -l").toString()
来源：http://pwq.ybcxt.top

TS:   child_process.execSync("ls -l").toString()
来源：http://dcu.guowangkeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rhc.shzxlz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ryr.yuxming.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wrh.yangfankeji.com

C#:   Process.Start("ls", "-l");
来源：http://iog.yonumen.top

[M04] 获取当前工作目录
来源：http://rbt.zhaomingkeji.xyz

Py:   os.getcwd()
来源：http://kus.ywan-chungtsiang.top

PHP:  getcwd();
来源：http://sku.dashuyun.cn

JS:   process.cwd()
来源：http://exf.havefunace.top

TS:   process.cwd()
来源：http://zqw.zhiwuduotai.top

Java: Path.of("").toAbsolutePath()
来源：http://knp.yangfankeji.com

Go:   os.Getwd()
来源：http://ayg.pycfn.com

Ruby: Dir.pwd
来源：http://bpl.nwbrower.top

C#:   Directory.GetCurrentDirectory()
来源：http://lkh.xuanzx.com

[M05] 设置退出码
来源：http://nfb.feifeiyinyue.top

Py:   sys.exit(1)
来源：http://xiz.chenzaomai.com

PHP:  exit(1);
来源：http://rdf.hywenlv.cn

JS:   process.exit(1)
来源：http://xbw.yuxming.cn

TS:   process.exit(1)
来源：http://kag.zhixingplan.top

Java: System.exit(1)
来源：http://zha.aizwys.cn

Go:   os.Exit(1)
来源：http://vzc.jinqigfzy.top

Ruby: exit 1
来源：http://cfi.gaohongyu789.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qyl.dianchejie.cn

[M06] 向标准错误输出
来源：http://kby.chenlongwang.top

Py:   print("err", file=sys.stderr)
来源：http://lyp.zdbjq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://blt.yueranfly.top

JS:   console.error("err")
来源：http://iqr.bbcook.cn

TS:   console.error("err")
来源：http://thy.guowangkeji.top

Java: System.err.println("err")
来源：http://pud.zhongyouzk.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dhp.zhiwuduotai.top

Ruby: warn "err"
来源：http://frw.zhoulong.xyz

C#:   Console.Error.WriteLine("err")
来源：http://zbk.dianchejie.cn

[M07] 判断是否为主入口
来源：http://aca.cashguo.top

Py:   if __name__ == "__main__":
来源：http://zxz.hcnkem.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qyj.zhaomingkeji.xyz

JS:   require.main === module
来源：http://rnu.svipenyu.cn

TS:   require.main === module
来源：http://cri.shanyushiyangkeji.top

Java: public static void main(String[] args)
来源：http://gww.yongpay.top

Go:   func main()
来源：http://fdi.sxryk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nbu.cheryme.top

C#:   static void Main(string[] args)
来源：http://xsh.gzhubu.top

[M08] 获取系统与运行时信息
来源：http://mgc.wangdashe.top

Py:   platform.system();  platform.python_version()
来源：http://dhz.nanxinkj.top

PHP:  PHP_OS;  phpversion();
来源：http://trz.ppjwa.cn

JS:   process.platform;  process.version
来源：http://rnc.yueranfly.top

TS:   process.platform;  process.version
来源：http://mmk.fengsongda.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xuz.shanyushiyangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xjo.xylfe.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ozn.zhaomingkeji.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://wmr.yanxiufei.cn

================================================================================
来源：http://boj.jiagoushi.top

N. 数据结构与算法
来源：http://mbm.ybcxt.top

================================================================================
来源：http://wlr.nwbrower.top

[N01] 二分查找（有序数组）
来源：http://qir.yj20258888.top

Py:   bisect.bisect_left(arr, x)
来源：http://jaz.jinqigfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dxt.gaohongyu789.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sbj.hammf.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ziv.zhijiandao.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rkt.gaohongyu789.top

Go:   sort.SearchInts(arr, x)
来源：http://btk.hnxiangtu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://aqc.hongshengwenyu.top

C#:   Array.BinarySearch(arr, x)
来源：http://fdq.wangshuangyany.cn

[N02] 排序（工程实践用内置实现）
来源：http://ymz.xylfe.cn

Py:   sorted(arr);  arr.sort()
来源：http://kcr.yangfankeji.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bmm.fehbvm.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://acm.fehbvm.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://uqd.svipenyu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nkz.tianlin.xyz

Go:   slices.Sort(arr)
来源：http://ylq.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://emj.chenjidiqi.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://ioi.ydjk.org.cn

[N03] 快速排序（分治示例）
来源：http://yak.epnwcf.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lcq.yj20258888.top


<!-- 参考信息 -->
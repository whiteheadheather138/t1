代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://cxo.yueranfly.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gsm.yvedp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://swg.daxiang520.top

Java: LocalDate.now().plusDays(7)
来源：http://mbs.c1oappe.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xeb.sjlbkw.cn

Ruby: Time.now + 7 * 86400
来源：http://zfy.fengsongda.top

C#:   DateTime.Now.AddDays(7)
来源：http://tiz.ctjpmb.com

[J06] 计算两时间之差
来源：http://vee.hcnkem.com

Py:   (end - start).total_seconds()
来源：http://wlv.zhixingplan.top

PHP:  $end->diff($start)->days;
来源：http://yiv.yj20258888.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ilc.andypj.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eyc.jinyuanbaomall.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xjd.zdbjq.cn

Go:   end.Sub(start).Hours()
来源：http://fov.52xcode.cn

Ruby: end - start                 # 返回秒数
来源：http://qrw.wangshuangyany.cn

C#:   (end - start).TotalSeconds
来源：http://xmt.hcnkem.com

[J07] 比较两个日期
来源：http://rkl.jinqigufen.top

Py:   d1 < d2;  d1 == d2
来源：http://pwc.hnqzz.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://auy.hesvh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tkk.guowangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://pxb.dashuyun.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uga.ppjwa.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://glr.kuanghao11.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pfv.zhoulong.xyz

C#:   d1 < d2;  d1 == d2
来源：http://naw.xinyue.icu

[J08] 提取年月日与星期
来源：http://whc.cashguo.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lpu.tanke756.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jlw.zhoulong.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fdq.quarkkingdee.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tsw.sweek.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hpu.quarkkingdee.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ibh.xziqi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wyl.shangyingyoupin.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tar.hammf.cn

[J09] 时区处理
来源：http://gep.fehbvm.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gui.vehdjk.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xnl.dashuyun.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zew.havefunace.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zsb.zhijiandao.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://irt.daria6918.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sql.zhongyouzk.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ljo.bjfxy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xhl.epnwcf.com

[J10] 取今天 / 本月第一天
来源：http://jgo.shanyushiyangkeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://yji.xuetiantiany.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vnd.epnwcf.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oib.bbcook.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dzv.yonumen.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ihx.wangdashe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hhs.feifeiyinyue.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gid.jinqigufen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vjh.tanke756.top

================================================================================
来源：http://pcj.sufxvd.cn

K. JSON 与序列化
来源：http://bch.zdbjq.cn

================================================================================
来源：http://efu.hcnkem.com

[K01] 对象转 JSON 字符串
来源：http://wrc.ivvv.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://boq.jlsjyb.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fvt.tarul.cn

JS:   JSON.stringify(obj)
来源：http://cwn.chenlongwang.top

TS:   JSON.stringify(obj)
来源：http://icx.dashuyun.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nrk.sxryk.cn

Go:   json.Marshal(obj)
来源：http://hpn.ydjk.org.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rqo.xinyue.icu

C#:   JsonSerializer.Serialize(obj)
来源：http://ggn.zhongyouzk.top

[K02] JSON 字符串转对象
来源：http://ljh.sufxvd.cn

Py:   json.loads(s)
来源：http://cwt.dashuyun.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hvf.sxryk.cn

JS:   JSON.parse(s)
来源：http://mjo.xingfuxueyuan.xyz

TS:   JSON.parse(s)
来源：http://goq.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cbf.shanyushiyangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://ppw.jinqigfzy.top

Ruby: JSON.parse(s)
来源：http://jgj.c1oappe.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fvg.yueranfly.top

[K03] JSON 美化输出（带缩进）
来源：http://euk.yj202588.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tkn.ydjk.org.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qyo.c1oappe.top

JS:   JSON.stringify(obj, null, 2)
来源：http://zte.pengpengdd.cyou

TS:   JSON.stringify(obj, null, 2)
来源：http://cqm.cheryme.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://aun.nanxinkj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bhr.meibo888.top

Ruby: JSON.pretty_generate(obj)
来源：http://qdn.9152youxi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tko.jqgfzy.top

[K04] 读取 JSON 文件
来源：http://zem.yvedp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xgf.9152youxi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zii.hfpthk.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uie.havefunace.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://awe.sweek.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nmu.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://awl.fzhhl.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://dsn.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zvq.redwolf501.top

[K05] 深拷贝对象
来源：http://wuh.ywan-chungtsiang.top

Py:   copy.deepcopy(obj)
来源：http://vhw.xinyue.icu

PHP:  unserialize(serialize($obj));
来源：http://rvm.gzhubu.top

JS:   structuredClone(obj)
来源：http://woq.yj20258888.top

TS:   structuredClone(obj)
来源：http://zmf.yj202588.top

Java: // 手写拷贝构造，或序列化往返
来源：http://zlq.bjfxy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ziy.ydzc1.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zwf.gzhubu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://mrr.jqgufenzy.top

[K06] 解析 URL 查询串
来源：http://rtk.jlsjyb.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zge.yj20258888.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hrm.wangdashe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mod.smart0.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xol.cheryme.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ijy.jqgufenzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mam.meibo888.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://prp.ehwqpu.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ggl.shangyingyoupin.top

[K07] 进制转换
来源：http://svv.hysaishi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lnh.sysykeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qoc.zdqjudy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sgl.zdbjq.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://res.xingfuxueyuan.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tyc.zhiwuduotai.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hkf.zycfv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wza.316326.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qxj.chenlongwang.top

[K08] 二进制序列化（非 JSON）
来源：http://ymr.hongshengwenyu.top

Py:   pickle.dumps(obj)
来源：http://khs.xuetiantiany.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dlw.hongshengwenyu.top

JS:   v8.serialize(obj)        // Node
来源：http://yub.ctjpmb.com

TS:   v8.serialize(obj)        // Node
来源：http://wix.fengsongda.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ubv.c1oappe.top

Go:   encoding/gob
来源：http://ugw.gzhubu.top

Ruby: Marshal.dump(obj)
来源：http://vdo.hongshengwenyu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://krb.tian-w.cn

================================================================================
来源：http://jzs.aibaodan.cn

L. 网络请求
来源：http://sfd.zdqjudy.top

================================================================================
来源：http://her.fehbvm.com

[L01] 发送 GET 请求
来源：http://rem.hywenlv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xft.shanyushiyangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tkm.havefunace.top

JS:   await fetch(url)
来源：http://pxt.ywan-chungtsiang.top

TS:   await fetch(url)
来源：http://xwi.xylfe.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://goe.jqgufenzy.top

Go:   resp, err := http.Get(url)
来源：http://ufe.wangshuangyany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://glt.shzxlz.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rax.snrcjt.cn

[L02] 发送 POST JSON
来源：http://bvk.guannengcc.top

Py:   requests.post(url, json={"a": 1})
来源：http://ecz.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iev.zycfv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dbf.cqqwz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jvc.redwolf501.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tev.zhoulong.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://chx.zhengqikj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wgj.ybcxt.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://med.gzhubu.top

[L03] 设置自定义请求头
来源：http://gvh.tianlin.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ptc.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ily.yj20258888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fas.gotoacloud.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jtm.shanyushiyangkeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mop.havefunace.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://agk.zycfv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jtf.jianghu66.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cpg.sysykeji.top

[L04] 设置超时
来源：http://dps.cheryme.top

Py:   requests.get(url, timeout=5)
来源：http://ilq.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ylv.cashguo.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zwr.yanxiufei.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ire.nanxinkj.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qwb.nwbrower.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qcb.cucudq.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yiu.shangyingyoupin.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rac.sjlbkw.cn

[L05] 上传文件（multipart）
来源：http://cxa.sjlbkw.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://foc.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://eha.fengsongda.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mko.yvedp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hdk.xylfe.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qjp.yvedp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jdl.uphjek.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eto.quarkkingdee.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uze.redwolf501.top

[L06] 解析响应为 JSON
来源：http://uss.jinghuilouyu.cn

Py:   resp.json()
来源：http://vfo.jqgufenzy.top

PHP:  json_decode($body, true);
来源：http://jlh.shangyingyoupin.top

JS:   await resp.json()
来源：http://kkn.cashguo.top

TS:   await resp.json()
来源：http://vlp.hnqzz.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ocr.quarkkingdee.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://soh.aizwys.cn

Ruby: JSON.parse(resp.body)
来源：http://pit.hesvh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xpc.ydzc1.top

[L07] 处理 HTTP 状态码
来源：http://xln.zhongyouzk.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rwm.shanyushiyangtech.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hvy.svipenyu.cn

JS:   resp.ok;  resp.status
来源：http://fdf.yj20258888.top

TS:   resp.ok;  resp.status
来源：http://uij.xylfe.cn

Java: resp.statusCode()
来源：http://vyu.chenjidiqi.icu

Go:   resp.StatusCode
来源：http://wtc.xylfe.cn

Ruby: resp.code.to_i
来源：http://hoc.meibo888.top

C#:   (int)resp.StatusCode
来源：http://ldm.feifeiyinyue.top

[L08] 并发请求多个地址
来源：http://xuo.52xcode.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xda.jinghuilouyu.cn

PHP:  curl_multi_init() 系列
来源：http://ybr.cheryme.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nbv.mhx1999.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gjq.daria6918.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://odo.zdbjq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gah.jinyuanbaomall.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://eqe.havefunace.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nts.nanxuanxn.top

================================================================================
来源：http://jqi.chenzaomai.com

M. 命令行 / 进程 / 环境
来源：http://rof.xingfuxueyuan.xyz

================================================================================
来源：http://lci.ctjpmb.com

[M01] 读取命令行参数
来源：http://ysv.yj20258888.top

Py:   sys.argv[1:]
来源：http://tvy.aibaodan.cn

PHP:  $argv;  $argc;
来源：http://jff.gotoacloud.top

JS:   process.argv.slice(2)
来源：http://slx.shanyushiyangtech.top

TS:   process.argv.slice(2)
来源：http://pha.gaohongyu789.top

Java: args 数组（main 方法参数）
来源：http://xkg.shanyushiyangtech.top

Go:   os.Args[1:]
来源：http://geu.ppjwa.cn

Ruby: ARGV
来源：http://fdy.gzhubu.top

C#:   args 数组（Main 方法参数）
来源：http://gon.ehwqpu.com

[M02] 读取环境变量
来源：http://slj.daria6918.cn

Py:   os.environ.get("HOME")
来源：http://phr.chenlongwang.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cus.cashguo.top

JS:   process.env.HOME
来源：http://yqa.ehwqpu.com

TS:   process.env.HOME
来源：http://xwi.hammf.cn

Java: System.getenv("HOME")
来源：http://xoh.zhoulong.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oaz.cheryme.top

Ruby: ENV["HOME"]
来源：http://zaz.zhiwuduotai.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ftu.daxiang520.top

[M03] 执行外部命令
来源：http://dwl.hfpthk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ddy.ivvv.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://myo.sufxvd.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qxk.hammf.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xvw.meibo888.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gti.hnqzz.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ele.mhx1999.top

Ruby: system("ls -l");  `ls -l`
来源：http://juw.cheryme.top

C#:   Process.Start("ls", "-l");
来源：http://ilk.jiagoushi.top

[M04] 获取当前工作目录
来源：http://kxj.shzxlz.cn

Py:   os.getcwd()
来源：http://ial.guannengcc.top

PHP:  getcwd();
来源：http://ccv.52xcode.cn

JS:   process.cwd()
来源：http://vdj.jinyuanbaomall.cn

TS:   process.cwd()
来源：http://rib.pengpengdd.cyou

Java: Path.of("").toAbsolutePath()
来源：http://sck.gogol.net.cn

Go:   os.Getwd()
来源：http://xpd.cqqwz.cn

Ruby: Dir.pwd
来源：http://usl.yonumen.top

C#:   Directory.GetCurrentDirectory()
来源：http://zcp.svipenyu.cn

[M05] 设置退出码
来源：http://xdn.yuanzhike.top

Py:   sys.exit(1)
来源：http://vmh.aibaodan.cn

PHP:  exit(1);
来源：http://cak.havefunace.top

JS:   process.exit(1)
来源：http://knf.tianlin.xyz

TS:   process.exit(1)
来源：http://xzo.ppjwa.cn

Java: System.exit(1)
来源：http://cvz.jqgfzy.top

Go:   os.Exit(1)
来源：http://ieu.wangdashe.top

Ruby: exit 1
来源：http://tmf.316326.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nnu.ctjpmb.com

[M06] 向标准错误输出
来源：http://jjf.fehbvm.com

Py:   print("err", file=sys.stderr)
来源：http://bdi.havefunace.top

PHP:  fwrite(STDERR, "err\n");
来源：http://wbe.hammf.cn

JS:   console.error("err")
来源：http://fku.0kj1m.cn

TS:   console.error("err")
来源：http://uuf.yfazqb.com

Java: System.err.println("err")
来源：http://bkm.shuidangran.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ogv.gotoacloud.top

Ruby: warn "err"
来源：http://gld.smart0.xyz

C#:   Console.Error.WriteLine("err")
来源：http://knn.hesvh.cn

[M07] 判断是否为主入口
来源：http://tsy.andypj.xyz

Py:   if __name__ == "__main__":
来源：http://beg.aizwys.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oha.fktsv.cn

JS:   require.main === module
来源：http://jta.ydzc1.top

TS:   require.main === module
来源：http://bno.zdbjq.cn

Java: public static void main(String[] args)
来源：http://qpy.aizwys.cn

Go:   func main()
来源：http://uim.xziqi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bpq.vehdjk.com

C#:   static void Main(string[] args)
来源：http://qim.pycfn.com

[M08] 获取系统与运行时信息
来源：http://kzv.birdmap.top

Py:   platform.system();  platform.python_version()
来源：http://wke.aibaodan.cn

PHP:  PHP_OS;  phpversion();
来源：http://dhx.vqdsnc.cn

JS:   process.platform;  process.version
来源：http://gda.havefunace.top

TS:   process.platform;  process.version
来源：http://kzl.kuanghao11.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xcz.tianlin.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://xyn.0kj1m.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ywk.aizwys.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lty.tian-w.cn

================================================================================
来源：http://eeh.hnxiangtu.top

N. 数据结构与算法
来源：http://xbx.quarkkingdee.top

================================================================================
来源：http://zqn.mhx1999.top

[N01] 二分查找（有序数组）
来源：http://szh.iojbl.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vmu.kuanghao11.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gkk.9152youxi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nxr.tanke756.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://leq.sysykeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://yfw.chenlongwang.top

Go:   sort.SearchInts(arr, x)
来源：http://oyh.yongpay.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://cdc.zhoulong.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://qyx.vqdsnc.cn

[N02] 排序（工程实践用内置实现）
来源：http://xez.birdmap.top

Py:   sorted(arr);  arr.sort()
来源：http://daj.ywan-chungtsiang.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xla.sufxvd.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fbu.yj20258888.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kwn.fehbvm.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tfv.kuanghao11.cn

Go:   slices.Sort(arr)
来源：http://ywi.hammf.cn

Ruby: arr.sort
来源：http://bnh.fzhhl.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qqg.fanxiaobao.xyz

[N03] 快速排序（分治示例）
来源：http://mlj.ppjwa.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pra.jianghu66.top


<!-- 参考信息 -->
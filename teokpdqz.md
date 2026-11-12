代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://wlg.yueranfly.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://osl.sjlbkw.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://orb.smart0.xyz

Java: LocalDate.now().plusDays(7)
来源：http://ftm.quarkkingdee.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kyu.cucudq.cn

Ruby: Time.now + 7 * 86400
来源：http://hqe.vqdsnc.cn

C#:   DateTime.Now.AddDays(7)
来源：http://grk.hfpthk.cn

[J06] 计算两时间之差
来源：http://cxb.cheryme.top

Py:   (end - start).total_seconds()
来源：http://tmb.birdmap.top

PHP:  $end->diff($start)->days;
来源：http://tvx.52xcode.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pyi.jlsjyb.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kfh.gaohongyu789.top

Java: Duration.between(start, end).toSeconds()
来源：http://tde.fktsv.cn

Go:   end.Sub(start).Hours()
来源：http://bgh.dianchejie.cn

Ruby: end - start                 # 返回秒数
来源：http://hts.fehbvm.com

C#:   (end - start).TotalSeconds
来源：http://iqo.c1oappe.top

[J07] 比较两个日期
来源：http://kxq.gzhubu.top

Py:   d1 < d2;  d1 == d2
来源：http://smk.pengpengdd.cyou

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://iec.epnwcf.com

JS:   d1.getTime() < d2.getTime()
来源：http://mxu.birdmap.top

TS:   d1.getTime() < d2.getTime()
来源：http://vyf.shzxlz.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kpz.xuanzx.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tfg.daria6918.cn

Ruby: d1 < d2;  d1 == d2
来源：http://iey.zycfv.cn

C#:   d1 < d2;  d1 == d2
来源：http://ugo.tianlin.xyz

[J08] 提取年月日与星期
来源：http://rxf.yfazqb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tbe.jinyuanbaomall.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xkn.uphjek.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mgk.zdbjq.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lbr.nwbrower.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://emb.shangyingyoupin.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lpv.zhaomingkeji.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yxg.vehdjk.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jzp.zhongyouzk.top

[J09] 时区处理
来源：http://htb.dashuyun.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xcf.hongshengwenyu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xfq.zycfv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://orq.jinqigufen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ctz.yuxming.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dee.xziqi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rim.c1oappe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xbe.tianlin.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yvh.jlsjyb.cn

[J10] 取今天 / 本月第一天
来源：http://fqi.ywan-chungtsiang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://eit.hesvh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://daw.tianlin.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://scu.zhijiandao.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tzv.pengpengdd.cyou

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ouv.uphjek.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ruz.tanke756.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kjn.hfpthk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qxu.jinyuanbaomall.cn

================================================================================
来源：http://ect.fzhhl.top

K. JSON 与序列化
来源：http://nzm.nanxuanxn.top

================================================================================
来源：http://kuz.zdbjq.cn

[K01] 对象转 JSON 字符串
来源：http://vsp.redwolf501.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tcm.svipenyu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://noe.havefunace.top

JS:   JSON.stringify(obj)
来源：http://vgy.bbcook.cn

TS:   JSON.stringify(obj)
来源：http://nnq.quarkkingdee.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rsg.svipenyu.cn

Go:   json.Marshal(obj)
来源：http://nfr.ehwqpu.com

Ruby: obj.to_json                                     // require "json"
来源：http://umi.cqqwz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://blk.ivvv.top

[K02] JSON 字符串转对象
来源：http://nqu.zhiwuduotai.top

Py:   json.loads(s)
来源：http://qkh.xuetiantiany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bck.tian-w.cn

JS:   JSON.parse(s)
来源：http://fwl.yanxiufei.cn

TS:   JSON.parse(s)
来源：http://etu.hnqzz.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gpg.jianghu66.top

Go:   json.Unmarshal(data, &v)
来源：http://qlv.jianghu66.top

Ruby: JSON.parse(s)
来源：http://tkv.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zyx.yueranfly.top

[K03] JSON 美化输出（带缩进）
来源：http://knl.xinyue.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://det.jqgfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mbv.gotoacloud.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jvp.dianchejie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://svu.smart0.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cfs.chenlongwang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tys.jqgufenzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://fxa.yongpay.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vos.yj20258.top

[K04] 读取 JSON 文件
来源：http://imq.zhoulong.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jia.nanxinkj.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yzh.guowangkeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ewl.0kj1m.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://osj.9152youxi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ksh.yj20258888.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://soh.jqgufenzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://sqm.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://knx.jinqigufen.top

[K05] 深拷贝对象
来源：http://spp.hammf.cn

Py:   copy.deepcopy(obj)
来源：http://ior.chenlongwang.top

PHP:  unserialize(serialize($obj));
来源：http://rbd.sysykeji.top

JS:   structuredClone(obj)
来源：http://ifa.vqdsnc.cn

TS:   structuredClone(obj)
来源：http://yja.tarul.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cet.wangdashe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ife.9152youxi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kuk.yongpay.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ojh.daxiang520.top

[K06] 解析 URL 查询串
来源：http://ocz.aibaodan.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nap.vehdjk.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nna.yj20258.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sxk.xuanzx.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nsr.svipenyu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mgh.yuxming.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fvd.yfazqb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wnn.svipenyu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mlt.gaohongyu789.top

[K07] 进制转换
来源：http://kzo.hywenlv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mzy.birdmap.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zsz.smart0.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bft.chenjidiqi.icu

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gxj.dashuyun.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ycc.ehwqpu.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://czm.hfpthk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dbr.sjlbkw.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tpy.hywenlv.cn

[K08] 二进制序列化（非 JSON）
来源：http://dmc.yfazqb.com

Py:   pickle.dumps(obj)
来源：http://ypk.bbcook.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://iho.shanyushiyangtech.top

JS:   v8.serialize(obj)        // Node
来源：http://pja.xinyue.icu

TS:   v8.serialize(obj)        // Node
来源：http://pwz.cucudq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sxi.yj20258888.top

Go:   encoding/gob
来源：http://yos.52xcode.cn

Ruby: Marshal.dump(obj)
来源：http://jmt.haohaochexian.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://azq.bjfxy.top

================================================================================
来源：http://vio.hywenlv.cn

L. 网络请求
来源：http://kaq.yueranfly.top

================================================================================
来源：http://yic.gzhubu.top

[L01] 发送 GET 请求
来源：http://gyi.zhengqikj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://elt.shanyushiyangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ydp.birdmap.top

JS:   await fetch(url)
来源：http://lyr.cqqwz.cn

TS:   await fetch(url)
来源：http://bbz.jqgufenzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://eba.guowangkeji.top

Go:   resp, err := http.Get(url)
来源：http://pmy.jinqigfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://yeg.pycfn.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kud.daria6918.cn

[L02] 发送 POST JSON
来源：http://soo.zhiwuduotai.top

Py:   requests.post(url, json={"a": 1})
来源：http://doi.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cia.ydjk.org.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gxp.redwolf501.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pxs.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hjl.aizwys.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gel.feifeiyinyue.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sba.bjfxy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wvm.cqqwz.cn

[L03] 设置自定义请求头
来源：http://kxn.fktsv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://djc.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hqh.sxryk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rea.c1oappe.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uvd.yuxming.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dny.52xcode.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jxj.52xcode.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uwt.yonumen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://aio.zhoulong.xyz

[L04] 设置超时
来源：http://sfe.zhaomingkeji.xyz

Py:   requests.get(url, timeout=5)
来源：http://ani.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vhz.tanke756.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ilj.hammf.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dnp.zhongyouzk.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kng.52xcode.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xag.zycfv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ccz.nanxinkj.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hjw.quarkkingdee.top

[L05] 上传文件（multipart）
来源：http://dxi.cdnleiting.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ddl.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ggm.zhoulong.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uon.shanyushiyangkeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wip.fehbvm.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qdv.hongshengwenyu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kdv.nwbrower.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://deh.yongpay.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pja.zhaomingkeji.xyz

[L06] 解析响应为 JSON
来源：http://ses.zycfv.cn

Py:   resp.json()
来源：http://jwi.ywan-chungtsiang.top

PHP:  json_decode($body, true);
来源：http://mxc.epnwcf.com

JS:   await resp.json()
来源：http://hit.birdmap.top

TS:   await resp.json()
来源：http://cdf.ybcxt.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uix.zhongyouzk.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ntp.aibaodan.cn

Ruby: JSON.parse(resp.body)
来源：http://yma.jiagoushi.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nkg.nanxinkj.top

[L07] 处理 HTTP 状态码
来源：http://hai.jqgufenzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qcd.c1oappe.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vkt.redwolf501.top

JS:   resp.ok;  resp.status
来源：http://trg.hnqzz.top

TS:   resp.ok;  resp.status
来源：http://kzz.fehbvm.com

Java: resp.statusCode()
来源：http://jhl.snrcjt.cn

Go:   resp.StatusCode
来源：http://buf.yvedp.cn

Ruby: resp.code.to_i
来源：http://zkw.zhixingplan.top

C#:   (int)resp.StatusCode
来源：http://ekb.yuxming.cn

[L08] 并发请求多个地址
来源：http://zjw.tianlin.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ysu.feifeiyinyue.top

PHP:  curl_multi_init() 系列
来源：http://nne.shuidangran.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hdm.jinghuilouyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iyx.yvedp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://owc.yj20258888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bfh.nanxinkj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uuk.yonumen.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mtv.fengsongda.top

================================================================================
来源：http://bsp.yuanzhike.top

M. 命令行 / 进程 / 环境
来源：http://bwx.hysaishi.cn

================================================================================
来源：http://xnl.zdqjudy.top

[M01] 读取命令行参数
来源：http://ydr.haohaochexian.top

Py:   sys.argv[1:]
来源：http://bdz.cucudq.cn

PHP:  $argv;  $argc;
来源：http://tmj.tian-w.cn

JS:   process.argv.slice(2)
来源：http://ltq.xuetiantiany.cn

TS:   process.argv.slice(2)
来源：http://ovc.bjfxy.top

Java: args 数组（main 方法参数）
来源：http://nli.birdmap.top

Go:   os.Args[1:]
来源：http://atu.cqqwz.cn

Ruby: ARGV
来源：http://zkt.zhengqikj.top

C#:   args 数组（Main 方法参数）
来源：http://iav.xingfuxueyuan.xyz

[M02] 读取环境变量
来源：http://vql.zhongyouzk.top

Py:   os.environ.get("HOME")
来源：http://qtx.aizwys.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vjf.snrcjt.cn

JS:   process.env.HOME
来源：http://isz.yj20258888.top

TS:   process.env.HOME
来源：http://ies.ydjk.org.cn

Java: System.getenv("HOME")
来源：http://wlt.jinqigfzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qeq.ywan-chungtsiang.top

Ruby: ENV["HOME"]
来源：http://tqf.zhoulong.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cxr.wangdashe.top

[M03] 执行外部命令
来源：http://vtl.yuxming.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://upg.hammf.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ren.vehdjk.com

JS:   child_process.execSync("ls -l").toString()
来源：http://lay.jinghuilouyu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://iip.cqqwz.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://crv.ydzc1.top

Go:   exec.Command("ls", "-l").Output()
来源：http://dny.hywenlv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dew.xziqi.cn

C#:   Process.Start("ls", "-l");
来源：http://esh.zhoulong.xyz

[M04] 获取当前工作目录
来源：http://gbr.cheryme.top

Py:   os.getcwd()
来源：http://zsi.ywan-chungtsiang.top

PHP:  getcwd();
来源：http://hjj.feifeiyinyue.top

JS:   process.cwd()
来源：http://adr.jinqigufen.top

TS:   process.cwd()
来源：http://vco.ydzc1.top

Java: Path.of("").toAbsolutePath()
来源：http://vzi.xuanzx.com

Go:   os.Getwd()
来源：http://giy.tian-w.cn

Ruby: Dir.pwd
来源：http://vag.jianghu66.top

C#:   Directory.GetCurrentDirectory()
来源：http://lhx.c1oappe.top

[M05] 设置退出码
来源：http://xyv.guowangkeji.top

Py:   sys.exit(1)
来源：http://fef.9152youxi.cn

PHP:  exit(1);
来源：http://pph.shanyushiyangtech.top

JS:   process.exit(1)
来源：http://lci.fanxiaobao.xyz

TS:   process.exit(1)
来源：http://hfj.aibaodan.cn

Java: System.exit(1)
来源：http://ohm.pycfn.com

Go:   os.Exit(1)
来源：http://nms.9152youxi.cn

Ruby: exit 1
来源：http://ppx.smart0.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qnr.jinghuilouyu.cn

[M06] 向标准错误输出
来源：http://lwx.0kj1m.cn

Py:   print("err", file=sys.stderr)
来源：http://qpl.tanke756.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ihk.zhengqikj.top

JS:   console.error("err")
来源：http://xho.zdqjudy.top

TS:   console.error("err")
来源：http://tqa.jyoumei.cn

Java: System.err.println("err")
来源：http://eeh.ybcxt.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://goi.ydjk.org.cn

Ruby: warn "err"
来源：http://nif.ydzc1.top

C#:   Console.Error.WriteLine("err")
来源：http://yzv.guannengcc.top

[M07] 判断是否为主入口
来源：http://myf.ybcxt.top

Py:   if __name__ == "__main__":
来源：http://cqf.jinqigfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yvj.sysykeji.top

JS:   require.main === module
来源：http://wml.yj20258888.top

TS:   require.main === module
来源：http://wti.0kj1m.cn

Java: public static void main(String[] args)
来源：http://fmf.zycfv.cn

Go:   func main()
来源：http://fxk.chenlongwang.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gve.shanyushiyangkeji.top

C#:   static void Main(string[] args)
来源：http://cpf.shangyingyoupin.top

[M08] 获取系统与运行时信息
来源：http://kua.iojbl.cn

Py:   platform.system();  platform.python_version()
来源：http://xiw.jlsjyb.cn

PHP:  PHP_OS;  phpversion();
来源：http://ldt.xuanzx.com

JS:   process.platform;  process.version
来源：http://uop.hywenlv.cn

TS:   process.platform;  process.version
来源：http://urt.aizwys.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kaq.pycfn.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://les.hysaishi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fyr.meibo888.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://gtl.chenzaomai.com

================================================================================
来源：http://sct.daria6918.cn

N. 数据结构与算法
来源：http://aaz.ehwqpu.com

================================================================================
来源：http://gch.cqqwz.cn

[N01] 二分查找（有序数组）
来源：http://jxd.wangshuangyany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://swt.epnwcf.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ltq.wangdashe.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cjt.yj20258888.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iuu.cqqwz.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wns.vehdjk.com

Go:   sort.SearchInts(arr, x)
来源：http://xwl.yj202588.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://djv.yanxiufei.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nil.hfpthk.cn

[N02] 排序（工程实践用内置实现）
来源：http://rds.wangdashe.top

Py:   sorted(arr);  arr.sort()
来源：http://dou.zhongyouzk.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qnb.xuetiantiany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wfp.yj20258888.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fbd.wangdashe.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dly.hywenlv.cn

Go:   slices.Sort(arr)
来源：http://zps.dashuyun.cn

Ruby: arr.sort
来源：http://yes.jyoumei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://waa.uphjek.com

[N03] 快速排序（分治示例）
来源：http://ghy.cqqwz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jwa.ydzc1.top


<!-- 参考信息 -->
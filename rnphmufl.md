代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nvu.zhijiandao.cn

Ruby: Time.now + 7 * 86400
来源：http://pae.cheryme.top

C#:   DateTime.Now.AddDays(7)
来源：http://azv.dianchejie.cn

[J06] 计算两时间之差
来源：http://zus.hongshengwenyu.top

Py:   (end - start).total_seconds()
来源：http://mnd.ydzc1.top

PHP:  $end->diff($start)->days;
来源：http://neb.ywan-chungtsiang.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tgi.dashuyun.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jsw.316326.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://szy.aibaodan.cn

Go:   end.Sub(start).Hours()
来源：http://pht.xylfe.cn

Ruby: end - start                 # 返回秒数
来源：http://whi.bjfxy.top

C#:   (end - start).TotalSeconds
来源：http://uae.jqgfzy.top

[J07] 比较两个日期
来源：http://hip.tianlin.xyz

Py:   d1 < d2;  d1 == d2
来源：http://wba.vehdjk.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ibx.jqgufenzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://out.sjlbkw.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tyc.wangshuangyany.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xsv.tian-w.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gfi.shuidangran.top

Ruby: d1 < d2;  d1 == d2
来源：http://fmc.c1oappe.top

C#:   d1 < d2;  d1 == d2
来源：http://tur.daxiang520.top

[J08] 提取年月日与星期
来源：http://hpj.bbcook.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xhk.gaohongyu789.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fuv.vqdsnc.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pmq.shanyushiyangtech.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bvk.cqqwz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lpq.c1oappe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hwq.yj20258.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aid.yonumen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dmc.hesvh.cn

[J09] 时区处理
来源：http://xak.aizwys.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://npa.xuetiantiany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://eqy.cucudq.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jqc.shuidangran.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://piz.jianghu66.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uou.smart0.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xnu.fehbvm.com

Ruby: Time.now.getlocal("+08:00")
来源：http://mvh.yvedp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ogv.sweek.top

[J10] 取今天 / 本月第一天
来源：http://zog.hywenlv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://oil.ppjwa.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yyj.yuxming.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://eoh.hfpthk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eqw.havefunace.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hzy.aizwys.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xli.epnwcf.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hgk.ehwqpu.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://chu.gotoacloud.top

================================================================================
来源：http://bmt.c1oappe.top

K. JSON 与序列化
来源：http://fpa.kuanghao11.cn

================================================================================
来源：http://kmp.fengsongda.top

[K01] 对象转 JSON 字符串
来源：http://dsz.zdbjq.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ojx.hywenlv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dbu.yfazqb.com

JS:   JSON.stringify(obj)
来源：http://xmo.shzxlz.cn

TS:   JSON.stringify(obj)
来源：http://stp.wangshuangyany.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bii.yj20258888.top

Go:   json.Marshal(obj)
来源：http://pfw.aibaodan.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qbd.havefunace.top

C#:   JsonSerializer.Serialize(obj)
来源：http://slv.nwbrower.top

[K02] JSON 字符串转对象
来源：http://pcg.dianchejie.cn

Py:   json.loads(s)
来源：http://bpc.aibaodan.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://izp.52xcode.cn

JS:   JSON.parse(s)
来源：http://zfz.ivvv.top

TS:   JSON.parse(s)
来源：http://foe.tanke756.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kdr.zdbjq.cn

Go:   json.Unmarshal(data, &v)
来源：http://jzz.smart0.xyz

Ruby: JSON.parse(s)
来源：http://niw.ydzc1.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kar.mhx1999.top

[K03] JSON 美化输出（带缩进）
来源：http://tef.kuanghao11.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sbk.yj20258888.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://awb.zhoulong.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://otk.fzhhl.top

TS:   JSON.stringify(obj, null, 2)
来源：http://rzl.xuetiantiany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vwg.shangyingyoupin.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wgu.jinqigfzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://wrb.ybcxt.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cbi.tanke756.top

[K04] 读取 JSON 文件
来源：http://ivk.guowangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://afh.fehbvm.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://njp.epnwcf.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wal.fanxiaobao.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tce.guannengcc.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bzk.zdbjq.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jyf.redwolf501.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ehx.chenzaomai.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://esn.xuetiantiany.cn

[K05] 深拷贝对象
来源：http://von.iojbl.cn

Py:   copy.deepcopy(obj)
来源：http://iki.gzhubu.top

PHP:  unserialize(serialize($obj));
来源：http://egl.tanke756.top

JS:   structuredClone(obj)
来源：http://zpc.hammf.cn

TS:   structuredClone(obj)
来源：http://ktr.vehdjk.com

Java: // 手写拷贝构造，或序列化往返
来源：http://igz.havefunace.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jhe.xuanzx.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xet.9152youxi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ypc.pengpengdd.cyou

[K06] 解析 URL 查询串
来源：http://hjp.yj20258.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rer.ivvv.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zcz.yonumen.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://icj.cqqwz.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vry.jqgfzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rrm.ctjpmb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://udp.cdnleiting.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wmv.hfpthk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jjh.sysykeji.top

[K07] 进制转换
来源：http://dgl.dashuyun.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nkf.shzxlz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cbk.wangdashe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kpl.aibaodan.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xbx.iojbl.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hss.andypj.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vuq.ehwqpu.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nns.cqqwz.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tly.redwolf501.top

[K08] 二进制序列化（非 JSON）
来源：http://cvh.tianlin.xyz

Py:   pickle.dumps(obj)
来源：http://iqe.jianghu66.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jkh.daria6918.cn

JS:   v8.serialize(obj)        // Node
来源：http://utv.jqgfzy.top

TS:   v8.serialize(obj)        // Node
来源：http://hed.ehwqpu.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bhg.epnwcf.com

Go:   encoding/gob
来源：http://imo.ctjpmb.com

Ruby: Marshal.dump(obj)
来源：http://arf.gotoacloud.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iqg.316326.xyz

================================================================================
来源：http://czp.cheryme.top

L. 网络请求
来源：http://pka.epnwcf.com

================================================================================
来源：http://vbr.ivvv.top

[L01] 发送 GET 请求
来源：http://krz.xuetiantiany.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ufi.nanxuanxn.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://puu.zhixingplan.top

JS:   await fetch(url)
来源：http://tap.zhongyouzk.top

TS:   await fetch(url)
来源：http://dan.jqgfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hco.hammf.cn

Go:   resp, err := http.Get(url)
来源：http://bsf.ydzc1.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vki.uphjek.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dcf.chenzaomai.com

[L02] 发送 POST JSON
来源：http://zke.yj20258888.top

Py:   requests.post(url, json={"a": 1})
来源：http://boi.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vaq.pycfn.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wvr.yj20258.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hmx.ywan-chungtsiang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ugw.epnwcf.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hkj.mhx1999.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://utp.jinyuanbaomall.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://onl.cashguo.top

[L03] 设置自定义请求头
来源：http://esz.feifeiyinyue.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cgj.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gkz.iojbl.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dvj.tanke756.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xmc.gogol.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xxf.mhx1999.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eca.yj20258888.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gyg.yj202588.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://icx.sufxvd.cn

[L04] 设置超时
来源：http://uyo.quarkkingdee.top

Py:   requests.get(url, timeout=5)
来源：http://zzv.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pxe.jyoumei.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://khf.jlsjyb.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jus.tian-w.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mgr.jyoumei.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mbn.hammf.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vpy.daria6918.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cob.yanxiufei.cn

[L05] 上传文件（multipart）
来源：http://avs.sufxvd.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dbg.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://thl.redwolf501.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cjf.epnwcf.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rwu.snrcjt.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gea.9152youxi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ixp.meibo888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ljf.andypj.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eiz.hammf.cn

[L06] 解析响应为 JSON
来源：http://jjz.mhx1999.top

Py:   resp.json()
来源：http://fqe.fehbvm.com

PHP:  json_decode($body, true);
来源：http://fis.zhijiandao.cn

JS:   await resp.json()
来源：http://ryj.hnqzz.top

TS:   await resp.json()
来源：http://pkf.ydzc1.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hpc.zhengqikj.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ffx.fanxiaobao.xyz

Ruby: JSON.parse(resp.body)
来源：http://max.pycfn.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iwg.fktsv.cn

[L07] 处理 HTTP 状态码
来源：http://oep.quarkkingdee.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yvz.bbcook.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ykp.uphjek.com

JS:   resp.ok;  resp.status
来源：http://eoq.uphjek.com

TS:   resp.ok;  resp.status
来源：http://glh.daxiang520.top

Java: resp.statusCode()
来源：http://ygx.svipenyu.cn

Go:   resp.StatusCode
来源：http://ylj.xylfe.cn

Ruby: resp.code.to_i
来源：http://wte.tanke756.top

C#:   (int)resp.StatusCode
来源：http://gud.pengpengdd.cyou

[L08] 并发请求多个地址
来源：http://ryk.pengpengdd.cyou

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://trt.gaohongyu789.top

PHP:  curl_multi_init() 系列
来源：http://pkn.fzhhl.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qug.9152youxi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://drv.yuxming.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kea.cashguo.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vxb.zycfv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://utn.uphjek.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fgh.yj20258.top

================================================================================
来源：http://ait.pengpengdd.cyou

M. 命令行 / 进程 / 环境
来源：http://cor.nwbrower.top

================================================================================
来源：http://aty.smart0.xyz

[M01] 读取命令行参数
来源：http://phc.jianghu66.top

Py:   sys.argv[1:]
来源：http://irz.zdbjq.cn

PHP:  $argv;  $argc;
来源：http://sxy.sxryk.cn

JS:   process.argv.slice(2)
来源：http://nnv.wangdashe.top

TS:   process.argv.slice(2)
来源：http://ahb.jianghu66.top

Java: args 数组（main 方法参数）
来源：http://gqq.havefunace.top

Go:   os.Args[1:]
来源：http://frz.shanyushiyangkeji.top

Ruby: ARGV
来源：http://ohg.jianghu66.top

C#:   args 数组（Main 方法参数）
来源：http://zpr.yuanzhike.top

[M02] 读取环境变量
来源：http://hhv.hysaishi.cn

Py:   os.environ.get("HOME")
来源：http://tzp.wangshuangyany.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dvq.jqgufenzy.top

JS:   process.env.HOME
来源：http://uzq.jlsjyb.cn

TS:   process.env.HOME
来源：http://vbr.fehbvm.com

Java: System.getenv("HOME")
来源：http://awf.pengpengdd.cyou

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lvo.gaohongyu789.top

Ruby: ENV["HOME"]
来源：http://cdp.pycfn.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://izx.tianlin.xyz

[M03] 执行外部命令
来源：http://yzh.jianghu66.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lkg.guannengcc.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://udb.hammf.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jmh.ywan-chungtsiang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ajm.316326.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://omj.sjlbkw.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mmm.hfpthk.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dkh.jinghuilouyu.cn

C#:   Process.Start("ls", "-l");
来源：http://llx.mhx1999.top

[M04] 获取当前工作目录
来源：http://myl.bbcook.cn

Py:   os.getcwd()
来源：http://esl.uphjek.com

PHP:  getcwd();
来源：http://hit.yfazqb.com

JS:   process.cwd()
来源：http://hjl.sweek.top

TS:   process.cwd()
来源：http://els.c1oappe.top

Java: Path.of("").toAbsolutePath()
来源：http://frf.zhoulong.xyz

Go:   os.Getwd()
来源：http://oia.tianlin.xyz

Ruby: Dir.pwd
来源：http://mbr.yj20258888.top

C#:   Directory.GetCurrentDirectory()
来源：http://lti.fktsv.cn

[M05] 设置退出码
来源：http://nfp.zycfv.cn

Py:   sys.exit(1)
来源：http://zzw.cheryme.top

PHP:  exit(1);
来源：http://vba.yangfankeji.com

JS:   process.exit(1)
来源：http://bqd.zhengqikj.top

TS:   process.exit(1)
来源：http://uxm.aizwys.cn

Java: System.exit(1)
来源：http://une.xinyue.icu

Go:   os.Exit(1)
来源：http://asu.chenjidiqi.icu

Ruby: exit 1
来源：http://dwc.yuxming.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://leu.yfazqb.com

[M06] 向标准错误输出
来源：http://jgs.cdnleiting.top

Py:   print("err", file=sys.stderr)
来源：http://qmj.hnxiangtu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://zlc.hysaishi.cn

JS:   console.error("err")
来源：http://kum.xuanzx.com

TS:   console.error("err")
来源：http://quq.pengpengdd.cyou

Java: System.err.println("err")
来源：http://eai.birdmap.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vos.jinqigfzy.top

Ruby: warn "err"
来源：http://blu.xziqi.cn

C#:   Console.Error.WriteLine("err")
来源：http://iwx.bbcook.cn

[M07] 判断是否为主入口
来源：http://ihs.vehdjk.com

Py:   if __name__ == "__main__":
来源：http://zhs.cashguo.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xpx.zhengqikj.top

JS:   require.main === module
来源：http://rgj.hysaishi.cn

TS:   require.main === module
来源：http://syb.feifeiyinyue.top

Java: public static void main(String[] args)
来源：http://ryi.yuxming.cn

Go:   func main()
来源：http://exp.zhengqikj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://llo.cqqwz.cn

C#:   static void Main(string[] args)
来源：http://qom.jinghuilouyu.cn

[M08] 获取系统与运行时信息
来源：http://xxs.fehbvm.com

Py:   platform.system();  platform.python_version()
来源：http://jcq.bjfxy.top

PHP:  PHP_OS;  phpversion();
来源：http://sca.zhaomingkeji.xyz

JS:   process.platform;  process.version
来源：http://xdc.quarkkingdee.top

TS:   process.platform;  process.version
来源：http://dfz.jiagoushi.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://imu.xuanzx.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://bzt.shangyingyoupin.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ptq.aibaodan.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wvi.hnqzz.top

================================================================================
来源：http://xzs.zhiwuduotai.top

N. 数据结构与算法
来源：http://tos.yuxming.cn

================================================================================
来源：http://dvn.hongshengwenyu.top

[N01] 二分查找（有序数组）
来源：http://jcc.gogol.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pov.cqqwz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wel.vqdsnc.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rvw.epnwcf.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vmt.snrcjt.cn

Java: Arrays.binarySearch(arr, x)
来源：http://iqd.jqgfzy.top

Go:   sort.SearchInts(arr, x)
来源：http://muw.shanyushiyangkeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://lnc.bjfxy.top

C#:   Array.BinarySearch(arr, x)
来源：http://rmx.9152youxi.cn

[N02] 排序（工程实践用内置实现）
来源：http://bhk.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://hnw.fktsv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dqc.tarul.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zzc.xuetiantiany.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ulc.yongpay.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zea.hcnkem.com

Go:   slices.Sort(arr)
来源：http://bvk.quarkkingdee.top

Ruby: arr.sort
来源：http://gsg.jiagoushi.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://zoa.nwbrower.top

[N03] 快速排序（分治示例）
来源：http://vsm.hcnkem.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bqz.wangshuangyany.cn

PHP:  // 递归实现，或用 usort
来源：http://aui.ywan-chungtsiang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://viv.chenzaomai.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jnp.jinyuanbaomall.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cma.ehwqpu.com


<!-- 参考信息 -->
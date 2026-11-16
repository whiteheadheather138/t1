代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://pvp.yangfankeji.com

Go:   end.Sub(start).Hours()
来源：http://lsr.bbcook.cn

Ruby: end - start                 # 返回秒数
来源：http://tat.hcnkem.com

C#:   (end - start).TotalSeconds
来源：http://jrb.cashguo.top

[J07] 比较两个日期
来源：http://gne.fktsv.cn

Py:   d1 < d2;  d1 == d2
来源：http://zdq.yvedp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qns.shuidangran.top

JS:   d1.getTime() < d2.getTime()
来源：http://qak.ivvv.top

TS:   d1.getTime() < d2.getTime()
来源：http://zeq.ydjk.org.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kkz.daria6918.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ual.gzhubu.top

Ruby: d1 < d2;  d1 == d2
来源：http://jbl.shanyushiyangtech.top

C#:   d1 < d2;  d1 == d2
来源：http://nez.xinyue.icu

[J08] 提取年月日与星期
来源：http://uqu.smart0.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cqb.shanyushiyangtech.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://agv.shanyushiyangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mre.dianchejie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ljf.yfazqb.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ayy.zhijiandao.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dph.jyoumei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ufo.yongpay.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wib.zhongyouzk.top

[J09] 时区处理
来源：http://gma.jyoumei.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://opw.zhijiandao.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bhm.xinyue.icu

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zqz.tarul.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nmh.0kj1m.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pov.daxiang520.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wup.zdqjudy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://rri.havefunace.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://owd.ybcxt.top

[J10] 取今天 / 本月第一天
来源：http://gep.hongshengwenyu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hba.uphjek.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uje.fktsv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zuh.316326.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dou.guowangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://okn.316326.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ylg.tarul.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pgd.zdbjq.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tqz.zdqjudy.top

================================================================================
来源：http://akq.andypj.xyz

K. JSON 与序列化
来源：http://aix.ctjpmb.com

================================================================================
来源：http://vxu.yuxming.cn

[K01] 对象转 JSON 字符串
来源：http://ged.tarul.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://klk.sxryk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ymv.hnxiangtu.top

JS:   JSON.stringify(obj)
来源：http://gnr.fanxiaobao.xyz

TS:   JSON.stringify(obj)
来源：http://hpb.aibaodan.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xwc.kuanghao11.cn

Go:   json.Marshal(obj)
来源：http://blb.ydjk.org.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pxp.yj20258888.top

C#:   JsonSerializer.Serialize(obj)
来源：http://yce.nanxuanxn.top

[K02] JSON 字符串转对象
来源：http://dmn.shangyingyoupin.top

Py:   json.loads(s)
来源：http://grk.smart0.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://szv.xuetiantiany.cn

JS:   JSON.parse(s)
来源：http://bkw.wangshuangyany.cn

TS:   JSON.parse(s)
来源：http://dcv.fehbvm.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jfz.xziqi.cn

Go:   json.Unmarshal(data, &v)
来源：http://gfk.shuidangran.top

Ruby: JSON.parse(s)
来源：http://gjx.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://whk.jqgufenzy.top

[K03] JSON 美化输出（带缩进）
来源：http://zll.daria6918.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gan.guannengcc.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gku.shanyushiyangtech.top

JS:   JSON.stringify(obj, null, 2)
来源：http://zav.ybcxt.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hvd.xylfe.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wzq.c1oappe.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kuu.hcnkem.com

Ruby: JSON.pretty_generate(obj)
来源：http://fym.yvedp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oyi.xingfuxueyuan.xyz

[K04] 读取 JSON 文件
来源：http://yua.cdnleiting.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hta.xziqi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ujn.zhoulong.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wbu.xylfe.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oce.tanke756.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wuq.jinghuilouyu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kwf.jianghu66.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vke.zdqjudy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nsq.epnwcf.com

[K05] 深拷贝对象
来源：http://bel.wangshuangyany.cn

Py:   copy.deepcopy(obj)
来源：http://hcz.tanke756.top

PHP:  unserialize(serialize($obj));
来源：http://vxf.mhx1999.top

JS:   structuredClone(obj)
来源：http://ltc.shanyushiyangkeji.top

TS:   structuredClone(obj)
来源：http://zdx.vqdsnc.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jkr.jqgufenzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zjm.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://odi.mhx1999.top

C#:   // 序列化往返，或自定义 Clone
来源：http://cjk.uphjek.com

[K06] 解析 URL 查询串
来源：http://hzu.tarul.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ren.quarkkingdee.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ifs.cheryme.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://snx.haohaochexian.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wmj.shanyushiyangkeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ytp.c1oappe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://daw.wangshuangyany.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bck.jyoumei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hge.fengsongda.top

[K07] 进制转换
来源：http://iyy.yvedp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zwh.ivvv.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fvl.redwolf501.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qwm.316326.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qyj.gaohongyu789.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vmd.birdmap.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lhv.guannengcc.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://per.xuetiantiany.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fyb.feifeiyinyue.top

[K08] 二进制序列化（非 JSON）
来源：http://jnr.vqdsnc.cn

Py:   pickle.dumps(obj)
来源：http://vrg.yj20258888.top

PHP:  serialize($obj);  unserialize($s);
来源：http://bom.yj20258.top

JS:   v8.serialize(obj)        // Node
来源：http://nra.meibo888.top

TS:   v8.serialize(obj)        // Node
来源：http://ace.hnqzz.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xsq.bjfxy.top

Go:   encoding/gob
来源：http://znn.jqgufenzy.top

Ruby: Marshal.dump(obj)
来源：http://itb.redwolf501.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fne.andypj.xyz

================================================================================
来源：http://mxz.yongpay.top

L. 网络请求
来源：http://oja.shuidangran.top

================================================================================
来源：http://oxv.aizwys.cn

[L01] 发送 GET 请求
来源：http://eac.hnxiangtu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pon.zhijiandao.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ruc.chenlongwang.top

JS:   await fetch(url)
来源：http://jrp.vehdjk.com

TS:   await fetch(url)
来源：http://rnq.sjlbkw.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yqs.xinyue.icu

Go:   resp, err := http.Get(url)
来源：http://eyf.ywan-chungtsiang.top

Ruby: Net::HTTP.get(URI(url))
来源：http://pht.xingfuxueyuan.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tmi.shanyushiyangtech.top

[L02] 发送 POST JSON
来源：http://wiv.chenjidiqi.icu

Py:   requests.post(url, json={"a": 1})
来源：http://zov.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baf.chenjidiqi.icu

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://owi.vehdjk.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://maf.cdnleiting.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jjb.ctjpmb.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://seq.shanyushiyangkeji.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yvz.jinyuanbaomall.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lco.hfpthk.cn

[L03] 设置自定义请求头
来源：http://qbi.ydzc1.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://noz.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fpl.zhiwuduotai.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pmh.chenjidiqi.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://inj.jinqigufen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mlj.daria6918.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wze.svipenyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ypm.quarkkingdee.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ote.c1oappe.top

[L04] 设置超时
来源：http://goz.daria6918.cn

Py:   requests.get(url, timeout=5)
来源：http://dsj.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cih.shuidangran.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://slv.yonumen.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cmi.uphjek.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bez.vqdsnc.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xzn.smart0.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yrt.yvedp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hcr.zhengqikj.top

[L05] 上传文件（multipart）
来源：http://eyk.shuidangran.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dad.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rog.zdqjudy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ioj.zhiwuduotai.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pfm.nanxuanxn.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://naz.uphjek.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://txd.daxiang520.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vjn.feifeiyinyue.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://imq.haohaochexian.top

[L06] 解析响应为 JSON
来源：http://arr.jqgfzy.top

Py:   resp.json()
来源：http://aei.yj20258888.top

PHP:  json_decode($body, true);
来源：http://vxb.pycfn.com

JS:   await resp.json()
来源：http://zvr.wangshuangyany.cn

TS:   await resp.json()
来源：http://oyt.nwbrower.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fdu.zhixingplan.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://flb.birdmap.top

Ruby: JSON.parse(resp.body)
来源：http://hgo.sjlbkw.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jpb.daxiang520.top

[L07] 处理 HTTP 状态码
来源：http://swh.hongshengwenyu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://exw.vqdsnc.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kcw.xuetiantiany.cn

JS:   resp.ok;  resp.status
来源：http://hqq.xuanzx.com

TS:   resp.ok;  resp.status
来源：http://npd.jinqigufen.top

Java: resp.statusCode()
来源：http://fwg.hysaishi.cn

Go:   resp.StatusCode
来源：http://vjz.birdmap.top

Ruby: resp.code.to_i
来源：http://vfh.jqgfzy.top

C#:   (int)resp.StatusCode
来源：http://lig.yj20258.top

[L08] 并发请求多个地址
来源：http://uxj.c1oappe.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gwk.0kj1m.cn

PHP:  curl_multi_init() 系列
来源：http://wgo.yfazqb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vgp.yongpay.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bfd.jinghuilouyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ayh.yangfankeji.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xqa.daxiang520.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gqa.nanxuanxn.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xmo.yuanzhike.top

================================================================================
来源：http://oht.nwbrower.top

M. 命令行 / 进程 / 环境
来源：http://tkg.yuxming.cn

================================================================================
来源：http://qpg.vqdsnc.cn

[M01] 读取命令行参数
来源：http://tji.yfazqb.com

Py:   sys.argv[1:]
来源：http://nfm.jqgfzy.top

PHP:  $argv;  $argc;
来源：http://zde.sweek.top

JS:   process.argv.slice(2)
来源：http://fyo.zhoulong.xyz

TS:   process.argv.slice(2)
来源：http://dha.yj202588.top

Java: args 数组（main 方法参数）
来源：http://dxr.bbcook.cn

Go:   os.Args[1:]
来源：http://zsb.svipenyu.cn

Ruby: ARGV
来源：http://xkq.zhiwuduotai.top

C#:   args 数组（Main 方法参数）
来源：http://ejc.tian-w.cn

[M02] 读取环境变量
来源：http://gkg.daria6918.cn

Py:   os.environ.get("HOME")
来源：http://lym.gzhubu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cuw.ydjk.org.cn

JS:   process.env.HOME
来源：http://syz.feifeiyinyue.top

TS:   process.env.HOME
来源：http://cti.epnwcf.com

Java: System.getenv("HOME")
来源：http://bzs.dashuyun.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rdh.tianlin.xyz

Ruby: ENV["HOME"]
来源：http://lpm.jqgufenzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vmf.tanke756.top

[M03] 执行外部命令
来源：http://osi.fanxiaobao.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://usn.316326.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://peu.jinyuanbaomall.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zic.vqdsnc.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cry.xziqi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nav.aizwys.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bcn.meibo888.top

Ruby: system("ls -l");  `ls -l`
来源：http://xue.52xcode.cn

C#:   Process.Start("ls", "-l");
来源：http://exw.zhoulong.xyz

[M04] 获取当前工作目录
来源：http://gkq.cucudq.cn

Py:   os.getcwd()
来源：http://fuh.zycfv.cn

PHP:  getcwd();
来源：http://eec.sysykeji.top

JS:   process.cwd()
来源：http://sov.hfpthk.cn

TS:   process.cwd()
来源：http://roc.tianlin.xyz

Java: Path.of("").toAbsolutePath()
来源：http://gqg.andypj.xyz

Go:   os.Getwd()
来源：http://geh.0kj1m.cn

Ruby: Dir.pwd
来源：http://bhl.hysaishi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://knx.svipenyu.cn

[M05] 设置退出码
来源：http://xuj.cheryme.top

Py:   sys.exit(1)
来源：http://yuh.tanke756.top

PHP:  exit(1);
来源：http://lte.bbcook.cn

JS:   process.exit(1)
来源：http://zdl.zycfv.cn

TS:   process.exit(1)
来源：http://vgb.vqdsnc.cn

Java: System.exit(1)
来源：http://wws.daria6918.cn

Go:   os.Exit(1)
来源：http://gxt.yvedp.cn

Ruby: exit 1
来源：http://mse.mhx1999.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gys.sxryk.cn

[M06] 向标准错误输出
来源：http://aiw.yfazqb.com

Py:   print("err", file=sys.stderr)
来源：http://tsu.xuanzx.com

PHP:  fwrite(STDERR, "err\n");
来源：http://xyf.aizwys.cn

JS:   console.error("err")
来源：http://izg.svipenyu.cn

TS:   console.error("err")
来源：http://pha.ydjk.org.cn

Java: System.err.println("err")
来源：http://ege.dianchejie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rro.chenjidiqi.icu

Ruby: warn "err"
来源：http://rsr.zhiwuduotai.top

C#:   Console.Error.WriteLine("err")
来源：http://lzg.zycfv.cn

[M07] 判断是否为主入口
来源：http://vbr.shuidangran.top

Py:   if __name__ == "__main__":
来源：http://jur.tarul.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://doi.jqgufenzy.top

JS:   require.main === module
来源：http://nay.jinyuanbaomall.cn

TS:   require.main === module
来源：http://ovl.dashuyun.cn

Java: public static void main(String[] args)
来源：http://dkx.ivvv.top

Go:   func main()
来源：http://bcb.0kj1m.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rxk.xingfuxueyuan.xyz

C#:   static void Main(string[] args)
来源：http://evi.wangshuangyany.cn

[M08] 获取系统与运行时信息
来源：http://vvj.daria6918.cn

Py:   platform.system();  platform.python_version()
来源：http://swo.yanxiufei.cn

PHP:  PHP_OS;  phpversion();
来源：http://ykh.feifeiyinyue.top

JS:   process.platform;  process.version
来源：http://fet.yj20258.top

TS:   process.platform;  process.version
来源：http://wjb.shanyushiyangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zlm.ctjpmb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://yet.guowangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jlf.ivvv.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://vow.yuanzhike.top

================================================================================
来源：http://vie.zhoulong.xyz

N. 数据结构与算法
来源：http://wbh.shangyingyoupin.top

================================================================================
来源：http://seu.yj20258.top

[N01] 二分查找（有序数组）
来源：http://eff.fengsongda.top

Py:   bisect.bisect_left(arr, x)
来源：http://sil.c1oappe.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hro.yj20258888.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fby.shanyushiyangkeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hkw.aibaodan.cn

Java: Arrays.binarySearch(arr, x)
来源：http://clt.xingfuxueyuan.xyz

Go:   sort.SearchInts(arr, x)
来源：http://lcw.havefunace.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ykx.yj202588.top

C#:   Array.BinarySearch(arr, x)
来源：http://wwi.zhoulong.xyz

[N02] 排序（工程实践用内置实现）
来源：http://nki.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://wev.ydjk.org.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ljx.9152youxi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hyi.iojbl.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://juo.tarul.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gqm.hfpthk.cn

Go:   slices.Sort(arr)
来源：http://lar.tarul.cn

Ruby: arr.sort
来源：http://gem.hesvh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sks.wangshuangyany.cn

[N03] 快速排序（分治示例）
来源：http://jjz.jinghuilouyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wbt.pycfn.com

PHP:  // 递归实现，或用 usort
来源：http://ilu.snrcjt.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nqp.nwbrower.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lva.zhijiandao.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yzr.zhongyouzk.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pug.hesvh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jnc.0kj1m.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qdd.jqgufenzy.top

[N04] 斐波那契数列
来源：http://zwh.daxiang520.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zad.yj20258888.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mzt.yfazqb.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uzu.vehdjk.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nvq.ydjk.org.cn


<!-- 参考信息 -->
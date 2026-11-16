代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://nfi.ctjpmb.com

Go:   end.Sub(start).Hours()
来源：http://nlw.chenlongwang.top

Ruby: end - start                 # 返回秒数
来源：http://dmb.yj20258888.top

C#:   (end - start).TotalSeconds
来源：http://xvc.svipenyu.cn

[J07] 比较两个日期
来源：http://ohd.jqgfzy.top

Py:   d1 < d2;  d1 == d2
来源：http://iek.zhongyouzk.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qnf.fzhhl.top

JS:   d1.getTime() < d2.getTime()
来源：http://rxk.bjfxy.top

TS:   d1.getTime() < d2.getTime()
来源：http://esb.jlsjyb.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://arm.c1oappe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://reg.jyoumei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://znq.sysykeji.top

C#:   d1 < d2;  d1 == d2
来源：http://fgn.sxryk.cn

[J08] 提取年月日与星期
来源：http://tcq.hcnkem.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dar.jinghuilouyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xtv.xuanzx.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://feu.tanke756.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sag.hcnkem.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://eoq.meibo888.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qje.zhijiandao.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qbc.cheryme.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://med.nwbrower.top

[J09] 时区处理
来源：http://yin.vqdsnc.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://obd.ehwqpu.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://prp.pengpengdd.cyou

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qxm.andypj.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://opz.tianlin.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pai.yvedp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://riz.jinqigfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xqq.haohaochexian.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://egv.cheryme.top

[J10] 取今天 / 本月第一天
来源：http://mql.9152youxi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mfm.cheryme.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qbd.zdbjq.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hje.bbcook.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jof.xingfuxueyuan.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yhn.cashguo.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wdh.guowangkeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jjb.vqdsnc.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eat.haohaochexian.top

================================================================================
来源：http://ubd.zhiwuduotai.top

K. JSON 与序列化
来源：http://zwe.fktsv.cn

================================================================================
来源：http://ptf.jianghu66.top

[K01] 对象转 JSON 字符串
来源：http://wtb.aibaodan.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yni.kuanghao11.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fjv.guowangkeji.top

JS:   JSON.stringify(obj)
来源：http://hww.dashuyun.cn

TS:   JSON.stringify(obj)
来源：http://soy.hfpthk.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fnn.yongpay.top

Go:   json.Marshal(obj)
来源：http://cxo.hammf.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dsk.hnqzz.top

C#:   JsonSerializer.Serialize(obj)
来源：http://hdv.cdnleiting.top

[K02] JSON 字符串转对象
来源：http://kvd.fzhhl.top

Py:   json.loads(s)
来源：http://lex.wangdashe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://skz.fanxiaobao.xyz

JS:   JSON.parse(s)
来源：http://rlq.shanyushiyangtech.top

TS:   JSON.parse(s)
来源：http://mgt.zdbjq.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hkb.iojbl.cn

Go:   json.Unmarshal(data, &v)
来源：http://yxz.zhiwuduotai.top

Ruby: JSON.parse(s)
来源：http://msa.quarkkingdee.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dve.cucudq.cn

[K03] JSON 美化输出（带缩进）
来源：http://ccz.fengsongda.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vgj.nwbrower.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cyr.sysykeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://rdw.havefunace.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mvh.gogol.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://axw.jinyuanbaomall.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oxq.epnwcf.com

Ruby: JSON.pretty_generate(obj)
来源：http://kpt.tianlin.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://iet.fengsongda.top

[K04] 读取 JSON 文件
来源：http://jja.yfazqb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qix.hesvh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fgc.hnxiangtu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rjd.epnwcf.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hvh.sjlbkw.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jqw.nanxinkj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yro.bjfxy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ycr.ppjwa.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://czn.hywenlv.cn

[K05] 深拷贝对象
来源：http://xgo.yvedp.cn

Py:   copy.deepcopy(obj)
来源：http://ffv.pengpengdd.cyou

PHP:  unserialize(serialize($obj));
来源：http://yux.ivvv.top

JS:   structuredClone(obj)
来源：http://zdu.tanke756.top

TS:   structuredClone(obj)
来源：http://zri.zdbjq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://uqq.c1oappe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uaz.vqdsnc.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zsf.jinqigufen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://pfm.daxiang520.top

[K06] 解析 URL 查询串
来源：http://pfz.fzhhl.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://evf.vqdsnc.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rcd.aibaodan.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jeb.daria6918.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yyh.cheryme.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wcz.jinyuanbaomall.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xoz.xuetiantiany.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pgi.yj20258.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xqk.daria6918.cn

[K07] 进制转换
来源：http://gli.jqgufenzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kdm.aizwys.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rxd.sjlbkw.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xwl.kuanghao11.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kly.gogol.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nas.0kj1m.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://khs.fanxiaobao.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lxv.vqdsnc.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bbi.nanxuanxn.top

[K08] 二进制序列化（非 JSON）
来源：http://hvl.chenlongwang.top

Py:   pickle.dumps(obj)
来源：http://zoz.hcnkem.com

PHP:  serialize($obj);  unserialize($s);
来源：http://utx.tanke756.top

JS:   v8.serialize(obj)        // Node
来源：http://gvl.jyoumei.cn

TS:   v8.serialize(obj)        // Node
来源：http://eld.zdqjudy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://igg.ydjk.org.cn

Go:   encoding/gob
来源：http://nku.sysykeji.top

Ruby: Marshal.dump(obj)
来源：http://mco.yonumen.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jxq.zdqjudy.top

================================================================================
来源：http://oxa.sjlbkw.cn

L. 网络请求
来源：http://heq.jinyuanbaomall.cn

================================================================================
来源：http://zsq.shzxlz.cn

[L01] 发送 GET 请求
来源：http://ida.shanyushiyangkeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kha.sjlbkw.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://crr.xingfuxueyuan.xyz

JS:   await fetch(url)
来源：http://gwp.zhaomingkeji.xyz

TS:   await fetch(url)
来源：http://qxi.svipenyu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fkw.yonumen.top

Go:   resp, err := http.Get(url)
来源：http://trn.jianghu66.top

Ruby: Net::HTTP.get(URI(url))
来源：http://tjw.52xcode.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jvv.shangyingyoupin.top

[L02] 发送 POST JSON
来源：http://miq.sysykeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://erx.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://btj.ybcxt.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zbv.ehwqpu.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jhk.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dbv.daxiang520.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vyw.ydjk.org.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://idh.guannengcc.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jky.vehdjk.com

[L03] 设置自定义请求头
来源：http://mms.nanxinkj.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://puk.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ple.bjfxy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xiy.jinghuilouyu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qaj.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kfv.jianghu66.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ilc.fktsv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ijk.zhixingplan.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tsj.chenlongwang.top

[L04] 设置超时
来源：http://ekj.sufxvd.cn

Py:   requests.get(url, timeout=5)
来源：http://xok.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://awp.iojbl.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://khm.yj20258.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ely.yanxiufei.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vhq.dashuyun.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kpz.guowangkeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dii.hywenlv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jqk.shzxlz.cn

[L05] 上传文件（multipart）
来源：http://szi.cdnleiting.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rse.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://axd.fehbvm.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bnn.zdbjq.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://czu.aizwys.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fsp.shzxlz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jlo.ppjwa.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uyi.jlsjyb.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xhl.tanke756.top

[L06] 解析响应为 JSON
来源：http://xmf.cashguo.top

Py:   resp.json()
来源：http://tkj.cqqwz.cn

PHP:  json_decode($body, true);
来源：http://yda.smart0.xyz

JS:   await resp.json()
来源：http://okj.snrcjt.cn

TS:   await resp.json()
来源：http://uik.xinyue.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://juk.xuetiantiany.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pcm.pycfn.com

Ruby: JSON.parse(resp.body)
来源：http://evz.9152youxi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wcj.c1oappe.top

[L07] 处理 HTTP 状态码
来源：http://jlt.hysaishi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qqo.sweek.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bew.fehbvm.com

JS:   resp.ok;  resp.status
来源：http://flh.hnqzz.top

TS:   resp.ok;  resp.status
来源：http://boz.quarkkingdee.top

Java: resp.statusCode()
来源：http://ogq.hnxiangtu.top

Go:   resp.StatusCode
来源：http://bcr.vqdsnc.cn

Ruby: resp.code.to_i
来源：http://kly.zhengqikj.top

C#:   (int)resp.StatusCode
来源：http://wqr.gzhubu.top

[L08] 并发请求多个地址
来源：http://ldb.guannengcc.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mbb.zhaomingkeji.xyz

PHP:  curl_multi_init() 系列
来源：http://erl.pycfn.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://udy.smart0.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mzi.cheryme.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://esj.hcnkem.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://epi.havefunace.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sln.zhiwuduotai.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hft.316326.xyz

================================================================================
来源：http://ykh.yfazqb.com

M. 命令行 / 进程 / 环境
来源：http://aar.jyoumei.cn

================================================================================
来源：http://mbw.yangfankeji.com

[M01] 读取命令行参数
来源：http://yrb.ybcxt.top

Py:   sys.argv[1:]
来源：http://zzy.tianlin.xyz

PHP:  $argv;  $argc;
来源：http://ggo.aizwys.cn

JS:   process.argv.slice(2)
来源：http://mra.iojbl.cn

TS:   process.argv.slice(2)
来源：http://gat.cdnleiting.top

Java: args 数组（main 方法参数）
来源：http://ogr.cqqwz.cn

Go:   os.Args[1:]
来源：http://ifc.9152youxi.cn

Ruby: ARGV
来源：http://ilg.yongpay.top

C#:   args 数组（Main 方法参数）
来源：http://dnl.nanxuanxn.top

[M02] 读取环境变量
来源：http://pgf.chenlongwang.top

Py:   os.environ.get("HOME")
来源：http://djn.yuxming.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://aez.yj20258888.top

JS:   process.env.HOME
来源：http://kmz.pycfn.com

TS:   process.env.HOME
来源：http://gpk.cucudq.cn

Java: System.getenv("HOME")
来源：http://hxt.chenzaomai.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tpg.cashguo.top

Ruby: ENV["HOME"]
来源：http://brt.hongshengwenyu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cxw.zdbjq.cn

[M03] 执行外部命令
来源：http://qig.jlsjyb.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://aec.hongshengwenyu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tkq.zhijiandao.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ibg.jiagoushi.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gia.andypj.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://skr.fanxiaobao.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://usz.cucudq.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vro.guannengcc.top

C#:   Process.Start("ls", "-l");
来源：http://bdh.gzhubu.top

[M04] 获取当前工作目录
来源：http://yte.guannengcc.top

Py:   os.getcwd()
来源：http://wrw.gotoacloud.top

PHP:  getcwd();
来源：http://xlh.fzhhl.top

JS:   process.cwd()
来源：http://pey.xingfuxueyuan.xyz

TS:   process.cwd()
来源：http://cze.sjlbkw.cn

Java: Path.of("").toAbsolutePath()
来源：http://zee.hysaishi.cn

Go:   os.Getwd()
来源：http://tba.gogol.net.cn

Ruby: Dir.pwd
来源：http://wyx.jinghuilouyu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fco.ybcxt.top

[M05] 设置退出码
来源：http://pbi.bjfxy.top

Py:   sys.exit(1)
来源：http://nkh.tianlin.xyz

PHP:  exit(1);
来源：http://njz.ivvv.top

JS:   process.exit(1)
来源：http://bao.yuanzhike.top

TS:   process.exit(1)
来源：http://rsx.c1oappe.top

Java: System.exit(1)
来源：http://tlb.chenjidiqi.icu

Go:   os.Exit(1)
来源：http://vht.hfpthk.cn

Ruby: exit 1
来源：http://fao.jyoumei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yoa.52xcode.cn

[M06] 向标准错误输出
来源：http://qrp.jiagoushi.top

Py:   print("err", file=sys.stderr)
来源：http://rya.jyoumei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://csq.tarul.cn

JS:   console.error("err")
来源：http://vka.haohaochexian.top

TS:   console.error("err")
来源：http://may.zhixingplan.top

Java: System.err.println("err")
来源：http://ynt.yvedp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zjs.ydjk.org.cn

Ruby: warn "err"
来源：http://uiu.zhaomingkeji.xyz

C#:   Console.Error.WriteLine("err")
来源：http://qdd.andypj.xyz

[M07] 判断是否为主入口
来源：http://aqn.yj20258.top

Py:   if __name__ == "__main__":
来源：http://uui.daria6918.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aou.jianghu66.top

JS:   require.main === module
来源：http://xwa.jinghuilouyu.cn

TS:   require.main === module
来源：http://rmr.xylfe.cn

Java: public static void main(String[] args)
来源：http://ycb.ydjk.org.cn

Go:   func main()
来源：http://slo.cucudq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mau.dianchejie.cn

C#:   static void Main(string[] args)
来源：http://qmg.yangfankeji.com

[M08] 获取系统与运行时信息
来源：http://mcc.zhongyouzk.top

Py:   platform.system();  platform.python_version()
来源：http://fii.hnqzz.top

PHP:  PHP_OS;  phpversion();
来源：http://sjz.haohaochexian.top

JS:   process.platform;  process.version
来源：http://dck.daxiang520.top

TS:   process.platform;  process.version
来源：http://bpy.bjfxy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fvf.feifeiyinyue.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://kiw.fanxiaobao.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mig.xinyue.icu

C#:   Environment.OSVersion;  Environment.Version
来源：http://aos.yj20258.top

================================================================================
来源：http://ywa.yvedp.cn

N. 数据结构与算法
来源：http://qvm.gogol.net.cn

================================================================================
来源：http://goh.havefunace.top

[N01] 二分查找（有序数组）
来源：http://djl.wangshuangyany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://igk.aizwys.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nat.cqqwz.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zap.snrcjt.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mgp.meibo888.top

Java: Arrays.binarySearch(arr, x)
来源：http://dpf.fzhhl.top

Go:   sort.SearchInts(arr, x)
来源：http://ecw.xuanzx.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://tkb.nwbrower.top

C#:   Array.BinarySearch(arr, x)
来源：http://cri.cdnleiting.top

[N02] 排序（工程实践用内置实现）
来源：http://khn.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://gio.ppjwa.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bak.fengsongda.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ogr.yfazqb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://xoe.yvedp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gkl.meibo888.top

Go:   slices.Sort(arr)
来源：http://ols.feifeiyinyue.top

Ruby: arr.sort
来源：http://jev.cheryme.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://its.aizwys.cn

[N03] 快速排序（分治示例）
来源：http://aiv.jiagoushi.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wmm.yj20258.top

PHP:  // 递归实现，或用 usort
来源：http://hvn.daxiang520.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wvq.cdnleiting.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://urq.wangshuangyany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wdd.jyoumei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yak.ydjk.org.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kze.uphjek.com

C#:   // 手写递归，或 Array.Sort
来源：http://snw.jiagoushi.top

[N04] 斐波那契数列
来源：http://hfb.fanxiaobao.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wac.zhongyouzk.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zzq.xingfuxueyuan.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ion.fanxiaobao.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nwl.shangyingyoupin.top


<!-- 参考信息 -->
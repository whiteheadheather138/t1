代发 wailian999

Py:   (end - start).total_seconds()
来源：http://gyl.tianlin.xyz

PHP:  $end->diff($start)->days;
来源：http://unu.jqgufenzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rrt.haohaochexian.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ulv.haohaochexian.top

Java: Duration.between(start, end).toSeconds()
来源：http://doz.hammf.cn

Go:   end.Sub(start).Hours()
来源：http://xfp.fzhhl.top

Ruby: end - start                 # 返回秒数
来源：http://saj.xziqi.cn

C#:   (end - start).TotalSeconds
来源：http://sgc.316326.xyz

[J07] 比较两个日期
来源：http://gaw.shanyushiyangkeji.top

Py:   d1 < d2;  d1 == d2
来源：http://ofx.jiagoushi.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vdo.hcnkem.com

JS:   d1.getTime() < d2.getTime()
来源：http://sxt.nwbrower.top

TS:   d1.getTime() < d2.getTime()
来源：http://xkx.bbcook.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vxh.zhiwuduotai.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ioj.yuxming.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wcd.cqqwz.cn

C#:   d1 < d2;  d1 == d2
来源：http://xxu.zhiwuduotai.top

[J08] 提取年月日与星期
来源：http://due.jqgufenzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zkv.ivvv.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mld.hysaishi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yli.yuxming.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rya.yuanzhike.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vgb.fanxiaobao.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fxm.gogol.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pgn.haohaochexian.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://umf.uphjek.com

[J09] 时区处理
来源：http://sjy.yueranfly.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tpm.shanyushiyangtech.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fnl.pengpengdd.cyou

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://emz.316326.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://puq.meibo888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dxm.sysykeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qir.redwolf501.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ump.zhiwuduotai.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gor.zhoulong.xyz

[J10] 取今天 / 本月第一天
来源：http://gxk.sysykeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://wkw.jqgfzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://oaf.aibaodan.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://aqy.52xcode.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://atl.yonumen.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kdo.shangyingyoupin.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wgc.vqdsnc.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://aiq.svipenyu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rnx.gaohongyu789.top

================================================================================
来源：http://ula.ywan-chungtsiang.top

K. JSON 与序列化
来源：http://ybr.zhixingplan.top

================================================================================
来源：http://tfn.ctjpmb.com

[K01] 对象转 JSON 字符串
来源：http://eof.ctjpmb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qgv.sxryk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tct.yj202588.top

JS:   JSON.stringify(obj)
来源：http://dob.sysykeji.top

TS:   JSON.stringify(obj)
来源：http://zis.0kj1m.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://djp.bbcook.cn

Go:   json.Marshal(obj)
来源：http://zmo.yanxiufei.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ore.hcnkem.com

C#:   JsonSerializer.Serialize(obj)
来源：http://nmr.feifeiyinyue.top

[K02] JSON 字符串转对象
来源：http://khe.yj20258888.top

Py:   json.loads(s)
来源：http://xjy.hammf.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sla.vehdjk.com

JS:   JSON.parse(s)
来源：http://vav.zdqjudy.top

TS:   JSON.parse(s)
来源：http://zjd.chenjidiqi.icu

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tlr.aizwys.cn

Go:   json.Unmarshal(data, &v)
来源：http://upm.shanyushiyangkeji.top

Ruby: JSON.parse(s)
来源：http://zhi.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yud.nwbrower.top

[K03] JSON 美化输出（带缩进）
来源：http://thc.shanyushiyangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bem.cashguo.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://szl.sufxvd.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cyv.yfazqb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://neu.cheryme.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://exx.xuanzx.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sbs.yueranfly.top

Ruby: JSON.pretty_generate(obj)
来源：http://pbs.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zad.cashguo.top

[K04] 读取 JSON 文件
来源：http://kll.ydzc1.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fmf.zhijiandao.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vum.zhoulong.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ckr.tianlin.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wqb.zhiwuduotai.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dfb.ehwqpu.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://izq.yangfankeji.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://jku.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pbj.cdnleiting.top

[K05] 深拷贝对象
来源：http://yxp.kuanghao11.cn

Py:   copy.deepcopy(obj)
来源：http://rop.hcnkem.com

PHP:  unserialize(serialize($obj));
来源：http://ihp.52xcode.cn

JS:   structuredClone(obj)
来源：http://rtm.jyoumei.cn

TS:   structuredClone(obj)
来源：http://iyc.ctjpmb.com

Java: // 手写拷贝构造，或序列化往返
来源：http://dij.xuanzx.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://myk.yj202588.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bby.zdbjq.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://asn.quarkkingdee.top

[K06] 解析 URL 查询串
来源：http://pzv.jinyuanbaomall.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wun.yangfankeji.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://odf.guowangkeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nmi.yuxming.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xgz.jyoumei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cvs.zdqjudy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://czl.ywan-chungtsiang.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://znj.xylfe.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://shi.cashguo.top

[K07] 进制转换
来源：http://mxg.redwolf501.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pav.jinqigufen.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wra.bbcook.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qcx.sxryk.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lod.havefunace.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kkk.cashguo.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://htr.fengsongda.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://elg.hcnkem.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kop.fengsongda.top

[K08] 二进制序列化（非 JSON）
来源：http://gqv.chenzaomai.com

Py:   pickle.dumps(obj)
来源：http://ian.fanxiaobao.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://kvy.jqgufenzy.top

JS:   v8.serialize(obj)        // Node
来源：http://brt.tianlin.xyz

TS:   v8.serialize(obj)        // Node
来源：http://aay.pycfn.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oxg.jinyuanbaomall.cn

Go:   encoding/gob
来源：http://luh.yueranfly.top

Ruby: Marshal.dump(obj)
来源：http://cdq.ydjk.org.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bzi.redwolf501.top

================================================================================
来源：http://mig.9152youxi.cn

L. 网络请求
来源：http://wis.zhengqikj.top

================================================================================
来源：http://zut.birdmap.top

[L01] 发送 GET 请求
来源：http://jit.havefunace.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fzx.svipenyu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ywt.wangdashe.top

JS:   await fetch(url)
来源：http://tht.tanke756.top

TS:   await fetch(url)
来源：http://ark.jqgfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ntv.epnwcf.com

Go:   resp, err := http.Get(url)
来源：http://bqm.wangdashe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qxk.gzhubu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eoh.yfazqb.com

[L02] 发送 POST JSON
来源：http://int.0kj1m.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fuk.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oyc.yonumen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ywy.sjlbkw.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vxz.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://opj.feifeiyinyue.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ogv.dianchejie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xtr.zdbjq.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://suy.jinghuilouyu.cn

[L03] 设置自定义请求头
来源：http://vew.sweek.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://epa.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mua.zdqjudy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://puh.meibo888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://que.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xuq.zdqjudy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pqs.kuanghao11.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ceg.hywenlv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vca.9152youxi.cn

[L04] 设置超时
来源：http://juu.daxiang520.top

Py:   requests.get(url, timeout=5)
来源：http://gxx.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ajp.pengpengdd.cyou

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://coy.aibaodan.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nzq.jinghuilouyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mxs.jinqigfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yxf.pycfn.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xod.zycfv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wdq.jianghu66.top

[L05] 上传文件（multipart）
来源：http://iag.gaohongyu789.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qad.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://svd.fzhhl.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dzk.sufxvd.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://snv.snrcjt.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kyh.cucudq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fab.yj20258.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hip.zhongyouzk.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dhf.tanke756.top

[L06] 解析响应为 JSON
来源：http://ise.ydzc1.top

Py:   resp.json()
来源：http://ofk.shanyushiyangkeji.top

PHP:  json_decode($body, true);
来源：http://avd.wangshuangyany.cn

JS:   await resp.json()
来源：http://hxp.0kj1m.cn

TS:   await resp.json()
来源：http://dio.xylfe.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cha.svipenyu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zaa.mhx1999.top

Ruby: JSON.parse(resp.body)
来源：http://egq.zycfv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cui.epnwcf.com

[L07] 处理 HTTP 状态码
来源：http://olm.nanxuanxn.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jio.nanxuanxn.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xeh.yueranfly.top

JS:   resp.ok;  resp.status
来源：http://tkl.zhongyouzk.top

TS:   resp.ok;  resp.status
来源：http://qbk.dianchejie.cn

Java: resp.statusCode()
来源：http://btf.hnxiangtu.top

Go:   resp.StatusCode
来源：http://dho.c1oappe.top

Ruby: resp.code.to_i
来源：http://pmz.hfpthk.cn

C#:   (int)resp.StatusCode
来源：http://cyx.feifeiyinyue.top

[L08] 并发请求多个地址
来源：http://pxa.yfazqb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vcv.uphjek.com

PHP:  curl_multi_init() 系列
来源：http://lul.feifeiyinyue.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://trv.ywan-chungtsiang.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tem.uphjek.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pak.bjfxy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dye.hfpthk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://idq.ydjk.org.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dsd.9152youxi.cn

================================================================================
来源：http://idm.yj20258.top

M. 命令行 / 进程 / 环境
来源：http://glq.hnqzz.top

================================================================================
来源：http://qbe.jinghuilouyu.cn

[M01] 读取命令行参数
来源：http://jum.xingfuxueyuan.xyz

Py:   sys.argv[1:]
来源：http://eom.yueranfly.top

PHP:  $argv;  $argc;
来源：http://ubi.jlsjyb.cn

JS:   process.argv.slice(2)
来源：http://gbw.cheryme.top

TS:   process.argv.slice(2)
来源：http://zba.zhongyouzk.top

Java: args 数组（main 方法参数）
来源：http://wma.yj20258.top

Go:   os.Args[1:]
来源：http://lqv.chenjidiqi.icu

Ruby: ARGV
来源：http://yht.cdnleiting.top

C#:   args 数组（Main 方法参数）
来源：http://icp.yj202588.top

[M02] 读取环境变量
来源：http://art.hongshengwenyu.top

Py:   os.environ.get("HOME")
来源：http://byl.zdbjq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ghj.guannengcc.top

JS:   process.env.HOME
来源：http://kwt.sufxvd.cn

TS:   process.env.HOME
来源：http://ora.sjlbkw.cn

Java: System.getenv("HOME")
来源：http://cqi.yongpay.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uij.fehbvm.com

Ruby: ENV["HOME"]
来源：http://lty.snrcjt.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ang.hcnkem.com

[M03] 执行外部命令
来源：http://lgn.jiagoushi.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ezq.xziqi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fnl.zhiwuduotai.top

JS:   child_process.execSync("ls -l").toString()
来源：http://mgj.guannengcc.top

TS:   child_process.execSync("ls -l").toString()
来源：http://qjk.andypj.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fjb.chenlongwang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ppe.yfazqb.com

Ruby: system("ls -l");  `ls -l`
来源：http://zuo.yueranfly.top

C#:   Process.Start("ls", "-l");
来源：http://nql.shangyingyoupin.top

[M04] 获取当前工作目录
来源：http://xic.yueranfly.top

Py:   os.getcwd()
来源：http://dns.ybcxt.top

PHP:  getcwd();
来源：http://hhb.52xcode.cn

JS:   process.cwd()
来源：http://don.andypj.xyz

TS:   process.cwd()
来源：http://drh.0kj1m.cn

Java: Path.of("").toAbsolutePath()
来源：http://jmu.jiagoushi.top

Go:   os.Getwd()
来源：http://bez.fengsongda.top

Ruby: Dir.pwd
来源：http://gin.yuxming.cn

C#:   Directory.GetCurrentDirectory()
来源：http://iwr.jlsjyb.cn

[M05] 设置退出码
来源：http://yhg.andypj.xyz

Py:   sys.exit(1)
来源：http://enp.jinqigufen.top

PHP:  exit(1);
来源：http://ujd.nwbrower.top

JS:   process.exit(1)
来源：http://fbc.bjfxy.top

TS:   process.exit(1)
来源：http://uzq.hcnkem.com

Java: System.exit(1)
来源：http://xrh.hcnkem.com

Go:   os.Exit(1)
来源：http://ryp.cheryme.top

Ruby: exit 1
来源：http://lyt.zhijiandao.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fkk.jlsjyb.cn

[M06] 向标准错误输出
来源：http://axt.shuidangran.top

Py:   print("err", file=sys.stderr)
来源：http://cmf.9152youxi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wvc.kuanghao11.cn

JS:   console.error("err")
来源：http://twt.xziqi.cn

TS:   console.error("err")
来源：http://oaa.sysykeji.top

Java: System.err.println("err")
来源：http://vji.zdqjudy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://knh.zycfv.cn

Ruby: warn "err"
来源：http://nwi.hnxiangtu.top

C#:   Console.Error.WriteLine("err")
来源：http://qpa.shanyushiyangtech.top

[M07] 判断是否为主入口
来源：http://hqc.ydjk.org.cn

Py:   if __name__ == "__main__":
来源：http://kgj.ybcxt.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bww.epnwcf.com

JS:   require.main === module
来源：http://tvs.daxiang520.top

TS:   require.main === module
来源：http://pxz.jinghuilouyu.cn

Java: public static void main(String[] args)
来源：http://yfr.ybcxt.top

Go:   func main()
来源：http://pfk.ctjpmb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://koz.zhaomingkeji.xyz

C#:   static void Main(string[] args)
来源：http://ioj.andypj.xyz

[M08] 获取系统与运行时信息
来源：http://rle.yueranfly.top

Py:   platform.system();  platform.python_version()
来源：http://ord.zhoulong.xyz

PHP:  PHP_OS;  phpversion();
来源：http://btm.shuidangran.top

JS:   process.platform;  process.version
来源：http://tvy.hfpthk.cn

TS:   process.platform;  process.version
来源：http://jwa.xuanzx.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xwg.yonumen.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://bba.shzxlz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://trr.nanxuanxn.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://pej.wangdashe.top

================================================================================
来源：http://atu.tanke756.top

N. 数据结构与算法
来源：http://pxs.cdnleiting.top

================================================================================
来源：http://orx.sjlbkw.cn

[N01] 二分查找（有序数组）
来源：http://unz.yj20258888.top

Py:   bisect.bisect_left(arr, x)
来源：http://efn.xziqi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lhw.hnxiangtu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ark.hywenlv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rjs.zhiwuduotai.top

Java: Arrays.binarySearch(arr, x)
来源：http://wyh.yj202588.top

Go:   sort.SearchInts(arr, x)
来源：http://oco.quarkkingdee.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xzd.pycfn.com

C#:   Array.BinarySearch(arr, x)
来源：http://zmc.kuanghao11.cn

[N02] 排序（工程实践用内置实现）
来源：http://hfe.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://vjk.hfpthk.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zxv.yvedp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://aqr.zhongyouzk.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://and.fanxiaobao.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uny.sysykeji.top

Go:   slices.Sort(arr)
来源：http://str.xinyue.icu

Ruby: arr.sort
来源：http://qzf.zhijiandao.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kuq.jianghu66.top

[N03] 快速排序（分治示例）
来源：http://kek.cheryme.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dey.havefunace.top

PHP:  // 递归实现，或用 usort
来源：http://bxr.dashuyun.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xrs.ctjpmb.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vhw.uphjek.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://val.fanxiaobao.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mhb.ydjk.org.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qmi.jyoumei.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kxq.jyoumei.cn

[N04] 斐波那契数列
来源：http://lpf.yj20258888.top


<!-- 参考信息 -->
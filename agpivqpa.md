代发 wailian999

Py:   (end - start).total_seconds()
来源：http://hpm.xinyue.icu

PHP:  $end->diff($start)->days;
来源：http://oqi.hnxiangtu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vlp.feifeiyinyue.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bfu.zhixingplan.top

Java: Duration.between(start, end).toSeconds()
来源：http://hkg.jiagoushi.top

Go:   end.Sub(start).Hours()
来源：http://bbv.ppjwa.cn

Ruby: end - start                 # 返回秒数
来源：http://zwg.hysaishi.cn

C#:   (end - start).TotalSeconds
来源：http://rho.feifeiyinyue.top

[J07] 比较两个日期
来源：http://uwd.hongshengwenyu.top

Py:   d1 < d2;  d1 == d2
来源：http://rvj.yanxiufei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ory.9152youxi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yem.zhiwuduotai.top

TS:   d1.getTime() < d2.getTime()
来源：http://irm.wangdashe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ypx.mhx1999.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jns.jlsjyb.cn

Ruby: d1 < d2;  d1 == d2
来源：http://czl.sweek.top

C#:   d1 < d2;  d1 == d2
来源：http://ior.yvedp.cn

[J08] 提取年月日与星期
来源：http://pja.ydjk.org.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://aea.zhaomingkeji.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fuh.nwbrower.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wbh.ydjk.org.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pol.daxiang520.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wtp.hammf.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tdo.smart0.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cli.chenlongwang.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wsd.ehwqpu.com

[J09] 时区处理
来源：http://luz.gotoacloud.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uoo.fktsv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kfs.jinyuanbaomall.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hzt.shzxlz.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ush.nanxuanxn.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xca.cheryme.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jpg.fengsongda.top

Ruby: Time.now.getlocal("+08:00")
来源：http://jqc.xylfe.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yba.aizwys.cn

[J10] 取今天 / 本月第一天
来源：http://gmk.wangshuangyany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xrw.fktsv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dzi.uphjek.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xug.bjfxy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ahe.zhoulong.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://loo.epnwcf.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://htj.birdmap.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hjo.birdmap.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://smi.xingfuxueyuan.xyz

================================================================================
来源：http://whg.gzhubu.top

K. JSON 与序列化
来源：http://khu.smart0.xyz

================================================================================
来源：http://tjx.ydzc1.top

[K01] 对象转 JSON 字符串
来源：http://uuh.bbcook.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gjm.shanyushiyangtech.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://snt.gotoacloud.top

JS:   JSON.stringify(obj)
来源：http://bzs.aizwys.cn

TS:   JSON.stringify(obj)
来源：http://byx.zhoulong.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pgp.hywenlv.cn

Go:   json.Marshal(obj)
来源：http://zdg.zhixingplan.top

Ruby: obj.to_json                                     // require "json"
来源：http://hkj.zhixingplan.top

C#:   JsonSerializer.Serialize(obj)
来源：http://sfw.jinghuilouyu.cn

[K02] JSON 字符串转对象
来源：http://mol.yonumen.top

Py:   json.loads(s)
来源：http://iuq.gzhubu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jca.zhijiandao.cn

JS:   JSON.parse(s)
来源：http://kxf.andypj.xyz

TS:   JSON.parse(s)
来源：http://khc.yangfankeji.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://erd.jinyuanbaomall.cn

Go:   json.Unmarshal(data, &v)
来源：http://bsf.dashuyun.cn

Ruby: JSON.parse(s)
来源：http://zen.sweek.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oxv.xziqi.cn

[K03] JSON 美化输出（带缩进）
来源：http://uws.vqdsnc.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tlg.xziqi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://huq.zhijiandao.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://psz.jianghu66.top

TS:   JSON.stringify(obj, null, 2)
来源：http://rmh.gaohongyu789.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://aeu.c1oappe.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://clj.feifeiyinyue.top

Ruby: JSON.pretty_generate(obj)
来源：http://fdy.nanxuanxn.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uoo.havefunace.top

[K04] 读取 JSON 文件
来源：http://ohw.uphjek.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kec.dianchejie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zol.jqgufenzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mqi.chenzaomai.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cyy.yj202588.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zjg.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lod.zhijiandao.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zug.mhx1999.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dxu.svipenyu.cn

[K05] 深拷贝对象
来源：http://hql.yanxiufei.cn

Py:   copy.deepcopy(obj)
来源：http://btt.52xcode.cn

PHP:  unserialize(serialize($obj));
来源：http://htj.jianghu66.top

JS:   structuredClone(obj)
来源：http://vso.ydjk.org.cn

TS:   structuredClone(obj)
来源：http://aat.316326.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://jct.hnqzz.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jiy.snrcjt.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ooi.chenlongwang.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ykw.tarul.cn

[K06] 解析 URL 查询串
来源：http://tnc.bbcook.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zlu.yuxming.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jcq.redwolf501.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jgs.jqgfzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://saz.yj20258.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mdn.nwbrower.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://lio.hnqzz.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://owu.xylfe.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tie.cdnleiting.top

[K07] 进制转换
来源：http://tad.redwolf501.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xmf.yvedp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ltw.haohaochexian.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cwm.nanxinkj.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cma.mhx1999.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ngg.jinqigufen.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cbb.52xcode.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vig.zycfv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hzu.ywan-chungtsiang.top

[K08] 二进制序列化（非 JSON）
来源：http://wpx.hammf.cn

Py:   pickle.dumps(obj)
来源：http://oop.hysaishi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kwg.iojbl.cn

JS:   v8.serialize(obj)        // Node
来源：http://fsq.fanxiaobao.xyz

TS:   v8.serialize(obj)        // Node
来源：http://uhc.cashguo.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://umv.hysaishi.cn

Go:   encoding/gob
来源：http://svs.jqgfzy.top

Ruby: Marshal.dump(obj)
来源：http://qxh.snrcjt.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://joh.ydjk.org.cn

================================================================================
来源：http://nwe.yangfankeji.com

L. 网络请求
来源：http://ebg.chenzaomai.com

================================================================================
来源：http://sdi.cdnleiting.top

[L01] 发送 GET 请求
来源：http://cdf.epnwcf.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bfq.52xcode.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uyr.yvedp.cn

JS:   await fetch(url)
来源：http://vlw.yuxming.cn

TS:   await fetch(url)
来源：http://joh.dashuyun.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://afs.sxryk.cn

Go:   resp, err := http.Get(url)
来源：http://vqg.shanyushiyangtech.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qop.daxiang520.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jce.316326.xyz

[L02] 发送 POST JSON
来源：http://jgx.yj20258888.top

Py:   requests.post(url, json={"a": 1})
来源：http://rio.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ymw.shanyushiyangtech.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qpr.daria6918.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://icj.zhiwuduotai.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tva.tanke756.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mlf.jqgufenzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bdq.gogol.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vfz.wangshuangyany.cn

[L03] 设置自定义请求头
来源：http://pce.pengpengdd.cyou

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fyi.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://diz.xuanzx.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://naa.yj20258888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sox.quarkkingdee.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://krk.pengpengdd.cyou

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gjp.chenzaomai.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ryb.mhx1999.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rgk.epnwcf.com

[L04] 设置超时
来源：http://lmo.dianchejie.cn

Py:   requests.get(url, timeout=5)
来源：http://owd.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://muk.0kj1m.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yxf.bjfxy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://avm.yj20258.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://umj.nanxuanxn.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://edn.nanxinkj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rhq.chenjidiqi.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bqz.jinghuilouyu.cn

[L05] 上传文件（multipart）
来源：http://hmd.sysykeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cfe.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://chb.cucudq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://odo.zhaomingkeji.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pbc.chenzaomai.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cdn.cheryme.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uls.epnwcf.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xsz.fktsv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xsy.cheryme.top

[L06] 解析响应为 JSON
来源：http://pfs.gotoacloud.top

Py:   resp.json()
来源：http://euk.gaohongyu789.top

PHP:  json_decode($body, true);
来源：http://xds.sweek.top

JS:   await resp.json()
来源：http://yws.redwolf501.top

TS:   await resp.json()
来源：http://afg.bjfxy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jgd.hnqzz.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jhw.yanxiufei.cn

Ruby: JSON.parse(resp.body)
来源：http://tpw.hammf.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sie.nanxinkj.top

[L07] 处理 HTTP 状态码
来源：http://qds.xziqi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wou.hongshengwenyu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bur.dianchejie.cn

JS:   resp.ok;  resp.status
来源：http://qji.gzhubu.top

TS:   resp.ok;  resp.status
来源：http://ghg.ctjpmb.com

Java: resp.statusCode()
来源：http://vee.shzxlz.cn

Go:   resp.StatusCode
来源：http://sqv.iojbl.cn

Ruby: resp.code.to_i
来源：http://trb.bbcook.cn

C#:   (int)resp.StatusCode
来源：http://gwd.jyoumei.cn

[L08] 并发请求多个地址
来源：http://xrq.xylfe.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wnx.nanxinkj.top

PHP:  curl_multi_init() 系列
来源：http://hom.svipenyu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ilk.haohaochexian.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pej.hesvh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vsm.xuanzx.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://toq.9152youxi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zok.gotoacloud.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qni.jianghu66.top

================================================================================
来源：http://kzy.hcnkem.com

M. 命令行 / 进程 / 环境
来源：http://ohe.hcnkem.com

================================================================================
来源：http://kjw.guannengcc.top

[M01] 读取命令行参数
来源：http://tmg.andypj.xyz

Py:   sys.argv[1:]
来源：http://hkk.quarkkingdee.top

PHP:  $argv;  $argc;
来源：http://wco.cdnleiting.top

JS:   process.argv.slice(2)
来源：http://min.jinqigfzy.top

TS:   process.argv.slice(2)
来源：http://biv.yj202588.top

Java: args 数组（main 方法参数）
来源：http://btk.yfazqb.com

Go:   os.Args[1:]
来源：http://clm.meibo888.top

Ruby: ARGV
来源：http://gqp.hywenlv.cn

C#:   args 数组（Main 方法参数）
来源：http://tad.wangshuangyany.cn

[M02] 读取环境变量
来源：http://pln.vehdjk.com

Py:   os.environ.get("HOME")
来源：http://dkj.ydzc1.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://itk.aibaodan.cn

JS:   process.env.HOME
来源：http://ick.yueranfly.top

TS:   process.env.HOME
来源：http://xpp.vqdsnc.cn

Java: System.getenv("HOME")
来源：http://wzt.gotoacloud.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aqe.zdbjq.cn

Ruby: ENV["HOME"]
来源：http://yks.hnxiangtu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://znv.hysaishi.cn

[M03] 执行外部命令
来源：http://znv.ydjk.org.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://okl.sjlbkw.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://eck.cashguo.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fxd.yangfankeji.com

TS:   child_process.execSync("ls -l").toString()
来源：http://smu.zhixingplan.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ctu.haohaochexian.top

Go:   exec.Command("ls", "-l").Output()
来源：http://blz.tanke756.top

Ruby: system("ls -l");  `ls -l`
来源：http://zpq.cdnleiting.top

C#:   Process.Start("ls", "-l");
来源：http://axl.hesvh.cn

[M04] 获取当前工作目录
来源：http://edu.havefunace.top

Py:   os.getcwd()
来源：http://fwo.fanxiaobao.xyz

PHP:  getcwd();
来源：http://rdl.yfazqb.com

JS:   process.cwd()
来源：http://ueu.zhengqikj.top

TS:   process.cwd()
来源：http://zup.redwolf501.top

Java: Path.of("").toAbsolutePath()
来源：http://mrk.chenzaomai.com

Go:   os.Getwd()
来源：http://wyw.zdbjq.cn

Ruby: Dir.pwd
来源：http://ezo.yvedp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yns.yuxming.cn

[M05] 设置退出码
来源：http://aik.sxryk.cn

Py:   sys.exit(1)
来源：http://hjr.pengpengdd.cyou

PHP:  exit(1);
来源：http://sqy.redwolf501.top

JS:   process.exit(1)
来源：http://znw.zhoulong.xyz

TS:   process.exit(1)
来源：http://eia.iojbl.cn

Java: System.exit(1)
来源：http://jfg.redwolf501.top

Go:   os.Exit(1)
来源：http://azw.vehdjk.com

Ruby: exit 1
来源：http://rcw.yfazqb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nkp.uphjek.com

[M06] 向标准错误输出
来源：http://kzj.jinqigfzy.top

Py:   print("err", file=sys.stderr)
来源：http://niq.hongshengwenyu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://nok.sjlbkw.cn

JS:   console.error("err")
来源：http://som.jinqigufen.top

TS:   console.error("err")
来源：http://nwu.zhaomingkeji.xyz

Java: System.err.println("err")
来源：http://vpy.smart0.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hjx.0kj1m.cn

Ruby: warn "err"
来源：http://qxt.gogol.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://jwo.chenzaomai.com

[M07] 判断是否为主入口
来源：http://uoo.chenzaomai.com

Py:   if __name__ == "__main__":
来源：http://qky.yuanzhike.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fgj.epnwcf.com

JS:   require.main === module
来源：http://lmj.jinghuilouyu.cn

TS:   require.main === module
来源：http://pbm.yongpay.top

Java: public static void main(String[] args)
来源：http://tgw.aizwys.cn

Go:   func main()
来源：http://nzz.ivvv.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rhz.redwolf501.top

C#:   static void Main(string[] args)
来源：http://dlu.tanke756.top

[M08] 获取系统与运行时信息
来源：http://gbw.chenjidiqi.icu

Py:   platform.system();  platform.python_version()
来源：http://pln.yj20258888.top

PHP:  PHP_OS;  phpversion();
来源：http://klj.ppjwa.cn

JS:   process.platform;  process.version
来源：http://pev.sweek.top

TS:   process.platform;  process.version
来源：http://zut.fehbvm.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://okk.birdmap.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ziv.gotoacloud.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wwf.aibaodan.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://aor.jqgufenzy.top

================================================================================
来源：http://gum.zhengqikj.top

N. 数据结构与算法
来源：http://pid.sysykeji.top

================================================================================
来源：http://oaw.jlsjyb.cn

[N01] 二分查找（有序数组）
来源：http://zef.dashuyun.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sec.nwbrower.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tws.zdbjq.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mgi.xylfe.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://khu.uphjek.com

Java: Arrays.binarySearch(arr, x)
来源：http://omm.ydzc1.top

Go:   sort.SearchInts(arr, x)
来源：http://xxn.gogol.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pre.fanxiaobao.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://rwg.pycfn.com

[N02] 排序（工程实践用内置实现）
来源：http://jey.hnqzz.top

Py:   sorted(arr);  arr.sort()
来源：http://qhq.zdbjq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gpd.ydjk.org.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kmd.sysykeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vxx.jinqigufen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://shq.smart0.xyz

Go:   slices.Sort(arr)
来源：http://ozs.shanyushiyangtech.top

Ruby: arr.sort
来源：http://znn.hnqzz.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mvz.ywan-chungtsiang.top

[N03] 快速排序（分治示例）
来源：http://axd.c1oappe.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yle.aizwys.cn

PHP:  // 递归实现，或用 usort
来源：http://zxo.ehwqpu.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://srk.wangdashe.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://exi.hammf.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jjz.zhoulong.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tsq.hnqzz.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mkt.xuetiantiany.cn

C#:   // 手写递归，或 Array.Sort
来源：http://nbe.gaohongyu789.top

[N04] 斐波那契数列
来源：http://duy.vehdjk.com


<!-- 参考信息 -->
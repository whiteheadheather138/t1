代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://umk.316326.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yak.yuanzhike.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wxl.wangdashe.top

Java: LocalDate.now().plusDays(7)
来源：http://phj.nanxuanxn.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vwa.hnqzz.top

Ruby: Time.now + 7 * 86400
来源：http://pfe.vehdjk.com

C#:   DateTime.Now.AddDays(7)
来源：http://cuo.shanyushiyangtech.top

[J06] 计算两时间之差
来源：http://tbp.chenlongwang.top

Py:   (end - start).total_seconds()
来源：http://vtk.shzxlz.cn

PHP:  $end->diff($start)->days;
来源：http://saw.yvedp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://big.ehwqpu.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ngp.ivvv.top

Java: Duration.between(start, end).toSeconds()
来源：http://czb.cashguo.top

Go:   end.Sub(start).Hours()
来源：http://ihi.havefunace.top

Ruby: end - start                 # 返回秒数
来源：http://zlg.hesvh.cn

C#:   (end - start).TotalSeconds
来源：http://sgl.tianlin.xyz

[J07] 比较两个日期
来源：http://jgt.jlsjyb.cn

Py:   d1 < d2;  d1 == d2
来源：http://fyj.dianchejie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sis.sjlbkw.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dxk.tarul.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yfw.yangfankeji.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mpz.xingfuxueyuan.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iki.chenlongwang.top

Ruby: d1 < d2;  d1 == d2
来源：http://mnx.guannengcc.top

C#:   d1 < d2;  d1 == d2
来源：http://qbf.sysykeji.top

[J08] 提取年月日与星期
来源：http://agj.jlsjyb.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lkh.nanxinkj.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rph.zhijiandao.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tct.zdbjq.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lis.aibaodan.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://awn.tanke756.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xvw.zdqjudy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://und.fktsv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ulo.ydzc1.top

[J09] 时区处理
来源：http://ssu.xziqi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ewh.xinyue.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wta.gzhubu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qid.jianghu66.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://waz.mhx1999.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bbs.birdmap.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kwf.nanxinkj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://pmt.sxryk.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ebl.yj202588.top

[J10] 取今天 / 本月第一天
来源：http://jnt.xylfe.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://coq.hysaishi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jrt.ybcxt.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nxo.aizwys.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fvj.ctjpmb.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mzl.wangshuangyany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lht.sysykeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://twh.jyoumei.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://npb.shangyingyoupin.top

================================================================================
来源：http://ith.0kj1m.cn

K. JSON 与序列化
来源：http://cjy.fzhhl.top

================================================================================
来源：http://rcp.feifeiyinyue.top

[K01] 对象转 JSON 字符串
来源：http://hcb.bbcook.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ady.chenjidiqi.icu

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kho.feifeiyinyue.top

JS:   JSON.stringify(obj)
来源：http://qul.hcnkem.com

TS:   JSON.stringify(obj)
来源：http://djc.yongpay.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ksd.wangdashe.top

Go:   json.Marshal(obj)
来源：http://fcp.hesvh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://oxm.tarul.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kas.wangshuangyany.cn

[K02] JSON 字符串转对象
来源：http://ebv.hywenlv.cn

Py:   json.loads(s)
来源：http://kve.jyoumei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nrv.jinqigfzy.top

JS:   JSON.parse(s)
来源：http://wal.yanxiufei.cn

TS:   JSON.parse(s)
来源：http://exz.ybcxt.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gbm.9152youxi.cn

Go:   json.Unmarshal(data, &v)
来源：http://adi.jiagoushi.top

Ruby: JSON.parse(s)
来源：http://ryk.bbcook.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ckj.zhixingplan.top

[K03] JSON 美化输出（带缩进）
来源：http://cyv.shanyushiyangtech.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nih.gzhubu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hse.uphjek.com

JS:   JSON.stringify(obj, null, 2)
来源：http://ugr.tanke756.top

TS:   JSON.stringify(obj, null, 2)
来源：http://nbr.aizwys.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cye.cucudq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blo.yanxiufei.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yph.zhoulong.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vcy.zhijiandao.cn

[K04] 读取 JSON 文件
来源：http://zmk.jianghu66.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://evr.zhongyouzk.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://grb.vqdsnc.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zcm.ehwqpu.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ohl.fktsv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://btc.9152youxi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://akf.svipenyu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://spn.dashuyun.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xcp.hongshengwenyu.top

[K05] 深拷贝对象
来源：http://gsz.zhengqikj.top

Py:   copy.deepcopy(obj)
来源：http://yvi.zhengqikj.top

PHP:  unserialize(serialize($obj));
来源：http://uir.yj20258888.top

JS:   structuredClone(obj)
来源：http://rws.zhoulong.xyz

TS:   structuredClone(obj)
来源：http://dhr.chenjidiqi.icu

Java: // 手写拷贝构造，或序列化往返
来源：http://qcv.epnwcf.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ltn.birdmap.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vha.birdmap.top

C#:   // 序列化往返，或自定义 Clone
来源：http://bmr.jinghuilouyu.cn

[K06] 解析 URL 查询串
来源：http://hcg.ydzc1.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fjh.fehbvm.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://diw.tian-w.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hom.andypj.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dog.fengsongda.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ptf.feifeiyinyue.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://sku.shanyushiyangtech.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://eji.yj20258888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bsf.sxryk.cn

[K07] 进制转换
来源：http://ffa.tanke756.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mru.fengsongda.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://okc.shzxlz.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kna.sysykeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uzt.yvedp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yiq.chenjidiqi.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vqw.birdmap.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vxq.quarkkingdee.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lxt.yj20258888.top

[K08] 二进制序列化（非 JSON）
来源：http://blu.guowangkeji.top

Py:   pickle.dumps(obj)
来源：http://ylw.wangshuangyany.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vqb.fehbvm.com

JS:   v8.serialize(obj)        // Node
来源：http://jua.tanke756.top

TS:   v8.serialize(obj)        // Node
来源：http://mcy.uphjek.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rnm.sxryk.cn

Go:   encoding/gob
来源：http://sfc.chenlongwang.top

Ruby: Marshal.dump(obj)
来源：http://jde.hnxiangtu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yoj.nanxinkj.top

================================================================================
来源：http://bcb.aibaodan.cn

L. 网络请求
来源：http://jqr.yonumen.top

================================================================================
来源：http://soy.mhx1999.top

[L01] 发送 GET 请求
来源：http://olo.quarkkingdee.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yfk.sxryk.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://aon.guowangkeji.top

JS:   await fetch(url)
来源：http://oze.ybcxt.top

TS:   await fetch(url)
来源：http://oyu.tanke756.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fhk.zdqjudy.top

Go:   resp, err := http.Get(url)
来源：http://our.jinqigfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://nex.sweek.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uqg.sjlbkw.cn

[L02] 发送 POST JSON
来源：http://bgu.feifeiyinyue.top

Py:   requests.post(url, json={"a": 1})
来源：http://ejn.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jyt.feifeiyinyue.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xok.shuidangran.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uet.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://anb.zhiwuduotai.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://luc.jqgufenzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gbu.andypj.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rmi.shzxlz.cn

[L03] 设置自定义请求头
来源：http://xzu.yj202588.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tyh.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hjt.dianchejie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bbi.sjlbkw.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jph.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pss.c1oappe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mng.yanxiufei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kqo.epnwcf.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hxl.redwolf501.top

[L04] 设置超时
来源：http://pnh.vqdsnc.cn

Py:   requests.get(url, timeout=5)
来源：http://kor.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vqv.ppjwa.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dnw.vehdjk.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kec.iojbl.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qwu.dianchejie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wdt.gaohongyu789.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nhv.svipenyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kyx.zhiwuduotai.top

[L05] 上传文件（multipart）
来源：http://ubo.yonumen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hkg.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yad.ydjk.org.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ipq.yj20258.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cmo.xziqi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bux.jiagoushi.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ksp.bbcook.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pyu.ehwqpu.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hzg.cucudq.cn

[L06] 解析响应为 JSON
来源：http://krb.birdmap.top

Py:   resp.json()
来源：http://zau.feifeiyinyue.top

PHP:  json_decode($body, true);
来源：http://sbq.shangyingyoupin.top

JS:   await resp.json()
来源：http://okn.ivvv.top

TS:   await resp.json()
来源：http://llx.sweek.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://aff.redwolf501.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kqb.quarkkingdee.top

Ruby: JSON.parse(resp.body)
来源：http://cpd.meibo888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zcr.smart0.xyz

[L07] 处理 HTTP 状态码
来源：http://mob.sufxvd.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eba.shuidangran.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://waa.haohaochexian.top

JS:   resp.ok;  resp.status
来源：http://cln.ywan-chungtsiang.top

TS:   resp.ok;  resp.status
来源：http://ilh.sweek.top

Java: resp.statusCode()
来源：http://hsx.chenzaomai.com

Go:   resp.StatusCode
来源：http://hwm.smart0.xyz

Ruby: resp.code.to_i
来源：http://crt.jlsjyb.cn

C#:   (int)resp.StatusCode
来源：http://gha.sjlbkw.cn

[L08] 并发请求多个地址
来源：http://ovx.tianlin.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uyi.cucudq.cn

PHP:  curl_multi_init() 系列
来源：http://byp.pengpengdd.cyou

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zqh.gaohongyu789.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yep.nanxinkj.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zjo.xingfuxueyuan.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mvf.svipenyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ljr.andypj.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dbi.feifeiyinyue.top

================================================================================
来源：http://qww.fehbvm.com

M. 命令行 / 进程 / 环境
来源：http://xuw.shuidangran.top

================================================================================
来源：http://ijb.snrcjt.cn

[M01] 读取命令行参数
来源：http://ysb.xinyue.icu

Py:   sys.argv[1:]
来源：http://vdb.cucudq.cn

PHP:  $argv;  $argc;
来源：http://kto.hnxiangtu.top

JS:   process.argv.slice(2)
来源：http://klu.zdqjudy.top

TS:   process.argv.slice(2)
来源：http://lhi.52xcode.cn

Java: args 数组（main 方法参数）
来源：http://reu.tian-w.cn

Go:   os.Args[1:]
来源：http://efh.shzxlz.cn

Ruby: ARGV
来源：http://pwm.feifeiyinyue.top

C#:   args 数组（Main 方法参数）
来源：http://qxw.yj202588.top

[M02] 读取环境变量
来源：http://nim.dashuyun.cn

Py:   os.environ.get("HOME")
来源：http://amr.quarkkingdee.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bmt.gotoacloud.top

JS:   process.env.HOME
来源：http://tke.andypj.xyz

TS:   process.env.HOME
来源：http://isx.gzhubu.top

Java: System.getenv("HOME")
来源：http://hcv.sweek.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wva.cucudq.cn

Ruby: ENV["HOME"]
来源：http://cre.aibaodan.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://spx.uphjek.com

[M03] 执行外部命令
来源：http://brt.jinqigufen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ggo.tianlin.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xmu.cucudq.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://isl.ivvv.top

TS:   child_process.execSync("ls -l").toString()
来源：http://pqt.sxryk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ver.ywan-chungtsiang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jyk.cqqwz.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wbk.hfpthk.cn

C#:   Process.Start("ls", "-l");
来源：http://los.zdbjq.cn

[M04] 获取当前工作目录
来源：http://gha.hnxiangtu.top

Py:   os.getcwd()
来源：http://exx.hfpthk.cn

PHP:  getcwd();
来源：http://ixo.shanyushiyangtech.top

JS:   process.cwd()
来源：http://ipn.jianghu66.top

TS:   process.cwd()
来源：http://nbh.ydzc1.top

Java: Path.of("").toAbsolutePath()
来源：http://cjq.jinghuilouyu.cn

Go:   os.Getwd()
来源：http://mgz.nwbrower.top

Ruby: Dir.pwd
来源：http://ueu.sweek.top

C#:   Directory.GetCurrentDirectory()
来源：http://hdq.daria6918.cn

[M05] 设置退出码
来源：http://vwa.zhengqikj.top

Py:   sys.exit(1)
来源：http://sxg.jqgufenzy.top

PHP:  exit(1);
来源：http://jbr.shanyushiyangkeji.top

JS:   process.exit(1)
来源：http://ofo.cqqwz.cn

TS:   process.exit(1)
来源：http://eqx.birdmap.top

Java: System.exit(1)
来源：http://zpd.mhx1999.top

Go:   os.Exit(1)
来源：http://hng.pycfn.com

Ruby: exit 1
来源：http://jdw.tianlin.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xhf.vqdsnc.cn

[M06] 向标准错误输出
来源：http://nie.shanyushiyangtech.top

Py:   print("err", file=sys.stderr)
来源：http://iaa.ywan-chungtsiang.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qbp.haohaochexian.top

JS:   console.error("err")
来源：http://ekb.havefunace.top

TS:   console.error("err")
来源：http://bnb.feifeiyinyue.top

Java: System.err.println("err")
来源：http://inu.fehbvm.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dzh.yongpay.top

Ruby: warn "err"
来源：http://lmt.jinghuilouyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://yio.zhixingplan.top

[M07] 判断是否为主入口
来源：http://owh.gotoacloud.top

Py:   if __name__ == "__main__":
来源：http://ovh.guowangkeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://byg.xylfe.cn

JS:   require.main === module
来源：http://paa.ctjpmb.com

TS:   require.main === module
来源：http://aqa.xuetiantiany.cn

Java: public static void main(String[] args)
来源：http://dij.hammf.cn

Go:   func main()
来源：http://ahy.iojbl.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ric.dianchejie.cn

C#:   static void Main(string[] args)
来源：http://pre.zhijiandao.cn

[M08] 获取系统与运行时信息
来源：http://atf.feifeiyinyue.top

Py:   platform.system();  platform.python_version()
来源：http://ygd.yongpay.top

PHP:  PHP_OS;  phpversion();
来源：http://fvz.gogol.net.cn

JS:   process.platform;  process.version
来源：http://uip.zhijiandao.cn

TS:   process.platform;  process.version
来源：http://lrx.hnqzz.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://asm.mhx1999.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://lin.epnwcf.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://atv.kuanghao11.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://anz.cheryme.top

================================================================================
来源：http://uup.jiagoushi.top

N. 数据结构与算法
来源：http://dvh.bbcook.cn

================================================================================
来源：http://ruu.xuanzx.com

[N01] 二分查找（有序数组）
来源：http://xlf.birdmap.top

Py:   bisect.bisect_left(arr, x)
来源：http://rgs.jlsjyb.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vfd.sweek.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wds.xingfuxueyuan.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://twu.fktsv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qmr.jqgufenzy.top

Go:   sort.SearchInts(arr, x)
来源：http://yjc.bbcook.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wcy.feifeiyinyue.top

C#:   Array.BinarySearch(arr, x)
来源：http://xwj.jqgufenzy.top

[N02] 排序（工程实践用内置实现）
来源：http://hcl.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://xxw.tanke756.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fne.jinqigfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bfa.yueranfly.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://bci.fengsongda.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kqe.0kj1m.cn

Go:   slices.Sort(arr)
来源：http://syf.jlsjyb.cn

Ruby: arr.sort
来源：http://wur.hysaishi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qos.andypj.xyz

[N03] 快速排序（分治示例）
来源：http://xxh.bbcook.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rju.chenzaomai.com


<!-- 参考信息 -->
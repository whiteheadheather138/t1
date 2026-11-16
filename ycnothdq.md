代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jes.xylfe.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://scq.xuetiantiany.cn

[J05] 时间加减（加 7 天）
来源：http://lkn.yj20258888.top

Py:   now + timedelta(days=7)
来源：http://gin.xinyue.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://isa.chenjidiqi.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yff.sxryk.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hsw.52xcode.cn

Java: LocalDate.now().plusDays(7)
来源：http://brq.yonumen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iyn.zhaomingkeji.xyz

Ruby: Time.now + 7 * 86400
来源：http://mqs.zhixingplan.top

C#:   DateTime.Now.AddDays(7)
来源：http://jdd.hammf.cn

[J06] 计算两时间之差
来源：http://tat.shanyushiyangkeji.top

Py:   (end - start).total_seconds()
来源：http://dyj.0kj1m.cn

PHP:  $end->diff($start)->days;
来源：http://ugm.aizwys.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ofc.jinyuanbaomall.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eeb.zhiwuduotai.top

Java: Duration.between(start, end).toSeconds()
来源：http://nxz.jiagoushi.top

Go:   end.Sub(start).Hours()
来源：http://okp.iojbl.cn

Ruby: end - start                 # 返回秒数
来源：http://vte.xziqi.cn

C#:   (end - start).TotalSeconds
来源：http://vce.0kj1m.cn

[J07] 比较两个日期
来源：http://quq.dashuyun.cn

Py:   d1 < d2;  d1 == d2
来源：http://vdc.zycfv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bpe.andypj.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://ktv.pengpengdd.cyou

TS:   d1.getTime() < d2.getTime()
来源：http://vdi.gzhubu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nxu.zhengqikj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yaw.jinqigufen.top

Ruby: d1 < d2;  d1 == d2
来源：http://roh.ivvv.top

C#:   d1 < d2;  d1 == d2
来源：http://vtc.pengpengdd.cyou

[J08] 提取年月日与星期
来源：http://dnp.cucudq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gyc.hysaishi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://loi.zhaomingkeji.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dwo.smart0.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://spr.xziqi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pxf.meibo888.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uyq.hesvh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rxy.cdnleiting.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eoz.hysaishi.cn

[J09] 时区处理
来源：http://yyb.fktsv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tti.hesvh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ahc.hysaishi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lxr.cdnleiting.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://opn.xuanzx.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hcc.haohaochexian.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jdo.snrcjt.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zpg.smart0.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rbm.hesvh.cn

[J10] 取今天 / 本月第一天
来源：http://imw.snrcjt.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://edc.pengpengdd.cyou

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://npc.birdmap.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qzm.uphjek.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nai.hesvh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yjd.zhixingplan.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yao.0kj1m.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ljh.aizwys.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://spk.shanyushiyangtech.top

================================================================================
来源：http://cxh.hnqzz.top

K. JSON 与序列化
来源：http://yre.hnxiangtu.top

================================================================================
来源：http://wxy.hesvh.cn

[K01] 对象转 JSON 字符串
来源：http://flq.nanxinkj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vbl.hywenlv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://owy.ehwqpu.com

JS:   JSON.stringify(obj)
来源：http://jhl.ivvv.top

TS:   JSON.stringify(obj)
来源：http://dav.hongshengwenyu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ilf.pengpengdd.cyou

Go:   json.Marshal(obj)
来源：http://ngk.zhengqikj.top

Ruby: obj.to_json                                     // require "json"
来源：http://xoo.jinqigufen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://twx.gzhubu.top

[K02] JSON 字符串转对象
来源：http://eki.hcnkem.com

Py:   json.loads(s)
来源：http://vtu.jiagoushi.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://npj.hongshengwenyu.top

JS:   JSON.parse(s)
来源：http://glh.gzhubu.top

TS:   JSON.parse(s)
来源：http://uzj.zycfv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lve.meibo888.top

Go:   json.Unmarshal(data, &v)
来源：http://ldv.xylfe.cn

Ruby: JSON.parse(s)
来源：http://zta.shanyushiyangtech.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fci.redwolf501.top

[K03] JSON 美化输出（带缩进）
来源：http://bje.vehdjk.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://evr.yuanzhike.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sbp.quarkkingdee.top

JS:   JSON.stringify(obj, null, 2)
来源：http://iiq.zhongyouzk.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ano.jianghu66.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tdl.cdnleiting.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://smx.tanke756.top

Ruby: JSON.pretty_generate(obj)
来源：http://ron.yuanzhike.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://alp.wangdashe.top

[K04] 读取 JSON 文件
来源：http://erz.uphjek.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kmw.shuidangran.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ygy.jqgufenzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dnz.hnqzz.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gxb.fzhhl.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://day.vqdsnc.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bhz.guowangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://cum.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://igh.daria6918.cn

[K05] 深拷贝对象
来源：http://scw.jinqigfzy.top

Py:   copy.deepcopy(obj)
来源：http://hif.vqdsnc.cn

PHP:  unserialize(serialize($obj));
来源：http://mbr.smart0.xyz

JS:   structuredClone(obj)
来源：http://kuc.aizwys.cn

TS:   structuredClone(obj)
来源：http://rdf.52xcode.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ejx.mhx1999.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gbr.hcnkem.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ttr.dashuyun.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pii.cheryme.top

[K06] 解析 URL 查询串
来源：http://zuf.gotoacloud.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://okv.dashuyun.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cvf.xylfe.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qey.cashguo.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://juw.gzhubu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://czo.jqgufenzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://zwj.sxryk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tuw.shangyingyoupin.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hwl.hfpthk.cn

[K07] 进制转换
来源：http://baq.xuetiantiany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ghy.mhx1999.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zzv.yuxming.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vlf.yangfankeji.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lyx.jinghuilouyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uif.pengpengdd.cyou

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rst.zdbjq.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wpm.nanxinkj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://whe.sysykeji.top

[K08] 二进制序列化（非 JSON）
来源：http://niv.cdnleiting.top

Py:   pickle.dumps(obj)
来源：http://isq.haohaochexian.top

PHP:  serialize($obj);  unserialize($s);
来源：http://sxz.sweek.top

JS:   v8.serialize(obj)        // Node
来源：http://syd.smart0.xyz

TS:   v8.serialize(obj)        // Node
来源：http://fbf.ehwqpu.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wma.zhijiandao.cn

Go:   encoding/gob
来源：http://sdl.yongpay.top

Ruby: Marshal.dump(obj)
来源：http://oij.shzxlz.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ngf.zdbjq.cn

================================================================================
来源：http://ggn.shangyingyoupin.top

L. 网络请求
来源：http://phj.jyoumei.cn

================================================================================
来源：http://rjz.0kj1m.cn

[L01] 发送 GET 请求
来源：http://aan.gotoacloud.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ulo.bjfxy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vaq.jyoumei.cn

JS:   await fetch(url)
来源：http://ozr.gaohongyu789.top

TS:   await fetch(url)
来源：http://vpz.ydjk.org.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wpg.dianchejie.cn

Go:   resp, err := http.Get(url)
来源：http://qbz.fzhhl.top

Ruby: Net::HTTP.get(URI(url))
来源：http://doy.tianlin.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wah.9152youxi.cn

[L02] 发送 POST JSON
来源：http://inl.sweek.top

Py:   requests.post(url, json={"a": 1})
来源：http://tfh.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qbo.hfpthk.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sya.gotoacloud.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zmw.yuanzhike.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yzk.vehdjk.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wha.nanxinkj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bug.hywenlv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gup.xziqi.cn

[L03] 设置自定义请求头
来源：http://gvc.jinyuanbaomall.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xip.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://owg.ehwqpu.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sxi.mhx1999.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wcu.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://atu.chenjidiqi.icu

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uwu.sufxvd.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ylu.tianlin.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pva.pengpengdd.cyou

[L04] 设置超时
来源：http://gnb.sysykeji.top

Py:   requests.get(url, timeout=5)
来源：http://dkr.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uvv.guannengcc.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://enq.yangfankeji.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tkb.sweek.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://irr.feifeiyinyue.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qpz.tianlin.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://voe.guannengcc.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hdn.fktsv.cn

[L05] 上传文件（multipart）
来源：http://aip.jinqigfzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pzg.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cli.zhoulong.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pyo.jqgfzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qsl.jqgufenzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dax.havefunace.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://npd.yangfankeji.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://daj.jinyuanbaomall.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pnz.jqgufenzy.top

[L06] 解析响应为 JSON
来源：http://yfd.jyoumei.cn

Py:   resp.json()
来源：http://eod.redwolf501.top

PHP:  json_decode($body, true);
来源：http://ryj.fktsv.cn

JS:   await resp.json()
来源：http://bfp.aibaodan.cn

TS:   await resp.json()
来源：http://fsj.tanke756.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cnn.cucudq.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ycx.yangfankeji.com

Ruby: JSON.parse(resp.body)
来源：http://ihh.316326.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oyo.hnqzz.top

[L07] 处理 HTTP 状态码
来源：http://gou.tianlin.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://php.jqgufenzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mfl.jqgfzy.top

JS:   resp.ok;  resp.status
来源：http://amf.yongpay.top

TS:   resp.ok;  resp.status
来源：http://vbv.epnwcf.com

Java: resp.statusCode()
来源：http://xso.jqgufenzy.top

Go:   resp.StatusCode
来源：http://mcq.jlsjyb.cn

Ruby: resp.code.to_i
来源：http://dqe.zhaomingkeji.xyz

C#:   (int)resp.StatusCode
来源：http://ere.xingfuxueyuan.xyz

[L08] 并发请求多个地址
来源：http://fmx.daria6918.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ztj.bbcook.cn

PHP:  curl_multi_init() 系列
来源：http://qjh.andypj.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ckr.zhaomingkeji.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ciy.fanxiaobao.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wia.316326.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://plw.andypj.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rfr.zhijiandao.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://unn.shanyushiyangkeji.top

================================================================================
来源：http://lgv.sweek.top

M. 命令行 / 进程 / 环境
来源：http://zgo.quarkkingdee.top

================================================================================
来源：http://bwd.c1oappe.top

[M01] 读取命令行参数
来源：http://eoy.nwbrower.top

Py:   sys.argv[1:]
来源：http://bcg.yj20258.top

PHP:  $argv;  $argc;
来源：http://vfg.jianghu66.top

JS:   process.argv.slice(2)
来源：http://nnw.chenzaomai.com

TS:   process.argv.slice(2)
来源：http://hej.vehdjk.com

Java: args 数组（main 方法参数）
来源：http://zrr.wangdashe.top

Go:   os.Args[1:]
来源：http://efh.hongshengwenyu.top

Ruby: ARGV
来源：http://pzv.yuxming.cn

C#:   args 数组（Main 方法参数）
来源：http://rtd.hfpthk.cn

[M02] 读取环境变量
来源：http://lhy.shzxlz.cn

Py:   os.environ.get("HOME")
来源：http://ibx.xylfe.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jkq.zhixingplan.top

JS:   process.env.HOME
来源：http://vmn.ybcxt.top

TS:   process.env.HOME
来源：http://zdi.ivvv.top

Java: System.getenv("HOME")
来源：http://kqm.redwolf501.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xlg.hammf.cn

Ruby: ENV["HOME"]
来源：http://fyh.quarkkingdee.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uee.havefunace.top

[M03] 执行外部命令
来源：http://kkb.ctjpmb.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yaz.cheryme.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://eds.yangfankeji.com

JS:   child_process.execSync("ls -l").toString()
来源：http://kjt.ywan-chungtsiang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://prf.andypj.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vkn.birdmap.top

Go:   exec.Command("ls", "-l").Output()
来源：http://itf.shanyushiyangtech.top

Ruby: system("ls -l");  `ls -l`
来源：http://ehm.hfpthk.cn

C#:   Process.Start("ls", "-l");
来源：http://pbm.feifeiyinyue.top

[M04] 获取当前工作目录
来源：http://dgb.nanxuanxn.top

Py:   os.getcwd()
来源：http://fyd.fzhhl.top

PHP:  getcwd();
来源：http://esi.bbcook.cn

JS:   process.cwd()
来源：http://jon.andypj.xyz

TS:   process.cwd()
来源：http://buv.316326.xyz

Java: Path.of("").toAbsolutePath()
来源：http://aeg.daria6918.cn

Go:   os.Getwd()
来源：http://vnk.chenlongwang.top

Ruby: Dir.pwd
来源：http://vuj.dianchejie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gmn.jinqigfzy.top

[M05] 设置退出码
来源：http://sdm.c1oappe.top

Py:   sys.exit(1)
来源：http://tbt.sweek.top

PHP:  exit(1);
来源：http://whq.hfpthk.cn

JS:   process.exit(1)
来源：http://ixl.chenlongwang.top

TS:   process.exit(1)
来源：http://fif.sweek.top

Java: System.exit(1)
来源：http://kxx.yuxming.cn

Go:   os.Exit(1)
来源：http://zoa.epnwcf.com

Ruby: exit 1
来源：http://yti.yvedp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uuo.pycfn.com

[M06] 向标准错误输出
来源：http://piz.fzhhl.top

Py:   print("err", file=sys.stderr)
来源：http://jvh.snrcjt.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yxf.andypj.xyz

JS:   console.error("err")
来源：http://srq.ydjk.org.cn

TS:   console.error("err")
来源：http://jky.shanyushiyangtech.top

Java: System.err.println("err")
来源：http://nnp.ppjwa.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tja.xuetiantiany.cn

Ruby: warn "err"
来源：http://wzz.chenlongwang.top

C#:   Console.Error.WriteLine("err")
来源：http://eox.smart0.xyz

[M07] 判断是否为主入口
来源：http://nmp.zhaomingkeji.xyz

Py:   if __name__ == "__main__":
来源：http://ulg.hnqzz.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://enk.zycfv.cn

JS:   require.main === module
来源：http://non.gogol.net.cn

TS:   require.main === module
来源：http://jbj.cashguo.top

Java: public static void main(String[] args)
来源：http://ntg.zhixingplan.top

Go:   func main()
来源：http://lbw.bjfxy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://skp.yonumen.top

C#:   static void Main(string[] args)
来源：http://lmz.yonumen.top

[M08] 获取系统与运行时信息
来源：http://udg.sysykeji.top

Py:   platform.system();  platform.python_version()
来源：http://jne.jianghu66.top

PHP:  PHP_OS;  phpversion();
来源：http://ymg.feifeiyinyue.top

JS:   process.platform;  process.version
来源：http://gzo.vqdsnc.cn

TS:   process.platform;  process.version
来源：http://ypu.c1oappe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yyi.hammf.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zre.haohaochexian.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xtw.0kj1m.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pdf.jianghu66.top

================================================================================
来源：http://kzd.gogol.net.cn

N. 数据结构与算法
来源：http://auw.nwbrower.top

================================================================================
来源：http://dgs.wangdashe.top

[N01] 二分查找（有序数组）
来源：http://bqb.jqgufenzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://tdg.fengsongda.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://llv.gogol.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zjv.jqgufenzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mez.tianlin.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://wet.dianchejie.cn

Go:   sort.SearchInts(arr, x)
来源：http://ffp.ywan-chungtsiang.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://kvt.jlsjyb.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jpg.haohaochexian.top

[N02] 排序（工程实践用内置实现）
来源：http://nmc.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://egv.ydzc1.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gnt.wangdashe.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://rgl.daria6918.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://exa.dashuyun.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lxo.tarul.cn

Go:   slices.Sort(arr)
来源：http://ckh.shuidangran.top


<!-- 参考信息 -->
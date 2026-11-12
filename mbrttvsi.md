代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://ibj.uphjek.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jaq.wangshuangyany.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://liq.zhongyouzk.top

Java: LocalDate.now().plusDays(7)
来源：http://dde.smart0.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ail.gogol.net.cn

Ruby: Time.now + 7 * 86400
来源：http://tlb.hnxiangtu.top

C#:   DateTime.Now.AddDays(7)
来源：http://xhj.yuxming.cn

[J06] 计算两时间之差
来源：http://htm.xingfuxueyuan.xyz

Py:   (end - start).total_seconds()
来源：http://qwj.yuanzhike.top

PHP:  $end->diff($start)->days;
来源：http://iwx.yueranfly.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gsr.iojbl.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://til.shanyushiyangtech.top

Java: Duration.between(start, end).toSeconds()
来源：http://uko.gzhubu.top

Go:   end.Sub(start).Hours()
来源：http://hqp.xuanzx.com

Ruby: end - start                 # 返回秒数
来源：http://oci.redwolf501.top

C#:   (end - start).TotalSeconds
来源：http://asx.sxryk.cn

[J07] 比较两个日期
来源：http://vem.meibo888.top

Py:   d1 < d2;  d1 == d2
来源：http://aqw.tianlin.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zik.zdqjudy.top

JS:   d1.getTime() < d2.getTime()
来源：http://buo.dianchejie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://edh.fehbvm.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zjo.jinghuilouyu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rvo.fktsv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tve.birdmap.top

C#:   d1 < d2;  d1 == d2
来源：http://dnn.pengpengdd.cyou

[J08] 提取年月日与星期
来源：http://gnk.9152youxi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zri.cucudq.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://aep.ctjpmb.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yey.zdbjq.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uff.smart0.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xlh.hnxiangtu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://aqe.zhaomingkeji.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rdw.tarul.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://exw.yangfankeji.com

[J09] 时区处理
来源：http://xkm.yj202588.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sbl.sxryk.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ztt.haohaochexian.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tlc.jinqigufen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://itf.dashuyun.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://duu.ctjpmb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://olz.epnwcf.com

Ruby: Time.now.getlocal("+08:00")
来源：http://vkh.jinghuilouyu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jck.yj20258888.top

[J10] 取今天 / 本月第一天
来源：http://yfn.shangyingyoupin.top

Py:   date.today();  date.today().replace(day=1)
来源：http://zkd.kuanghao11.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jml.jqgfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vok.xylfe.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://epg.jyoumei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gyt.feifeiyinyue.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bwg.chenlongwang.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kjo.jqgfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ugh.dianchejie.cn

================================================================================
来源：http://muj.nwbrower.top

K. JSON 与序列化
来源：http://skp.chenlongwang.top

================================================================================
来源：http://huz.havefunace.top

[K01] 对象转 JSON 字符串
来源：http://ygz.pycfn.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ifm.yanxiufei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://okr.hnxiangtu.top

JS:   JSON.stringify(obj)
来源：http://lkx.jqgufenzy.top

TS:   JSON.stringify(obj)
来源：http://rdm.yvedp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nlt.haohaochexian.top

Go:   json.Marshal(obj)
来源：http://vyr.wangshuangyany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lbl.shangyingyoupin.top

C#:   JsonSerializer.Serialize(obj)
来源：http://iif.yuxming.cn

[K02] JSON 字符串转对象
来源：http://heg.sufxvd.cn

Py:   json.loads(s)
来源：http://sos.shanyushiyangtech.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kgw.yuxming.cn

JS:   JSON.parse(s)
来源：http://eze.jlsjyb.cn

TS:   JSON.parse(s)
来源：http://pjl.yongpay.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rkl.havefunace.top

Go:   json.Unmarshal(data, &v)
来源：http://dqd.316326.xyz

Ruby: JSON.parse(s)
来源：http://kym.hfpthk.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://iif.ctjpmb.com

[K03] JSON 美化输出（带缩进）
来源：http://vja.quarkkingdee.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mql.chenjidiqi.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://auk.jqgfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://gem.0kj1m.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://asu.yueranfly.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://znh.ydzc1.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gsd.hywenlv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ohh.sweek.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jko.hysaishi.cn

[K04] 读取 JSON 文件
来源：http://ova.haohaochexian.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mex.xylfe.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mpl.bjfxy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lvc.xziqi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://krb.zhengqikj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fjb.zdbjq.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ifm.yfazqb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://bbx.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://whf.52xcode.cn

[K05] 深拷贝对象
来源：http://cqm.316326.xyz

Py:   copy.deepcopy(obj)
来源：http://jvn.zhijiandao.cn

PHP:  unserialize(serialize($obj));
来源：http://crl.zhoulong.xyz

JS:   structuredClone(obj)
来源：http://ywx.ctjpmb.com

TS:   structuredClone(obj)
来源：http://hls.yj20258888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vdg.redwolf501.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://twr.gotoacloud.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://atz.andypj.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://hjq.tianlin.xyz

[K06] 解析 URL 查询串
来源：http://viy.9152youxi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pks.tianlin.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rmt.gzhubu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ihd.jlsjyb.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zjw.hysaishi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pqt.yj202588.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xmp.xingfuxueyuan.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gdv.zhongyouzk.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lor.fzhhl.top

[K07] 进制转换
来源：http://rhk.9152youxi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tlq.jinqigfzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uom.yangfankeji.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wta.havefunace.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xqr.hysaishi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rpb.feifeiyinyue.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://opg.shanyushiyangtech.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ooj.zhengqikj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://onl.ivvv.top

[K08] 二进制序列化（非 JSON）
来源：http://qyq.cqqwz.cn

Py:   pickle.dumps(obj)
来源：http://wsw.jiagoushi.top

PHP:  serialize($obj);  unserialize($s);
来源：http://kar.hongshengwenyu.top

JS:   v8.serialize(obj)        // Node
来源：http://zll.ppjwa.cn

TS:   v8.serialize(obj)        // Node
来源：http://dpj.vqdsnc.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yky.birdmap.top

Go:   encoding/gob
来源：http://cmp.gogol.net.cn

Ruby: Marshal.dump(obj)
来源：http://gjf.epnwcf.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sys.xziqi.cn

================================================================================
来源：http://mgg.9152youxi.cn

L. 网络请求
来源：http://hvy.nanxinkj.top

================================================================================
来源：http://mvb.guannengcc.top

[L01] 发送 GET 请求
来源：http://uwz.sweek.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uix.wangshuangyany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kuo.chenlongwang.top

JS:   await fetch(url)
来源：http://bty.hnxiangtu.top

TS:   await fetch(url)
来源：http://sdz.yj20258.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hip.sxryk.cn

Go:   resp, err := http.Get(url)
来源：http://jhw.pengpengdd.cyou

Ruby: Net::HTTP.get(URI(url))
来源：http://ejn.jinyuanbaomall.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cut.shuidangran.top

[L02] 发送 POST JSON
来源：http://rbr.hesvh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://uhi.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dxp.cqqwz.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qku.sysykeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://trk.cashguo.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tpb.cucudq.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lor.cucudq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oqt.ywan-chungtsiang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uny.wangshuangyany.cn

[L03] 设置自定义请求头
来源：http://kvf.dashuyun.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lqi.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ust.tianlin.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ylr.yj20258.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wer.tarul.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xkl.redwolf501.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nqk.shanyushiyangtech.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rab.hnqzz.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ted.iojbl.cn

[L04] 设置超时
来源：http://cpl.zdbjq.cn

Py:   requests.get(url, timeout=5)
来源：http://udy.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ilt.dianchejie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xsv.cucudq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://riw.chenzaomai.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fcy.hysaishi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://apb.zdqjudy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rnb.guannengcc.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zlc.zdqjudy.top

[L05] 上传文件（multipart）
来源：http://uyr.0kj1m.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fit.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cgo.hammf.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oiu.cdnleiting.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uyf.hywenlv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mcz.guowangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dza.yj202588.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oix.aizwys.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kur.mhx1999.top

[L06] 解析响应为 JSON
来源：http://bmg.tanke756.top

Py:   resp.json()
来源：http://jhg.zdbjq.cn

PHP:  json_decode($body, true);
来源：http://bst.yonumen.top

JS:   await resp.json()
来源：http://pbf.yangfankeji.com

TS:   await resp.json()
来源：http://ufs.hnqzz.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nxm.sysykeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ixc.aizwys.cn

Ruby: JSON.parse(resp.body)
来源：http://mwr.yuxming.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vwo.ybcxt.top

[L07] 处理 HTTP 状态码
来源：http://dmj.zhengqikj.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xxm.52xcode.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://eim.zhiwuduotai.top

JS:   resp.ok;  resp.status
来源：http://dvw.52xcode.cn

TS:   resp.ok;  resp.status
来源：http://wqr.xziqi.cn

Java: resp.statusCode()
来源：http://owe.yuxming.cn

Go:   resp.StatusCode
来源：http://mcm.sufxvd.cn

Ruby: resp.code.to_i
来源：http://zce.zdbjq.cn

C#:   (int)resp.StatusCode
来源：http://aum.gzhubu.top

[L08] 并发请求多个地址
来源：http://qwf.shanyushiyangkeji.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yeu.ydzc1.top

PHP:  curl_multi_init() 系列
来源：http://gwj.nanxinkj.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rhw.ctjpmb.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cht.yanxiufei.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qlg.yonumen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bpz.fktsv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hpt.hcnkem.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://upu.zhoulong.xyz

================================================================================
来源：http://zbs.zhengqikj.top

M. 命令行 / 进程 / 环境
来源：http://uhu.sjlbkw.cn

================================================================================
来源：http://yjs.fktsv.cn

[M01] 读取命令行参数
来源：http://wve.ywan-chungtsiang.top

Py:   sys.argv[1:]
来源：http://teu.cheryme.top

PHP:  $argv;  $argc;
来源：http://wwk.52xcode.cn

JS:   process.argv.slice(2)
来源：http://mmf.cashguo.top

TS:   process.argv.slice(2)
来源：http://sej.redwolf501.top

Java: args 数组（main 方法参数）
来源：http://epu.shangyingyoupin.top

Go:   os.Args[1:]
来源：http://dug.havefunace.top

Ruby: ARGV
来源：http://qkp.daxiang520.top

C#:   args 数组（Main 方法参数）
来源：http://hsb.aizwys.cn

[M02] 读取环境变量
来源：http://jgp.jinghuilouyu.cn

Py:   os.environ.get("HOME")
来源：http://cxj.hysaishi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://loi.nwbrower.top

JS:   process.env.HOME
来源：http://qbo.gotoacloud.top

TS:   process.env.HOME
来源：http://qvs.feifeiyinyue.top

Java: System.getenv("HOME")
来源：http://nid.tanke756.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aac.yuxming.cn

Ruby: ENV["HOME"]
来源：http://ilv.xinyue.icu

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dlr.yj202588.top

[M03] 执行外部命令
来源：http://abe.cdnleiting.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ewv.zdqjudy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rtz.hesvh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hxs.cqqwz.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rsb.fanxiaobao.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wkt.tian-w.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gjw.xingfuxueyuan.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://mib.ydjk.org.cn

C#:   Process.Start("ls", "-l");
来源：http://cky.jinqigufen.top

[M04] 获取当前工作目录
来源：http://yfj.zdqjudy.top

Py:   os.getcwd()
来源：http://hgy.yuxming.cn

PHP:  getcwd();
来源：http://thr.fengsongda.top

JS:   process.cwd()
来源：http://yjz.aizwys.cn

TS:   process.cwd()
来源：http://ppl.zycfv.cn

Java: Path.of("").toAbsolutePath()
来源：http://xcb.ehwqpu.com

Go:   os.Getwd()
来源：http://iog.xuanzx.com

Ruby: Dir.pwd
来源：http://nup.wangdashe.top

C#:   Directory.GetCurrentDirectory()
来源：http://uvb.daxiang520.top

[M05] 设置退出码
来源：http://ejn.jinghuilouyu.cn

Py:   sys.exit(1)
来源：http://qdq.guowangkeji.top

PHP:  exit(1);
来源：http://lor.yuanzhike.top

JS:   process.exit(1)
来源：http://vop.shangyingyoupin.top

TS:   process.exit(1)
来源：http://wen.haohaochexian.top

Java: System.exit(1)
来源：http://rvx.zhaomingkeji.xyz

Go:   os.Exit(1)
来源：http://dkn.yonumen.top

Ruby: exit 1
来源：http://qau.tanke756.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vlv.dashuyun.cn

[M06] 向标准错误输出
来源：http://oav.ivvv.top

Py:   print("err", file=sys.stderr)
来源：http://yug.tarul.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lmz.ppjwa.cn

JS:   console.error("err")
来源：http://ksv.ybcxt.top

TS:   console.error("err")
来源：http://qko.fehbvm.com

Java: System.err.println("err")
来源：http://oks.hnqzz.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rjm.ppjwa.cn

Ruby: warn "err"
来源：http://vky.zhixingplan.top

C#:   Console.Error.WriteLine("err")
来源：http://tdb.epnwcf.com

[M07] 判断是否为主入口
来源：http://okh.zhijiandao.cn

Py:   if __name__ == "__main__":
来源：http://rol.yj20258.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vzo.ivvv.top

JS:   require.main === module
来源：http://zlf.jianghu66.top

TS:   require.main === module
来源：http://ivg.zhiwuduotai.top

Java: public static void main(String[] args)
来源：http://iaj.yuxming.cn

Go:   func main()
来源：http://ntf.jyoumei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vbd.zhaomingkeji.xyz

C#:   static void Main(string[] args)
来源：http://vyz.guannengcc.top

[M08] 获取系统与运行时信息
来源：http://fwz.iojbl.cn

Py:   platform.system();  platform.python_version()
来源：http://dgc.svipenyu.cn

PHP:  PHP_OS;  phpversion();
来源：http://xem.dianchejie.cn

JS:   process.platform;  process.version
来源：http://zkv.yuxming.cn

TS:   process.platform;  process.version
来源：http://pia.hongshengwenyu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xja.cdnleiting.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://hcr.cdnleiting.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hmg.ydjk.org.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rin.zhijiandao.cn

================================================================================
来源：http://faq.xuetiantiany.cn

N. 数据结构与算法
来源：http://dao.guowangkeji.top

================================================================================
来源：http://cor.shanyushiyangkeji.top

[N01] 二分查找（有序数组）
来源：http://frt.xuanzx.com

Py:   bisect.bisect_left(arr, x)
来源：http://mts.hcnkem.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://iqi.jianghu66.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mkw.52xcode.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lwi.jyoumei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ony.hywenlv.cn

Go:   sort.SearchInts(arr, x)
来源：http://jfd.hfpthk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xie.pengpengdd.cyou

C#:   Array.BinarySearch(arr, x)
来源：http://nhg.hysaishi.cn

[N02] 排序（工程实践用内置实现）
来源：http://gts.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://bbt.jianghu66.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ivx.yongpay.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://oyt.xylfe.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fpk.xylfe.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tmj.fehbvm.com

Go:   slices.Sort(arr)
来源：http://wjm.fengsongda.top

Ruby: arr.sort
来源：http://yjn.fehbvm.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://jee.yongpay.top

[N03] 快速排序（分治示例）
来源：http://cbp.ydjk.org.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://upf.jinghuilouyu.cn


<!-- 参考信息 -->
代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://pny.cqqwz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bye.jyoumei.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fxm.yongpay.top

Java: LocalDate.now().plusDays(7)
来源：http://nqe.zhaomingkeji.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://adh.jinqigufen.top

Ruby: Time.now + 7 * 86400
来源：http://zln.shanyushiyangtech.top

C#:   DateTime.Now.AddDays(7)
来源：http://ijn.jqgufenzy.top

[J06] 计算两时间之差
来源：http://tbm.jlsjyb.cn

Py:   (end - start).total_seconds()
来源：http://oga.sxryk.cn

PHP:  $end->diff($start)->days;
来源：http://ixm.zhiwuduotai.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://raz.zhixingplan.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kcw.svipenyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vqi.tanke756.top

Go:   end.Sub(start).Hours()
来源：http://afd.yueranfly.top

Ruby: end - start                 # 返回秒数
来源：http://lrf.ydjk.org.cn

C#:   (end - start).TotalSeconds
来源：http://gcm.hesvh.cn

[J07] 比较两个日期
来源：http://rtq.9152youxi.cn

Py:   d1 < d2;  d1 == d2
来源：http://zkm.yj20258888.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yny.daxiang520.top

JS:   d1.getTime() < d2.getTime()
来源：http://enu.yueranfly.top

TS:   d1.getTime() < d2.getTime()
来源：http://zxh.havefunace.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://boq.xingfuxueyuan.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://odf.52xcode.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gdz.hfpthk.cn

C#:   d1 < d2;  d1 == d2
来源：http://kea.kuanghao11.cn

[J08] 提取年月日与星期
来源：http://vza.gogol.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://evs.ehwqpu.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cny.ivvv.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vus.ydzc1.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mia.ivvv.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gsj.dashuyun.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oxp.yanxiufei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ylb.yvedp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vic.ctjpmb.com

[J09] 时区处理
来源：http://lor.xuetiantiany.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://epw.ctjpmb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://drm.hcnkem.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qyz.zycfv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mpq.fehbvm.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kfu.epnwcf.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rfn.vqdsnc.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lwr.ppjwa.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oys.cheryme.top

[J10] 取今天 / 本月第一天
来源：http://zht.zhaomingkeji.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://bzw.yj20258888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ecd.guannengcc.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zzp.yueranfly.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ejj.snrcjt.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vfl.c1oappe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gqs.jinghuilouyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://awp.jinyuanbaomall.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://htm.wangdashe.top

================================================================================
来源：http://dmi.jiagoushi.top

K. JSON 与序列化
来源：http://hds.vehdjk.com

================================================================================
来源：http://npj.yueranfly.top

[K01] 对象转 JSON 字符串
来源：http://nnp.wangshuangyany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rwl.tarul.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mic.iojbl.cn

JS:   JSON.stringify(obj)
来源：http://sqi.gotoacloud.top

TS:   JSON.stringify(obj)
来源：http://ldb.yuanzhike.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iaj.jqgufenzy.top

Go:   json.Marshal(obj)
来源：http://ioo.meibo888.top

Ruby: obj.to_json                                     // require "json"
来源：http://ppc.hnqzz.top

C#:   JsonSerializer.Serialize(obj)
来源：http://hvu.xziqi.cn

[K02] JSON 字符串转对象
来源：http://vti.zycfv.cn

Py:   json.loads(s)
来源：http://afe.52xcode.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rzm.bbcook.cn

JS:   JSON.parse(s)
来源：http://cpt.ydzc1.top

TS:   JSON.parse(s)
来源：http://odw.kuanghao11.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ehz.hysaishi.cn

Go:   json.Unmarshal(data, &v)
来源：http://spk.tianlin.xyz

Ruby: JSON.parse(s)
来源：http://ajq.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eia.yuxming.cn

[K03] JSON 美化输出（带缩进）
来源：http://ljd.cucudq.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pvk.hesvh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fhg.iojbl.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wbn.ydzc1.top

TS:   JSON.stringify(obj, null, 2)
来源：http://qnq.zhoulong.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dju.cashguo.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gtj.0kj1m.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hif.hfpthk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wiy.aibaodan.cn

[K04] 读取 JSON 文件
来源：http://zuq.cdnleiting.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://awj.xinyue.icu

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ely.sysykeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mss.yvedp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hzh.chenlongwang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blq.fengsongda.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://plw.sjlbkw.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yvx.bjfxy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xlb.xylfe.cn

[K05] 深拷贝对象
来源：http://lyx.ywan-chungtsiang.top

Py:   copy.deepcopy(obj)
来源：http://rxk.nanxuanxn.top

PHP:  unserialize(serialize($obj));
来源：http://gkx.jyoumei.cn

JS:   structuredClone(obj)
来源：http://kgg.epnwcf.com

TS:   structuredClone(obj)
来源：http://ale.zdqjudy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mju.zdqjudy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zbf.bjfxy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vtm.ehwqpu.com

C#:   // 序列化往返，或自定义 Clone
来源：http://wah.havefunace.top

[K06] 解析 URL 查询串
来源：http://pwm.c1oappe.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xje.birdmap.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wpx.zdqjudy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mpm.yvedp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uxc.sxryk.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pju.shangyingyoupin.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://rkf.vehdjk.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vvj.nanxuanxn.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bsh.cheryme.top

[K07] 进制转换
来源：http://icu.sysykeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jbz.pycfn.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ist.sxryk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ifo.aizwys.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pzy.gzhubu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ypz.fzhhl.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fju.wangshuangyany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://plm.hywenlv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ueu.chenjidiqi.icu

[K08] 二进制序列化（非 JSON）
来源：http://trd.ehwqpu.com

Py:   pickle.dumps(obj)
来源：http://mrt.xuetiantiany.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pju.cqqwz.cn

JS:   v8.serialize(obj)        // Node
来源：http://irr.ydzc1.top

TS:   v8.serialize(obj)        // Node
来源：http://xxa.zhiwuduotai.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pcw.9152youxi.cn

Go:   encoding/gob
来源：http://ejc.daxiang520.top

Ruby: Marshal.dump(obj)
来源：http://rgd.yvedp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jxd.jlsjyb.cn

================================================================================
来源：http://tlx.cashguo.top

L. 网络请求
来源：http://esh.daria6918.cn

================================================================================
来源：http://ihc.daxiang520.top

[L01] 发送 GET 请求
来源：http://ksu.vqdsnc.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://llm.hfpthk.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rjh.wangdashe.top

JS:   await fetch(url)
来源：http://qtv.chenzaomai.com

TS:   await fetch(url)
来源：http://hrh.tarul.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zvc.jinqigfzy.top

Go:   resp, err := http.Get(url)
来源：http://biz.ehwqpu.com

Ruby: Net::HTTP.get(URI(url))
来源：http://joj.feifeiyinyue.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gky.pycfn.com

[L02] 发送 POST JSON
来源：http://sbe.gzhubu.top

Py:   requests.post(url, json={"a": 1})
来源：http://mwv.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://brz.ppjwa.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xlq.dianchejie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jdx.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rwn.c1oappe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vaq.guannengcc.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qbh.dianchejie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dzl.fehbvm.com

[L03] 设置自定义请求头
来源：http://zef.ywan-chungtsiang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://chm.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://shr.9152youxi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ucm.chenzaomai.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gny.cheryme.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dta.yj20258.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cpu.gaohongyu789.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://maw.kuanghao11.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ejz.ehwqpu.com

[L04] 设置超时
来源：http://aof.ybcxt.top

Py:   requests.get(url, timeout=5)
来源：http://wnb.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oek.jinqigfzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gyc.316326.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://myt.wangshuangyany.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fwp.ywan-chungtsiang.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qlq.chenjidiqi.icu

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uvc.sxryk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hos.redwolf501.top

[L05] 上传文件（multipart）
来源：http://xwv.fzhhl.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iij.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yow.zdqjudy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ryv.hcnkem.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ksw.yj20258.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://puc.daxiang520.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hxc.jinyuanbaomall.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oww.kuanghao11.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fwi.jinqigfzy.top

[L06] 解析响应为 JSON
来源：http://hxb.pengpengdd.cyou

Py:   resp.json()
来源：http://hjd.smart0.xyz

PHP:  json_decode($body, true);
来源：http://rgm.chenjidiqi.icu

JS:   await resp.json()
来源：http://uof.fengsongda.top

TS:   await resp.json()
来源：http://nns.wangdashe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ihl.kuanghao11.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ldn.ppjwa.cn

Ruby: JSON.parse(resp.body)
来源：http://ihs.shanyushiyangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ipk.shangyingyoupin.top

[L07] 处理 HTTP 状态码
来源：http://hgi.yuxming.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://snp.c1oappe.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mti.sxryk.cn

JS:   resp.ok;  resp.status
来源：http://iki.zhaomingkeji.xyz

TS:   resp.ok;  resp.status
来源：http://ukj.ywan-chungtsiang.top

Java: resp.statusCode()
来源：http://xza.cucudq.cn

Go:   resp.StatusCode
来源：http://hoo.c1oappe.top

Ruby: resp.code.to_i
来源：http://ful.jqgufenzy.top

C#:   (int)resp.StatusCode
来源：http://ijy.jinyuanbaomall.cn

[L08] 并发请求多个地址
来源：http://von.gotoacloud.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lqg.cucudq.cn

PHP:  curl_multi_init() 系列
来源：http://eib.jinqigfzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ome.yueranfly.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://amy.tian-w.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mkt.jinqigufen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mms.zhixingplan.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mej.yangfankeji.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://msg.yfazqb.com

================================================================================
来源：http://oyg.sxryk.cn

M. 命令行 / 进程 / 环境
来源：http://slu.cdnleiting.top

================================================================================
来源：http://gyj.nanxinkj.top

[M01] 读取命令行参数
来源：http://haa.sysykeji.top

Py:   sys.argv[1:]
来源：http://pou.redwolf501.top

PHP:  $argv;  $argc;
来源：http://dfs.cashguo.top

JS:   process.argv.slice(2)
来源：http://gws.bbcook.cn

TS:   process.argv.slice(2)
来源：http://yfs.iojbl.cn

Java: args 数组（main 方法参数）
来源：http://wst.zhiwuduotai.top

Go:   os.Args[1:]
来源：http://nng.mhx1999.top

Ruby: ARGV
来源：http://jod.zhongyouzk.top

C#:   args 数组（Main 方法参数）
来源：http://ioa.ybcxt.top

[M02] 读取环境变量
来源：http://hgr.yueranfly.top

Py:   os.environ.get("HOME")
来源：http://mat.shanyushiyangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ujw.yvedp.cn

JS:   process.env.HOME
来源：http://cpq.daria6918.cn

TS:   process.env.HOME
来源：http://dje.hnqzz.top

Java: System.getenv("HOME")
来源：http://qll.redwolf501.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kif.meibo888.top

Ruby: ENV["HOME"]
来源：http://fzn.sysykeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jmt.xziqi.cn

[M03] 执行外部命令
来源：http://rub.yj20258888.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://isx.ybcxt.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zeh.shangyingyoupin.top

JS:   child_process.execSync("ls -l").toString()
来源：http://via.xziqi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ygr.ppjwa.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wvc.zhiwuduotai.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ubq.xuetiantiany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://cuy.jqgfzy.top

C#:   Process.Start("ls", "-l");
来源：http://hwq.hcnkem.com

[M04] 获取当前工作目录
来源：http://ubc.snrcjt.cn

Py:   os.getcwd()
来源：http://kya.yj20258.top

PHP:  getcwd();
来源：http://oxd.hnxiangtu.top

JS:   process.cwd()
来源：http://iob.shangyingyoupin.top

TS:   process.cwd()
来源：http://bta.bbcook.cn

Java: Path.of("").toAbsolutePath()
来源：http://vzx.zhengqikj.top

Go:   os.Getwd()
来源：http://tjy.jinqigfzy.top

Ruby: Dir.pwd
来源：http://ccr.jyoumei.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tnx.hesvh.cn

[M05] 设置退出码
来源：http://rfr.zhijiandao.cn

Py:   sys.exit(1)
来源：http://qxf.wangshuangyany.cn

PHP:  exit(1);
来源：http://vip.jiagoushi.top

JS:   process.exit(1)
来源：http://wgt.jinqigufen.top

TS:   process.exit(1)
来源：http://dsq.zhoulong.xyz

Java: System.exit(1)
来源：http://yvt.jqgufenzy.top

Go:   os.Exit(1)
来源：http://igk.jqgufenzy.top

Ruby: exit 1
来源：http://idv.hcnkem.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tqn.ctjpmb.com

[M06] 向标准错误输出
来源：http://poh.wangdashe.top

Py:   print("err", file=sys.stderr)
来源：http://ghh.cucudq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ovo.yj20258888.top

JS:   console.error("err")
来源：http://wnh.jianghu66.top

TS:   console.error("err")
来源：http://emv.zdqjudy.top

Java: System.err.println("err")
来源：http://fqf.yangfankeji.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wnn.shanyushiyangkeji.top

Ruby: warn "err"
来源：http://snx.zdbjq.cn

C#:   Console.Error.WriteLine("err")
来源：http://yid.yangfankeji.com

[M07] 判断是否为主入口
来源：http://vqr.zhijiandao.cn

Py:   if __name__ == "__main__":
来源：http://rmd.vehdjk.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qbh.zdqjudy.top

JS:   require.main === module
来源：http://won.yvedp.cn

TS:   require.main === module
来源：http://gnz.9152youxi.cn

Java: public static void main(String[] args)
来源：http://btk.daria6918.cn

Go:   func main()
来源：http://rbn.cucudq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mvi.ydjk.org.cn

C#:   static void Main(string[] args)
来源：http://rpv.gotoacloud.top

[M08] 获取系统与运行时信息
来源：http://gia.hesvh.cn

Py:   platform.system();  platform.python_version()
来源：http://ypl.jqgufenzy.top

PHP:  PHP_OS;  phpversion();
来源：http://igd.hesvh.cn

JS:   process.platform;  process.version
来源：http://yxz.aibaodan.cn

TS:   process.platform;  process.version
来源：http://okz.jinqigufen.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sxw.sufxvd.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://emv.yj202588.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://djk.jyoumei.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pmz.cucudq.cn

================================================================================
来源：http://xtl.ybcxt.top

N. 数据结构与算法
来源：http://iob.cashguo.top

================================================================================
来源：http://sbu.yuxming.cn

[N01] 二分查找（有序数组）
来源：http://usg.cdnleiting.top

Py:   bisect.bisect_left(arr, x)
来源：http://jsc.svipenyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pyg.yanxiufei.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://srn.xingfuxueyuan.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://knq.hywenlv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ntd.fehbvm.com

Go:   sort.SearchInts(arr, x)
来源：http://fjt.cucudq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ked.yueranfly.top

C#:   Array.BinarySearch(arr, x)
来源：http://yet.jlsjyb.cn

[N02] 排序（工程实践用内置实现）
来源：http://vzm.yangfankeji.com

Py:   sorted(arr);  arr.sort()
来源：http://xwl.chenzaomai.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://byl.hnxiangtu.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ign.yueranfly.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://sxy.nanxuanxn.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fdk.shzxlz.cn

Go:   slices.Sort(arr)
来源：http://dss.gzhubu.top

Ruby: arr.sort
来源：http://qga.mhx1999.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xuz.ctjpmb.com

[N03] 快速排序（分治示例）
来源：http://bvx.zhengqikj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vfv.wangdashe.top


<!-- 参考信息 -->
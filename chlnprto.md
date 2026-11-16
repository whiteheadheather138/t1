代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://nwv.daxiang520.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jtg.sufxvd.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hyp.xuanzx.com

Java: LocalDate.now().plusDays(7)
来源：http://ipq.yj202588.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uio.fanxiaobao.xyz

Ruby: Time.now + 7 * 86400
来源：http://hgn.kuanghao11.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pht.vqdsnc.cn

[J06] 计算两时间之差
来源：http://yts.gogol.net.cn

Py:   (end - start).total_seconds()
来源：http://uhi.jinqigufen.top

PHP:  $end->diff($start)->days;
来源：http://yhk.hammf.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dfx.xinyue.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hxr.xylfe.cn

Java: Duration.between(start, end).toSeconds()
来源：http://oyq.zhoulong.xyz

Go:   end.Sub(start).Hours()
来源：http://myf.andypj.xyz

Ruby: end - start                 # 返回秒数
来源：http://bkh.vehdjk.com

C#:   (end - start).TotalSeconds
来源：http://spp.ybcxt.top

[J07] 比较两个日期
来源：http://zuo.sjlbkw.cn

Py:   d1 < d2;  d1 == d2
来源：http://ymv.gogol.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://unh.cheryme.top

JS:   d1.getTime() < d2.getTime()
来源：http://hnu.jqgfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://hjt.zycfv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rkf.cucudq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nqy.shangyingyoupin.top

Ruby: d1 < d2;  d1 == d2
来源：http://wrg.jqgfzy.top

C#:   d1 < d2;  d1 == d2
来源：http://glt.jinqigufen.top

[J08] 提取年月日与星期
来源：http://xmg.jiagoushi.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://seq.snrcjt.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wrc.haohaochexian.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qcj.aibaodan.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dvw.zdbjq.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gox.c1oappe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://voz.ydzc1.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bsi.gotoacloud.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xpr.sjlbkw.cn

[J09] 时区处理
来源：http://ikd.ydzc1.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ozn.ydjk.org.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://weh.quarkkingdee.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://inc.havefunace.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://czt.cdnleiting.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vpy.yangfankeji.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vsl.tarul.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jjq.xuanzx.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://aem.cheryme.top

[J10] 取今天 / 本月第一天
来源：http://qqr.yj202588.top

Py:   date.today();  date.today().replace(day=1)
来源：http://kui.xuanzx.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://knj.cashguo.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yxe.yongpay.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://aqv.tian-w.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hhd.fehbvm.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wlu.cucudq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vez.jinqigufen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tgz.tarul.cn

================================================================================
来源：http://fjc.bbcook.cn

K. JSON 与序列化
来源：http://vzs.jiagoushi.top

================================================================================
来源：http://wri.zdbjq.cn

[K01] 对象转 JSON 字符串
来源：http://cao.pycfn.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://svb.hnqzz.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dta.yj20258888.top

JS:   JSON.stringify(obj)
来源：http://rrb.yangfankeji.com

TS:   JSON.stringify(obj)
来源：http://sor.yongpay.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hxr.xinyue.icu

Go:   json.Marshal(obj)
来源：http://tgf.ybcxt.top

Ruby: obj.to_json                                     // require "json"
来源：http://qkh.hnqzz.top

C#:   JsonSerializer.Serialize(obj)
来源：http://smt.zhaomingkeji.xyz

[K02] JSON 字符串转对象
来源：http://pch.redwolf501.top

Py:   json.loads(s)
来源：http://pkr.jiagoushi.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yjh.tarul.cn

JS:   JSON.parse(s)
来源：http://rcn.shangyingyoupin.top

TS:   JSON.parse(s)
来源：http://lid.zhijiandao.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qwz.kuanghao11.cn

Go:   json.Unmarshal(data, &v)
来源：http://bey.ybcxt.top

Ruby: JSON.parse(s)
来源：http://rai.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://thl.sysykeji.top

[K03] JSON 美化输出（带缩进）
来源：http://xfu.shanyushiyangtech.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zkz.pengpengdd.cyou

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://krm.hnqzz.top

JS:   JSON.stringify(obj, null, 2)
来源：http://rwo.jianghu66.top

TS:   JSON.stringify(obj, null, 2)
来源：http://gsd.c1oappe.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vgw.hnxiangtu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yyy.havefunace.top

Ruby: JSON.pretty_generate(obj)
来源：http://zbk.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cta.zhixingplan.top

[K04] 读取 JSON 文件
来源：http://yya.sysykeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://upk.xinyue.icu

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://teb.feifeiyinyue.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blc.xylfe.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kvs.kuanghao11.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kms.guowangkeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://isa.vehdjk.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://aee.gotoacloud.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xql.ivvv.top

[K05] 深拷贝对象
来源：http://wwy.sjlbkw.cn

Py:   copy.deepcopy(obj)
来源：http://ucg.haohaochexian.top

PHP:  unserialize(serialize($obj));
来源：http://osb.aibaodan.cn

JS:   structuredClone(obj)
来源：http://kec.ctjpmb.com

TS:   structuredClone(obj)
来源：http://mwc.fanxiaobao.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://bva.vqdsnc.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vji.sweek.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dwb.cashguo.top

C#:   // 序列化往返，或自定义 Clone
来源：http://wnx.yfazqb.com

[K06] 解析 URL 查询串
来源：http://ual.zhengqikj.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://roc.sysykeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://epp.bbcook.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bny.yuanzhike.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qta.sweek.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xki.dashuyun.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://obh.gaohongyu789.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jkh.jyoumei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ahf.hywenlv.cn

[K07] 进制转换
来源：http://hrj.zycfv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://odb.fanxiaobao.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://clc.9152youxi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nsl.xingfuxueyuan.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://scu.sxryk.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://epu.wangshuangyany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yju.gogol.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lmc.aizwys.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mzw.nanxuanxn.top

[K08] 二进制序列化（非 JSON）
来源：http://hxb.jinqigfzy.top

Py:   pickle.dumps(obj)
来源：http://zcj.svipenyu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://opu.zhengqikj.top

JS:   v8.serialize(obj)        // Node
来源：http://bmp.xinyue.icu

TS:   v8.serialize(obj)        // Node
来源：http://ddo.316326.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vab.sxryk.cn

Go:   encoding/gob
来源：http://txo.cheryme.top

Ruby: Marshal.dump(obj)
来源：http://vjn.yangfankeji.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mfo.aibaodan.cn

================================================================================
来源：http://fns.yvedp.cn

L. 网络请求
来源：http://fev.guowangkeji.top

================================================================================
来源：http://ufp.jianghu66.top

[L01] 发送 GET 请求
来源：http://enx.yonumen.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qfj.gaohongyu789.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lru.hcnkem.com

JS:   await fetch(url)
来源：http://aog.sjlbkw.cn

TS:   await fetch(url)
来源：http://lnw.nanxuanxn.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fjf.0kj1m.cn

Go:   resp, err := http.Get(url)
来源：http://dvn.yuanzhike.top

Ruby: Net::HTTP.get(URI(url))
来源：http://giw.wangshuangyany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zsv.yj20258888.top

[L02] 发送 POST JSON
来源：http://vke.hnqzz.top

Py:   requests.post(url, json={"a": 1})
来源：http://grb.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dwj.daxiang520.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://npl.yj202588.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xpe.yuanzhike.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wcb.hcnkem.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wbc.epnwcf.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ggf.jqgfzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lko.xuetiantiany.cn

[L03] 设置自定义请求头
来源：http://nou.guowangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xbc.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vip.sjlbkw.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ykc.jyoumei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kiu.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://aoi.zycfv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eai.sufxvd.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ztx.yuanzhike.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gzy.yfazqb.com

[L04] 设置超时
来源：http://jbj.yj20258.top

Py:   requests.get(url, timeout=5)
来源：http://qym.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wht.yj202588.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bod.zhixingplan.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://spn.mhx1999.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://itn.ywan-chungtsiang.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nat.tian-w.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://djm.yangfankeji.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zpw.gotoacloud.top

[L05] 上传文件（multipart）
来源：http://oct.xylfe.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kjc.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nzx.smart0.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oug.fehbvm.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xcq.jinghuilouyu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nqu.jqgufenzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://egc.ydzc1.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nqr.jqgufenzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uos.gotoacloud.top

[L06] 解析响应为 JSON
来源：http://tko.ybcxt.top

Py:   resp.json()
来源：http://mni.cheryme.top

PHP:  json_decode($body, true);
来源：http://omm.gaohongyu789.top

JS:   await resp.json()
来源：http://csx.chenzaomai.com

TS:   await resp.json()
来源：http://ddh.yueranfly.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dxi.zhongyouzk.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jyj.nanxinkj.top

Ruby: JSON.parse(resp.body)
来源：http://mlf.52xcode.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yob.tianlin.xyz

[L07] 处理 HTTP 状态码
来源：http://vty.c1oappe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wkk.guannengcc.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ovq.ppjwa.cn

JS:   resp.ok;  resp.status
来源：http://jhk.tianlin.xyz

TS:   resp.ok;  resp.status
来源：http://fjz.gzhubu.top

Java: resp.statusCode()
来源：http://smp.jiagoushi.top

Go:   resp.StatusCode
来源：http://puz.yuanzhike.top

Ruby: resp.code.to_i
来源：http://zne.redwolf501.top

C#:   (int)resp.StatusCode
来源：http://chp.0kj1m.cn

[L08] 并发请求多个地址
来源：http://bbq.jianghu66.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zhm.nanxinkj.top

PHP:  curl_multi_init() 系列
来源：http://wkb.snrcjt.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uuh.sjlbkw.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jmq.sxryk.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hna.zhiwuduotai.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zvk.0kj1m.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://paa.snrcjt.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mkk.shuidangran.top

================================================================================
来源：http://ojj.vehdjk.com

M. 命令行 / 进程 / 环境
来源：http://akz.fzhhl.top

================================================================================
来源：http://cgz.aizwys.cn

[M01] 读取命令行参数
来源：http://bbv.hammf.cn

Py:   sys.argv[1:]
来源：http://vad.jyoumei.cn

PHP:  $argv;  $argc;
来源：http://wvh.fengsongda.top

JS:   process.argv.slice(2)
来源：http://ynw.316326.xyz

TS:   process.argv.slice(2)
来源：http://sjc.zhijiandao.cn

Java: args 数组（main 方法参数）
来源：http://svh.shzxlz.cn

Go:   os.Args[1:]
来源：http://lml.cashguo.top

Ruby: ARGV
来源：http://ieo.jinyuanbaomall.cn

C#:   args 数组（Main 方法参数）
来源：http://oaj.aizwys.cn

[M02] 读取环境变量
来源：http://yzn.fktsv.cn

Py:   os.environ.get("HOME")
来源：http://bzd.fanxiaobao.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fsy.yueranfly.top

JS:   process.env.HOME
来源：http://efr.redwolf501.top

TS:   process.env.HOME
来源：http://inx.shuidangran.top

Java: System.getenv("HOME")
来源：http://shh.xuanzx.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tgc.epnwcf.com

Ruby: ENV["HOME"]
来源：http://dcr.smart0.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uxb.cucudq.cn

[M03] 执行外部命令
来源：http://zdo.dashuyun.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fij.kuanghao11.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://drb.daria6918.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://krx.guannengcc.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xjx.9152youxi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://okp.hcnkem.com

Go:   exec.Command("ls", "-l").Output()
来源：http://lpd.hysaishi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vvu.zhiwuduotai.top

C#:   Process.Start("ls", "-l");
来源：http://nzu.guowangkeji.top

[M04] 获取当前工作目录
来源：http://kph.hywenlv.cn

Py:   os.getcwd()
来源：http://qxf.hnqzz.top

PHP:  getcwd();
来源：http://erv.sysykeji.top

JS:   process.cwd()
来源：http://fpx.snrcjt.cn

TS:   process.cwd()
来源：http://ikl.cashguo.top

Java: Path.of("").toAbsolutePath()
来源：http://dyi.yj202588.top

Go:   os.Getwd()
来源：http://iil.ywan-chungtsiang.top

Ruby: Dir.pwd
来源：http://dmq.zycfv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yih.316326.xyz

[M05] 设置退出码
来源：http://zzp.bbcook.cn

Py:   sys.exit(1)
来源：http://fby.svipenyu.cn

PHP:  exit(1);
来源：http://upe.0kj1m.cn

JS:   process.exit(1)
来源：http://fxl.zycfv.cn

TS:   process.exit(1)
来源：http://oji.jqgufenzy.top

Java: System.exit(1)
来源：http://tsw.cashguo.top

Go:   os.Exit(1)
来源：http://qrx.chenzaomai.com

Ruby: exit 1
来源：http://vls.smart0.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vtc.ydzc1.top

[M06] 向标准错误输出
来源：http://cyk.tianlin.xyz

Py:   print("err", file=sys.stderr)
来源：http://lhf.hesvh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wzw.quarkkingdee.top

JS:   console.error("err")
来源：http://nzd.jlsjyb.cn

TS:   console.error("err")
来源：http://msw.feifeiyinyue.top

Java: System.err.println("err")
来源：http://grg.sufxvd.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lxg.cdnleiting.top

Ruby: warn "err"
来源：http://van.jiagoushi.top

C#:   Console.Error.WriteLine("err")
来源：http://yqy.quarkkingdee.top

[M07] 判断是否为主入口
来源：http://sxq.guowangkeji.top

Py:   if __name__ == "__main__":
来源：http://gqo.jlsjyb.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xzg.ehwqpu.com

JS:   require.main === module
来源：http://kur.hongshengwenyu.top

TS:   require.main === module
来源：http://gpz.smart0.xyz

Java: public static void main(String[] args)
来源：http://won.zdbjq.cn

Go:   func main()
来源：http://pba.zhoulong.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://udm.zycfv.cn

C#:   static void Main(string[] args)
来源：http://gvs.hongshengwenyu.top

[M08] 获取系统与运行时信息
来源：http://qce.nwbrower.top

Py:   platform.system();  platform.python_version()
来源：http://qlr.shangyingyoupin.top

PHP:  PHP_OS;  phpversion();
来源：http://rmj.uphjek.com

JS:   process.platform;  process.version
来源：http://gly.hcnkem.com

TS:   process.platform;  process.version
来源：http://qic.shuidangran.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kqi.sjlbkw.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vtw.yangfankeji.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gru.vqdsnc.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jom.hammf.cn

================================================================================
来源：http://iza.yj202588.top

N. 数据结构与算法
来源：http://hjf.yanxiufei.cn

================================================================================
来源：http://twp.hammf.cn

[N01] 二分查找（有序数组）
来源：http://zbo.havefunace.top

Py:   bisect.bisect_left(arr, x)
来源：http://lwf.yvedp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sfx.aibaodan.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ohy.birdmap.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uhg.hnxiangtu.top

Java: Arrays.binarySearch(arr, x)
来源：http://xyi.fanxiaobao.xyz

Go:   sort.SearchInts(arr, x)
来源：http://ekq.smart0.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://xbj.ydjk.org.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gar.zhaomingkeji.xyz

[N02] 排序（工程实践用内置实现）
来源：http://ail.cheryme.top

Py:   sorted(arr);  arr.sort()
来源：http://pyg.bjfxy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fjy.yj20258.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://dmo.feifeiyinyue.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ren.vqdsnc.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wzh.sweek.top

Go:   slices.Sort(arr)
来源：http://kzv.chenlongwang.top

Ruby: arr.sort
来源：http://sht.jlsjyb.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zqy.jyoumei.cn

[N03] 快速排序（分治示例）
来源：http://hdp.xziqi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rjk.jyoumei.cn


<!-- 参考信息 -->
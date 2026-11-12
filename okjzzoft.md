代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ffg.zycfv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://svf.havefunace.top

[J05] 时间加减（加 7 天）
来源：http://plt.fktsv.cn

Py:   now + timedelta(days=7)
来源：http://ydh.haohaochexian.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qah.cdnleiting.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hnj.jinqigfzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ahl.yj20258888.top

Java: LocalDate.now().plusDays(7)
来源：http://ajb.jinqigufen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dsv.gotoacloud.top

Ruby: Time.now + 7 * 86400
来源：http://ido.zdqjudy.top

C#:   DateTime.Now.AddDays(7)
来源：http://tkn.kuanghao11.cn

[J06] 计算两时间之差
来源：http://otv.nwbrower.top

Py:   (end - start).total_seconds()
来源：http://fdw.bjfxy.top

PHP:  $end->diff($start)->days;
来源：http://bgq.sxryk.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jba.nanxuanxn.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ybw.zhixingplan.top

Java: Duration.between(start, end).toSeconds()
来源：http://ofc.cucudq.cn

Go:   end.Sub(start).Hours()
来源：http://zjb.mhx1999.top

Ruby: end - start                 # 返回秒数
来源：http://xet.gogol.net.cn

C#:   (end - start).TotalSeconds
来源：http://lwr.xylfe.cn

[J07] 比较两个日期
来源：http://lmz.shuidangran.top

Py:   d1 < d2;  d1 == d2
来源：http://svy.jinqigufen.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dfv.yangfankeji.com

JS:   d1.getTime() < d2.getTime()
来源：http://fph.vqdsnc.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mrs.hammf.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://muu.tarul.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ddw.pengpengdd.cyou

Ruby: d1 < d2;  d1 == d2
来源：http://oox.vehdjk.com

C#:   d1 < d2;  d1 == d2
来源：http://oaq.zhixingplan.top

[J08] 提取年月日与星期
来源：http://mun.fktsv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vde.yonumen.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kvq.ybcxt.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pon.chenzaomai.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tmg.quarkkingdee.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pud.pycfn.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zso.jqgfzy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nzj.dianchejie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fcn.yvedp.cn

[J09] 时区处理
来源：http://sje.xinyue.icu

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zgz.xingfuxueyuan.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://chb.fehbvm.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://usg.ywan-chungtsiang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gjw.gzhubu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zix.iojbl.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mbd.yuanzhike.top

Ruby: Time.now.getlocal("+08:00")
来源：http://eij.zdbjq.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uxz.ppjwa.cn

[J10] 取今天 / 本月第一天
来源：http://cds.wangshuangyany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rkq.jqgufenzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ppi.vehdjk.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mfw.gaohongyu789.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mjl.bjfxy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rsp.sufxvd.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vhv.xziqi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nrf.wangdashe.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fws.yanxiufei.cn

================================================================================
来源：http://rcn.yj20258.top

K. JSON 与序列化
来源：http://vzd.xuanzx.com

================================================================================
来源：http://owp.c1oappe.top

[K01] 对象转 JSON 字符串
来源：http://bzf.feifeiyinyue.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dut.chenjidiqi.icu

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ybd.ydzc1.top

JS:   JSON.stringify(obj)
来源：http://tkx.sxryk.cn

TS:   JSON.stringify(obj)
来源：http://yif.zhengqikj.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ebw.jinqigfzy.top

Go:   json.Marshal(obj)
来源：http://pmz.jiagoushi.top

Ruby: obj.to_json                                     // require "json"
来源：http://ibn.guowangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://faf.zhijiandao.cn

[K02] JSON 字符串转对象
来源：http://ugx.fzhhl.top

Py:   json.loads(s)
来源：http://qjy.ywan-chungtsiang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iri.zhengqikj.top

JS:   JSON.parse(s)
来源：http://obh.9152youxi.cn

TS:   JSON.parse(s)
来源：http://ziz.fzhhl.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mdt.jqgfzy.top

Go:   json.Unmarshal(data, &v)
来源：http://tmj.wangshuangyany.cn

Ruby: JSON.parse(s)
来源：http://rga.kuanghao11.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ute.xingfuxueyuan.xyz

[K03] JSON 美化输出（带缩进）
来源：http://ohj.zhijiandao.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dxs.yongpay.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://est.nanxinkj.top

JS:   JSON.stringify(obj, null, 2)
来源：http://eqn.sweek.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wcu.kuanghao11.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kar.pycfn.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hew.fzhhl.top

Ruby: JSON.pretty_generate(obj)
来源：http://efu.yonumen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ihn.cdnleiting.top

[K04] 读取 JSON 文件
来源：http://fap.c1oappe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yuk.nwbrower.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nod.xylfe.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nbi.hcnkem.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dur.ydjk.org.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://szc.ehwqpu.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nkr.ivvv.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://krp.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://knk.meibo888.top

[K05] 深拷贝对象
来源：http://xey.yj20258.top

Py:   copy.deepcopy(obj)
来源：http://wlm.cashguo.top

PHP:  unserialize(serialize($obj));
来源：http://ihy.zhiwuduotai.top

JS:   structuredClone(obj)
来源：http://pdq.zhaomingkeji.xyz

TS:   structuredClone(obj)
来源：http://iwj.aibaodan.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vit.iojbl.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://adh.kuanghao11.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oxz.fanxiaobao.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://xqr.daxiang520.top

[K06] 解析 URL 查询串
来源：http://uhp.yvedp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qwr.jinyuanbaomall.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zfk.cdnleiting.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://akg.yj202588.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gjj.fengsongda.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jic.bjfxy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ojq.hywenlv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://eeq.ivvv.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ptw.cucudq.cn

[K07] 进制转换
来源：http://cle.uphjek.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cic.zhaomingkeji.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ywt.smart0.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://svb.gotoacloud.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pcs.cqqwz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fau.hywenlv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blj.ydjk.org.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ain.xingfuxueyuan.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wbs.xziqi.cn

[K08] 二进制序列化（非 JSON）
来源：http://bxo.shanyushiyangkeji.top

Py:   pickle.dumps(obj)
来源：http://hgg.ctjpmb.com

PHP:  serialize($obj);  unserialize($s);
来源：http://kbc.redwolf501.top

JS:   v8.serialize(obj)        // Node
来源：http://ihk.xuetiantiany.cn

TS:   v8.serialize(obj)        // Node
来源：http://dwo.chenlongwang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vip.yj20258888.top

Go:   encoding/gob
来源：http://nid.meibo888.top

Ruby: Marshal.dump(obj)
来源：http://foh.sweek.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://skd.nanxinkj.top

================================================================================
来源：http://aqj.redwolf501.top

L. 网络请求
来源：http://xsx.zhaomingkeji.xyz

================================================================================
来源：http://enp.pycfn.com

[L01] 发送 GET 请求
来源：http://wqt.ivvv.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ubf.xinyue.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kur.fzhhl.top

JS:   await fetch(url)
来源：http://njd.sxryk.cn

TS:   await fetch(url)
来源：http://zlj.fehbvm.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wqz.sweek.top

Go:   resp, err := http.Get(url)
来源：http://rvg.xinyue.icu

Ruby: Net::HTTP.get(URI(url))
来源：http://cej.jlsjyb.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qda.yonumen.top

[L02] 发送 POST JSON
来源：http://uxl.0kj1m.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mgq.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://onb.hfpthk.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jul.aizwys.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pga.pycfn.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vsp.ivvv.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://usv.ydzc1.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ghl.jinqigfzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dvv.zhijiandao.cn

[L03] 设置自定义请求头
来源：http://pyu.yj202588.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pui.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lhl.cqqwz.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mdr.hnxiangtu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kpd.hongshengwenyu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://axx.ydzc1.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kjt.hywenlv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iya.guannengcc.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cgh.pycfn.com

[L04] 设置超时
来源：http://bcc.cashguo.top

Py:   requests.get(url, timeout=5)
来源：http://xsy.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cvb.jyoumei.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sgw.fengsongda.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nib.zdqjudy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tya.zycfv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bpy.cheryme.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://aug.yanxiufei.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xvv.xinyue.icu

[L05] 上传文件（multipart）
来源：http://yfy.hesvh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://khp.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://osf.hammf.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wzr.chenzaomai.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yzw.sjlbkw.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zer.iojbl.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://not.yuxming.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wqy.yangfankeji.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lar.sufxvd.cn

[L06] 解析响应为 JSON
来源：http://pdb.dashuyun.cn

Py:   resp.json()
来源：http://wan.wangdashe.top

PHP:  json_decode($body, true);
来源：http://rif.ctjpmb.com

JS:   await resp.json()
来源：http://bgs.hesvh.cn

TS:   await resp.json()
来源：http://iot.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xml.hfpthk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xzx.shanyushiyangtech.top

Ruby: JSON.parse(resp.body)
来源：http://wbi.jqgfzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fch.52xcode.cn

[L07] 处理 HTTP 状态码
来源：http://mpr.zhoulong.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fym.gogol.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yqz.ctjpmb.com

JS:   resp.ok;  resp.status
来源：http://bxp.hcnkem.com

TS:   resp.ok;  resp.status
来源：http://pmo.jlsjyb.cn

Java: resp.statusCode()
来源：http://gjl.gogol.net.cn

Go:   resp.StatusCode
来源：http://fhe.hywenlv.cn

Ruby: resp.code.to_i
来源：http://ywv.cucudq.cn

C#:   (int)resp.StatusCode
来源：http://oqv.zdbjq.cn

[L08] 并发请求多个地址
来源：http://czc.fanxiaobao.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://onw.shanyushiyangkeji.top

PHP:  curl_multi_init() 系列
来源：http://aql.sufxvd.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gbg.zhixingplan.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://niw.jinqigufen.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ppq.tian-w.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dxk.yangfankeji.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jju.sysykeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gvz.epnwcf.com

================================================================================
来源：http://vtk.yj20258.top

M. 命令行 / 进程 / 环境
来源：http://gvk.cqqwz.cn

================================================================================
来源：http://blk.dianchejie.cn

[M01] 读取命令行参数
来源：http://pvb.pengpengdd.cyou

Py:   sys.argv[1:]
来源：http://mbw.cdnleiting.top

PHP:  $argv;  $argc;
来源：http://gle.zhoulong.xyz

JS:   process.argv.slice(2)
来源：http://wla.ctjpmb.com

TS:   process.argv.slice(2)
来源：http://ajy.haohaochexian.top

Java: args 数组（main 方法参数）
来源：http://ael.yj20258.top

Go:   os.Args[1:]
来源：http://yyu.tarul.cn

Ruby: ARGV
来源：http://zbj.hesvh.cn

C#:   args 数组（Main 方法参数）
来源：http://ofh.yj20258888.top

[M02] 读取环境变量
来源：http://bby.zhaomingkeji.xyz

Py:   os.environ.get("HOME")
来源：http://hxg.aizwys.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ewc.shanyushiyangtech.top

JS:   process.env.HOME
来源：http://lge.jinqigfzy.top

TS:   process.env.HOME
来源：http://upu.kuanghao11.cn

Java: System.getenv("HOME")
来源：http://xco.zycfv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tks.jinyuanbaomall.cn

Ruby: ENV["HOME"]
来源：http://tgn.fengsongda.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gya.ehwqpu.com

[M03] 执行外部命令
来源：http://vxj.aizwys.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vvi.fktsv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ndh.iojbl.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nzr.yanxiufei.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://aze.yuanzhike.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://evh.dashuyun.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qdq.ehwqpu.com

Ruby: system("ls -l");  `ls -l`
来源：http://yfc.tian-w.cn

C#:   Process.Start("ls", "-l");
来源：http://qzz.tarul.cn

[M04] 获取当前工作目录
来源：http://ble.gotoacloud.top

Py:   os.getcwd()
来源：http://bng.ctjpmb.com

PHP:  getcwd();
来源：http://vuf.ybcxt.top

JS:   process.cwd()
来源：http://iix.guannengcc.top

TS:   process.cwd()
来源：http://ctv.zhixingplan.top

Java: Path.of("").toAbsolutePath()
来源：http://ehp.ywan-chungtsiang.top

Go:   os.Getwd()
来源：http://uyn.jinyuanbaomall.cn

Ruby: Dir.pwd
来源：http://hoq.aizwys.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dzg.ybcxt.top

[M05] 设置退出码
来源：http://aok.sufxvd.cn

Py:   sys.exit(1)
来源：http://sfz.zhengqikj.top

PHP:  exit(1);
来源：http://lfi.fengsongda.top

JS:   process.exit(1)
来源：http://prc.vqdsnc.cn

TS:   process.exit(1)
来源：http://spq.vehdjk.com

Java: System.exit(1)
来源：http://str.yangfankeji.com

Go:   os.Exit(1)
来源：http://kdh.chenjidiqi.icu

Ruby: exit 1
来源：http://kgo.jinqigufen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kbg.nanxinkj.top

[M06] 向标准错误输出
来源：http://vsv.jinqigfzy.top

Py:   print("err", file=sys.stderr)
来源：http://nsf.ivvv.top

PHP:  fwrite(STDERR, "err\n");
来源：http://rmp.ehwqpu.com

JS:   console.error("err")
来源：http://gzl.xylfe.cn

TS:   console.error("err")
来源：http://eyl.vqdsnc.cn

Java: System.err.println("err")
来源：http://mxg.hammf.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dgr.nanxuanxn.top

Ruby: warn "err"
来源：http://daq.0kj1m.cn

C#:   Console.Error.WriteLine("err")
来源：http://lse.jiagoushi.top

[M07] 判断是否为主入口
来源：http://tpa.yongpay.top

Py:   if __name__ == "__main__":
来源：http://tze.yueranfly.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uif.jianghu66.top

JS:   require.main === module
来源：http://abz.fktsv.cn

TS:   require.main === module
来源：http://cbo.nanxinkj.top

Java: public static void main(String[] args)
来源：http://yzm.ehwqpu.com

Go:   func main()
来源：http://hfl.xinyue.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gvy.shangyingyoupin.top

C#:   static void Main(string[] args)
来源：http://lgi.yanxiufei.cn

[M08] 获取系统与运行时信息
来源：http://yzn.hnxiangtu.top

Py:   platform.system();  platform.python_version()
来源：http://iyb.zhijiandao.cn

PHP:  PHP_OS;  phpversion();
来源：http://klt.hcnkem.com

JS:   process.platform;  process.version
来源：http://awh.jianghu66.top

TS:   process.platform;  process.version
来源：http://fqs.pengpengdd.cyou

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ldx.xuetiantiany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mmb.pycfn.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blk.yfazqb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://wpk.tianlin.xyz

================================================================================
来源：http://iwi.andypj.xyz

N. 数据结构与算法
来源：http://uxv.cheryme.top

================================================================================
来源：http://lik.jinqigfzy.top

[N01] 二分查找（有序数组）
来源：http://tgg.hammf.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fic.guowangkeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xiy.ivvv.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tku.0kj1m.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tas.hfpthk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kjt.nwbrower.top

Go:   sort.SearchInts(arr, x)
来源：http://qmh.smart0.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://oko.uphjek.com

C#:   Array.BinarySearch(arr, x)
来源：http://bjy.jlsjyb.cn

[N02] 排序（工程实践用内置实现）
来源：http://xis.0kj1m.cn

Py:   sorted(arr);  arr.sort()
来源：http://xkh.ydjk.org.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gcv.pycfn.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://dvs.yuxming.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ieh.wangdashe.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://coy.fehbvm.com

Go:   slices.Sort(arr)
来源：http://ysm.ivvv.top


<!-- 参考信息 -->
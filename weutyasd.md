代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jor.yanxiufei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lhe.wangshuangyany.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fta.yj202588.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hwe.chenlongwang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ezs.svipenyu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hod.daxiang520.top

[J05] 时间加减（加 7 天）
来源：http://vsp.fanxiaobao.xyz

Py:   now + timedelta(days=7)
来源：http://pmo.shanyushiyangtech.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://vft.yj20258888.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://roj.316326.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rko.uphjek.com

Java: LocalDate.now().plusDays(7)
来源：http://uaa.yuanzhike.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qrc.shuidangran.top

Ruby: Time.now + 7 * 86400
来源：http://kkb.ydzc1.top

C#:   DateTime.Now.AddDays(7)
来源：http://kqp.jqgufenzy.top

[J06] 计算两时间之差
来源：http://bof.chenjidiqi.icu

Py:   (end - start).total_seconds()
来源：http://qer.zhongyouzk.top

PHP:  $end->diff($start)->days;
来源：http://vhu.fzhhl.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://crx.gzhubu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xfq.jqgfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://lph.hnqzz.top

Go:   end.Sub(start).Hours()
来源：http://iti.zhaomingkeji.xyz

Ruby: end - start                 # 返回秒数
来源：http://ivk.hcnkem.com

C#:   (end - start).TotalSeconds
来源：http://rqs.chenjidiqi.icu

[J07] 比较两个日期
来源：http://veh.52xcode.cn

Py:   d1 < d2;  d1 == d2
来源：http://pje.snrcjt.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ovg.xuanzx.com

JS:   d1.getTime() < d2.getTime()
来源：http://jrl.ydzc1.top

TS:   d1.getTime() < d2.getTime()
来源：http://zav.iojbl.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qhv.jyoumei.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rgp.cdnleiting.top

Ruby: d1 < d2;  d1 == d2
来源：http://bac.hammf.cn

C#:   d1 < d2;  d1 == d2
来源：http://sah.sjlbkw.cn

[J08] 提取年月日与星期
来源：http://zbe.kuanghao11.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ngf.hfpthk.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tzv.hysaishi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://llh.tianlin.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://coi.guannengcc.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ogp.fehbvm.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://aar.xziqi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tgs.fanxiaobao.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nbb.yj20258888.top

[J09] 时区处理
来源：http://xic.fzhhl.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vgp.chenjidiqi.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gec.pycfn.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bfr.fehbvm.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tkq.xziqi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tbn.cheryme.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lvm.xingfuxueyuan.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://hkc.feifeiyinyue.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ies.zycfv.cn

[J10] 取今天 / 本月第一天
来源：http://qnm.sysykeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://gjc.shangyingyoupin.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://txw.fktsv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vwj.shzxlz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yjl.smart0.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cjk.zdbjq.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cxn.yj20258.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mol.ppjwa.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tfb.gaohongyu789.top

================================================================================
来源：http://xac.hfpthk.cn

K. JSON 与序列化
来源：http://fan.sxryk.cn

================================================================================
来源：http://mwm.haohaochexian.top

[K01] 对象转 JSON 字符串
来源：http://jfi.havefunace.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rev.jyoumei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oeh.haohaochexian.top

JS:   JSON.stringify(obj)
来源：http://xzj.fehbvm.com

TS:   JSON.stringify(obj)
来源：http://vku.chenlongwang.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://eid.hfpthk.cn

Go:   json.Marshal(obj)
来源：http://dwj.yfazqb.com

Ruby: obj.to_json                                     // require "json"
来源：http://fky.daxiang520.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qpg.jqgufenzy.top

[K02] JSON 字符串转对象
来源：http://sqc.ydzc1.top

Py:   json.loads(s)
来源：http://qxd.sxryk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://akl.jlsjyb.cn

JS:   JSON.parse(s)
来源：http://qfx.hfpthk.cn

TS:   JSON.parse(s)
来源：http://mtv.zdbjq.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cph.aizwys.cn

Go:   json.Unmarshal(data, &v)
来源：http://ehs.9152youxi.cn

Ruby: JSON.parse(s)
来源：http://awj.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kts.zhiwuduotai.top

[K03] JSON 美化输出（带缩进）
来源：http://pcm.nanxuanxn.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zxx.fehbvm.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wiw.nanxinkj.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xqq.smart0.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://hol.jqgufenzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vcq.wangshuangyany.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sei.yfazqb.com

Ruby: JSON.pretty_generate(obj)
来源：http://gdo.tarul.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://juj.zhengqikj.top

[K04] 读取 JSON 文件
来源：http://cqy.zhoulong.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hgw.yueranfly.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pgn.birdmap.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pcc.aizwys.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kbq.yangfankeji.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://npd.fengsongda.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hyn.yfazqb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://zhx.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lgy.tarul.cn

[K05] 深拷贝对象
来源：http://wzq.wangshuangyany.cn

Py:   copy.deepcopy(obj)
来源：http://hkn.ppjwa.cn

PHP:  unserialize(serialize($obj));
来源：http://fng.epnwcf.com

JS:   structuredClone(obj)
来源：http://gfc.9152youxi.cn

TS:   structuredClone(obj)
来源：http://oax.52xcode.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mey.pengpengdd.cyou

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tua.hongshengwenyu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://azh.vehdjk.com

C#:   // 序列化往返，或自定义 Clone
来源：http://whj.yueranfly.top

[K06] 解析 URL 查询串
来源：http://frr.guowangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rfm.yvedp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ffi.jyoumei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rvq.tianlin.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lak.mhx1999.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yyb.jqgufenzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kgc.wangdashe.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wnc.dianchejie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vav.gogol.net.cn

[K07] 进制转换
来源：http://qvw.zhixingplan.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mba.nanxuanxn.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://drf.dianchejie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mus.fehbvm.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://koc.shangyingyoupin.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://etz.vqdsnc.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rfz.ivvv.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xui.jinqigfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uml.daria6918.cn

[K08] 二进制序列化（非 JSON）
来源：http://vbv.andypj.xyz

Py:   pickle.dumps(obj)
来源：http://sbq.tanke756.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nct.ywan-chungtsiang.top

JS:   v8.serialize(obj)        // Node
来源：http://gye.sufxvd.cn

TS:   v8.serialize(obj)        // Node
来源：http://vbo.kuanghao11.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qgb.ctjpmb.com

Go:   encoding/gob
来源：http://gnu.tanke756.top

Ruby: Marshal.dump(obj)
来源：http://yog.kuanghao11.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yst.hywenlv.cn

================================================================================
来源：http://soo.jlsjyb.cn

L. 网络请求
来源：http://rib.tian-w.cn

================================================================================
来源：http://pzg.gogol.net.cn

[L01] 发送 GET 请求
来源：http://mho.nanxuanxn.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dng.sweek.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uwp.fktsv.cn

JS:   await fetch(url)
来源：http://wwk.ybcxt.top

TS:   await fetch(url)
来源：http://cwg.sxryk.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qdn.sjlbkw.cn

Go:   resp, err := http.Get(url)
来源：http://xzw.hysaishi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://scf.tian-w.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ped.52xcode.cn

[L02] 发送 POST JSON
来源：http://uby.daxiang520.top

Py:   requests.post(url, json={"a": 1})
来源：http://agr.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gxp.andypj.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kgq.hesvh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ved.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wpb.jqgfzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lat.hammf.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://odn.gogol.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mqn.zhengqikj.top

[L03] 设置自定义请求头
来源：http://zko.9152youxi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bvb.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jkc.gotoacloud.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ces.birdmap.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hxg.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nms.ppjwa.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zoz.guannengcc.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://svl.chenlongwang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cpw.pengpengdd.cyou

[L04] 设置超时
来源：http://vfp.fehbvm.com

Py:   requests.get(url, timeout=5)
来源：http://mpc.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sqo.yj202588.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://apq.yuanzhike.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wwl.yuanzhike.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rjz.pycfn.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uvi.yonumen.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://psm.uphjek.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qml.dianchejie.cn

[L05] 上传文件（multipart）
来源：http://ccx.yj20258.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uqu.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jrt.mhx1999.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gcf.ydzc1.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yld.havefunace.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fsw.daxiang520.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://imd.yuxming.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kfm.fzhhl.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oit.dashuyun.cn

[L06] 解析响应为 JSON
来源：http://obe.vqdsnc.cn

Py:   resp.json()
来源：http://ypm.tarul.cn

PHP:  json_decode($body, true);
来源：http://khd.dianchejie.cn

JS:   await resp.json()
来源：http://oxs.hcnkem.com

TS:   await resp.json()
来源：http://pxn.yanxiufei.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://exi.jlsjyb.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yhk.hysaishi.cn

Ruby: JSON.parse(resp.body)
来源：http://stu.xingfuxueyuan.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://knt.yueranfly.top

[L07] 处理 HTTP 状态码
来源：http://fyl.zhengqikj.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lyn.uphjek.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kvr.shzxlz.cn

JS:   resp.ok;  resp.status
来源：http://uto.zhongyouzk.top

TS:   resp.ok;  resp.status
来源：http://xjo.hesvh.cn

Java: resp.statusCode()
来源：http://ecn.fanxiaobao.xyz

Go:   resp.StatusCode
来源：http://kds.jqgfzy.top

Ruby: resp.code.to_i
来源：http://jqp.jianghu66.top

C#:   (int)resp.StatusCode
来源：http://vlb.kuanghao11.cn

[L08] 并发请求多个地址
来源：http://kmz.sufxvd.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jhs.ydzc1.top

PHP:  curl_multi_init() 系列
来源：http://boi.bjfxy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ojx.cdnleiting.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pka.fzhhl.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yki.316326.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ojh.cdnleiting.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://axx.guowangkeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jns.jiagoushi.top

================================================================================
来源：http://tye.jqgfzy.top

M. 命令行 / 进程 / 环境
来源：http://hgu.zhixingplan.top

================================================================================
来源：http://nvy.nwbrower.top

[M01] 读取命令行参数
来源：http://bwf.yvedp.cn

Py:   sys.argv[1:]
来源：http://izb.yvedp.cn

PHP:  $argv;  $argc;
来源：http://xrh.iojbl.cn

JS:   process.argv.slice(2)
来源：http://uau.jyoumei.cn

TS:   process.argv.slice(2)
来源：http://dho.zhoulong.xyz

Java: args 数组（main 方法参数）
来源：http://sjk.hongshengwenyu.top

Go:   os.Args[1:]
来源：http://asn.yanxiufei.cn

Ruby: ARGV
来源：http://tjl.sufxvd.cn

C#:   args 数组（Main 方法参数）
来源：http://fcz.zhixingplan.top

[M02] 读取环境变量
来源：http://hwq.vehdjk.com

Py:   os.environ.get("HOME")
来源：http://aea.ivvv.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ndx.cucudq.cn

JS:   process.env.HOME
来源：http://eje.sweek.top

TS:   process.env.HOME
来源：http://duk.guannengcc.top

Java: System.getenv("HOME")
来源：http://vtk.guannengcc.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oiz.tian-w.cn

Ruby: ENV["HOME"]
来源：http://gkk.chenjidiqi.icu

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ros.yuanzhike.top

[M03] 执行外部命令
来源：http://wyu.dashuyun.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mup.52xcode.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yny.nanxinkj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xps.jianghu66.top

TS:   child_process.execSync("ls -l").toString()
来源：http://qvn.52xcode.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://djs.yuanzhike.top

Go:   exec.Command("ls", "-l").Output()
来源：http://dhd.redwolf501.top

Ruby: system("ls -l");  `ls -l`
来源：http://yhs.fengsongda.top

C#:   Process.Start("ls", "-l");
来源：http://xft.cheryme.top

[M04] 获取当前工作目录
来源：http://sif.gaohongyu789.top

Py:   os.getcwd()
来源：http://pst.pengpengdd.cyou

PHP:  getcwd();
来源：http://xpw.kuanghao11.cn

JS:   process.cwd()
来源：http://gby.jinqigufen.top

TS:   process.cwd()
来源：http://kim.jinqigufen.top

Java: Path.of("").toAbsolutePath()
来源：http://uwc.bbcook.cn

Go:   os.Getwd()
来源：http://qef.fzhhl.top

Ruby: Dir.pwd
来源：http://aam.ivvv.top

C#:   Directory.GetCurrentDirectory()
来源：http://gtp.xuanzx.com

[M05] 设置退出码
来源：http://yvn.shanyushiyangtech.top

Py:   sys.exit(1)
来源：http://dkf.hesvh.cn

PHP:  exit(1);
来源：http://sfz.fzhhl.top

JS:   process.exit(1)
来源：http://tyb.cucudq.cn

TS:   process.exit(1)
来源：http://anj.guowangkeji.top

Java: System.exit(1)
来源：http://uia.ybcxt.top

Go:   os.Exit(1)
来源：http://svf.tianlin.xyz

Ruby: exit 1
来源：http://icw.zhoulong.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mtz.ctjpmb.com

[M06] 向标准错误输出
来源：http://gpr.zhoulong.xyz

Py:   print("err", file=sys.stderr)
来源：http://riy.guannengcc.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qpm.zycfv.cn

JS:   console.error("err")
来源：http://uub.guowangkeji.top

TS:   console.error("err")
来源：http://mes.yuanzhike.top

Java: System.err.println("err")
来源：http://gmy.mhx1999.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ugn.birdmap.top

Ruby: warn "err"
来源：http://fga.9152youxi.cn

C#:   Console.Error.WriteLine("err")
来源：http://aln.sweek.top

[M07] 判断是否为主入口
来源：http://tym.hywenlv.cn

Py:   if __name__ == "__main__":
来源：http://ypp.jlsjyb.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lec.yvedp.cn

JS:   require.main === module
来源：http://uqy.gzhubu.top

TS:   require.main === module
来源：http://tpv.yuanzhike.top

Java: public static void main(String[] args)
来源：http://iec.gzhubu.top

Go:   func main()
来源：http://mnk.jinghuilouyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vtg.zhixingplan.top

C#:   static void Main(string[] args)
来源：http://qxm.havefunace.top

[M08] 获取系统与运行时信息
来源：http://ohz.jinyuanbaomall.cn

Py:   platform.system();  platform.python_version()
来源：http://kfe.hnqzz.top

PHP:  PHP_OS;  phpversion();
来源：http://dmv.gogol.net.cn

JS:   process.platform;  process.version
来源：http://miy.zhijiandao.cn

TS:   process.platform;  process.version
来源：http://aje.daria6918.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://scz.pycfn.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://mkl.yj20258.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rnd.jinghuilouyu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nnl.wangshuangyany.cn

================================================================================
来源：http://azi.cashguo.top

N. 数据结构与算法
来源：http://hvx.zycfv.cn

================================================================================
来源：http://lrr.jinghuilouyu.cn

[N01] 二分查找（有序数组）
来源：http://azm.hammf.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mwd.gotoacloud.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eff.xziqi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iqp.cucudq.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://moa.chenlongwang.top

Java: Arrays.binarySearch(arr, x)
来源：http://nhg.hfpthk.cn

Go:   sort.SearchInts(arr, x)
来源：http://fkj.gogol.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xlq.cucudq.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hao.yangfankeji.com

[N02] 排序（工程实践用内置实现）
来源：http://tac.bjfxy.top

Py:   sorted(arr);  arr.sort()
来源：http://qpk.shanyushiyangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://icz.zdbjq.cn


<!-- 参考信息 -->
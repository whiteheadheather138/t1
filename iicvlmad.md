代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oxd.jinqigfzy.top

Ruby: Time.now + 7 * 86400
来源：http://obt.tanke756.top

C#:   DateTime.Now.AddDays(7)
来源：http://gej.quarkkingdee.top

[J06] 计算两时间之差
来源：http://hxl.cheryme.top

Py:   (end - start).total_seconds()
来源：http://zlu.fzhhl.top

PHP:  $end->diff($start)->days;
来源：http://kyr.birdmap.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eax.yueranfly.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vxa.yuanzhike.top

Java: Duration.between(start, end).toSeconds()
来源：http://rdg.cdnleiting.top

Go:   end.Sub(start).Hours()
来源：http://oqx.jinqigufen.top

Ruby: end - start                 # 返回秒数
来源：http://krz.bbcook.cn

C#:   (end - start).TotalSeconds
来源：http://loo.chenlongwang.top

[J07] 比较两个日期
来源：http://ghb.quarkkingdee.top

Py:   d1 < d2;  d1 == d2
来源：http://ssj.cashguo.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xcx.chenjidiqi.icu

JS:   d1.getTime() < d2.getTime()
来源：http://rvm.iojbl.cn

TS:   d1.getTime() < d2.getTime()
来源：http://isd.jianghu66.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dov.sweek.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qbu.fzhhl.top

Ruby: d1 < d2;  d1 == d2
来源：http://kvr.ppjwa.cn

C#:   d1 < d2;  d1 == d2
来源：http://pth.hnxiangtu.top

[J08] 提取年月日与星期
来源：http://vhq.birdmap.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nsk.fengsongda.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ptj.xziqi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lgd.hfpthk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hgl.jinyuanbaomall.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pce.vehdjk.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zxe.yangfankeji.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hqm.daxiang520.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cyd.quarkkingdee.top

[J09] 时区处理
来源：http://jqp.ehwqpu.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pgu.snrcjt.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xbm.hnxiangtu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://njo.redwolf501.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yks.sxryk.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qrm.jqgfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zot.jqgufenzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ypy.yfazqb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fnv.havefunace.top

[J10] 取今天 / 本月第一天
来源：http://hnn.jiagoushi.top

Py:   date.today();  date.today().replace(day=1)
来源：http://wbo.snrcjt.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cps.jinqigfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pso.cqqwz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xro.hnxiangtu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bub.hongshengwenyu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gjm.jyoumei.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://abf.xuanzx.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hyo.svipenyu.cn

================================================================================
来源：http://wee.xylfe.cn

K. JSON 与序列化
来源：http://vas.gzhubu.top

================================================================================
来源：http://fum.gotoacloud.top

[K01] 对象转 JSON 字符串
来源：http://ugr.zhengqikj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fsq.yuanzhike.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wgp.iojbl.cn

JS:   JSON.stringify(obj)
来源：http://hfq.cheryme.top

TS:   JSON.stringify(obj)
来源：http://izw.shangyingyoupin.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qpm.cashguo.top

Go:   json.Marshal(obj)
来源：http://ekx.0kj1m.cn

Ruby: obj.to_json                                     // require "json"
来源：http://has.xuanzx.com

C#:   JsonSerializer.Serialize(obj)
来源：http://kcn.gotoacloud.top

[K02] JSON 字符串转对象
来源：http://dcf.cashguo.top

Py:   json.loads(s)
来源：http://gra.yfazqb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pkh.jyoumei.cn

JS:   JSON.parse(s)
来源：http://gvs.jqgfzy.top

TS:   JSON.parse(s)
来源：http://kok.tian-w.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jjo.tanke756.top

Go:   json.Unmarshal(data, &v)
来源：http://cjj.daxiang520.top

Ruby: JSON.parse(s)
来源：http://enj.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://glg.jlsjyb.cn

[K03] JSON 美化输出（带缩进）
来源：http://qbd.daria6918.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mka.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dpk.feifeiyinyue.top

JS:   JSON.stringify(obj, null, 2)
来源：http://bdk.havefunace.top

TS:   JSON.stringify(obj, null, 2)
来源：http://odr.kuanghao11.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jkc.hnqzz.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://prx.epnwcf.com

Ruby: JSON.pretty_generate(obj)
来源：http://fbh.hnxiangtu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fjl.yuanzhike.top

[K04] 读取 JSON 文件
来源：http://bho.jlsjyb.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lic.daxiang520.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ucp.havefunace.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nlw.ehwqpu.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://icc.nanxuanxn.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kcn.jinyuanbaomall.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aqx.guannengcc.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://foj.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hic.guowangkeji.top

[K05] 深拷贝对象
来源：http://rmo.hnxiangtu.top

Py:   copy.deepcopy(obj)
来源：http://kyi.daxiang520.top

PHP:  unserialize(serialize($obj));
来源：http://igs.dashuyun.cn

JS:   structuredClone(obj)
来源：http://iqd.shanyushiyangkeji.top

TS:   structuredClone(obj)
来源：http://msm.sjlbkw.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mjs.pengpengdd.cyou

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qjs.jinghuilouyu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://adl.nwbrower.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zzn.uphjek.com

[K06] 解析 URL 查询串
来源：http://sed.gaohongyu789.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kzp.nanxinkj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rfw.guowangkeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cdu.sjlbkw.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lna.fengsongda.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zxe.tarul.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zaz.zhengqikj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kxy.yonumen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dvs.ydjk.org.cn

[K07] 进制转换
来源：http://rbc.52xcode.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rgq.yj202588.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oea.sjlbkw.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fpz.yj20258.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://unu.cucudq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zft.vqdsnc.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ghc.zdbjq.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xzo.epnwcf.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mvk.yfazqb.com

[K08] 二进制序列化（非 JSON）
来源：http://liy.vqdsnc.cn

Py:   pickle.dumps(obj)
来源：http://sef.tarul.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bfc.nanxinkj.top

JS:   v8.serialize(obj)        // Node
来源：http://ach.yangfankeji.com

TS:   v8.serialize(obj)        // Node
来源：http://mhg.cqqwz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pho.vehdjk.com

Go:   encoding/gob
来源：http://fvy.tarul.cn

Ruby: Marshal.dump(obj)
来源：http://lry.hcnkem.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vuw.aibaodan.cn

================================================================================
来源：http://laf.ywan-chungtsiang.top

L. 网络请求
来源：http://spr.zhijiandao.cn

================================================================================
来源：http://jvz.sufxvd.cn

[L01] 发送 GET 请求
来源：http://wmd.shangyingyoupin.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tsf.tianlin.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rpe.jinqigfzy.top

JS:   await fetch(url)
来源：http://vkx.yj202588.top

TS:   await fetch(url)
来源：http://msp.9152youxi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sfx.gotoacloud.top

Go:   resp, err := http.Get(url)
来源：http://lsq.ywan-chungtsiang.top

Ruby: Net::HTTP.get(URI(url))
来源：http://eyj.kuanghao11.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oru.pengpengdd.cyou

[L02] 发送 POST JSON
来源：http://bwy.mhx1999.top

Py:   requests.post(url, json={"a": 1})
来源：http://ulj.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zbi.hcnkem.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mas.svipenyu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vbi.sufxvd.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lcf.meibo888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dfo.xinyue.icu

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uxl.nanxinkj.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hay.xinyue.icu

[L03] 设置自定义请求头
来源：http://nik.jqgfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kvq.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qah.tianlin.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xny.nanxinkj.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uzj.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ajd.ywan-chungtsiang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sgi.smart0.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lkc.wangdashe.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://giw.meibo888.top

[L04] 设置超时
来源：http://kri.ywan-chungtsiang.top

Py:   requests.get(url, timeout=5)
来源：http://pyg.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vsm.ywan-chungtsiang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qyt.jianghu66.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://twq.zhixingplan.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kkz.nwbrower.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xgg.fktsv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wep.sysykeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mjp.hnqzz.top

[L05] 上传文件（multipart）
来源：http://doe.jqgufenzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bri.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ctf.sweek.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yea.bjfxy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://aks.shzxlz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dyt.pengpengdd.cyou

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nep.wangshuangyany.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://upv.pengpengdd.cyou

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uzb.jyoumei.cn

[L06] 解析响应为 JSON
来源：http://gst.wangdashe.top

Py:   resp.json()
来源：http://uqr.zhixingplan.top

PHP:  json_decode($body, true);
来源：http://gzg.meibo888.top

JS:   await resp.json()
来源：http://fvb.nanxuanxn.top

TS:   await resp.json()
来源：http://mzs.hcnkem.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kcg.bbcook.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://emw.yonumen.top

Ruby: JSON.parse(resp.body)
来源：http://nct.jqgfzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tmy.bjfxy.top

[L07] 处理 HTTP 状态码
来源：http://wnn.jianghu66.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://buf.birdmap.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mho.chenzaomai.com

JS:   resp.ok;  resp.status
来源：http://ofo.jlsjyb.cn

TS:   resp.ok;  resp.status
来源：http://rwg.bbcook.cn

Java: resp.statusCode()
来源：http://xvp.fktsv.cn

Go:   resp.StatusCode
来源：http://wbm.zdbjq.cn

Ruby: resp.code.to_i
来源：http://nmn.ctjpmb.com

C#:   (int)resp.StatusCode
来源：http://fbv.aibaodan.cn

[L08] 并发请求多个地址
来源：http://vai.jinyuanbaomall.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zfh.hammf.cn

PHP:  curl_multi_init() 系列
来源：http://olg.hfpthk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ktb.sxryk.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ocu.cucudq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dya.zhengqikj.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pmr.ppjwa.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cmv.jqgufenzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xhs.bjfxy.top

================================================================================
来源：http://qow.shzxlz.cn

M. 命令行 / 进程 / 环境
来源：http://esw.gotoacloud.top

================================================================================
来源：http://hfg.jinqigfzy.top

[M01] 读取命令行参数
来源：http://ldp.xziqi.cn

Py:   sys.argv[1:]
来源：http://svx.jinqigufen.top

PHP:  $argv;  $argc;
来源：http://han.jinqigfzy.top

JS:   process.argv.slice(2)
来源：http://mvs.shzxlz.cn

TS:   process.argv.slice(2)
来源：http://uhh.zhengqikj.top

Java: args 数组（main 方法参数）
来源：http://afh.svipenyu.cn

Go:   os.Args[1:]
来源：http://ojn.sufxvd.cn

Ruby: ARGV
来源：http://hbq.yj20258.top

C#:   args 数组（Main 方法参数）
来源：http://zjs.gogol.net.cn

[M02] 读取环境变量
来源：http://bbx.birdmap.top

Py:   os.environ.get("HOME")
来源：http://czn.zdbjq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hpd.tianlin.xyz

JS:   process.env.HOME
来源：http://zek.jqgufenzy.top

TS:   process.env.HOME
来源：http://zyd.hongshengwenyu.top

Java: System.getenv("HOME")
来源：http://oba.yueranfly.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qse.zhengqikj.top

Ruby: ENV["HOME"]
来源：http://ykg.jinyuanbaomall.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xfa.nanxinkj.top

[M03] 执行外部命令
来源：http://ryj.nwbrower.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://msf.wangshuangyany.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mie.jlsjyb.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zvk.9152youxi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cmz.shanyushiyangtech.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://how.yangfankeji.com

Go:   exec.Command("ls", "-l").Output()
来源：http://bwo.fanxiaobao.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://olt.gogol.net.cn

C#:   Process.Start("ls", "-l");
来源：http://vsl.cdnleiting.top

[M04] 获取当前工作目录
来源：http://lkk.kuanghao11.cn

Py:   os.getcwd()
来源：http://vme.guannengcc.top

PHP:  getcwd();
来源：http://gud.tianlin.xyz

JS:   process.cwd()
来源：http://rys.iojbl.cn

TS:   process.cwd()
来源：http://syr.zhijiandao.cn

Java: Path.of("").toAbsolutePath()
来源：http://anj.shanyushiyangkeji.top

Go:   os.Getwd()
来源：http://smp.uphjek.com

Ruby: Dir.pwd
来源：http://vqr.cucudq.cn

C#:   Directory.GetCurrentDirectory()
来源：http://feq.9152youxi.cn

[M05] 设置退出码
来源：http://jjq.kuanghao11.cn

Py:   sys.exit(1)
来源：http://tgw.daria6918.cn

PHP:  exit(1);
来源：http://xly.jianghu66.top

JS:   process.exit(1)
来源：http://nww.9152youxi.cn

TS:   process.exit(1)
来源：http://cdn.jianghu66.top

Java: System.exit(1)
来源：http://dey.jyoumei.cn

Go:   os.Exit(1)
来源：http://eww.zdbjq.cn

Ruby: exit 1
来源：http://zvy.fengsongda.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wrb.sjlbkw.cn

[M06] 向标准错误输出
来源：http://fvt.havefunace.top

Py:   print("err", file=sys.stderr)
来源：http://boh.xuetiantiany.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qnx.xingfuxueyuan.xyz

JS:   console.error("err")
来源：http://cgk.meibo888.top

TS:   console.error("err")
来源：http://hct.cdnleiting.top

Java: System.err.println("err")
来源：http://pxo.52xcode.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://irv.wangdashe.top

Ruby: warn "err"
来源：http://oli.quarkkingdee.top

C#:   Console.Error.WriteLine("err")
来源：http://mty.c1oappe.top

[M07] 判断是否为主入口
来源：http://hyn.cdnleiting.top

Py:   if __name__ == "__main__":
来源：http://rfc.tanke756.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cpw.cdnleiting.top

JS:   require.main === module
来源：http://ify.ywan-chungtsiang.top

TS:   require.main === module
来源：http://pja.wangdashe.top

Java: public static void main(String[] args)
来源：http://ltg.haohaochexian.top

Go:   func main()
来源：http://bau.haohaochexian.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pps.yj20258888.top

C#:   static void Main(string[] args)
来源：http://lrv.chenjidiqi.icu

[M08] 获取系统与运行时信息
来源：http://wdd.gogol.net.cn

Py:   platform.system();  platform.python_version()
来源：http://blw.daxiang520.top

PHP:  PHP_OS;  phpversion();
来源：http://ged.hammf.cn

JS:   process.platform;  process.version
来源：http://fdy.feifeiyinyue.top

TS:   process.platform;  process.version
来源：http://rqp.sufxvd.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cne.mhx1999.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ple.yj20258888.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://you.jqgfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://tfr.ctjpmb.com

================================================================================
来源：http://cek.ivvv.top

N. 数据结构与算法
来源：http://rft.gzhubu.top

================================================================================
来源：http://lrp.xinyue.icu

[N01] 二分查找（有序数组）
来源：http://jku.ybcxt.top

Py:   bisect.bisect_left(arr, x)
来源：http://cba.mhx1999.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://giv.ivvv.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vmr.9152youxi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xrz.hywenlv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ska.shangyingyoupin.top

Go:   sort.SearchInts(arr, x)
来源：http://rjc.yj202588.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://kky.xingfuxueyuan.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://noy.dashuyun.cn

[N02] 排序（工程实践用内置实现）
来源：http://wjl.yangfankeji.com

Py:   sorted(arr);  arr.sort()
来源：http://txs.hnqzz.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cub.ybcxt.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xxt.sxryk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tyz.ybcxt.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rdt.redwolf501.top

Go:   slices.Sort(arr)
来源：http://ijq.nwbrower.top

Ruby: arr.sort
来源：http://doq.wangshuangyany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ptb.cucudq.cn

[N03] 快速排序（分治示例）
来源：http://aoq.xuetiantiany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zdq.316326.xyz

PHP:  // 递归实现，或用 usort
来源：http://lwu.hnqzz.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jje.zhijiandao.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vpd.hysaishi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cye.jinqigufen.top


<!-- 参考信息 -->
代发 wailian999

Py:   (end - start).total_seconds()
来源：http://vec.52xcode.cn

PHP:  $end->diff($start)->days;
来源：http://zcn.hnqzz.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vna.vehdjk.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bnn.tanke756.top

Java: Duration.between(start, end).toSeconds()
来源：http://jor.shuidangran.top

Go:   end.Sub(start).Hours()
来源：http://qkb.cheryme.top

Ruby: end - start                 # 返回秒数
来源：http://oge.svipenyu.cn

C#:   (end - start).TotalSeconds
来源：http://cgh.zhengqikj.top

[J07] 比较两个日期
来源：http://wcc.yangfankeji.com

Py:   d1 < d2;  d1 == d2
来源：http://plm.tian-w.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dds.hongshengwenyu.top

JS:   d1.getTime() < d2.getTime()
来源：http://iqe.xylfe.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rhe.dianchejie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://evs.ehwqpu.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yrl.jyoumei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zab.yangfankeji.com

C#:   d1 < d2;  d1 == d2
来源：http://bfh.wangdashe.top

[J08] 提取年月日与星期
来源：http://oni.jlsjyb.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xxr.xziqi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://krq.zhijiandao.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://clx.ydzc1.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zsk.pycfn.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lro.xziqi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dbf.yj202588.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dnh.vehdjk.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yzs.xziqi.cn

[J09] 时区处理
来源：http://reb.yj20258888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xbm.jyoumei.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://suh.yfazqb.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fwe.zhijiandao.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qnv.wangshuangyany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qrm.ywan-chungtsiang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gdg.sjlbkw.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hyi.ctjpmb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jrj.cashguo.top

[J10] 取今天 / 本月第一天
来源：http://ebs.cheryme.top

Py:   date.today();  date.today().replace(day=1)
来源：http://lty.jyoumei.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qgr.hammf.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sbu.yvedp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ucz.cashguo.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://alz.yanxiufei.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wtv.wangshuangyany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pss.yangfankeji.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eqb.hfpthk.cn

================================================================================
来源：http://poe.daxiang520.top

K. JSON 与序列化
来源：http://bbf.daxiang520.top

================================================================================
来源：http://mid.dashuyun.cn

[K01] 对象转 JSON 字符串
来源：http://bzg.wangshuangyany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zaa.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qqh.shanyushiyangtech.top

JS:   JSON.stringify(obj)
来源：http://eap.chenlongwang.top

TS:   JSON.stringify(obj)
来源：http://sni.tanke756.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fzr.dashuyun.cn

Go:   json.Marshal(obj)
来源：http://msb.xinyue.icu

Ruby: obj.to_json                                     // require "json"
来源：http://crv.birdmap.top

C#:   JsonSerializer.Serialize(obj)
来源：http://mxr.zycfv.cn

[K02] JSON 字符串转对象
来源：http://lbx.hesvh.cn

Py:   json.loads(s)
来源：http://ney.jqgufenzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uws.shanyushiyangkeji.top

JS:   JSON.parse(s)
来源：http://dvb.jqgfzy.top

TS:   JSON.parse(s)
来源：http://qyu.dashuyun.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tgs.bbcook.cn

Go:   json.Unmarshal(data, &v)
来源：http://nyp.aizwys.cn

Ruby: JSON.parse(s)
来源：http://wox.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sye.shanyushiyangtech.top

[K03] JSON 美化输出（带缩进）
来源：http://mvb.hcnkem.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://poj.daxiang520.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rpf.jinghuilouyu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lrs.yuanzhike.top

TS:   JSON.stringify(obj, null, 2)
来源：http://asb.cheryme.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bda.zhaomingkeji.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vrl.andypj.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://wtb.guannengcc.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vjz.wangdashe.top

[K04] 读取 JSON 文件
来源：http://cfw.bjfxy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uoj.uphjek.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fel.316326.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://anw.cdnleiting.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rwv.shanyushiyangtech.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lkr.52xcode.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dtc.zhijiandao.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wiy.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ocl.jyoumei.cn

[K05] 深拷贝对象
来源：http://swy.gotoacloud.top

Py:   copy.deepcopy(obj)
来源：http://ajg.cdnleiting.top

PHP:  unserialize(serialize($obj));
来源：http://fzo.epnwcf.com

JS:   structuredClone(obj)
来源：http://ubi.shangyingyoupin.top

TS:   structuredClone(obj)
来源：http://ajg.hywenlv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rta.ehwqpu.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dto.epnwcf.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qiw.cdnleiting.top

C#:   // 序列化往返，或自定义 Clone
来源：http://uzz.fktsv.cn

[K06] 解析 URL 查询串
来源：http://oux.svipenyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iur.shzxlz.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wvz.sweek.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://loe.ydjk.org.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oei.yj20258.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vil.mhx1999.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ukl.yangfankeji.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tto.cqqwz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xmp.xylfe.cn

[K07] 进制转换
来源：http://pml.zhengqikj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://klk.jlsjyb.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://crk.fehbvm.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wcu.zhiwuduotai.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://suu.52xcode.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ojs.gaohongyu789.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pwc.hongshengwenyu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gjj.cheryme.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wwq.jiagoushi.top

[K08] 二进制序列化（非 JSON）
来源：http://fee.chenjidiqi.icu

Py:   pickle.dumps(obj)
来源：http://znq.kuanghao11.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tcl.hfpthk.cn

JS:   v8.serialize(obj)        // Node
来源：http://azm.hysaishi.cn

TS:   v8.serialize(obj)        // Node
来源：http://hmg.redwolf501.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cgy.vqdsnc.cn

Go:   encoding/gob
来源：http://jvg.shuidangran.top

Ruby: Marshal.dump(obj)
来源：http://zfk.jlsjyb.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xqi.chenlongwang.top

================================================================================
来源：http://jkl.yueranfly.top

L. 网络请求
来源：http://fnv.zycfv.cn

================================================================================
来源：http://bhb.c1oappe.top

[L01] 发送 GET 请求
来源：http://pqy.dianchejie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nyc.epnwcf.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bax.chenjidiqi.icu

JS:   await fetch(url)
来源：http://fdv.gotoacloud.top

TS:   await fetch(url)
来源：http://hve.xinyue.icu

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mjo.jinyuanbaomall.cn

Go:   resp, err := http.Get(url)
来源：http://hiv.ehwqpu.com

Ruby: Net::HTTP.get(URI(url))
来源：http://uip.jianghu66.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ctd.yongpay.top

[L02] 发送 POST JSON
来源：http://esy.hesvh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dze.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tcv.dianchejie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vlh.jinqigfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zgx.yanxiufei.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oaz.zhengqikj.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zjz.jyoumei.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qbx.gaohongyu789.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ias.jqgfzy.top

[L03] 设置自定义请求头
来源：http://izg.fzhhl.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://roq.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dgq.yongpay.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hid.hesvh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xnp.yuxming.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gym.vehdjk.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yge.feifeiyinyue.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wgu.xingfuxueyuan.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qfz.ppjwa.cn

[L04] 设置超时
来源：http://zxc.sjlbkw.cn

Py:   requests.get(url, timeout=5)
来源：http://ino.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qpj.yangfankeji.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dug.pengpengdd.cyou

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://twj.cqqwz.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qik.gzhubu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://laq.jqgfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bfe.bbcook.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eih.shuidangran.top

[L05] 上传文件（multipart）
来源：http://hjs.pycfn.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://aqd.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sop.tian-w.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dta.daxiang520.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ppi.ydjk.org.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qff.dashuyun.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pjy.yonumen.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xxb.smart0.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ddi.316326.xyz

[L06] 解析响应为 JSON
来源：http://wpk.jinyuanbaomall.cn

Py:   resp.json()
来源：http://zuc.ehwqpu.com

PHP:  json_decode($body, true);
来源：http://fvz.zhaomingkeji.xyz

JS:   await resp.json()
来源：http://zrr.yuxming.cn

TS:   await resp.json()
来源：http://uzc.zycfv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iit.kuanghao11.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mdv.redwolf501.top

Ruby: JSON.parse(resp.body)
来源：http://gza.zhijiandao.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://flp.hongshengwenyu.top

[L07] 处理 HTTP 状态码
来源：http://sdu.sysykeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gkr.hesvh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dup.birdmap.top

JS:   resp.ok;  resp.status
来源：http://lte.shangyingyoupin.top

TS:   resp.ok;  resp.status
来源：http://qai.hnxiangtu.top

Java: resp.statusCode()
来源：http://nae.zhixingplan.top

Go:   resp.StatusCode
来源：http://ovh.zhiwuduotai.top

Ruby: resp.code.to_i
来源：http://mfd.ivvv.top

C#:   (int)resp.StatusCode
来源：http://ujq.kuanghao11.cn

[L08] 并发请求多个地址
来源：http://gqv.zhongyouzk.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zbb.yongpay.top

PHP:  curl_multi_init() 系列
来源：http://viw.yongpay.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://owu.pycfn.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wqs.sysykeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qgy.yongpay.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pqg.birdmap.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nyt.guowangkeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vpr.jinqigufen.top

================================================================================
来源：http://hsb.quarkkingdee.top

M. 命令行 / 进程 / 环境
来源：http://try.zdqjudy.top

================================================================================
来源：http://eej.yangfankeji.com

[M01] 读取命令行参数
来源：http://zsj.ppjwa.cn

Py:   sys.argv[1:]
来源：http://phf.havefunace.top

PHP:  $argv;  $argc;
来源：http://fue.guowangkeji.top

JS:   process.argv.slice(2)
来源：http://qbl.jqgufenzy.top

TS:   process.argv.slice(2)
来源：http://qnx.snrcjt.cn

Java: args 数组（main 方法参数）
来源：http://bkm.hnqzz.top

Go:   os.Args[1:]
来源：http://gkr.daria6918.cn

Ruby: ARGV
来源：http://pjr.hammf.cn

C#:   args 数组（Main 方法参数）
来源：http://unr.epnwcf.com

[M02] 读取环境变量
来源：http://ocb.fanxiaobao.xyz

Py:   os.environ.get("HOME")
来源：http://ucs.sxryk.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jvn.cheryme.top

JS:   process.env.HOME
来源：http://ubk.ybcxt.top

TS:   process.env.HOME
来源：http://zll.zdqjudy.top

Java: System.getenv("HOME")
来源：http://nnw.9152youxi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mya.quarkkingdee.top

Ruby: ENV["HOME"]
来源：http://zqt.hongshengwenyu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hwb.fengsongda.top

[M03] 执行外部命令
来源：http://wze.chenlongwang.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tnr.guannengcc.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hlw.jqgufenzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://tur.ppjwa.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xrb.sxryk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ciy.nwbrower.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jbj.wangshuangyany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hkl.aizwys.cn

C#:   Process.Start("ls", "-l");
来源：http://xxb.xingfuxueyuan.xyz

[M04] 获取当前工作目录
来源：http://azx.vqdsnc.cn

Py:   os.getcwd()
来源：http://eia.yongpay.top

PHP:  getcwd();
来源：http://don.tianlin.xyz

JS:   process.cwd()
来源：http://xop.zhoulong.xyz

TS:   process.cwd()
来源：http://ftj.shzxlz.cn

Java: Path.of("").toAbsolutePath()
来源：http://tja.nanxuanxn.top

Go:   os.Getwd()
来源：http://ron.gogol.net.cn

Ruby: Dir.pwd
来源：http://cjj.yueranfly.top

C#:   Directory.GetCurrentDirectory()
来源：http://ogz.9152youxi.cn

[M05] 设置退出码
来源：http://esf.iojbl.cn

Py:   sys.exit(1)
来源：http://aox.hywenlv.cn

PHP:  exit(1);
来源：http://nxz.kuanghao11.cn

JS:   process.exit(1)
来源：http://uhx.ybcxt.top

TS:   process.exit(1)
来源：http://sgn.fehbvm.com

Java: System.exit(1)
来源：http://irv.zhongyouzk.top

Go:   os.Exit(1)
来源：http://mfv.nwbrower.top

Ruby: exit 1
来源：http://umm.yj20258.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iph.zhijiandao.cn

[M06] 向标准错误输出
来源：http://vuv.fengsongda.top

Py:   print("err", file=sys.stderr)
来源：http://lvp.gogol.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mxd.sufxvd.cn

JS:   console.error("err")
来源：http://hlr.cqqwz.cn

TS:   console.error("err")
来源：http://ezu.quarkkingdee.top

Java: System.err.println("err")
来源：http://txs.uphjek.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jzb.jiagoushi.top

Ruby: warn "err"
来源：http://kzl.hfpthk.cn

C#:   Console.Error.WriteLine("err")
来源：http://psh.pycfn.com

[M07] 判断是否为主入口
来源：http://scm.redwolf501.top

Py:   if __name__ == "__main__":
来源：http://hds.chenzaomai.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rqf.tanke756.top

JS:   require.main === module
来源：http://zeh.yj202588.top

TS:   require.main === module
来源：http://idm.yuanzhike.top

Java: public static void main(String[] args)
来源：http://otl.xuanzx.com

Go:   func main()
来源：http://fbr.guowangkeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pdq.yj202588.top

C#:   static void Main(string[] args)
来源：http://zot.redwolf501.top

[M08] 获取系统与运行时信息
来源：http://vlw.yongpay.top

Py:   platform.system();  platform.python_version()
来源：http://zpz.sweek.top

PHP:  PHP_OS;  phpversion();
来源：http://rza.gzhubu.top

JS:   process.platform;  process.version
来源：http://ndf.ppjwa.cn

TS:   process.platform;  process.version
来源：http://rys.gogol.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ugx.haohaochexian.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mxu.svipenyu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vjg.tianlin.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://hkf.hnxiangtu.top

================================================================================
来源：http://day.tian-w.cn

N. 数据结构与算法
来源：http://oug.meibo888.top

================================================================================
来源：http://vdq.bjfxy.top

[N01] 二分查找（有序数组）
来源：http://gab.yj20258888.top

Py:   bisect.bisect_left(arr, x)
来源：http://aqu.guannengcc.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dhz.nanxinkj.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tzb.sweek.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xtj.zhiwuduotai.top

Java: Arrays.binarySearch(arr, x)
来源：http://fgz.ydzc1.top

Go:   sort.SearchInts(arr, x)
来源：http://xvr.yuxming.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://aoq.ehwqpu.com

C#:   Array.BinarySearch(arr, x)
来源：http://dzl.c1oappe.top

[N02] 排序（工程实践用内置实现）
来源：http://vmv.cheryme.top

Py:   sorted(arr);  arr.sort()
来源：http://czl.gzhubu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mhl.zycfv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sdv.haohaochexian.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ocv.fengsongda.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mrk.zhiwuduotai.top

Go:   slices.Sort(arr)
来源：http://bku.wangshuangyany.cn

Ruby: arr.sort
来源：http://erq.aizwys.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wsc.bbcook.cn

[N03] 快速排序（分治示例）
来源：http://rgx.dianchejie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nna.ppjwa.cn

PHP:  // 递归实现，或用 usort
来源：http://pok.smart0.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rry.zhoulong.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aqn.havefunace.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yys.zdqjudy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://txj.xuanzx.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fjc.zdqjudy.top

C#:   // 手写递归，或 Array.Sort
来源：http://fxr.yfazqb.com

[N04] 斐波那契数列
来源：http://vqv.zhixingplan.top


<!-- 参考信息 -->
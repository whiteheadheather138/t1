代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://pvm.yonumen.top

Go:   end.Sub(start).Hours()
来源：http://dgm.nanxuanxn.top

Ruby: end - start                 # 返回秒数
来源：http://tkf.redwolf501.top

C#:   (end - start).TotalSeconds
来源：http://aph.epnwcf.com

[J07] 比较两个日期
来源：http://lrp.guowangkeji.top

Py:   d1 < d2;  d1 == d2
来源：http://ion.xinyue.icu

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xcc.aizwys.cn

JS:   d1.getTime() < d2.getTime()
来源：http://iei.yvedp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kgw.zhengqikj.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rbv.guannengcc.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zcn.aizwys.cn

Ruby: d1 < d2;  d1 == d2
来源：http://eop.svipenyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://mxp.nanxinkj.top

[J08] 提取年月日与星期
来源：http://lvg.jinghuilouyu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qki.fanxiaobao.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qgn.xuanzx.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lki.nanxuanxn.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ico.jqgfzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gjl.fengsongda.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tqf.redwolf501.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pgg.fanxiaobao.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kaw.0kj1m.cn

[J09] 时区处理
来源：http://fpj.kuanghao11.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://oot.jinyuanbaomall.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://snu.yanxiufei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://otp.c1oappe.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nxx.guannengcc.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zce.havefunace.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://axa.jlsjyb.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cjp.feifeiyinyue.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xec.uphjek.com

[J10] 取今天 / 本月第一天
来源：http://mhw.iojbl.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pcx.snrcjt.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vba.yj202588.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wml.hnqzz.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hpi.nanxuanxn.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bcm.yj20258888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ltw.nanxuanxn.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://iah.dashuyun.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bro.gotoacloud.top

================================================================================
来源：http://mwh.zhaomingkeji.xyz

K. JSON 与序列化
来源：http://zau.meibo888.top

================================================================================
来源：http://fjd.kuanghao11.cn

[K01] 对象转 JSON 字符串
来源：http://xug.haohaochexian.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oul.hongshengwenyu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hsi.zhijiandao.cn

JS:   JSON.stringify(obj)
来源：http://fry.cdnleiting.top

TS:   JSON.stringify(obj)
来源：http://bsp.hnqzz.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://apk.jinghuilouyu.cn

Go:   json.Marshal(obj)
来源：http://syk.cdnleiting.top

Ruby: obj.to_json                                     // require "json"
来源：http://qtn.dianchejie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pkt.yonumen.top

[K02] JSON 字符串转对象
来源：http://xcg.yuxming.cn

Py:   json.loads(s)
来源：http://ltw.xziqi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qcb.smart0.xyz

JS:   JSON.parse(s)
来源：http://fcj.hywenlv.cn

TS:   JSON.parse(s)
来源：http://hen.jinghuilouyu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bew.jqgufenzy.top

Go:   json.Unmarshal(data, &v)
来源：http://afk.xuanzx.com

Ruby: JSON.parse(s)
来源：http://zsl.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ukg.shanyushiyangtech.top

[K03] JSON 美化输出（带缩进）
来源：http://wdc.hysaishi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nko.ppjwa.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://soo.hnqzz.top

JS:   JSON.stringify(obj, null, 2)
来源：http://nxz.ydzc1.top

TS:   JSON.stringify(obj, null, 2)
来源：http://sze.fktsv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://prr.yj20258.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://noy.zhaomingkeji.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://bxj.yueranfly.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://njq.ywan-chungtsiang.top

[K04] 读取 JSON 文件
来源：http://wkq.guowangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lhn.zdqjudy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wom.yfazqb.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mpe.jyoumei.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jhx.jinghuilouyu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hfu.cqqwz.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tyc.hnxiangtu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://nnr.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ync.xziqi.cn

[K05] 深拷贝对象
来源：http://mao.guannengcc.top

Py:   copy.deepcopy(obj)
来源：http://urr.dashuyun.cn

PHP:  unserialize(serialize($obj));
来源：http://nig.cucudq.cn

JS:   structuredClone(obj)
来源：http://nys.xinyue.icu

TS:   structuredClone(obj)
来源：http://gqd.ivvv.top

Java: // 手写拷贝构造，或序列化往返
来源：http://swe.yanxiufei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pzx.xinyue.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hha.zycfv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://uxd.redwolf501.top

[K06] 解析 URL 查询串
来源：http://yrn.zycfv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://slq.redwolf501.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wjn.jianghu66.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ivp.jinqigfzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fay.daxiang520.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qbb.nwbrower.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qwc.jqgfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lom.fzhhl.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jtq.gotoacloud.top

[K07] 进制转换
来源：http://fmv.yonumen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lnb.nwbrower.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cfv.sweek.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mnb.xuetiantiany.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vlu.jinghuilouyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://avk.chenlongwang.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qea.gogol.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ppe.52xcode.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://udm.zhixingplan.top

[K08] 二进制序列化（非 JSON）
来源：http://zli.yvedp.cn

Py:   pickle.dumps(obj)
来源：http://qno.chenzaomai.com

PHP:  serialize($obj);  unserialize($s);
来源：http://mnl.gaohongyu789.top

JS:   v8.serialize(obj)        // Node
来源：http://ogb.xinyue.icu

TS:   v8.serialize(obj)        // Node
来源：http://ogx.cdnleiting.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dzd.redwolf501.top

Go:   encoding/gob
来源：http://jtl.feifeiyinyue.top

Ruby: Marshal.dump(obj)
来源：http://azh.ydzc1.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ofc.hywenlv.cn

================================================================================
来源：http://xpb.0kj1m.cn

L. 网络请求
来源：http://umn.9152youxi.cn

================================================================================
来源：http://ite.cashguo.top

[L01] 发送 GET 请求
来源：http://aoi.zdqjudy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jca.yj20258888.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qes.yangfankeji.com

JS:   await fetch(url)
来源：http://lhq.0kj1m.cn

TS:   await fetch(url)
来源：http://bum.snrcjt.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nlq.smart0.xyz

Go:   resp, err := http.Get(url)
来源：http://vjp.52xcode.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dfp.ivvv.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gee.zycfv.cn

[L02] 发送 POST JSON
来源：http://yrd.xingfuxueyuan.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://hcu.sweek.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ixm.gaohongyu789.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aoo.jinghuilouyu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ieu.zhijiandao.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sdh.vqdsnc.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dqn.gotoacloud.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dxe.epnwcf.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rgj.fanxiaobao.xyz

[L03] 设置自定义请求头
来源：http://atg.yj20258.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pie.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://led.fanxiaobao.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tcb.xuetiantiany.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oog.cucudq.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pzv.ppjwa.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nbb.zhijiandao.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qgg.chenlongwang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dex.chenlongwang.top

[L04] 设置超时
来源：http://ype.vehdjk.com

Py:   requests.get(url, timeout=5)
来源：http://xkg.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zzt.yj202588.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pcs.jlsjyb.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pmw.ydzc1.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://oir.zhongyouzk.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mhy.zhengqikj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hhm.fengsongda.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nqy.ppjwa.cn

[L05] 上传文件（multipart）
来源：http://vay.ctjpmb.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://aww.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://imv.yanxiufei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wxc.yanxiufei.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kgb.gogol.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bhz.xinyue.icu

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ggg.zhengqikj.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://spv.jiagoushi.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://znf.ppjwa.cn

[L06] 解析响应为 JSON
来源：http://czx.fzhhl.top

Py:   resp.json()
来源：http://mxi.nwbrower.top

PHP:  json_decode($body, true);
来源：http://utr.hysaishi.cn

JS:   await resp.json()
来源：http://mnm.zycfv.cn

TS:   await resp.json()
来源：http://oxn.aibaodan.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lnf.zhongyouzk.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ztg.yuxming.cn

Ruby: JSON.parse(resp.body)
来源：http://fkc.zhengqikj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yvi.jinqigfzy.top

[L07] 处理 HTTP 状态码
来源：http://amt.zhiwuduotai.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cbl.9152youxi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zny.pycfn.com

JS:   resp.ok;  resp.status
来源：http://mjz.vehdjk.com

TS:   resp.ok;  resp.status
来源：http://vbb.fengsongda.top

Java: resp.statusCode()
来源：http://ayw.birdmap.top

Go:   resp.StatusCode
来源：http://dwv.dashuyun.cn

Ruby: resp.code.to_i
来源：http://ypq.gaohongyu789.top

C#:   (int)resp.StatusCode
来源：http://sja.yanxiufei.cn

[L08] 并发请求多个地址
来源：http://qhy.tian-w.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://djb.jqgfzy.top

PHP:  curl_multi_init() 系列
来源：http://iur.chenlongwang.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iie.jlsjyb.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gsj.cashguo.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bjb.xuetiantiany.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yjo.fehbvm.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dmo.yuanzhike.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zqy.fzhhl.top

================================================================================
来源：http://vga.sweek.top

M. 命令行 / 进程 / 环境
来源：http://osj.quarkkingdee.top

================================================================================
来源：http://oum.tanke756.top

[M01] 读取命令行参数
来源：http://flx.yuxming.cn

Py:   sys.argv[1:]
来源：http://wlb.shuidangran.top

PHP:  $argv;  $argc;
来源：http://ual.yonumen.top

JS:   process.argv.slice(2)
来源：http://xnv.ywan-chungtsiang.top

TS:   process.argv.slice(2)
来源：http://voo.zhiwuduotai.top

Java: args 数组（main 方法参数）
来源：http://dma.sysykeji.top

Go:   os.Args[1:]
来源：http://ubg.jinyuanbaomall.cn

Ruby: ARGV
来源：http://lbx.fktsv.cn

C#:   args 数组（Main 方法参数）
来源：http://qox.mhx1999.top

[M02] 读取环境变量
来源：http://qpj.ppjwa.cn

Py:   os.environ.get("HOME")
来源：http://xzp.yfazqb.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qwx.zhiwuduotai.top

JS:   process.env.HOME
来源：http://wxq.hcnkem.com

TS:   process.env.HOME
来源：http://whz.zhijiandao.cn

Java: System.getenv("HOME")
来源：http://lgu.hcnkem.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://emx.xuanzx.com

Ruby: ENV["HOME"]
来源：http://vdk.gaohongyu789.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nma.zhaomingkeji.xyz

[M03] 执行外部命令
来源：http://bbv.c1oappe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qah.ydzc1.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://okh.0kj1m.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wwm.snrcjt.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nxh.sysykeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://trh.wangdashe.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ktv.wangdashe.top

Ruby: system("ls -l");  `ls -l`
来源：http://wfk.yanxiufei.cn

C#:   Process.Start("ls", "-l");
来源：http://rgv.ppjwa.cn

[M04] 获取当前工作目录
来源：http://yey.shangyingyoupin.top

Py:   os.getcwd()
来源：http://dks.guannengcc.top

PHP:  getcwd();
来源：http://nwe.mhx1999.top

JS:   process.cwd()
来源：http://fcf.ydjk.org.cn

TS:   process.cwd()
来源：http://qts.tarul.cn

Java: Path.of("").toAbsolutePath()
来源：http://oxy.zdbjq.cn

Go:   os.Getwd()
来源：http://egc.pycfn.com

Ruby: Dir.pwd
来源：http://zno.jlsjyb.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uqj.quarkkingdee.top

[M05] 设置退出码
来源：http://uvy.nanxuanxn.top

Py:   sys.exit(1)
来源：http://yrf.ctjpmb.com

PHP:  exit(1);
来源：http://pdw.zhiwuduotai.top

JS:   process.exit(1)
来源：http://kkd.daria6918.cn

TS:   process.exit(1)
来源：http://zov.nanxuanxn.top

Java: System.exit(1)
来源：http://mpa.gzhubu.top

Go:   os.Exit(1)
来源：http://chg.yuanzhike.top

Ruby: exit 1
来源：http://kbx.sweek.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jur.zhongyouzk.top

[M06] 向标准错误输出
来源：http://skw.hnqzz.top

Py:   print("err", file=sys.stderr)
来源：http://xqy.birdmap.top

PHP:  fwrite(STDERR, "err\n");
来源：http://rqu.sxryk.cn

JS:   console.error("err")
来源：http://pjz.zdbjq.cn

TS:   console.error("err")
来源：http://lwh.wangdashe.top

Java: System.err.println("err")
来源：http://kpw.xinyue.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kxm.jinghuilouyu.cn

Ruby: warn "err"
来源：http://ucj.chenjidiqi.icu

C#:   Console.Error.WriteLine("err")
来源：http://udm.tian-w.cn

[M07] 判断是否为主入口
来源：http://fwx.hnqzz.top

Py:   if __name__ == "__main__":
来源：http://dil.vqdsnc.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://shm.guowangkeji.top

JS:   require.main === module
来源：http://tae.quarkkingdee.top

TS:   require.main === module
来源：http://lfe.andypj.xyz

Java: public static void main(String[] args)
来源：http://uwi.epnwcf.com

Go:   func main()
来源：http://lxz.shzxlz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xvt.vqdsnc.cn

C#:   static void Main(string[] args)
来源：http://jck.aibaodan.cn

[M08] 获取系统与运行时信息
来源：http://qtt.bjfxy.top

Py:   platform.system();  platform.python_version()
来源：http://lje.zhixingplan.top

PHP:  PHP_OS;  phpversion();
来源：http://rjk.yongpay.top

JS:   process.platform;  process.version
来源：http://qah.zhaomingkeji.xyz

TS:   process.platform;  process.version
来源：http://ppu.dianchejie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qxn.jiagoushi.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wah.feifeiyinyue.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dpo.gogol.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gvu.jinghuilouyu.cn

================================================================================
来源：http://bmx.vehdjk.com

N. 数据结构与算法
来源：http://lhf.dianchejie.cn

================================================================================
来源：http://jgb.zhongyouzk.top

[N01] 二分查找（有序数组）
来源：http://mub.yj202588.top

Py:   bisect.bisect_left(arr, x)
来源：http://fov.shuidangran.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fnh.andypj.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lkm.xylfe.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xxh.jlsjyb.cn

Java: Arrays.binarySearch(arr, x)
来源：http://srz.tian-w.cn

Go:   sort.SearchInts(arr, x)
来源：http://bmb.sysykeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ilw.bbcook.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rwm.fengsongda.top

[N02] 排序（工程实践用内置实现）
来源：http://tuv.hnxiangtu.top

Py:   sorted(arr);  arr.sort()
来源：http://tvw.andypj.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ryj.gzhubu.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://frz.ydjk.org.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pki.hysaishi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qeg.yvedp.cn

Go:   slices.Sort(arr)
来源：http://nmu.hysaishi.cn

Ruby: arr.sort
来源：http://klp.wangshuangyany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gur.bjfxy.top

[N03] 快速排序（分治示例）
来源：http://vgc.wangdashe.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nss.iojbl.cn

PHP:  // 递归实现，或用 usort
来源：http://edn.cdnleiting.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rro.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ziz.nwbrower.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ufv.xinyue.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zcv.wangshuangyany.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sqo.birdmap.top

C#:   // 手写递归，或 Array.Sort
来源：http://ljz.gaohongyu789.top

[N04] 斐波那契数列
来源：http://fuh.sxryk.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://epu.shanyushiyangtech.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ofj.snrcjt.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lwd.jlsjyb.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qke.yj20258.top


<!-- 参考信息 -->
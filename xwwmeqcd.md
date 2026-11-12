代发 wailian999

[J07] 比较两个日期
来源：http://zit.vehdjk.com

Py:   d1 < d2;  d1 == d2
来源：http://yen.shzxlz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wlc.pengpengdd.cyou

JS:   d1.getTime() < d2.getTime()
来源：http://xua.bbcook.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bkq.snrcjt.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xax.xylfe.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ajv.daxiang520.top

Ruby: d1 < d2;  d1 == d2
来源：http://elc.zhengqikj.top

C#:   d1 < d2;  d1 == d2
来源：http://szv.dianchejie.cn

[J08] 提取年月日与星期
来源：http://ttr.fktsv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zvk.hywenlv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ols.snrcjt.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dyi.chenlongwang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dlk.nanxinkj.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xsu.316326.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://huj.fehbvm.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tiy.jyoumei.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cna.c1oappe.top

[J09] 时区处理
来源：http://ssw.yangfankeji.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xmd.jinyuanbaomall.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zks.svipenyu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mtt.fengsongda.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bdh.316326.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rfs.jinqigfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jns.316326.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://ioi.aizwys.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cjp.gzhubu.top

[J10] 取今天 / 本月第一天
来源：http://vbu.dianchejie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hbi.zycfv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dic.jinghuilouyu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fsh.xziqi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jrm.sufxvd.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ntx.bjfxy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ezp.0kj1m.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pxt.fehbvm.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pwn.jianghu66.top

================================================================================
来源：http://myg.cucudq.cn

K. JSON 与序列化
来源：http://wxt.pycfn.com

================================================================================
来源：http://vbv.c1oappe.top

[K01] 对象转 JSON 字符串
来源：http://ncj.daxiang520.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://heg.aizwys.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hrh.fanxiaobao.xyz

JS:   JSON.stringify(obj)
来源：http://yky.svipenyu.cn

TS:   JSON.stringify(obj)
来源：http://ijj.epnwcf.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fjd.hysaishi.cn

Go:   json.Marshal(obj)
来源：http://uui.fengsongda.top

Ruby: obj.to_json                                     // require "json"
来源：http://qrz.aizwys.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lwv.yj20258.top

[K02] JSON 字符串转对象
来源：http://glm.cdnleiting.top

Py:   json.loads(s)
来源：http://tnd.nanxuanxn.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://syf.hammf.cn

JS:   JSON.parse(s)
来源：http://kqr.yj20258888.top

TS:   JSON.parse(s)
来源：http://xvt.shuidangran.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ums.yj202588.top

Go:   json.Unmarshal(data, &v)
来源：http://otv.chenlongwang.top

Ruby: JSON.parse(s)
来源：http://dmc.daxiang520.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nrs.yj20258.top

[K03] JSON 美化输出（带缩进）
来源：http://zav.gogol.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dbm.yfazqb.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qpn.mhx1999.top

JS:   JSON.stringify(obj, null, 2)
来源：http://byz.yvedp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zdg.haohaochexian.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fdh.yangfankeji.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zqi.cheryme.top

Ruby: JSON.pretty_generate(obj)
来源：http://byw.ybcxt.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lhh.ctjpmb.com

[K04] 读取 JSON 文件
来源：http://eqx.quarkkingdee.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://aov.fzhhl.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bzp.hcnkem.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rms.vqdsnc.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://icd.cashguo.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rkn.jianghu66.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qew.ctjpmb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://urs.svipenyu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tsu.chenlongwang.top

[K05] 深拷贝对象
来源：http://jys.kuanghao11.cn

Py:   copy.deepcopy(obj)
来源：http://isd.sxryk.cn

PHP:  unserialize(serialize($obj));
来源：http://veo.sweek.top

JS:   structuredClone(obj)
来源：http://oaa.zhixingplan.top

TS:   structuredClone(obj)
来源：http://zwm.hesvh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gap.guowangkeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ujs.yj20258888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pbj.fengsongda.top

C#:   // 序列化往返，或自定义 Clone
来源：http://oxx.guowangkeji.top

[K06] 解析 URL 查询串
来源：http://yul.andypj.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rgr.fktsv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tij.cqqwz.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cor.zhixingplan.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lsk.zycfv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dow.birdmap.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://oqk.shangyingyoupin.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://duv.hysaishi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kqq.jqgufenzy.top

[K07] 进制转换
来源：http://hqv.ywan-chungtsiang.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bdg.nwbrower.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xlu.c1oappe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yrj.ydzc1.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gek.zhongyouzk.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cvi.snrcjt.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://saf.shuidangran.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ahg.hcnkem.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pyj.andypj.xyz

[K08] 二进制序列化（非 JSON）
来源：http://bxa.svipenyu.cn

Py:   pickle.dumps(obj)
来源：http://bxp.sweek.top

PHP:  serialize($obj);  unserialize($s);
来源：http://yew.0kj1m.cn

JS:   v8.serialize(obj)        // Node
来源：http://qwy.gaohongyu789.top

TS:   v8.serialize(obj)        // Node
来源：http://qto.bbcook.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rbj.tian-w.cn

Go:   encoding/gob
来源：http://vhr.chenlongwang.top

Ruby: Marshal.dump(obj)
来源：http://prv.zhixingplan.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ggy.wangshuangyany.cn

================================================================================
来源：http://cke.epnwcf.com

L. 网络请求
来源：http://sat.haohaochexian.top

================================================================================
来源：http://yhm.haohaochexian.top

[L01] 发送 GET 请求
来源：http://hvy.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ruz.tianlin.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yqw.gzhubu.top

JS:   await fetch(url)
来源：http://wre.jinqigfzy.top

TS:   await fetch(url)
来源：http://iap.jiagoushi.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gqj.mhx1999.top

Go:   resp, err := http.Get(url)
来源：http://ngl.xziqi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://oji.tianlin.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fsr.jlsjyb.cn

[L02] 发送 POST JSON
来源：http://gdn.nwbrower.top

Py:   requests.post(url, json={"a": 1})
来源：http://ugx.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nlc.epnwcf.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jxj.yongpay.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cri.yuanzhike.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://boi.xinyue.icu

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ead.hnqzz.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ikw.nanxuanxn.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gjj.zhoulong.xyz

[L03] 设置自定义请求头
来源：http://tog.tianlin.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://iay.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mvc.zhiwuduotai.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ryg.hammf.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zyu.wangshuangyany.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rya.vehdjk.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://aet.xinyue.icu

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dvh.svipenyu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://giq.xuetiantiany.cn

[L04] 设置超时
来源：http://wan.sysykeji.top

Py:   requests.get(url, timeout=5)
来源：http://auk.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bgb.daxiang520.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://slu.jinqigfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bhj.xingfuxueyuan.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yye.ppjwa.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dcg.kuanghao11.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bbe.cheryme.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://quq.zhengqikj.top

[L05] 上传文件（multipart）
来源：http://tmv.shangyingyoupin.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qxf.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://twd.hnxiangtu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wnx.zdbjq.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cfb.hesvh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://weq.jinqigufen.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fdm.xziqi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wqi.cheryme.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cbb.gzhubu.top

[L06] 解析响应为 JSON
来源：http://uhd.zhoulong.xyz

Py:   resp.json()
来源：http://wba.nwbrower.top

PHP:  json_decode($body, true);
来源：http://llk.nanxinkj.top

JS:   await resp.json()
来源：http://zxa.c1oappe.top

TS:   await resp.json()
来源：http://etp.yangfankeji.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://obr.tarul.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://krw.guowangkeji.top

Ruby: JSON.parse(resp.body)
来源：http://lrm.jinyuanbaomall.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nxh.shuidangran.top

[L07] 处理 HTTP 状态码
来源：http://zgc.tanke756.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yzh.bbcook.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qdw.jqgufenzy.top

JS:   resp.ok;  resp.status
来源：http://zur.jinqigfzy.top

TS:   resp.ok;  resp.status
来源：http://jwh.chenzaomai.com

Java: resp.statusCode()
来源：http://vmn.daxiang520.top

Go:   resp.StatusCode
来源：http://zog.jinqigufen.top

Ruby: resp.code.to_i
来源：http://xhc.andypj.xyz

C#:   (int)resp.StatusCode
来源：http://zrc.jinqigufen.top

[L08] 并发请求多个地址
来源：http://gud.bjfxy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xxr.shzxlz.cn

PHP:  curl_multi_init() 系列
来源：http://zis.zycfv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://npz.sjlbkw.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kst.sysykeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kvd.jinghuilouyu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pnb.yvedp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ute.xingfuxueyuan.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xrg.yuanzhike.top

================================================================================
来源：http://kwv.zhengqikj.top

M. 命令行 / 进程 / 环境
来源：http://vin.zhijiandao.cn

================================================================================
来源：http://dfe.fengsongda.top

[M01] 读取命令行参数
来源：http://gxd.yonumen.top

Py:   sys.argv[1:]
来源：http://div.hfpthk.cn

PHP:  $argv;  $argc;
来源：http://mjk.fanxiaobao.xyz

JS:   process.argv.slice(2)
来源：http://mtf.dianchejie.cn

TS:   process.argv.slice(2)
来源：http://cyh.wangdashe.top

Java: args 数组（main 方法参数）
来源：http://xxs.yj20258.top

Go:   os.Args[1:]
来源：http://ynl.yanxiufei.cn

Ruby: ARGV
来源：http://rzi.zhengqikj.top

C#:   args 数组（Main 方法参数）
来源：http://xiw.jyoumei.cn

[M02] 读取环境变量
来源：http://lsp.cheryme.top

Py:   os.environ.get("HOME")
来源：http://nsg.ywan-chungtsiang.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jvk.pengpengdd.cyou

JS:   process.env.HOME
来源：http://gji.dashuyun.cn

TS:   process.env.HOME
来源：http://yot.xylfe.cn

Java: System.getenv("HOME")
来源：http://gsv.hongshengwenyu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://clr.jlsjyb.cn

Ruby: ENV["HOME"]
来源：http://kxv.yonumen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jlf.bbcook.cn

[M03] 执行外部命令
来源：http://ibw.jyoumei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://svs.c1oappe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hum.uphjek.com

JS:   child_process.execSync("ls -l").toString()
来源：http://naj.svipenyu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hng.epnwcf.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lpg.svipenyu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pgw.zdqjudy.top

Ruby: system("ls -l");  `ls -l`
来源：http://kii.vehdjk.com

C#:   Process.Start("ls", "-l");
来源：http://inm.mhx1999.top

[M04] 获取当前工作目录
来源：http://ans.jyoumei.cn

Py:   os.getcwd()
来源：http://cmz.ydzc1.top

PHP:  getcwd();
来源：http://yap.yongpay.top

JS:   process.cwd()
来源：http://lek.bjfxy.top

TS:   process.cwd()
来源：http://xdw.zdqjudy.top

Java: Path.of("").toAbsolutePath()
来源：http://bfp.dashuyun.cn

Go:   os.Getwd()
来源：http://vhj.hnqzz.top

Ruby: Dir.pwd
来源：http://ust.jinghuilouyu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nhf.52xcode.cn

[M05] 设置退出码
来源：http://odn.zycfv.cn

Py:   sys.exit(1)
来源：http://goq.smart0.xyz

PHP:  exit(1);
来源：http://bkp.dianchejie.cn

JS:   process.exit(1)
来源：http://lie.svipenyu.cn

TS:   process.exit(1)
来源：http://bnv.yonumen.top

Java: System.exit(1)
来源：http://iif.zhixingplan.top

Go:   os.Exit(1)
来源：http://slu.meibo888.top

Ruby: exit 1
来源：http://yjf.iojbl.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mee.iojbl.cn

[M06] 向标准错误输出
来源：http://vrh.jinqigufen.top

Py:   print("err", file=sys.stderr)
来源：http://mgp.ivvv.top

PHP:  fwrite(STDERR, "err\n");
来源：http://uie.zhixingplan.top

JS:   console.error("err")
来源：http://gog.wangdashe.top

TS:   console.error("err")
来源：http://srq.yonumen.top

Java: System.err.println("err")
来源：http://rdc.aibaodan.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rdj.quarkkingdee.top

Ruby: warn "err"
来源：http://xgl.daxiang520.top

C#:   Console.Error.WriteLine("err")
来源：http://qhv.jqgufenzy.top

[M07] 判断是否为主入口
来源：http://fws.nanxinkj.top

Py:   if __name__ == "__main__":
来源：http://zsy.tian-w.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://haa.pengpengdd.cyou

JS:   require.main === module
来源：http://ptr.yfazqb.com

TS:   require.main === module
来源：http://pns.redwolf501.top

Java: public static void main(String[] args)
来源：http://pvz.0kj1m.cn

Go:   func main()
来源：http://kmr.xinyue.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tqr.jiagoushi.top

C#:   static void Main(string[] args)
来源：http://hzn.zhiwuduotai.top

[M08] 获取系统与运行时信息
来源：http://kyy.yangfankeji.com

Py:   platform.system();  platform.python_version()
来源：http://ojn.bbcook.cn

PHP:  PHP_OS;  phpversion();
来源：http://siw.jqgufenzy.top

JS:   process.platform;  process.version
来源：http://tvi.jianghu66.top

TS:   process.platform;  process.version
来源：http://ehi.daria6918.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mey.gzhubu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://jsn.yvedp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sei.cqqwz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fil.xinyue.icu

================================================================================
来源：http://tud.gotoacloud.top

N. 数据结构与算法
来源：http://uyd.tanke756.top

================================================================================
来源：http://wcc.52xcode.cn

[N01] 二分查找（有序数组）
来源：http://bgg.fzhhl.top

Py:   bisect.bisect_left(arr, x)
来源：http://ogc.hnxiangtu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xdm.pengpengdd.cyou

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jqm.hfpthk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dgf.nanxinkj.top

Java: Arrays.binarySearch(arr, x)
来源：http://nyl.ybcxt.top

Go:   sort.SearchInts(arr, x)
来源：http://vgw.sweek.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zys.yj20258.top

C#:   Array.BinarySearch(arr, x)
来源：http://xkk.pycfn.com

[N02] 排序（工程实践用内置实现）
来源：http://mjc.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://bff.ppjwa.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://avh.chenzaomai.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://jng.fzhhl.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ljd.cucudq.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nhv.chenzaomai.com

Go:   slices.Sort(arr)
来源：http://rou.jinyuanbaomall.cn

Ruby: arr.sort
来源：http://efy.zhijiandao.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zjo.vehdjk.com

[N03] 快速排序（分治示例）
来源：http://ngs.nwbrower.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ryz.cashguo.top

PHP:  // 递归实现，或用 usort
来源：http://hvk.hammf.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xop.hcnkem.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://njb.iojbl.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qcf.hcnkem.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gdl.xinyue.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hrk.cheryme.top

C#:   // 手写递归，或 Array.Sort
来源：http://lav.zhongyouzk.top

[N04] 斐波那契数列
来源：http://dbe.ydzc1.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mlb.yvedp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://enh.yuxming.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ojb.ydjk.org.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ibi.hnxiangtu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://upd.tianlin.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xux.uphjek.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qec.vqdsnc.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kib.cheryme.top


<!-- 参考信息 -->
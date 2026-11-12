代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://dpm.gzhubu.top

Go:   end.Sub(start).Hours()
来源：http://dsr.9152youxi.cn

Ruby: end - start                 # 返回秒数
来源：http://awz.hammf.cn

C#:   (end - start).TotalSeconds
来源：http://dmx.gzhubu.top

[J07] 比较两个日期
来源：http://zyw.xuetiantiany.cn

Py:   d1 < d2;  d1 == d2
来源：http://kku.birdmap.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://osc.yonumen.top

JS:   d1.getTime() < d2.getTime()
来源：http://pex.ivvv.top

TS:   d1.getTime() < d2.getTime()
来源：http://yqj.shangyingyoupin.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ssp.fktsv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dzu.hongshengwenyu.top

Ruby: d1 < d2;  d1 == d2
来源：http://qly.wangshuangyany.cn

C#:   d1 < d2;  d1 == d2
来源：http://dmt.redwolf501.top

[J08] 提取年月日与星期
来源：http://zpm.shanyushiyangtech.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pvm.iojbl.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sxk.svipenyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ori.bbcook.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://iut.ydzc1.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pll.yj202588.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://amk.sjlbkw.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fkm.tian-w.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ntp.gotoacloud.top

[J09] 时区处理
来源：http://otj.jinyuanbaomall.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xci.yanxiufei.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hkw.pengpengdd.cyou

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yst.yuxming.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://djc.52xcode.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jtk.yfazqb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bhm.sxryk.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://owh.ivvv.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rul.ehwqpu.com

[J10] 取今天 / 本月第一天
来源：http://yok.xuetiantiany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mhu.uphjek.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uua.ppjwa.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pvp.yongpay.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rik.hnxiangtu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://idc.wangshuangyany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ivz.ctjpmb.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jpt.zdqjudy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ury.zhijiandao.cn

================================================================================
来源：http://zmi.zhongyouzk.top

K. JSON 与序列化
来源：http://uow.shangyingyoupin.top

================================================================================
来源：http://qmc.jqgfzy.top

[K01] 对象转 JSON 字符串
来源：http://snd.jqgufenzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://akg.52xcode.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tsm.sjlbkw.cn

JS:   JSON.stringify(obj)
来源：http://tcx.jinqigfzy.top

TS:   JSON.stringify(obj)
来源：http://qrf.ctjpmb.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pop.ppjwa.cn

Go:   json.Marshal(obj)
来源：http://apd.hywenlv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nrt.cqqwz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hcj.9152youxi.cn

[K02] JSON 字符串转对象
来源：http://cht.hnxiangtu.top

Py:   json.loads(s)
来源：http://btv.hnxiangtu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://muv.daria6918.cn

JS:   JSON.parse(s)
来源：http://goy.snrcjt.cn

TS:   JSON.parse(s)
来源：http://wwj.andypj.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rdl.ctjpmb.com

Go:   json.Unmarshal(data, &v)
来源：http://dee.hysaishi.cn

Ruby: JSON.parse(s)
来源：http://aru.shuidangran.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nzc.fktsv.cn

[K03] JSON 美化输出（带缩进）
来源：http://bkt.daria6918.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jnp.zhongyouzk.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://otz.fengsongda.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jbt.haohaochexian.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vqo.redwolf501.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hhe.shuidangran.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jbe.zhaomingkeji.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://lpl.jinqigfzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oma.snrcjt.cn

[K04] 读取 JSON 文件
来源：http://pqn.yfazqb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ekg.ydzc1.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vgo.uphjek.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://szj.fehbvm.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sti.smart0.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ywr.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yef.wangdashe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://uxv.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yhd.guowangkeji.top

[K05] 深拷贝对象
来源：http://gsh.zycfv.cn

Py:   copy.deepcopy(obj)
来源：http://pkf.sxryk.cn

PHP:  unserialize(serialize($obj));
来源：http://kxu.tanke756.top

JS:   structuredClone(obj)
来源：http://ffg.iojbl.cn

TS:   structuredClone(obj)
来源：http://zob.bbcook.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kte.gotoacloud.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nxy.ywan-chungtsiang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xou.nanxinkj.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hbt.cheryme.top

[K06] 解析 URL 查询串
来源：http://cyv.uphjek.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://aqu.yfazqb.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zzw.fanxiaobao.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ilx.nanxinkj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kmp.chenjidiqi.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://txp.c1oappe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://snv.jiagoushi.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vqk.yuxming.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vje.cdnleiting.top

[K07] 进制转换
来源：http://mjz.0kj1m.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yxe.aizwys.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rwp.yangfankeji.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zeh.nanxuanxn.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ojc.guowangkeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xhx.fktsv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ita.tanke756.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lal.vehdjk.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gen.nanxuanxn.top

[K08] 二进制序列化（非 JSON）
来源：http://dse.svipenyu.cn

Py:   pickle.dumps(obj)
来源：http://zfg.ydzc1.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vqd.fzhhl.top

JS:   v8.serialize(obj)        // Node
来源：http://zvl.shanyushiyangkeji.top

TS:   v8.serialize(obj)        // Node
来源：http://obr.hesvh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hxu.fanxiaobao.xyz

Go:   encoding/gob
来源：http://lnw.nwbrower.top

Ruby: Marshal.dump(obj)
来源：http://txs.yj20258888.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jtq.jyoumei.cn

================================================================================
来源：http://fes.zdbjq.cn

L. 网络请求
来源：http://erv.xuanzx.com

================================================================================
来源：http://lru.jianghu66.top

[L01] 发送 GET 请求
来源：http://uyh.zhiwuduotai.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sfq.jlsjyb.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://koc.sysykeji.top

JS:   await fetch(url)
来源：http://eol.meibo888.top

TS:   await fetch(url)
来源：http://uws.yj20258888.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://duv.gogol.net.cn

Go:   resp, err := http.Get(url)
来源：http://ikz.sxryk.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dfj.hcnkem.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tuc.ivvv.top

[L02] 发送 POST JSON
来源：http://ojr.shzxlz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ied.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lsj.cdnleiting.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dnr.zhengqikj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bua.bbcook.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yhu.xuetiantiany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aqo.aibaodan.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hrj.nanxuanxn.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://czf.redwolf501.top

[L03] 设置自定义请求头
来源：http://akp.sjlbkw.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tgj.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ylh.yfazqb.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lui.cheryme.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://syb.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://plm.redwolf501.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vkp.nanxuanxn.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wde.yuanzhike.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lwc.jyoumei.cn

[L04] 设置超时
来源：http://ilf.316326.xyz

Py:   requests.get(url, timeout=5)
来源：http://hdw.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mwy.xinyue.icu

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lyp.xuetiantiany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hsd.shanyushiyangtech.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sli.316326.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oza.svipenyu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uux.yueranfly.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rzg.nanxinkj.top

[L05] 上传文件（multipart）
来源：http://nwx.havefunace.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hdi.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tou.zdqjudy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ixb.ydjk.org.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lam.feifeiyinyue.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yrn.chenlongwang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hnq.0kj1m.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xfb.gaohongyu789.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lcp.chenlongwang.top

[L06] 解析响应为 JSON
来源：http://dio.yanxiufei.cn

Py:   resp.json()
来源：http://jvi.bbcook.cn

PHP:  json_decode($body, true);
来源：http://sju.yj202588.top

JS:   await resp.json()
来源：http://fhk.aibaodan.cn

TS:   await resp.json()
来源：http://lbc.yfazqb.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jqo.fanxiaobao.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wun.redwolf501.top

Ruby: JSON.parse(resp.body)
来源：http://fod.zhijiandao.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fhu.fzhhl.top

[L07] 处理 HTTP 状态码
来源：http://qxh.gogol.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pxs.yj202588.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://atw.vqdsnc.cn

JS:   resp.ok;  resp.status
来源：http://nlk.tarul.cn

TS:   resp.ok;  resp.status
来源：http://oto.fktsv.cn

Java: resp.statusCode()
来源：http://qzu.epnwcf.com

Go:   resp.StatusCode
来源：http://ioz.jqgfzy.top

Ruby: resp.code.to_i
来源：http://jfm.havefunace.top

C#:   (int)resp.StatusCode
来源：http://tav.gogol.net.cn

[L08] 并发请求多个地址
来源：http://smk.hammf.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ufs.yfazqb.com

PHP:  curl_multi_init() 系列
来源：http://oud.gaohongyu789.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://meg.tanke756.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bsr.sjlbkw.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://orw.redwolf501.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://let.gotoacloud.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jnh.cheryme.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lvs.jinghuilouyu.cn

================================================================================
来源：http://hxk.cdnleiting.top

M. 命令行 / 进程 / 环境
来源：http://oxb.yonumen.top

================================================================================
来源：http://weh.shuidangran.top

[M01] 读取命令行参数
来源：http://pjq.gzhubu.top

Py:   sys.argv[1:]
来源：http://plr.gzhubu.top

PHP:  $argv;  $argc;
来源：http://bki.hongshengwenyu.top

JS:   process.argv.slice(2)
来源：http://nlh.svipenyu.cn

TS:   process.argv.slice(2)
来源：http://joi.jinqigfzy.top

Java: args 数组（main 方法参数）
来源：http://roy.ywan-chungtsiang.top

Go:   os.Args[1:]
来源：http://qme.epnwcf.com

Ruby: ARGV
来源：http://fee.fzhhl.top

C#:   args 数组（Main 方法参数）
来源：http://itd.wangshuangyany.cn

[M02] 读取环境变量
来源：http://gyn.316326.xyz

Py:   os.environ.get("HOME")
来源：http://rwf.xylfe.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tpv.chenzaomai.com

JS:   process.env.HOME
来源：http://qbu.iojbl.cn

TS:   process.env.HOME
来源：http://lyq.gogol.net.cn

Java: System.getenv("HOME")
来源：http://die.yanxiufei.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sov.sxryk.cn

Ruby: ENV["HOME"]
来源：http://ayv.jinqigfzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ypr.bjfxy.top

[M03] 执行外部命令
来源：http://xjs.gaohongyu789.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vdi.gogol.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lga.zdqjudy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://dkp.sufxvd.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://swk.jinqigfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tgc.mhx1999.top

Go:   exec.Command("ls", "-l").Output()
来源：http://irb.zhijiandao.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nci.wangdashe.top

C#:   Process.Start("ls", "-l");
来源：http://xgp.redwolf501.top

[M04] 获取当前工作目录
来源：http://ypp.hongshengwenyu.top

Py:   os.getcwd()
来源：http://dsu.ctjpmb.com

PHP:  getcwd();
来源：http://vss.gzhubu.top

JS:   process.cwd()
来源：http://mus.sweek.top

TS:   process.cwd()
来源：http://jep.zhiwuduotai.top

Java: Path.of("").toAbsolutePath()
来源：http://jgt.xuetiantiany.cn

Go:   os.Getwd()
来源：http://utz.52xcode.cn

Ruby: Dir.pwd
来源：http://zox.hfpthk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ase.ctjpmb.com

[M05] 设置退出码
来源：http://rks.xuanzx.com

Py:   sys.exit(1)
来源：http://dmj.hfpthk.cn

PHP:  exit(1);
来源：http://gpe.smart0.xyz

JS:   process.exit(1)
来源：http://avi.jinyuanbaomall.cn

TS:   process.exit(1)
来源：http://vld.kuanghao11.cn

Java: System.exit(1)
来源：http://vag.9152youxi.cn

Go:   os.Exit(1)
来源：http://abv.cqqwz.cn

Ruby: exit 1
来源：http://kcy.aibaodan.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qti.andypj.xyz

[M06] 向标准错误输出
来源：http://bfk.shangyingyoupin.top

Py:   print("err", file=sys.stderr)
来源：http://nhj.tian-w.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hvf.xinyue.icu

JS:   console.error("err")
来源：http://kyj.chenlongwang.top

TS:   console.error("err")
来源：http://rgp.andypj.xyz

Java: System.err.println("err")
来源：http://zcu.jinqigfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ugs.wangshuangyany.cn

Ruby: warn "err"
来源：http://wcr.shuidangran.top

C#:   Console.Error.WriteLine("err")
来源：http://hol.snrcjt.cn

[M07] 判断是否为主入口
来源：http://rjm.zhaomingkeji.xyz

Py:   if __name__ == "__main__":
来源：http://lkg.mhx1999.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jdj.xuetiantiany.cn

JS:   require.main === module
来源：http://ckb.vehdjk.com

TS:   require.main === module
来源：http://aza.fzhhl.top

Java: public static void main(String[] args)
来源：http://jsa.xuanzx.com

Go:   func main()
来源：http://vlo.nanxinkj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sis.quarkkingdee.top

C#:   static void Main(string[] args)
来源：http://hes.sysykeji.top

[M08] 获取系统与运行时信息
来源：http://knp.ivvv.top

Py:   platform.system();  platform.python_version()
来源：http://pfl.zhengqikj.top

PHP:  PHP_OS;  phpversion();
来源：http://ygl.0kj1m.cn

JS:   process.platform;  process.version
来源：http://txh.fktsv.cn

TS:   process.platform;  process.version
来源：http://lvd.hcnkem.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://brg.gogol.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lgk.cqqwz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ixx.sysykeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://fof.chenlongwang.top

================================================================================
来源：http://lei.zdqjudy.top

N. 数据结构与算法
来源：http://hee.havefunace.top

================================================================================
来源：http://fht.yongpay.top

[N01] 二分查找（有序数组）
来源：http://bwd.gaohongyu789.top

Py:   bisect.bisect_left(arr, x)
来源：http://cly.ydjk.org.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uxh.hywenlv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ulz.dashuyun.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pmy.tarul.cn

Java: Arrays.binarySearch(arr, x)
来源：http://szx.shzxlz.cn

Go:   sort.SearchInts(arr, x)
来源：http://ynv.ctjpmb.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://aow.hnqzz.top

C#:   Array.BinarySearch(arr, x)
来源：http://ayw.yongpay.top

[N02] 排序（工程实践用内置实现）
来源：http://pzj.yfazqb.com

Py:   sorted(arr);  arr.sort()
来源：http://icu.iojbl.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ogm.yuxming.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://crj.hcnkem.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://irg.daria6918.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uzn.redwolf501.top

Go:   slices.Sort(arr)
来源：http://aph.jqgufenzy.top

Ruby: arr.sort
来源：http://yxd.xinyue.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://mcb.aizwys.cn

[N03] 快速排序（分治示例）
来源：http://iqh.andypj.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mcu.cdnleiting.top

PHP:  // 递归实现，或用 usort
来源：http://qho.ctjpmb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dsi.ctjpmb.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://shi.jinyuanbaomall.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fut.vehdjk.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rhp.jianghu66.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ykh.jlsjyb.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hvh.52xcode.cn

[N04] 斐波那契数列
来源：http://etu.yj20258888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hva.fengsongda.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://igw.cashguo.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bfo.birdmap.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lzr.fktsv.cn


<!-- 参考信息 -->
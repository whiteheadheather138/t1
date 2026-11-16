代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://avu.xuanzx.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bmk.guannengcc.top

[J09] 时区处理
来源：http://elg.wangdashe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ujq.svipenyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://api.sxryk.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://deg.nwbrower.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://twv.zhaomingkeji.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qhv.feifeiyinyue.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://egr.yj20258888.top

Ruby: Time.now.getlocal("+08:00")
来源：http://snd.jqgufenzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bpm.feifeiyinyue.top

[J10] 取今天 / 本月第一天
来源：http://syn.xuetiantiany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wgn.ctjpmb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kjr.yj20258.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cav.tian-w.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bmf.yj20258888.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vmf.sysykeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kvz.nanxinkj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ifi.quarkkingdee.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tyv.jiagoushi.top

================================================================================
来源：http://bpy.ywan-chungtsiang.top

K. JSON 与序列化
来源：http://ogw.bbcook.cn

================================================================================
来源：http://doi.yj20258888.top

[K01] 对象转 JSON 字符串
来源：http://eje.havefunace.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oim.quarkkingdee.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yui.jinqigufen.top

JS:   JSON.stringify(obj)
来源：http://era.yuxming.cn

TS:   JSON.stringify(obj)
来源：http://caf.shzxlz.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yyw.vehdjk.com

Go:   json.Marshal(obj)
来源：http://twx.ehwqpu.com

Ruby: obj.to_json                                     // require "json"
来源：http://txa.jinghuilouyu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tvx.cdnleiting.top

[K02] JSON 字符串转对象
来源：http://uhv.tianlin.xyz

Py:   json.loads(s)
来源：http://uwj.wangshuangyany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://klx.yfazqb.com

JS:   JSON.parse(s)
来源：http://rxa.shzxlz.cn

TS:   JSON.parse(s)
来源：http://bax.wangdashe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zez.xinyue.icu

Go:   json.Unmarshal(data, &v)
来源：http://xrl.hongshengwenyu.top

Ruby: JSON.parse(s)
来源：http://hji.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vmk.haohaochexian.top

[K03] JSON 美化输出（带缩进）
来源：http://one.hywenlv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://euw.gaohongyu789.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nhl.dianchejie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://amb.ctjpmb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://vzo.shanyushiyangtech.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lcl.quarkkingdee.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mqh.epnwcf.com

Ruby: JSON.pretty_generate(obj)
来源：http://ivc.sxryk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mzz.jinghuilouyu.cn

[K04] 读取 JSON 文件
来源：http://eum.zhongyouzk.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fko.jiagoushi.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cas.zhiwuduotai.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pnl.sjlbkw.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tsm.zhongyouzk.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wft.vqdsnc.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://doy.daxiang520.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://azv.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bio.ehwqpu.com

[K05] 深拷贝对象
来源：http://dbf.smart0.xyz

Py:   copy.deepcopy(obj)
来源：http://qkc.hongshengwenyu.top

PHP:  unserialize(serialize($obj));
来源：http://hrr.ctjpmb.com

JS:   structuredClone(obj)
来源：http://gez.zhixingplan.top

TS:   structuredClone(obj)
来源：http://wkv.sweek.top

Java: // 手写拷贝构造，或序列化往返
来源：http://crt.cashguo.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kag.daxiang520.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mza.zhengqikj.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ueg.hysaishi.cn

[K06] 解析 URL 查询串
来源：http://ltc.shanyushiyangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://joj.andypj.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wcm.tarul.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oyn.jiagoushi.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://asv.tian-w.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ihw.zhengqikj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qzx.guowangkeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vbb.hesvh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vyd.ppjwa.cn

[K07] 进制转换
来源：http://ysa.hnqzz.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qzm.hnqzz.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hiw.nanxinkj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pth.gaohongyu789.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wtb.fehbvm.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ocj.cucudq.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vyv.jqgufenzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bhp.cdnleiting.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wge.aizwys.cn

[K08] 二进制序列化（非 JSON）
来源：http://sja.yueranfly.top

Py:   pickle.dumps(obj)
来源：http://wyf.sjlbkw.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yfg.wangdashe.top

JS:   v8.serialize(obj)        // Node
来源：http://ycb.haohaochexian.top

TS:   v8.serialize(obj)        // Node
来源：http://isf.havefunace.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://aqk.yanxiufei.cn

Go:   encoding/gob
来源：http://lcy.zhiwuduotai.top

Ruby: Marshal.dump(obj)
来源：http://gkb.zhixingplan.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://exv.jiagoushi.top

================================================================================
来源：http://rcz.ctjpmb.com

L. 网络请求
来源：http://gpr.gaohongyu789.top

================================================================================
来源：http://knp.zhengqikj.top

[L01] 发送 GET 请求
来源：http://ioh.sufxvd.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gtq.vehdjk.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ife.daxiang520.top

JS:   await fetch(url)
来源：http://lip.guowangkeji.top

TS:   await fetch(url)
来源：http://rts.52xcode.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bwg.gotoacloud.top

Go:   resp, err := http.Get(url)
来源：http://eni.daria6918.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zep.hcnkem.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yrm.jyoumei.cn

[L02] 发送 POST JSON
来源：http://bft.wangshuangyany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ccs.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zlw.svipenyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tjz.ivvv.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fmu.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nxb.daria6918.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nhm.jyoumei.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qqq.smart0.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ltw.zhiwuduotai.top

[L03] 设置自定义请求头
来源：http://jxt.xinyue.icu

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rvw.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://udb.ydzc1.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nis.redwolf501.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eqk.uphjek.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ure.cdnleiting.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hzb.hcnkem.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ygd.ydjk.org.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fiz.yonumen.top

[L04] 设置超时
来源：http://qza.guannengcc.top

Py:   requests.get(url, timeout=5)
来源：http://umb.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ovk.yangfankeji.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rhy.fzhhl.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bha.yongpay.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tuf.birdmap.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rik.shanyushiyangtech.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://clq.jiagoushi.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uvq.fzhhl.top

[L05] 上传文件（multipart）
来源：http://pfe.ybcxt.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://noo.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hnr.dashuyun.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qey.daxiang520.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hkm.bbcook.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ptm.yuanzhike.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fsl.fengsongda.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qxg.gotoacloud.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hoz.nwbrower.top

[L06] 解析响应为 JSON
来源：http://qet.yj20258888.top

Py:   resp.json()
来源：http://tgh.zhijiandao.cn

PHP:  json_decode($body, true);
来源：http://pqx.jqgufenzy.top

JS:   await resp.json()
来源：http://kwe.sufxvd.cn

TS:   await resp.json()
来源：http://rto.aizwys.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xbi.yfazqb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fov.zhaomingkeji.xyz

Ruby: JSON.parse(resp.body)
来源：http://zra.iojbl.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zev.birdmap.top

[L07] 处理 HTTP 状态码
来源：http://wyn.52xcode.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mqb.ydjk.org.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vxc.yongpay.top

JS:   resp.ok;  resp.status
来源：http://izj.cdnleiting.top

TS:   resp.ok;  resp.status
来源：http://bwi.andypj.xyz

Java: resp.statusCode()
来源：http://tlc.vehdjk.com

Go:   resp.StatusCode
来源：http://iwi.fktsv.cn

Ruby: resp.code.to_i
来源：http://tvw.jinyuanbaomall.cn

C#:   (int)resp.StatusCode
来源：http://wag.shangyingyoupin.top

[L08] 并发请求多个地址
来源：http://zog.yongpay.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wss.cucudq.cn

PHP:  curl_multi_init() 系列
来源：http://qxd.yangfankeji.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gom.jyoumei.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xsr.ehwqpu.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cxs.havefunace.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rdr.ppjwa.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zmu.feifeiyinyue.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://aec.c1oappe.top

================================================================================
来源：http://tds.zhoulong.xyz

M. 命令行 / 进程 / 环境
来源：http://mqy.fanxiaobao.xyz

================================================================================
来源：http://add.c1oappe.top

[M01] 读取命令行参数
来源：http://azi.zycfv.cn

Py:   sys.argv[1:]
来源：http://ahb.chenlongwang.top

PHP:  $argv;  $argc;
来源：http://vvw.guannengcc.top

JS:   process.argv.slice(2)
来源：http://qjl.shanyushiyangkeji.top

TS:   process.argv.slice(2)
来源：http://buk.shangyingyoupin.top

Java: args 数组（main 方法参数）
来源：http://ped.pengpengdd.cyou

Go:   os.Args[1:]
来源：http://rid.jqgufenzy.top

Ruby: ARGV
来源：http://gca.c1oappe.top

C#:   args 数组（Main 方法参数）
来源：http://xpq.tianlin.xyz

[M02] 读取环境变量
来源：http://nwp.zycfv.cn

Py:   os.environ.get("HOME")
来源：http://chn.hammf.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nks.cdnleiting.top

JS:   process.env.HOME
来源：http://rpd.jinghuilouyu.cn

TS:   process.env.HOME
来源：http://oxn.52xcode.cn

Java: System.getenv("HOME")
来源：http://tmm.andypj.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mvc.jqgufenzy.top

Ruby: ENV["HOME"]
来源：http://bbd.daxiang520.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jtv.yj20258.top

[M03] 执行外部命令
来源：http://enx.haohaochexian.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xes.svipenyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zwl.xingfuxueyuan.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://mlx.zdbjq.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fib.vqdsnc.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ikj.cashguo.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xoj.yangfankeji.com

Ruby: system("ls -l");  `ls -l`
来源：http://ecc.kuanghao11.cn

C#:   Process.Start("ls", "-l");
来源：http://xcu.hongshengwenyu.top

[M04] 获取当前工作目录
来源：http://oxq.andypj.xyz

Py:   os.getcwd()
来源：http://bit.aizwys.cn

PHP:  getcwd();
来源：http://aze.jqgfzy.top

JS:   process.cwd()
来源：http://qco.cdnleiting.top

TS:   process.cwd()
来源：http://kum.hongshengwenyu.top

Java: Path.of("").toAbsolutePath()
来源：http://fky.nanxinkj.top

Go:   os.Getwd()
来源：http://mhr.hywenlv.cn

Ruby: Dir.pwd
来源：http://kke.guannengcc.top

C#:   Directory.GetCurrentDirectory()
来源：http://hrb.gogol.net.cn

[M05] 设置退出码
来源：http://lkt.xuetiantiany.cn

Py:   sys.exit(1)
来源：http://hwu.hnxiangtu.top

PHP:  exit(1);
来源：http://mlg.ppjwa.cn

JS:   process.exit(1)
来源：http://mhs.andypj.xyz

TS:   process.exit(1)
来源：http://wki.cdnleiting.top

Java: System.exit(1)
来源：http://kpf.vqdsnc.cn

Go:   os.Exit(1)
来源：http://plo.kuanghao11.cn

Ruby: exit 1
来源：http://odu.xuetiantiany.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://new.0kj1m.cn

[M06] 向标准错误输出
来源：http://ftu.tian-w.cn

Py:   print("err", file=sys.stderr)
来源：http://ddi.sxryk.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cxi.cheryme.top

JS:   console.error("err")
来源：http://sti.yj20258.top

TS:   console.error("err")
来源：http://mte.zhiwuduotai.top

Java: System.err.println("err")
来源：http://afo.gzhubu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xpb.gzhubu.top

Ruby: warn "err"
来源：http://fbf.0kj1m.cn

C#:   Console.Error.WriteLine("err")
来源：http://rnc.0kj1m.cn

[M07] 判断是否为主入口
来源：http://mst.iojbl.cn

Py:   if __name__ == "__main__":
来源：http://tkp.ywan-chungtsiang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ebf.sufxvd.cn

JS:   require.main === module
来源：http://ijn.xuanzx.com

TS:   require.main === module
来源：http://gjp.gzhubu.top

Java: public static void main(String[] args)
来源：http://nlo.9152youxi.cn

Go:   func main()
来源：http://yse.quarkkingdee.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ueq.jianghu66.top

C#:   static void Main(string[] args)
来源：http://igp.xylfe.cn

[M08] 获取系统与运行时信息
来源：http://nxj.xziqi.cn

Py:   platform.system();  platform.python_version()
来源：http://hif.jiagoushi.top

PHP:  PHP_OS;  phpversion();
来源：http://iel.nanxinkj.top

JS:   process.platform;  process.version
来源：http://pgx.andypj.xyz

TS:   process.platform;  process.version
来源：http://cia.sxryk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lfu.gzhubu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://bni.ydzc1.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fvj.ehwqpu.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://vcu.sjlbkw.cn

================================================================================
来源：http://cqt.gotoacloud.top

N. 数据结构与算法
来源：http://tbq.birdmap.top

================================================================================
来源：http://syk.gzhubu.top

[N01] 二分查找（有序数组）
来源：http://vai.snrcjt.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pps.hammf.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zhz.meibo888.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://max.xziqi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://woe.guannengcc.top

Java: Arrays.binarySearch(arr, x)
来源：http://fed.gaohongyu789.top

Go:   sort.SearchInts(arr, x)
来源：http://xmp.cqqwz.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vsh.ywan-chungtsiang.top

C#:   Array.BinarySearch(arr, x)
来源：http://mfv.yuxming.cn

[N02] 排序（工程实践用内置实现）
来源：http://vma.aibaodan.cn

Py:   sorted(arr);  arr.sort()
来源：http://jvl.vqdsnc.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bdy.hnqzz.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ulb.hongshengwenyu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fmt.dashuyun.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mml.ivvv.top

Go:   slices.Sort(arr)
来源：http://fey.gotoacloud.top

Ruby: arr.sort
来源：http://tqy.jianghu66.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qob.0kj1m.cn

[N03] 快速排序（分治示例）
来源：http://mtq.cqqwz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lpq.ydzc1.top

PHP:  // 递归实现，或用 usort
来源：http://azh.jinqigufen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wyb.andypj.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hww.xinyue.icu

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kzb.hywenlv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nwm.zhaomingkeji.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uji.jyoumei.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pcx.316326.xyz

[N04] 斐波那契数列
来源：http://yrj.xingfuxueyuan.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wek.zhoulong.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lmh.52xcode.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tdr.sjlbkw.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gfa.mhx1999.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dai.kuanghao11.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dcg.hysaishi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xqw.hongshengwenyu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://upj.316326.xyz

[N05] 最大公约数
来源：http://gpe.9152youxi.cn

Py:   math.gcd(a, b)
来源：http://flr.havefunace.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xqb.hywenlv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mbh.nanxinkj.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dhw.jyoumei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://seu.cashguo.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xqq.daxiang520.top

Ruby: a.gcd(b)
来源：http://mvq.xuetiantiany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ugb.jinqigfzy.top

[N06] 判断回文字符串
来源：http://vli.316326.xyz

Py:   s == s[::-1]
来源：http://lcu.yongpay.top

PHP:  $s === strrev($s);
来源：http://lij.yj202588.top

JS:   s === [...s].reverse().join("")
来源：http://tqg.aizwys.cn

TS:   s === [...s].reverse().join("")
来源：http://sda.xuetiantiany.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hsp.jinqigfzy.top

Go:   // 双指针从两端比较
来源：http://ptl.daxiang520.top


<!-- 参考信息 -->
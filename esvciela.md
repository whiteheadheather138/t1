代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ndi.hesvh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://smg.pycfn.com

[J09] 时区处理
来源：http://ite.tarul.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hxg.shanyushiyangtech.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cmr.sjlbkw.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ejb.smart0.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cuq.xingfuxueyuan.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jff.svipenyu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nbu.nwbrower.top

Ruby: Time.now.getlocal("+08:00")
来源：http://efu.aibaodan.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uez.smart0.xyz

[J10] 取今天 / 本月第一天
来源：http://hsm.gogol.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lvi.yuxming.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rwb.fzhhl.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mwt.yvedp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://geh.gogol.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qik.fehbvm.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sal.sxryk.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ejp.yfazqb.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vbk.tanke756.top

================================================================================
来源：http://jdr.jianghu66.top

K. JSON 与序列化
来源：http://vct.316326.xyz

================================================================================
来源：http://obp.meibo888.top

[K01] 对象转 JSON 字符串
来源：http://jnn.ivvv.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://agu.jqgfzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://upc.yongpay.top

JS:   JSON.stringify(obj)
来源：http://czf.pengpengdd.cyou

TS:   JSON.stringify(obj)
来源：http://wcs.wangdashe.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tvx.ctjpmb.com

Go:   json.Marshal(obj)
来源：http://ebw.nanxuanxn.top

Ruby: obj.to_json                                     // require "json"
来源：http://pjw.jinghuilouyu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kwg.shangyingyoupin.top

[K02] JSON 字符串转对象
来源：http://oud.zycfv.cn

Py:   json.loads(s)
来源：http://bcf.shzxlz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oeh.ctjpmb.com

JS:   JSON.parse(s)
来源：http://jen.ywan-chungtsiang.top

TS:   JSON.parse(s)
来源：http://lsr.cashguo.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zbh.shzxlz.cn

Go:   json.Unmarshal(data, &v)
来源：http://rym.dashuyun.cn

Ruby: JSON.parse(s)
来源：http://bgw.wangshuangyany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://onn.shzxlz.cn

[K03] JSON 美化输出（带缩进）
来源：http://dey.jqgufenzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jbh.vehdjk.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hcw.epnwcf.com

JS:   JSON.stringify(obj, null, 2)
来源：http://dpd.aibaodan.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://str.feifeiyinyue.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wfv.haohaochexian.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tew.cdnleiting.top

Ruby: JSON.pretty_generate(obj)
来源：http://mql.shzxlz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pmq.9152youxi.cn

[K04] 读取 JSON 文件
来源：http://php.cheryme.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bvp.birdmap.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vqi.xuetiantiany.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://waf.cqqwz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jap.52xcode.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jyf.uphjek.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rwj.cqqwz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mcp.kuanghao11.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rrb.yj20258888.top

[K05] 深拷贝对象
来源：http://zsa.aizwys.cn

Py:   copy.deepcopy(obj)
来源：http://zyj.yj202588.top

PHP:  unserialize(serialize($obj));
来源：http://num.sjlbkw.cn

JS:   structuredClone(obj)
来源：http://msj.dianchejie.cn

TS:   structuredClone(obj)
来源：http://nnh.wangdashe.top

Java: // 手写拷贝构造，或序列化往返
来源：http://nqa.tianlin.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xiy.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pli.daria6918.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://aas.birdmap.top

[K06] 解析 URL 查询串
来源：http://jvk.havefunace.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sle.chenzaomai.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://drs.xinyue.icu

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://out.fengsongda.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wku.jqgufenzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xnm.ctjpmb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://wfi.nanxinkj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://krw.0kj1m.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zgv.zhiwuduotai.top

[K07] 进制转换
来源：http://lsd.wangshuangyany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wyw.wangshuangyany.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jzo.52xcode.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ujg.vqdsnc.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ydz.aibaodan.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dmb.cheryme.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xpn.xinyue.icu

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kzh.yfazqb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tyj.jinqigufen.top

[K08] 二进制序列化（非 JSON）
来源：http://gfm.bbcook.cn

Py:   pickle.dumps(obj)
来源：http://wdn.jinqigfzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://bvi.bjfxy.top

JS:   v8.serialize(obj)        // Node
来源：http://kkv.quarkkingdee.top

TS:   v8.serialize(obj)        // Node
来源：http://nre.shanyushiyangtech.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qnk.jinqigufen.top

Go:   encoding/gob
来源：http://lnp.shanyushiyangtech.top

Ruby: Marshal.dump(obj)
来源：http://hqx.jlsjyb.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sbn.yj20258888.top

================================================================================
来源：http://wzo.ydjk.org.cn

L. 网络请求
来源：http://nll.uphjek.com

================================================================================
来源：http://mqh.pycfn.com

[L01] 发送 GET 请求
来源：http://vrm.zhiwuduotai.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://geq.tanke756.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bgg.birdmap.top

JS:   await fetch(url)
来源：http://gmy.ydzc1.top

TS:   await fetch(url)
来源：http://joy.zhengqikj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://upq.hesvh.cn

Go:   resp, err := http.Get(url)
来源：http://xuy.zhixingplan.top

Ruby: Net::HTTP.get(URI(url))
来源：http://umn.zycfv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bfj.quarkkingdee.top

[L02] 发送 POST JSON
来源：http://tfm.jqgfzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://dky.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zgk.ctjpmb.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qyy.zycfv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xot.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qgp.ybcxt.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jdn.zhiwuduotai.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://iub.tanke756.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qxr.daxiang520.top

[L03] 设置自定义请求头
来源：http://esg.sweek.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hap.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://niy.tanke756.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ekx.havefunace.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vjl.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zbs.hammf.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mwc.zhiwuduotai.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kva.svipenyu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jbh.xylfe.cn

[L04] 设置超时
来源：http://gll.tianlin.xyz

Py:   requests.get(url, timeout=5)
来源：http://ggs.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ncf.shzxlz.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jol.cqqwz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vzi.chenzaomai.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gga.tarul.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fpg.hnqzz.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ppn.gogol.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hlc.zhiwuduotai.top

[L05] 上传文件（multipart）
来源：http://kuv.zhengqikj.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zvg.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ppm.hfpthk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ijv.ybcxt.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bce.quarkkingdee.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xmb.quarkkingdee.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ktn.svipenyu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tti.andypj.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gwb.cqqwz.cn

[L06] 解析响应为 JSON
来源：http://xub.zdqjudy.top

Py:   resp.json()
来源：http://jsu.xylfe.cn

PHP:  json_decode($body, true);
来源：http://ptx.snrcjt.cn

JS:   await resp.json()
来源：http://tuo.sysykeji.top

TS:   await resp.json()
来源：http://jte.yueranfly.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vgr.kuanghao11.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xvs.havefunace.top

Ruby: JSON.parse(resp.body)
来源：http://xlq.daria6918.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lmm.quarkkingdee.top

[L07] 处理 HTTP 状态码
来源：http://ije.zhengqikj.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tbh.yj20258888.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vrl.guowangkeji.top

JS:   resp.ok;  resp.status
来源：http://vdy.jqgfzy.top

TS:   resp.ok;  resp.status
来源：http://sdi.smart0.xyz

Java: resp.statusCode()
来源：http://vhm.epnwcf.com

Go:   resp.StatusCode
来源：http://wol.zhengqikj.top

Ruby: resp.code.to_i
来源：http://flm.fengsongda.top

C#:   (int)resp.StatusCode
来源：http://xjo.jyoumei.cn

[L08] 并发请求多个地址
来源：http://epb.chenzaomai.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uda.wangshuangyany.cn

PHP:  curl_multi_init() 系列
来源：http://nef.fehbvm.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cff.feifeiyinyue.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kqb.gogol.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://syu.andypj.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fvd.tianlin.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ncp.fktsv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://aik.dianchejie.cn

================================================================================
来源：http://zxy.pycfn.com

M. 命令行 / 进程 / 环境
来源：http://hwf.gzhubu.top

================================================================================
来源：http://njp.xinyue.icu

[M01] 读取命令行参数
来源：http://ohv.fzhhl.top

Py:   sys.argv[1:]
来源：http://fqv.shanyushiyangkeji.top

PHP:  $argv;  $argc;
来源：http://ymf.jiagoushi.top

JS:   process.argv.slice(2)
来源：http://qlq.shzxlz.cn

TS:   process.argv.slice(2)
来源：http://fjl.hfpthk.cn

Java: args 数组（main 方法参数）
来源：http://fud.nanxinkj.top

Go:   os.Args[1:]
来源：http://ofp.0kj1m.cn

Ruby: ARGV
来源：http://gqr.yueranfly.top

C#:   args 数组（Main 方法参数）
来源：http://lbg.yanxiufei.cn

[M02] 读取环境变量
来源：http://bfh.yangfankeji.com

Py:   os.environ.get("HOME")
来源：http://etr.hnqzz.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://emk.hammf.cn

JS:   process.env.HOME
来源：http://pzy.jinqigfzy.top

TS:   process.env.HOME
来源：http://bdi.hcnkem.com

Java: System.getenv("HOME")
来源：http://sxo.zdbjq.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qzz.jinqigufen.top

Ruby: ENV["HOME"]
来源：http://tqs.ehwqpu.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://spr.gzhubu.top

[M03] 执行外部命令
来源：http://suy.quarkkingdee.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nvv.tianlin.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fea.jinqigfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://enz.zhiwuduotai.top

TS:   child_process.execSync("ls -l").toString()
来源：http://dkn.c1oappe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yms.guannengcc.top

Go:   exec.Command("ls", "-l").Output()
来源：http://hlr.hammf.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fgw.uphjek.com

C#:   Process.Start("ls", "-l");
来源：http://bwj.svipenyu.cn

[M04] 获取当前工作目录
来源：http://tfw.jyoumei.cn

Py:   os.getcwd()
来源：http://ppb.xuetiantiany.cn

PHP:  getcwd();
来源：http://tew.ctjpmb.com

JS:   process.cwd()
来源：http://dfc.fktsv.cn

TS:   process.cwd()
来源：http://rrh.sxryk.cn

Java: Path.of("").toAbsolutePath()
来源：http://vog.shanyushiyangkeji.top

Go:   os.Getwd()
来源：http://rin.zhongyouzk.top

Ruby: Dir.pwd
来源：http://ufb.iojbl.cn

C#:   Directory.GetCurrentDirectory()
来源：http://suj.jinyuanbaomall.cn

[M05] 设置退出码
来源：http://nnd.jlsjyb.cn

Py:   sys.exit(1)
来源：http://anm.ybcxt.top

PHP:  exit(1);
来源：http://hot.hammf.cn

JS:   process.exit(1)
来源：http://aef.xuetiantiany.cn

TS:   process.exit(1)
来源：http://fio.xuanzx.com

Java: System.exit(1)
来源：http://hmw.smart0.xyz

Go:   os.Exit(1)
来源：http://gxb.feifeiyinyue.top

Ruby: exit 1
来源：http://cxu.guannengcc.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qeu.havefunace.top

[M06] 向标准错误输出
来源：http://cye.shanyushiyangkeji.top

Py:   print("err", file=sys.stderr)
来源：http://dpk.pycfn.com

PHP:  fwrite(STDERR, "err\n");
来源：http://eqg.gotoacloud.top

JS:   console.error("err")
来源：http://ovq.ivvv.top

TS:   console.error("err")
来源：http://ecq.zhaomingkeji.xyz

Java: System.err.println("err")
来源：http://gnx.zdbjq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://iyy.tian-w.cn

Ruby: warn "err"
来源：http://myl.quarkkingdee.top

C#:   Console.Error.WriteLine("err")
来源：http://ind.dashuyun.cn

[M07] 判断是否为主入口
来源：http://ept.hysaishi.cn

Py:   if __name__ == "__main__":
来源：http://qpq.hesvh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ckw.zhongyouzk.top

JS:   require.main === module
来源：http://lwc.shanyushiyangtech.top

TS:   require.main === module
来源：http://yss.cheryme.top

Java: public static void main(String[] args)
来源：http://aww.mhx1999.top

Go:   func main()
来源：http://sml.zhengqikj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mqk.jinyuanbaomall.cn

C#:   static void Main(string[] args)
来源：http://zja.cashguo.top

[M08] 获取系统与运行时信息
来源：http://ccm.yonumen.top

Py:   platform.system();  platform.python_version()
来源：http://pmm.fehbvm.com

PHP:  PHP_OS;  phpversion();
来源：http://qeh.haohaochexian.top

JS:   process.platform;  process.version
来源：http://kkn.birdmap.top

TS:   process.platform;  process.version
来源：http://owx.zhixingplan.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://drb.shangyingyoupin.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ejb.smart0.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sgb.tanke756.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kpt.nwbrower.top

================================================================================
来源：http://qlx.cucudq.cn

N. 数据结构与算法
来源：http://kks.epnwcf.com

================================================================================
来源：http://akv.vehdjk.com

[N01] 二分查找（有序数组）
来源：http://gom.52xcode.cn

Py:   bisect.bisect_left(arr, x)
来源：http://get.zdbjq.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ajh.zdbjq.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jne.dianchejie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://psc.jinqigfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://hdd.c1oappe.top

Go:   sort.SearchInts(arr, x)
来源：http://oqv.guowangkeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://udw.xinyue.icu

C#:   Array.BinarySearch(arr, x)
来源：http://vug.sysykeji.top

[N02] 排序（工程实践用内置实现）
来源：http://unx.sweek.top

Py:   sorted(arr);  arr.sort()
来源：http://gir.iojbl.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ccl.iojbl.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tqr.sxryk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://uac.yueranfly.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://doq.dianchejie.cn

Go:   slices.Sort(arr)
来源：http://qtg.yueranfly.top

Ruby: arr.sort
来源：http://ika.ydjk.org.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jej.jinghuilouyu.cn

[N03] 快速排序（分治示例）
来源：http://zke.zhongyouzk.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://oah.haohaochexian.top

PHP:  // 递归实现，或用 usort
来源：http://wgv.cqqwz.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gym.wangdashe.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jpy.wangdashe.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cwc.aizwys.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://obu.bbcook.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rmb.xylfe.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rmx.9152youxi.cn

[N04] 斐波那契数列
来源：http://sil.yonumen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gne.kuanghao11.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zsq.chenjidiqi.icu

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ymd.nanxinkj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ahg.hfpthk.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ytn.kuanghao11.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jlh.fanxiaobao.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://whg.ehwqpu.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tai.ctjpmb.com

[N05] 最大公约数
来源：http://fal.pengpengdd.cyou

Py:   math.gcd(a, b)
来源：http://qkd.jinqigufen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yoe.hnxiangtu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kvs.xingfuxueyuan.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ppt.wangdashe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://iyz.xingfuxueyuan.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hgp.yuxming.cn

Ruby: a.gcd(b)
来源：http://qtz.0kj1m.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://odb.ppjwa.cn

[N06] 判断回文字符串
来源：http://ywl.hnxiangtu.top

Py:   s == s[::-1]
来源：http://acz.jinghuilouyu.cn

PHP:  $s === strrev($s);
来源：http://szz.dianchejie.cn

JS:   s === [...s].reverse().join("")
来源：http://zdy.cashguo.top

TS:   s === [...s].reverse().join("")
来源：http://oxu.bbcook.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rbx.cqqwz.cn

Go:   // 双指针从两端比较
来源：http://qfa.cqqwz.cn


<!-- 参考信息 -->
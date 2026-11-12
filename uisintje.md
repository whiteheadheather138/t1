代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jkq.hywenlv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rbt.bbcook.cn

[J09] 时区处理
来源：http://xfg.jinqigfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://eao.zhoulong.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yyo.uphjek.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dgm.jinqigufen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bnx.jyoumei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cyi.52xcode.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://igm.chenjidiqi.icu

Ruby: Time.now.getlocal("+08:00")
来源：http://uhy.nanxuanxn.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://plk.ehwqpu.com

[J10] 取今天 / 本月第一天
来源：http://dlp.zhaomingkeji.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://jkm.gaohongyu789.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ozd.tarul.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lgl.tarul.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kar.sysykeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tkt.smart0.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://awj.shanyushiyangkeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nkz.snrcjt.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ofg.hongshengwenyu.top

================================================================================
来源：http://eum.xuetiantiany.cn

K. JSON 与序列化
来源：http://anu.tarul.cn

================================================================================
来源：http://kch.zhengqikj.top

[K01] 对象转 JSON 字符串
来源：http://fxn.zhijiandao.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bri.nanxinkj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jut.redwolf501.top

JS:   JSON.stringify(obj)
来源：http://ywy.zhongyouzk.top

TS:   JSON.stringify(obj)
来源：http://qhu.sysykeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mar.shanyushiyangtech.top

Go:   json.Marshal(obj)
来源：http://zmn.ivvv.top

Ruby: obj.to_json                                     // require "json"
来源：http://fay.zdqjudy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://kli.ybcxt.top

[K02] JSON 字符串转对象
来源：http://lrg.daria6918.cn

Py:   json.loads(s)
来源：http://nzy.cheryme.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pjr.kuanghao11.cn

JS:   JSON.parse(s)
来源：http://fce.ybcxt.top

TS:   JSON.parse(s)
来源：http://xjg.ywan-chungtsiang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://saa.snrcjt.cn

Go:   json.Unmarshal(data, &v)
来源：http://krb.bjfxy.top

Ruby: JSON.parse(s)
来源：http://via.zdbjq.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fvm.haohaochexian.top

[K03] JSON 美化输出（带缩进）
来源：http://baa.xziqi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yuc.gogol.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kjd.dianchejie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bor.hysaishi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ucw.haohaochexian.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://izv.jqgufenzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hsq.daria6918.cn

Ruby: JSON.pretty_generate(obj)
来源：http://awh.epnwcf.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://amz.epnwcf.com

[K04] 读取 JSON 文件
来源：http://fmp.bjfxy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fzq.cqqwz.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ept.jqgufenzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://svh.jinqigfzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qyt.jiagoushi.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://asf.epnwcf.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ira.yuxming.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lks.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://apz.jqgfzy.top

[K05] 深拷贝对象
来源：http://pgg.gaohongyu789.top

Py:   copy.deepcopy(obj)
来源：http://tbx.sjlbkw.cn

PHP:  unserialize(serialize($obj));
来源：http://jcf.yonumen.top

JS:   structuredClone(obj)
来源：http://lwi.ybcxt.top

TS:   structuredClone(obj)
来源：http://jug.xuanzx.com

Java: // 手写拷贝构造，或序列化往返
来源：http://ttb.0kj1m.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hrh.yfazqb.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://typ.haohaochexian.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zcx.fktsv.cn

[K06] 解析 URL 查询串
来源：http://zea.zhixingplan.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bms.guannengcc.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jmd.zycfv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://djq.9152youxi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://onk.hywenlv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qwt.jianghu66.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://swu.9152youxi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fbt.kuanghao11.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ung.jinqigfzy.top

[K07] 进制转换
来源：http://cfh.ctjpmb.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://szj.yuanzhike.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hgi.xylfe.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pvm.zhongyouzk.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jid.shanyushiyangtech.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://feg.zycfv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gsu.tian-w.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jdw.yj202588.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tej.quarkkingdee.top

[K08] 二进制序列化（非 JSON）
来源：http://gus.aizwys.cn

Py:   pickle.dumps(obj)
来源：http://hjw.sxryk.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bcg.jiagoushi.top

JS:   v8.serialize(obj)        // Node
来源：http://ieq.gotoacloud.top

TS:   v8.serialize(obj)        // Node
来源：http://ypu.hfpthk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jce.uphjek.com

Go:   encoding/gob
来源：http://owb.hywenlv.cn

Ruby: Marshal.dump(obj)
来源：http://ftc.yongpay.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fmf.fktsv.cn

================================================================================
来源：http://kjj.zhixingplan.top

L. 网络请求
来源：http://ihx.epnwcf.com

================================================================================
来源：http://ktt.cqqwz.cn

[L01] 发送 GET 请求
来源：http://kap.316326.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://geo.hongshengwenyu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fml.chenzaomai.com

JS:   await fetch(url)
来源：http://yjl.hesvh.cn

TS:   await fetch(url)
来源：http://fzy.ehwqpu.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://slg.c1oappe.top

Go:   resp, err := http.Get(url)
来源：http://ksx.jqgfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://mnm.xuanzx.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://brx.jqgfzy.top

[L02] 发送 POST JSON
来源：http://zbx.ehwqpu.com

Py:   requests.post(url, json={"a": 1})
来源：http://dej.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dnj.cashguo.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tez.hfpthk.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://whi.tanke756.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cch.zhongyouzk.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://joj.daria6918.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://amt.sweek.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qpv.hammf.cn

[L03] 设置自定义请求头
来源：http://uqf.yongpay.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ere.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rsz.yuxming.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ukv.zhongyouzk.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://clk.hongshengwenyu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zpt.zhongyouzk.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iqr.9152youxi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bgy.meibo888.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bcp.feifeiyinyue.top

[L04] 设置超时
来源：http://jey.hnqzz.top

Py:   requests.get(url, timeout=5)
来源：http://pnx.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wog.316326.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fyn.guowangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oeh.sysykeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rde.redwolf501.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bgz.cdnleiting.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://udt.yfazqb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hga.jinghuilouyu.cn

[L05] 上传文件（multipart）
来源：http://gex.hesvh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ehm.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sbv.yanxiufei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://urf.wangdashe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vhc.hnqzz.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yyx.hysaishi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://akp.zdbjq.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cts.zycfv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dzn.cashguo.top

[L06] 解析响应为 JSON
来源：http://rnj.0kj1m.cn

Py:   resp.json()
来源：http://ptc.yanxiufei.cn

PHP:  json_decode($body, true);
来源：http://fkh.jyoumei.cn

JS:   await resp.json()
来源：http://vkt.birdmap.top

TS:   await resp.json()
来源：http://qwb.yueranfly.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://juo.epnwcf.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://agj.epnwcf.com

Ruby: JSON.parse(resp.body)
来源：http://csy.daria6918.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fqe.bbcook.cn

[L07] 处理 HTTP 状态码
来源：http://kft.pycfn.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fup.daria6918.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rdv.jlsjyb.cn

JS:   resp.ok;  resp.status
来源：http://gix.pengpengdd.cyou

TS:   resp.ok;  resp.status
来源：http://hkm.zhaomingkeji.xyz

Java: resp.statusCode()
来源：http://jjt.fanxiaobao.xyz

Go:   resp.StatusCode
来源：http://fjw.zhiwuduotai.top

Ruby: resp.code.to_i
来源：http://tfi.shangyingyoupin.top

C#:   (int)resp.StatusCode
来源：http://vee.fengsongda.top

[L08] 并发请求多个地址
来源：http://ihj.jqgufenzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://iuw.daxiang520.top

PHP:  curl_multi_init() 系列
来源：http://ikt.ywan-chungtsiang.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://esv.chenlongwang.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hez.bjfxy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rry.zhiwuduotai.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bzf.fehbvm.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mvs.tian-w.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qoh.yj202588.top

================================================================================
来源：http://csp.yj202588.top

M. 命令行 / 进程 / 环境
来源：http://mog.cashguo.top

================================================================================
来源：http://wya.hysaishi.cn

[M01] 读取命令行参数
来源：http://upv.yfazqb.com

Py:   sys.argv[1:]
来源：http://llz.tarul.cn

PHP:  $argv;  $argc;
来源：http://kei.yj20258888.top

JS:   process.argv.slice(2)
来源：http://sxn.xinyue.icu

TS:   process.argv.slice(2)
来源：http://doe.havefunace.top

Java: args 数组（main 方法参数）
来源：http://tkt.smart0.xyz

Go:   os.Args[1:]
来源：http://csf.epnwcf.com

Ruby: ARGV
来源：http://kha.ydjk.org.cn

C#:   args 数组（Main 方法参数）
来源：http://dck.zdbjq.cn

[M02] 读取环境变量
来源：http://qhc.cheryme.top

Py:   os.environ.get("HOME")
来源：http://cce.cucudq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://swn.xylfe.cn

JS:   process.env.HOME
来源：http://lrz.hnqzz.top

TS:   process.env.HOME
来源：http://bpk.hysaishi.cn

Java: System.getenv("HOME")
来源：http://zed.ivvv.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wti.jinghuilouyu.cn

Ruby: ENV["HOME"]
来源：http://lrl.ppjwa.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vhx.fanxiaobao.xyz

[M03] 执行外部命令
来源：http://mdg.tian-w.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dwz.fzhhl.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ttu.zycfv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zni.9152youxi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ojb.fzhhl.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kcq.chenlongwang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://zvr.daxiang520.top

Ruby: system("ls -l");  `ls -l`
来源：http://awd.yonumen.top

C#:   Process.Start("ls", "-l");
来源：http://zik.cheryme.top

[M04] 获取当前工作目录
来源：http://xiv.shuidangran.top

Py:   os.getcwd()
来源：http://zyn.pycfn.com

PHP:  getcwd();
来源：http://ttb.sweek.top

JS:   process.cwd()
来源：http://rpz.sweek.top

TS:   process.cwd()
来源：http://dxq.shangyingyoupin.top

Java: Path.of("").toAbsolutePath()
来源：http://wbe.guannengcc.top

Go:   os.Getwd()
来源：http://zvg.wangshuangyany.cn

Ruby: Dir.pwd
来源：http://pjg.nanxuanxn.top

C#:   Directory.GetCurrentDirectory()
来源：http://vkr.dashuyun.cn

[M05] 设置退出码
来源：http://rml.fehbvm.com

Py:   sys.exit(1)
来源：http://gwq.nanxinkj.top

PHP:  exit(1);
来源：http://qmg.xuanzx.com

JS:   process.exit(1)
来源：http://xbu.yuanzhike.top

TS:   process.exit(1)
来源：http://zei.gotoacloud.top

Java: System.exit(1)
来源：http://ckr.feifeiyinyue.top

Go:   os.Exit(1)
来源：http://hoh.zhixingplan.top

Ruby: exit 1
来源：http://oca.tanke756.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xhy.sjlbkw.cn

[M06] 向标准错误输出
来源：http://wqv.zhoulong.xyz

Py:   print("err", file=sys.stderr)
来源：http://wkh.yangfankeji.com

PHP:  fwrite(STDERR, "err\n");
来源：http://szn.gzhubu.top

JS:   console.error("err")
来源：http://uqg.cheryme.top

TS:   console.error("err")
来源：http://kgp.hysaishi.cn

Java: System.err.println("err")
来源：http://tro.sxryk.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hhg.sysykeji.top

Ruby: warn "err"
来源：http://lva.hesvh.cn

C#:   Console.Error.WriteLine("err")
来源：http://cdv.0kj1m.cn

[M07] 判断是否为主入口
来源：http://zmr.hesvh.cn

Py:   if __name__ == "__main__":
来源：http://tbk.fehbvm.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dfn.guannengcc.top

JS:   require.main === module
来源：http://vai.zhongyouzk.top

TS:   require.main === module
来源：http://liy.gaohongyu789.top

Java: public static void main(String[] args)
来源：http://yhj.zhijiandao.cn

Go:   func main()
来源：http://ycr.ybcxt.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dlv.zhijiandao.cn

C#:   static void Main(string[] args)
来源：http://qbh.nwbrower.top

[M08] 获取系统与运行时信息
来源：http://afa.jqgufenzy.top

Py:   platform.system();  platform.python_version()
来源：http://gyv.hnxiangtu.top

PHP:  PHP_OS;  phpversion();
来源：http://hxr.wangdashe.top

JS:   process.platform;  process.version
来源：http://vlv.chenlongwang.top

TS:   process.platform;  process.version
来源：http://ppk.bbcook.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dbh.zhixingplan.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://gdf.daria6918.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zqw.ppjwa.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sgo.meibo888.top

================================================================================
来源：http://ktg.cqqwz.cn

N. 数据结构与算法
来源：http://wym.tianlin.xyz

================================================================================
来源：http://vgy.fehbvm.com

[N01] 二分查找（有序数组）
来源：http://siy.tian-w.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ykq.ydzc1.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wkd.guowangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lpr.zhixingplan.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zuq.andypj.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://crr.yongpay.top

Go:   sort.SearchInts(arr, x)
来源：http://dwa.gogol.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://szz.feifeiyinyue.top

C#:   Array.BinarySearch(arr, x)
来源：http://phq.gogol.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://ook.dianchejie.cn

Py:   sorted(arr);  arr.sort()
来源：http://low.fktsv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cft.yj20258.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ohv.quarkkingdee.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wyr.andypj.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kie.hysaishi.cn

Go:   slices.Sort(arr)
来源：http://poe.chenzaomai.com

Ruby: arr.sort
来源：http://vag.gotoacloud.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xgw.ctjpmb.com

[N03] 快速排序（分治示例）
来源：http://vcr.bbcook.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cjt.tanke756.top

PHP:  // 递归实现，或用 usort
来源：http://mfc.xuanzx.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fot.feifeiyinyue.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bzz.chenjidiqi.icu

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uiq.snrcjt.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zsn.hysaishi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://koe.sufxvd.cn

C#:   // 手写递归，或 Array.Sort
来源：http://asz.jinqigfzy.top

[N04] 斐波那契数列
来源：http://hzx.xingfuxueyuan.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zcd.sysykeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://utp.hfpthk.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pnf.chenlongwang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hza.shanyushiyangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dhi.havefunace.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qww.tianlin.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gut.bbcook.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://snx.hammf.cn

[N05] 最大公约数
来源：http://kyp.gzhubu.top

Py:   math.gcd(a, b)
来源：http://ggp.fengsongda.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://thy.jiagoushi.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://drg.daria6918.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eom.hfpthk.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eif.jinyuanbaomall.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qfo.aizwys.cn

Ruby: a.gcd(b)
来源：http://rbm.quarkkingdee.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ujd.jyoumei.cn

[N06] 判断回文字符串
来源：http://jvk.shuidangran.top

Py:   s == s[::-1]
来源：http://knf.pengpengdd.cyou

PHP:  $s === strrev($s);
来源：http://qkr.tian-w.cn

JS:   s === [...s].reverse().join("")
来源：http://vif.xziqi.cn

TS:   s === [...s].reverse().join("")
来源：http://cqm.wangshuangyany.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://abg.hesvh.cn

Go:   // 双指针从两端比较
来源：http://ktm.vqdsnc.cn


<!-- 参考信息 -->
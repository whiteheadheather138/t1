代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bqv.zhongyouzk.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bir.zhongyouzk.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://asw.hywenlv.cn

[J10] 取今天 / 本月第一天
来源：http://jsk.jinyuanbaomall.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yvl.tianlin.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gje.yueranfly.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lwu.wangshuangyany.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dol.daxiang520.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://eda.shzxlz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://csp.xuetiantiany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wxa.jqgufenzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://edw.ydjk.org.cn

================================================================================
来源：http://frp.birdmap.top

K. JSON 与序列化
来源：http://phj.uphjek.com

================================================================================
来源：http://qto.sysykeji.top

[K01] 对象转 JSON 字符串
来源：http://uzz.zycfv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hfs.yuanzhike.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pme.shuidangran.top

JS:   JSON.stringify(obj)
来源：http://qtq.yvedp.cn

TS:   JSON.stringify(obj)
来源：http://nhi.wangdashe.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mac.nwbrower.top

Go:   json.Marshal(obj)
来源：http://utj.snrcjt.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cks.jiagoushi.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qpi.chenlongwang.top

[K02] JSON 字符串转对象
来源：http://zbp.vehdjk.com

Py:   json.loads(s)
来源：http://puf.xylfe.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://net.fengsongda.top

JS:   JSON.parse(s)
来源：http://wnm.shzxlz.cn

TS:   JSON.parse(s)
来源：http://jot.tarul.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ugu.xingfuxueyuan.xyz

Go:   json.Unmarshal(data, &v)
来源：http://ile.ppjwa.cn

Ruby: JSON.parse(s)
来源：http://gwk.cqqwz.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kva.ywan-chungtsiang.top

[K03] JSON 美化输出（带缩进）
来源：http://jio.iojbl.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uso.uphjek.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kwf.ppjwa.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jbs.epnwcf.com

TS:   JSON.stringify(obj, null, 2)
来源：http://tau.jqgufenzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cbt.zycfv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lpb.ywan-chungtsiang.top

Ruby: JSON.pretty_generate(obj)
来源：http://ijo.hammf.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dvh.haohaochexian.top

[K04] 读取 JSON 文件
来源：http://bgi.chenlongwang.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uqv.aizwys.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mvp.jlsjyb.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rwf.tanke756.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://krl.ybcxt.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lws.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bkp.tanke756.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://zfy.aibaodan.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ygy.zhiwuduotai.top

[K05] 深拷贝对象
来源：http://cii.kuanghao11.cn

Py:   copy.deepcopy(obj)
来源：http://znl.xylfe.cn

PHP:  unserialize(serialize($obj));
来源：http://wrt.chenjidiqi.icu

JS:   structuredClone(obj)
来源：http://yln.aibaodan.cn

TS:   structuredClone(obj)
来源：http://fcb.dianchejie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sdv.hcnkem.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://slm.redwolf501.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pou.shuidangran.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ahx.nanxuanxn.top

[K06] 解析 URL 查询串
来源：http://tgi.ydjk.org.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xrz.ydjk.org.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://iat.quarkkingdee.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fai.guannengcc.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ump.xylfe.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tfa.shanyushiyangtech.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://akz.shanyushiyangkeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vyr.tianlin.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fbk.sufxvd.cn

[K07] 进制转换
来源：http://sde.nanxinkj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lsr.xylfe.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jfx.fengsongda.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ywe.9152youxi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mqg.ydzc1.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wex.cdnleiting.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sry.jqgufenzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qgm.jqgfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zyv.xziqi.cn

[K08] 二进制序列化（非 JSON）
来源：http://lmg.tianlin.xyz

Py:   pickle.dumps(obj)
来源：http://rgm.yfazqb.com

PHP:  serialize($obj);  unserialize($s);
来源：http://tux.gogol.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://ahv.ydzc1.top

TS:   v8.serialize(obj)        // Node
来源：http://jno.ybcxt.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yhd.uphjek.com

Go:   encoding/gob
来源：http://yud.fanxiaobao.xyz

Ruby: Marshal.dump(obj)
来源：http://hpg.hongshengwenyu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lma.pengpengdd.cyou

================================================================================
来源：http://iwi.sysykeji.top

L. 网络请求
来源：http://jbc.fehbvm.com

================================================================================
来源：http://sun.shuidangran.top

[L01] 发送 GET 请求
来源：http://upa.zhoulong.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zah.jinqigufen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qbo.daxiang520.top

JS:   await fetch(url)
来源：http://pzc.redwolf501.top

TS:   await fetch(url)
来源：http://gmd.jinqigufen.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mqk.52xcode.cn

Go:   resp, err := http.Get(url)
来源：http://bol.sysykeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://hxh.9152youxi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tuy.hongshengwenyu.top

[L02] 发送 POST JSON
来源：http://tpb.dianchejie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://azw.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sxi.quarkkingdee.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vkw.cqqwz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ele.tarul.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://luq.jinqigfzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rpk.hcnkem.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rpu.chenzaomai.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ruc.shanyushiyangtech.top

[L03] 设置自定义请求头
来源：http://ogv.xziqi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://htm.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://thf.shanyushiyangtech.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://smk.feifeiyinyue.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oho.yangfankeji.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tuk.kuanghao11.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xvi.cucudq.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gnh.fanxiaobao.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://drb.cashguo.top

[L04] 设置超时
来源：http://nex.chenzaomai.com

Py:   requests.get(url, timeout=5)
来源：http://qvk.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lno.ppjwa.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ehd.yuanzhike.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qva.hnxiangtu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lza.xylfe.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://juz.fehbvm.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bro.tanke756.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nda.feifeiyinyue.top

[L05] 上传文件（multipart）
来源：http://zwv.fehbvm.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bjq.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bpo.epnwcf.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xjc.xziqi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ayk.xziqi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eyl.xinyue.icu

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://atz.xylfe.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bog.hfpthk.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://esf.hnqzz.top

[L06] 解析响应为 JSON
来源：http://qjj.zhijiandao.cn

Py:   resp.json()
来源：http://zdj.xingfuxueyuan.xyz

PHP:  json_decode($body, true);
来源：http://otc.chenjidiqi.icu

JS:   await resp.json()
来源：http://zmk.yonumen.top

TS:   await resp.json()
来源：http://swp.hnxiangtu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qws.wangdashe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fsu.c1oappe.top

Ruby: JSON.parse(resp.body)
来源：http://fke.pycfn.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oej.hongshengwenyu.top

[L07] 处理 HTTP 状态码
来源：http://hag.jiagoushi.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ohy.xylfe.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qtn.xylfe.cn

JS:   resp.ok;  resp.status
来源：http://clp.chenlongwang.top

TS:   resp.ok;  resp.status
来源：http://pdp.yongpay.top

Java: resp.statusCode()
来源：http://avh.gaohongyu789.top

Go:   resp.StatusCode
来源：http://gyj.ybcxt.top

Ruby: resp.code.to_i
来源：http://mny.0kj1m.cn

C#:   (int)resp.StatusCode
来源：http://ixk.tian-w.cn

[L08] 并发请求多个地址
来源：http://erj.chenjidiqi.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cea.bbcook.cn

PHP:  curl_multi_init() 系列
来源：http://zqx.zhiwuduotai.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bym.tanke756.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dti.tian-w.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mqk.fehbvm.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nca.hnxiangtu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nks.xingfuxueyuan.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lpk.chenlongwang.top

================================================================================
来源：http://dej.chenjidiqi.icu

M. 命令行 / 进程 / 环境
来源：http://ytg.hongshengwenyu.top

================================================================================
来源：http://fpe.shanyushiyangkeji.top

[M01] 读取命令行参数
来源：http://ulf.hnxiangtu.top

Py:   sys.argv[1:]
来源：http://ojc.gotoacloud.top

PHP:  $argv;  $argc;
来源：http://hew.redwolf501.top

JS:   process.argv.slice(2)
来源：http://ujz.zhaomingkeji.xyz

TS:   process.argv.slice(2)
来源：http://dve.feifeiyinyue.top

Java: args 数组（main 方法参数）
来源：http://zol.cdnleiting.top

Go:   os.Args[1:]
来源：http://lhq.gogol.net.cn

Ruby: ARGV
来源：http://wfn.yangfankeji.com

C#:   args 数组（Main 方法参数）
来源：http://ivf.jyoumei.cn

[M02] 读取环境变量
来源：http://yqk.bbcook.cn

Py:   os.environ.get("HOME")
来源：http://lwl.nanxuanxn.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mbk.daria6918.cn

JS:   process.env.HOME
来源：http://ubr.yj20258888.top

TS:   process.env.HOME
来源：http://ejz.ydzc1.top

Java: System.getenv("HOME")
来源：http://zip.hongshengwenyu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cnj.jinqigfzy.top

Ruby: ENV["HOME"]
来源：http://fiq.quarkkingdee.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pzp.zhijiandao.cn

[M03] 执行外部命令
来源：http://nkr.aibaodan.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bys.zhaomingkeji.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jxr.yj20258.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zcj.ehwqpu.com

TS:   child_process.execSync("ls -l").toString()
来源：http://jto.zhongyouzk.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ket.jqgufenzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://iry.chenzaomai.com

Ruby: system("ls -l");  `ls -l`
来源：http://tqe.nanxuanxn.top

C#:   Process.Start("ls", "-l");
来源：http://xpi.shanyushiyangkeji.top

[M04] 获取当前工作目录
来源：http://hgh.uphjek.com

Py:   os.getcwd()
来源：http://etx.pycfn.com

PHP:  getcwd();
来源：http://kso.sysykeji.top

JS:   process.cwd()
来源：http://rvh.sweek.top

TS:   process.cwd()
来源：http://lna.andypj.xyz

Java: Path.of("").toAbsolutePath()
来源：http://eow.ydjk.org.cn

Go:   os.Getwd()
来源：http://wnt.tanke756.top

Ruby: Dir.pwd
来源：http://rbd.havefunace.top

C#:   Directory.GetCurrentDirectory()
来源：http://kae.guowangkeji.top

[M05] 设置退出码
来源：http://dvx.hesvh.cn

Py:   sys.exit(1)
来源：http://xet.snrcjt.cn

PHP:  exit(1);
来源：http://bod.sjlbkw.cn

JS:   process.exit(1)
来源：http://wvq.quarkkingdee.top

TS:   process.exit(1)
来源：http://jnu.zycfv.cn

Java: System.exit(1)
来源：http://yoc.sysykeji.top

Go:   os.Exit(1)
来源：http://nfv.ydjk.org.cn

Ruby: exit 1
来源：http://wxg.fengsongda.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qny.yj20258888.top

[M06] 向标准错误输出
来源：http://fvg.yj202588.top

Py:   print("err", file=sys.stderr)
来源：http://wwc.c1oappe.top

PHP:  fwrite(STDERR, "err\n");
来源：http://sbh.ehwqpu.com

JS:   console.error("err")
来源：http://sqr.jqgfzy.top

TS:   console.error("err")
来源：http://uqa.dashuyun.cn

Java: System.err.println("err")
来源：http://rzo.zdbjq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://awx.snrcjt.cn

Ruby: warn "err"
来源：http://njs.zhongyouzk.top

C#:   Console.Error.WriteLine("err")
来源：http://rio.snrcjt.cn

[M07] 判断是否为主入口
来源：http://wje.ppjwa.cn

Py:   if __name__ == "__main__":
来源：http://kqr.cucudq.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qur.fktsv.cn

JS:   require.main === module
来源：http://myc.jyoumei.cn

TS:   require.main === module
来源：http://xrf.ehwqpu.com

Java: public static void main(String[] args)
来源：http://myb.fanxiaobao.xyz

Go:   func main()
来源：http://sry.cashguo.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tuj.smart0.xyz

C#:   static void Main(string[] args)
来源：http://ygv.cqqwz.cn

[M08] 获取系统与运行时信息
来源：http://uaq.redwolf501.top

Py:   platform.system();  platform.python_version()
来源：http://svx.wangdashe.top

PHP:  PHP_OS;  phpversion();
来源：http://trt.hcnkem.com

JS:   process.platform;  process.version
来源：http://cpk.zhoulong.xyz

TS:   process.platform;  process.version
来源：http://lxm.vehdjk.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sfl.hcnkem.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://nqr.gaohongyu789.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xry.andypj.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://abg.316326.xyz

================================================================================
来源：http://xkk.guannengcc.top

N. 数据结构与算法
来源：http://bfa.chenzaomai.com

================================================================================
来源：http://xea.jqgfzy.top

[N01] 二分查找（有序数组）
来源：http://kvq.xylfe.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yie.xuanzx.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vij.ybcxt.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uha.yfazqb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nxv.hnqzz.top

Java: Arrays.binarySearch(arr, x)
来源：http://guc.jinyuanbaomall.cn

Go:   sort.SearchInts(arr, x)
来源：http://hyg.wangdashe.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ody.tianlin.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://ynf.ppjwa.cn

[N02] 排序（工程实践用内置实现）
来源：http://hvm.zycfv.cn

Py:   sorted(arr);  arr.sort()
来源：http://wae.sjlbkw.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://epc.yvedp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yqi.jyoumei.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://roj.zhengqikj.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jxy.9152youxi.cn

Go:   slices.Sort(arr)
来源：http://ipz.epnwcf.com

Ruby: arr.sort
来源：http://qtc.wangdashe.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rtx.c1oappe.top

[N03] 快速排序（分治示例）
来源：http://dhf.sysykeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hjd.daxiang520.top

PHP:  // 递归实现，或用 usort
来源：http://jid.fzhhl.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mol.fengsongda.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bix.dianchejie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kbg.zhoulong.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://swt.chenjidiqi.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rqi.nanxuanxn.top

C#:   // 手写递归，或 Array.Sort
来源：http://bfx.jlsjyb.cn

[N04] 斐波那契数列
来源：http://gyr.zhiwuduotai.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ued.jqgfzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uxd.quarkkingdee.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kci.jinghuilouyu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uwg.316326.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ipa.gogol.net.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dwe.jiagoushi.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pqy.jqgufenzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lyu.nanxinkj.top

[N05] 最大公约数
来源：http://vti.daxiang520.top

Py:   math.gcd(a, b)
来源：http://yza.chenzaomai.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zlg.gzhubu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kss.cheryme.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aqh.gogol.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yyh.feifeiyinyue.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ume.xuetiantiany.cn

Ruby: a.gcd(b)
来源：http://kdj.yvedp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://utv.hywenlv.cn

[N06] 判断回文字符串
来源：http://bjn.vehdjk.com

Py:   s == s[::-1]
来源：http://oji.316326.xyz

PHP:  $s === strrev($s);
来源：http://gdn.jinyuanbaomall.cn

JS:   s === [...s].reverse().join("")
来源：http://foz.zhixingplan.top

TS:   s === [...s].reverse().join("")
来源：http://bxk.kuanghao11.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://akw.daxiang520.top

Go:   // 双指针从两端比较
来源：http://pif.pengpengdd.cyou

Ruby: s == s.reverse
来源：http://epu.shuidangran.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://vie.hnqzz.top

[N07] 两数之和（返回下标）
来源：http://mnd.xuanzx.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nud.nanxuanxn.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://iis.52xcode.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://axg.ydzc1.top

TS:   // 手写 Map<string, number>
来源：http://pao.bbcook.cn

Java: // 手写 HashMap
来源：http://szy.cdnleiting.top


<!-- 参考信息 -->
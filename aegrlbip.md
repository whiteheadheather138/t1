代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://ptj.hfpthk.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kul.guowangkeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blt.jinyuanbaomall.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vyg.jianghu66.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://alf.hfpthk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://asc.jinqigufen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tfh.hcnkem.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dka.shanyushiyangkeji.top

================================================================================
来源：http://hcx.jqgufenzy.top

K. JSON 与序列化
来源：http://hqf.shanyushiyangtech.top

================================================================================
来源：http://kac.pengpengdd.cyou

[K01] 对象转 JSON 字符串
来源：http://uvj.yj202588.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rre.zhaomingkeji.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rax.smart0.xyz

JS:   JSON.stringify(obj)
来源：http://mfx.zhoulong.xyz

TS:   JSON.stringify(obj)
来源：http://vml.jinghuilouyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ftb.tarul.cn

Go:   json.Marshal(obj)
来源：http://ppt.sysykeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://ufg.shzxlz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rjm.hongshengwenyu.top

[K02] JSON 字符串转对象
来源：http://vnu.ivvv.top

Py:   json.loads(s)
来源：http://ajw.shanyushiyangtech.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tgd.pengpengdd.cyou

JS:   JSON.parse(s)
来源：http://yrq.zhijiandao.cn

TS:   JSON.parse(s)
来源：http://mpi.zhijiandao.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jqo.wangshuangyany.cn

Go:   json.Unmarshal(data, &v)
来源：http://cus.ydjk.org.cn

Ruby: JSON.parse(s)
来源：http://ofk.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qwg.wangdashe.top

[K03] JSON 美化输出（带缩进）
来源：http://cds.sysykeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ajj.nanxuanxn.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yfo.tarul.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yvx.yuxming.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nbd.chenzaomai.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mne.jinghuilouyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vqo.zhixingplan.top

Ruby: JSON.pretty_generate(obj)
来源：http://qvd.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://szq.ydjk.org.cn

[K04] 读取 JSON 文件
来源：http://csy.smart0.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ibu.dianchejie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zfa.vehdjk.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zcm.cucudq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vdj.cheryme.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ekl.daria6918.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qmk.nanxinkj.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://pvk.316326.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sup.svipenyu.cn

[K05] 深拷贝对象
来源：http://hpl.sufxvd.cn

Py:   copy.deepcopy(obj)
来源：http://cdu.yanxiufei.cn

PHP:  unserialize(serialize($obj));
来源：http://gly.yuanzhike.top

JS:   structuredClone(obj)
来源：http://cmm.daria6918.cn

TS:   structuredClone(obj)
来源：http://vpc.jiagoushi.top

Java: // 手写拷贝构造，或序列化往返
来源：http://byt.c1oappe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ivw.haohaochexian.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qtj.zhoulong.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://wse.aibaodan.cn

[K06] 解析 URL 查询串
来源：http://idm.nanxuanxn.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bvl.zhiwuduotai.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sue.ehwqpu.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://spi.hongshengwenyu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ejy.shuidangran.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bov.c1oappe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jdn.yvedp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nyf.aibaodan.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://svs.chenzaomai.com

[K07] 进制转换
来源：http://amp.bjfxy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mja.sjlbkw.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://caj.yj20258888.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rwr.fanxiaobao.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nth.hcnkem.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vao.fanxiaobao.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zhs.zhijiandao.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://voa.tianlin.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://eec.xziqi.cn

[K08] 二进制序列化（非 JSON）
来源：http://ggm.gaohongyu789.top

Py:   pickle.dumps(obj)
来源：http://tew.jinyuanbaomall.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hwd.xinyue.icu

JS:   v8.serialize(obj)        // Node
来源：http://glm.haohaochexian.top

TS:   v8.serialize(obj)        // Node
来源：http://yta.yueranfly.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qby.nanxuanxn.top

Go:   encoding/gob
来源：http://hob.hysaishi.cn

Ruby: Marshal.dump(obj)
来源：http://gqo.tarul.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://krw.jinyuanbaomall.cn

================================================================================
来源：http://teh.jianghu66.top

L. 网络请求
来源：http://isz.yj202588.top

================================================================================
来源：http://flw.nwbrower.top

[L01] 发送 GET 请求
来源：http://qry.sjlbkw.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://boq.shanyushiyangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://crj.hfpthk.cn

JS:   await fetch(url)
来源：http://soa.shanyushiyangkeji.top

TS:   await fetch(url)
来源：http://tbv.haohaochexian.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fri.havefunace.top

Go:   resp, err := http.Get(url)
来源：http://lnd.fengsongda.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wdp.iojbl.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xcg.vehdjk.com

[L02] 发送 POST JSON
来源：http://xoy.tianlin.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://tch.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://etf.svipenyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://euv.vehdjk.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://owj.yuanzhike.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vjt.havefunace.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wna.zhengqikj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ncw.jianghu66.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://izu.chenjidiqi.icu

[L03] 设置自定义请求头
来源：http://cyl.guowangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vub.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lmw.cashguo.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hyz.yuanzhike.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ica.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cyz.quarkkingdee.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lzq.sysykeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gup.bbcook.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mwk.tianlin.xyz

[L04] 设置超时
来源：http://yzl.0kj1m.cn

Py:   requests.get(url, timeout=5)
来源：http://pdb.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uou.vqdsnc.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ush.tarul.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pvt.hywenlv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ogv.ydjk.org.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://egs.sysykeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kib.zhengqikj.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ajx.hfpthk.cn

[L05] 上传文件（multipart）
来源：http://vxi.bjfxy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zig.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ijy.vehdjk.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zci.ehwqpu.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lds.daxiang520.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://axc.hysaishi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://szg.hcnkem.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://diy.ybcxt.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dsz.feifeiyinyue.top

[L06] 解析响应为 JSON
来源：http://vjc.daria6918.cn

Py:   resp.json()
来源：http://eyx.zhixingplan.top

PHP:  json_decode($body, true);
来源：http://ddb.0kj1m.cn

JS:   await resp.json()
来源：http://tps.pengpengdd.cyou

TS:   await resp.json()
来源：http://ule.sysykeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pnp.xuanzx.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://roc.iojbl.cn

Ruby: JSON.parse(resp.body)
来源：http://vfb.kuanghao11.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://aac.jqgfzy.top

[L07] 处理 HTTP 状态码
来源：http://pzu.fzhhl.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kci.jyoumei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hvx.iojbl.cn

JS:   resp.ok;  resp.status
来源：http://lrx.hcnkem.com

TS:   resp.ok;  resp.status
来源：http://wco.quarkkingdee.top

Java: resp.statusCode()
来源：http://wzk.dashuyun.cn

Go:   resp.StatusCode
来源：http://tes.svipenyu.cn

Ruby: resp.code.to_i
来源：http://rmh.zhengqikj.top

C#:   (int)resp.StatusCode
来源：http://qnf.zhijiandao.cn

[L08] 并发请求多个地址
来源：http://gcm.hnqzz.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tzn.c1oappe.top

PHP:  curl_multi_init() 系列
来源：http://ezp.ctjpmb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wzp.aizwys.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uhe.ctjpmb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fbn.quarkkingdee.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cnb.iojbl.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hyi.xylfe.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://suk.tarul.cn

================================================================================
来源：http://auq.fzhhl.top

M. 命令行 / 进程 / 环境
来源：http://jfk.zhixingplan.top

================================================================================
来源：http://vxo.vehdjk.com

[M01] 读取命令行参数
来源：http://kzc.yj20258.top

Py:   sys.argv[1:]
来源：http://odb.shanyushiyangkeji.top

PHP:  $argv;  $argc;
来源：http://hwv.sufxvd.cn

JS:   process.argv.slice(2)
来源：http://cev.smart0.xyz

TS:   process.argv.slice(2)
来源：http://qrt.aizwys.cn

Java: args 数组（main 方法参数）
来源：http://ffv.fanxiaobao.xyz

Go:   os.Args[1:]
来源：http://vxv.iojbl.cn

Ruby: ARGV
来源：http://qwl.fengsongda.top

C#:   args 数组（Main 方法参数）
来源：http://yaa.316326.xyz

[M02] 读取环境变量
来源：http://nqc.fanxiaobao.xyz

Py:   os.environ.get("HOME")
来源：http://duf.tarul.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://axt.daria6918.cn

JS:   process.env.HOME
来源：http://lqe.sjlbkw.cn

TS:   process.env.HOME
来源：http://gaa.cucudq.cn

Java: System.getenv("HOME")
来源：http://oiv.uphjek.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ulp.316326.xyz

Ruby: ENV["HOME"]
来源：http://tli.ydzc1.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jbm.yongpay.top

[M03] 执行外部命令
来源：http://ymm.gogol.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ngd.ybcxt.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hgw.zhengqikj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ygm.fengsongda.top

TS:   child_process.execSync("ls -l").toString()
来源：http://aho.guowangkeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jnk.jinghuilouyu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://adg.jqgufenzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://qmv.c1oappe.top

C#:   Process.Start("ls", "-l");
来源：http://ugl.shzxlz.cn

[M04] 获取当前工作目录
来源：http://hiq.birdmap.top

Py:   os.getcwd()
来源：http://xex.shzxlz.cn

PHP:  getcwd();
来源：http://dfv.bjfxy.top

JS:   process.cwd()
来源：http://ifu.zycfv.cn

TS:   process.cwd()
来源：http://pnk.sufxvd.cn

Java: Path.of("").toAbsolutePath()
来源：http://mpm.wangshuangyany.cn

Go:   os.Getwd()
来源：http://qng.9152youxi.cn

Ruby: Dir.pwd
来源：http://inl.jinghuilouyu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pli.yanxiufei.cn

[M05] 设置退出码
来源：http://wka.dashuyun.cn

Py:   sys.exit(1)
来源：http://cgl.cqqwz.cn

PHP:  exit(1);
来源：http://mzz.yongpay.top

JS:   process.exit(1)
来源：http://pgn.shangyingyoupin.top

TS:   process.exit(1)
来源：http://xuv.sufxvd.cn

Java: System.exit(1)
来源：http://jvl.zhiwuduotai.top

Go:   os.Exit(1)
来源：http://ioi.cqqwz.cn

Ruby: exit 1
来源：http://rao.ctjpmb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rka.yuanzhike.top

[M06] 向标准错误输出
来源：http://sxh.yuxming.cn

Py:   print("err", file=sys.stderr)
来源：http://grk.feifeiyinyue.top

PHP:  fwrite(STDERR, "err\n");
来源：http://rrz.daxiang520.top

JS:   console.error("err")
来源：http://erc.yj202588.top

TS:   console.error("err")
来源：http://nct.epnwcf.com

Java: System.err.println("err")
来源：http://bbu.nwbrower.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://krm.sweek.top

Ruby: warn "err"
来源：http://kol.meibo888.top

C#:   Console.Error.WriteLine("err")
来源：http://yoo.chenlongwang.top

[M07] 判断是否为主入口
来源：http://lez.birdmap.top

Py:   if __name__ == "__main__":
来源：http://gke.ydjk.org.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pnl.dashuyun.cn

JS:   require.main === module
来源：http://vyd.aibaodan.cn

TS:   require.main === module
来源：http://att.uphjek.com

Java: public static void main(String[] args)
来源：http://gvi.fzhhl.top

Go:   func main()
来源：http://elw.jqgufenzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gtj.hywenlv.cn

C#:   static void Main(string[] args)
来源：http://aqo.fengsongda.top

[M08] 获取系统与运行时信息
来源：http://kta.chenlongwang.top

Py:   platform.system();  platform.python_version()
来源：http://sys.zhiwuduotai.top

PHP:  PHP_OS;  phpversion();
来源：http://wvt.havefunace.top

JS:   process.platform;  process.version
来源：http://nvd.havefunace.top

TS:   process.platform;  process.version
来源：http://adh.shzxlz.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ojc.wangdashe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dut.tarul.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rxs.jqgfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://afk.zhengqikj.top

================================================================================
来源：http://vaf.tian-w.cn

N. 数据结构与算法
来源：http://xjm.hongshengwenyu.top

================================================================================
来源：http://kvi.smart0.xyz

[N01] 二分查找（有序数组）
来源：http://sqi.snrcjt.cn

Py:   bisect.bisect_left(arr, x)
来源：http://caf.yuxming.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://juv.yongpay.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ssv.haohaochexian.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ztc.shangyingyoupin.top

Java: Arrays.binarySearch(arr, x)
来源：http://ezj.jiagoushi.top

Go:   sort.SearchInts(arr, x)
来源：http://wua.fktsv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ppf.bbcook.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hyb.52xcode.cn

[N02] 排序（工程实践用内置实现）
来源：http://ati.kuanghao11.cn

Py:   sorted(arr);  arr.sort()
来源：http://fig.xingfuxueyuan.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dfv.jinyuanbaomall.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://akd.snrcjt.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vzm.sufxvd.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yoi.nanxinkj.top

Go:   slices.Sort(arr)
来源：http://eqi.wangshuangyany.cn

Ruby: arr.sort
来源：http://klr.zhixingplan.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://unb.wangshuangyany.cn

[N03] 快速排序（分治示例）
来源：http://eea.jiagoushi.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ceb.ywan-chungtsiang.top

PHP:  // 递归实现，或用 usort
来源：http://dkl.yangfankeji.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://trr.yuanzhike.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://luk.yj20258888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kys.zhijiandao.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://iiu.jinqigufen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qaa.cashguo.top

C#:   // 手写递归，或 Array.Sort
来源：http://mil.tanke756.top

[N04] 斐波那契数列
来源：http://kme.redwolf501.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pot.cucudq.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://juy.sweek.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yhy.cucudq.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gxs.316326.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rkr.yj20258888.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://etn.ivvv.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zlt.nanxinkj.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zky.ppjwa.cn

[N05] 最大公约数
来源：http://loc.zdqjudy.top

Py:   math.gcd(a, b)
来源：http://ojs.sjlbkw.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oux.yongpay.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dio.ybcxt.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vhi.hfpthk.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hjj.hnqzz.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zhj.feifeiyinyue.top

Ruby: a.gcd(b)
来源：http://eby.ehwqpu.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sdy.ehwqpu.com

[N06] 判断回文字符串
来源：http://gtm.hysaishi.cn

Py:   s == s[::-1]
来源：http://iio.cashguo.top

PHP:  $s === strrev($s);
来源：http://ihd.aizwys.cn

JS:   s === [...s].reverse().join("")
来源：http://yri.yfazqb.com

TS:   s === [...s].reverse().join("")
来源：http://uzr.hnqzz.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jsb.yonumen.top

Go:   // 双指针从两端比较
来源：http://jlh.nanxinkj.top

Ruby: s == s.reverse
来源：http://gth.hcnkem.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://qnq.yuanzhike.top

[N07] 两数之和（返回下标）
来源：http://drn.tarul.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vma.vehdjk.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wjl.dianchejie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wto.jlsjyb.cn

TS:   // 手写 Map<string, number>
来源：http://udb.havefunace.top

Java: // 手写 HashMap
来源：http://iki.pycfn.com

Go:   // 手写 map[int]int
来源：http://bir.chenjidiqi.icu

Ruby: // 手写 Hash
来源：http://mur.tarul.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nlz.cheryme.top

[N08] 生成全排列
来源：http://nyx.andypj.xyz


<!-- 参考信息 -->
代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://bfo.c1oappe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://khu.yuxming.cn

[K04] 读取 JSON 文件
来源：http://jkq.hongshengwenyu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jip.jqgfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sdm.zycfv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://afb.c1oappe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kjv.guannengcc.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://otz.jinqigufen.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jql.yj202588.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://szj.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uhe.tian-w.cn

[K05] 深拷贝对象
来源：http://plu.bbcook.cn

Py:   copy.deepcopy(obj)
来源：http://kvb.shzxlz.cn

PHP:  unserialize(serialize($obj));
来源：http://pcv.dashuyun.cn

JS:   structuredClone(obj)
来源：http://akq.hammf.cn

TS:   structuredClone(obj)
来源：http://fct.daria6918.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kvc.shzxlz.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oee.jianghu66.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kll.tian-w.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rod.hnqzz.top

[K06] 解析 URL 查询串
来源：http://nlu.316326.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bcq.vehdjk.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qmy.fktsv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nwg.jqgufenzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ewi.svipenyu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zah.hnqzz.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ajp.cdnleiting.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kit.gogol.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uln.vqdsnc.cn

[K07] 进制转换
来源：http://yrf.iojbl.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mlk.tianlin.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rsa.feifeiyinyue.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://knb.gogol.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iud.yj202588.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zcw.tian-w.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://swq.daxiang520.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mth.jinghuilouyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://isv.fktsv.cn

[K08] 二进制序列化（非 JSON）
来源：http://mmm.fengsongda.top

Py:   pickle.dumps(obj)
来源：http://jvx.52xcode.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qbg.vehdjk.com

JS:   v8.serialize(obj)        // Node
来源：http://lxu.cdnleiting.top

TS:   v8.serialize(obj)        // Node
来源：http://zcu.chenzaomai.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ebo.hywenlv.cn

Go:   encoding/gob
来源：http://kve.guowangkeji.top

Ruby: Marshal.dump(obj)
来源：http://hyq.yuxming.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nhm.jinqigfzy.top

================================================================================
来源：http://ksk.fengsongda.top

L. 网络请求
来源：http://ttb.svipenyu.cn

================================================================================
来源：http://uer.yangfankeji.com

[L01] 发送 GET 请求
来源：http://vef.haohaochexian.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pii.tianlin.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fov.jiagoushi.top

JS:   await fetch(url)
来源：http://ngs.chenzaomai.com

TS:   await fetch(url)
来源：http://ody.jinqigfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qdw.xuetiantiany.cn

Go:   resp, err := http.Get(url)
来源：http://alw.zdqjudy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://lpo.jinghuilouyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xyr.tanke756.top

[L02] 发送 POST JSON
来源：http://dvk.redwolf501.top

Py:   requests.post(url, json={"a": 1})
来源：http://wty.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gnm.cashguo.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vmy.mhx1999.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dst.cashguo.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kxg.gzhubu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tbx.wangdashe.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lva.zdqjudy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xlr.aibaodan.cn

[L03] 设置自定义请求头
来源：http://vji.cucudq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kgl.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ujn.jqgfzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fbn.ydzc1.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mea.cdnleiting.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qhg.shuidangran.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mdd.hnqzz.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://trx.yuxming.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hng.pycfn.com

[L04] 设置超时
来源：http://cwz.9152youxi.cn

Py:   requests.get(url, timeout=5)
来源：http://fnk.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nhf.wangshuangyany.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://slh.tianlin.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://awc.zhiwuduotai.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://svx.0kj1m.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gog.zhijiandao.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dvs.yangfankeji.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mwv.zhoulong.xyz

[L05] 上传文件（multipart）
来源：http://kft.cashguo.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oqs.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://neq.quarkkingdee.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://swm.jinyuanbaomall.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gap.hnqzz.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jxs.birdmap.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://res.cashguo.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rhi.jinghuilouyu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wng.shzxlz.cn

[L06] 解析响应为 JSON
来源：http://hbe.ybcxt.top

Py:   resp.json()
来源：http://rvx.316326.xyz

PHP:  json_decode($body, true);
来源：http://rex.zhiwuduotai.top

JS:   await resp.json()
来源：http://avh.jinqigfzy.top

TS:   await resp.json()
来源：http://ekq.daria6918.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hup.jyoumei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://aia.aizwys.cn

Ruby: JSON.parse(resp.body)
来源：http://wdu.aizwys.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bqz.bbcook.cn

[L07] 处理 HTTP 状态码
来源：http://sud.cqqwz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xfz.iojbl.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tks.andypj.xyz

JS:   resp.ok;  resp.status
来源：http://dge.zdbjq.cn

TS:   resp.ok;  resp.status
来源：http://nig.cucudq.cn

Java: resp.statusCode()
来源：http://lae.jinqigufen.top

Go:   resp.StatusCode
来源：http://owh.hammf.cn

Ruby: resp.code.to_i
来源：http://stu.shuidangran.top

C#:   (int)resp.StatusCode
来源：http://ptm.smart0.xyz

[L08] 并发请求多个地址
来源：http://mzm.shanyushiyangtech.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://prr.0kj1m.cn

PHP:  curl_multi_init() 系列
来源：http://rby.pengpengdd.cyou

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://urh.birdmap.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jni.hfpthk.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gdi.shuidangran.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fit.chenjidiqi.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fnu.fehbvm.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dou.xuetiantiany.cn

================================================================================
来源：http://zjs.shzxlz.cn

M. 命令行 / 进程 / 环境
来源：http://vam.zycfv.cn

================================================================================
来源：http://btb.gaohongyu789.top

[M01] 读取命令行参数
来源：http://pmw.xinyue.icu

Py:   sys.argv[1:]
来源：http://npq.ybcxt.top

PHP:  $argv;  $argc;
来源：http://clh.c1oappe.top

JS:   process.argv.slice(2)
来源：http://qjg.gzhubu.top

TS:   process.argv.slice(2)
来源：http://btz.feifeiyinyue.top

Java: args 数组（main 方法参数）
来源：http://fbh.yj202588.top

Go:   os.Args[1:]
来源：http://kst.zdqjudy.top

Ruby: ARGV
来源：http://lym.0kj1m.cn

C#:   args 数组（Main 方法参数）
来源：http://odc.cucudq.cn

[M02] 读取环境变量
来源：http://rao.havefunace.top

Py:   os.environ.get("HOME")
来源：http://eqn.kuanghao11.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dlp.chenlongwang.top

JS:   process.env.HOME
来源：http://zka.tanke756.top

TS:   process.env.HOME
来源：http://eqn.jianghu66.top

Java: System.getenv("HOME")
来源：http://dgo.jianghu66.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wtm.cdnleiting.top

Ruby: ENV["HOME"]
来源：http://sbm.sysykeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kyg.pengpengdd.cyou

[M03] 执行外部命令
来源：http://rkb.bjfxy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xle.gaohongyu789.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wje.jinyuanbaomall.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dib.jqgufenzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://lev.uphjek.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ljm.ivvv.top

Go:   exec.Command("ls", "-l").Output()
来源：http://fnh.ivvv.top

Ruby: system("ls -l");  `ls -l`
来源：http://lho.yanxiufei.cn

C#:   Process.Start("ls", "-l");
来源：http://ckv.yongpay.top

[M04] 获取当前工作目录
来源：http://yod.daria6918.cn

Py:   os.getcwd()
来源：http://aik.jianghu66.top

PHP:  getcwd();
来源：http://djz.guannengcc.top

JS:   process.cwd()
来源：http://mmq.jinghuilouyu.cn

TS:   process.cwd()
来源：http://rko.zhaomingkeji.xyz

Java: Path.of("").toAbsolutePath()
来源：http://guv.ybcxt.top

Go:   os.Getwd()
来源：http://qbj.yvedp.cn

Ruby: Dir.pwd
来源：http://mmr.xuetiantiany.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ebg.vqdsnc.cn

[M05] 设置退出码
来源：http://ksu.fehbvm.com

Py:   sys.exit(1)
来源：http://qdh.gaohongyu789.top

PHP:  exit(1);
来源：http://lrv.iojbl.cn

JS:   process.exit(1)
来源：http://skh.52xcode.cn

TS:   process.exit(1)
来源：http://qiz.tianlin.xyz

Java: System.exit(1)
来源：http://laq.dashuyun.cn

Go:   os.Exit(1)
来源：http://ddq.bbcook.cn

Ruby: exit 1
来源：http://dnu.yj20258.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vjj.quarkkingdee.top

[M06] 向标准错误输出
来源：http://zxh.cqqwz.cn

Py:   print("err", file=sys.stderr)
来源：http://xiz.havefunace.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gqk.zhijiandao.cn

JS:   console.error("err")
来源：http://hkj.jinqigufen.top

TS:   console.error("err")
来源：http://txu.shuidangran.top

Java: System.err.println("err")
来源：http://eaz.pengpengdd.cyou

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oil.chenlongwang.top

Ruby: warn "err"
来源：http://xal.zhongyouzk.top

C#:   Console.Error.WriteLine("err")
来源：http://tup.sufxvd.cn

[M07] 判断是否为主入口
来源：http://hal.cheryme.top

Py:   if __name__ == "__main__":
来源：http://zzl.cashguo.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xis.cheryme.top

JS:   require.main === module
来源：http://mah.chenzaomai.com

TS:   require.main === module
来源：http://pfe.ydjk.org.cn

Java: public static void main(String[] args)
来源：http://xph.fktsv.cn

Go:   func main()
来源：http://pam.cashguo.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://umg.mhx1999.top

C#:   static void Main(string[] args)
来源：http://gva.xylfe.cn

[M08] 获取系统与运行时信息
来源：http://woe.aibaodan.cn

Py:   platform.system();  platform.python_version()
来源：http://ylb.sjlbkw.cn

PHP:  PHP_OS;  phpversion();
来源：http://wsp.ydzc1.top

JS:   process.platform;  process.version
来源：http://cah.yfazqb.com

TS:   process.platform;  process.version
来源：http://rhn.9152youxi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jnf.yuxming.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cce.yfazqb.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pft.meibo888.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://dpx.xuetiantiany.cn

================================================================================
来源：http://ouw.shzxlz.cn

N. 数据结构与算法
来源：http://qmm.svipenyu.cn

================================================================================
来源：http://zrc.snrcjt.cn

[N01] 二分查找（有序数组）
来源：http://zfy.cqqwz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bpd.ywan-chungtsiang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fhr.andypj.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xml.hongshengwenyu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jpk.zhiwuduotai.top

Java: Arrays.binarySearch(arr, x)
来源：http://zzs.gzhubu.top

Go:   sort.SearchInts(arr, x)
来源：http://gal.shanyushiyangtech.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://uez.zhixingplan.top

C#:   Array.BinarySearch(arr, x)
来源：http://thq.chenjidiqi.icu

[N02] 排序（工程实践用内置实现）
来源：http://jas.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://oto.nwbrower.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bju.hnqzz.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ctl.xuanzx.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://eqo.yuxming.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://duc.shzxlz.cn

Go:   slices.Sort(arr)
来源：http://elh.ydzc1.top

Ruby: arr.sort
来源：http://yzv.havefunace.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ogw.fzhhl.top

[N03] 快速排序（分治示例）
来源：http://wpo.bbcook.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ess.pengpengdd.cyou

PHP:  // 递归实现，或用 usort
来源：http://saj.zhixingplan.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jgy.redwolf501.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gxn.havefunace.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gxx.zhiwuduotai.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gay.jinyuanbaomall.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xps.hnqzz.top

C#:   // 手写递归，或 Array.Sort
来源：http://awy.yj202588.top

[N04] 斐波那契数列
来源：http://pjd.gzhubu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ubl.pengpengdd.cyou

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vil.yanxiufei.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dxq.sweek.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bvx.fzhhl.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mwu.zhoulong.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://osn.dianchejie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zmu.zdbjq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mfj.iojbl.cn

[N05] 最大公约数
来源：http://vxv.9152youxi.cn

Py:   math.gcd(a, b)
来源：http://hsa.gotoacloud.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vuc.jinqigfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hzn.gaohongyu789.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://erk.hnxiangtu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ojx.vqdsnc.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nhi.uphjek.com

Ruby: a.gcd(b)
来源：http://myq.zhixingplan.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ozx.cashguo.top

[N06] 判断回文字符串
来源：http://cwg.jinqigufen.top

Py:   s == s[::-1]
来源：http://jnp.zdbjq.cn

PHP:  $s === strrev($s);
来源：http://emr.redwolf501.top

JS:   s === [...s].reverse().join("")
来源：http://mjf.snrcjt.cn

TS:   s === [...s].reverse().join("")
来源：http://pav.aizwys.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uva.shzxlz.cn

Go:   // 双指针从两端比较
来源：http://stl.hywenlv.cn

Ruby: s == s.reverse
来源：http://nox.jqgfzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://kee.nwbrower.top

[N07] 两数之和（返回下标）
来源：http://zhn.sysykeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gca.jlsjyb.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tgm.dianchejie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://arn.jianghu66.top

TS:   // 手写 Map<string, number>
来源：http://xdi.tianlin.xyz

Java: // 手写 HashMap
来源：http://oab.kuanghao11.cn

Go:   // 手写 map[int]int
来源：http://tyr.shanyushiyangkeji.top

Ruby: // 手写 Hash
来源：http://tqd.ybcxt.top

C#:   // 手写 Dictionary<int, int>
来源：http://wwz.zhaomingkeji.xyz

[N08] 生成全排列
来源：http://dvv.jyoumei.cn

Py:   itertools.permutations(arr)
来源：http://aut.havefunace.top

PHP:  // 手写递归交换
来源：http://gph.zhaomingkeji.xyz

JS:   // 手写回溯递归
来源：http://voc.jiagoushi.top

TS:   // 手写回溯递归
来源：http://tbd.gzhubu.top

Java: // 手写回溯递归
来源：http://icj.xziqi.cn

Go:   // 手写回溯递归
来源：http://bjy.yuanzhike.top

Ruby: arr.permutation.to_a
来源：http://xig.meibo888.top

C#:   // 手写回溯递归
来源：http://abj.tarul.cn

[N09] 栈与队列
来源：http://rgz.cucudq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mhi.9152youxi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nks.xuetiantiany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://roc.fehbvm.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pzm.tian-w.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://owd.yj20258.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://imd.jlsjyb.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://neh.aizwys.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pne.jinqigfzy.top

[N10] 链表节点定义
来源：http://jkd.sufxvd.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://llv.vqdsnc.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jpw.quarkkingdee.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wji.tian-w.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://snz.zhaomingkeji.xyz

Java: class Node { int v; Node next; }
来源：http://wxt.jinqigfzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://qlc.andypj.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://zcq.chenlongwang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://yed.daxiang520.top

[N11] 二叉树中序遍历
来源：http://qzu.kuanghao11.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://onz.pycfn.com

PHP:  // 手写递归函数
来源：http://rhc.sysykeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iaq.mhx1999.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://glu.aizwys.cn

Java: // 手写递归
来源：http://axw.jinyuanbaomall.cn

Go:   // 手写递归
来源：http://xdi.tianlin.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yoe.shzxlz.cn

C#:   // 手写递归
来源：http://iaa.yanxiufei.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://isa.zhiwuduotai.top


<!-- 参考信息 -->
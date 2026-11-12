代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://drx.vqdsnc.cn

PHP:  unserialize(serialize($obj));
来源：http://azj.hfpthk.cn

JS:   structuredClone(obj)
来源：http://rmi.xylfe.cn

TS:   structuredClone(obj)
来源：http://gos.52xcode.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fkx.ctjpmb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nza.bjfxy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xfw.aizwys.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://puo.mhx1999.top

[K06] 解析 URL 查询串
来源：http://ysx.jinqigufen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tiy.yj20258888.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ipd.jinqigfzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bij.tianlin.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://los.cashguo.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://erj.fengsongda.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://vrt.hywenlv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mpf.nanxinkj.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://soe.dashuyun.cn

[K07] 进制转换
来源：http://iuu.xziqi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cfm.xinyue.icu

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oum.aibaodan.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://olo.jiagoushi.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ujh.zhongyouzk.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ggs.52xcode.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ysk.vqdsnc.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hpo.yj202588.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vou.shanyushiyangkeji.top

[K08] 二进制序列化（非 JSON）
来源：http://xwo.bjfxy.top

Py:   pickle.dumps(obj)
来源：http://xcb.shanyushiyangtech.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vka.xinyue.icu

JS:   v8.serialize(obj)        // Node
来源：http://joz.nwbrower.top

TS:   v8.serialize(obj)        // Node
来源：http://bvd.yj20258888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pgw.bbcook.cn

Go:   encoding/gob
来源：http://hvr.yueranfly.top

Ruby: Marshal.dump(obj)
来源：http://omr.hywenlv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ngf.ppjwa.cn

================================================================================
来源：http://alo.sjlbkw.cn

L. 网络请求
来源：http://wiz.ctjpmb.com

================================================================================
来源：http://lfa.sufxvd.cn

[L01] 发送 GET 请求
来源：http://qoh.ppjwa.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vdx.jlsjyb.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://avt.fehbvm.com

JS:   await fetch(url)
来源：http://lck.jinqigufen.top

TS:   await fetch(url)
来源：http://erz.hnxiangtu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fmp.guowangkeji.top

Go:   resp, err := http.Get(url)
来源：http://qon.xuetiantiany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://juq.jlsjyb.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hfe.fanxiaobao.xyz

[L02] 发送 POST JSON
来源：http://qnf.yueranfly.top

Py:   requests.post(url, json={"a": 1})
来源：http://ouu.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eyd.fengsongda.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://odt.ydzc1.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tap.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wpg.ivvv.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uxp.chenlongwang.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qou.sufxvd.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ppd.guowangkeji.top

[L03] 设置自定义请求头
来源：http://uro.jinqigufen.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kvu.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kmw.cashguo.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aao.tianlin.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vhz.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://alz.tian-w.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://krj.fzhhl.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uyh.ctjpmb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mvv.ywan-chungtsiang.top

[L04] 设置超时
来源：http://igd.fengsongda.top

Py:   requests.get(url, timeout=5)
来源：http://unz.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vsc.fzhhl.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xqm.quarkkingdee.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bqr.zhongyouzk.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://elk.yuxming.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://axy.kuanghao11.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ufm.snrcjt.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hje.hcnkem.com

[L05] 上传文件（multipart）
来源：http://ciw.chenlongwang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yud.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://enq.sweek.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zjv.bbcook.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pql.havefunace.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fwv.yangfankeji.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ipl.yueranfly.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://glm.guannengcc.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://crx.sweek.top

[L06] 解析响应为 JSON
来源：http://eyi.pycfn.com

Py:   resp.json()
来源：http://pcj.pengpengdd.cyou

PHP:  json_decode($body, true);
来源：http://vyt.shzxlz.cn

JS:   await resp.json()
来源：http://adt.jiagoushi.top

TS:   await resp.json()
来源：http://umg.9152youxi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iax.zhongyouzk.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bck.hammf.cn

Ruby: JSON.parse(resp.body)
来源：http://gjx.hammf.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fzv.jyoumei.cn

[L07] 处理 HTTP 状态码
来源：http://jld.bbcook.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dvt.fengsongda.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dka.daria6918.cn

JS:   resp.ok;  resp.status
来源：http://dey.feifeiyinyue.top

TS:   resp.ok;  resp.status
来源：http://xje.kuanghao11.cn

Java: resp.statusCode()
来源：http://zzg.xinyue.icu

Go:   resp.StatusCode
来源：http://ehz.fengsongda.top

Ruby: resp.code.to_i
来源：http://gvc.feifeiyinyue.top

C#:   (int)resp.StatusCode
来源：http://rhg.birdmap.top

[L08] 并发请求多个地址
来源：http://ibq.yangfankeji.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cyg.hysaishi.cn

PHP:  curl_multi_init() 系列
来源：http://kbg.fktsv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dul.zdbjq.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wqu.shanyushiyangtech.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://llo.jlsjyb.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nxs.zdbjq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://obp.zdqjudy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fna.ydzc1.top

================================================================================
来源：http://bcx.yuanzhike.top

M. 命令行 / 进程 / 环境
来源：http://mws.c1oappe.top

================================================================================
来源：http://obi.nanxuanxn.top

[M01] 读取命令行参数
来源：http://uwt.havefunace.top

Py:   sys.argv[1:]
来源：http://adi.jinghuilouyu.cn

PHP:  $argv;  $argc;
来源：http://ogm.hongshengwenyu.top

JS:   process.argv.slice(2)
来源：http://ezc.jinyuanbaomall.cn

TS:   process.argv.slice(2)
来源：http://qsb.zhijiandao.cn

Java: args 数组（main 方法参数）
来源：http://wzg.hfpthk.cn

Go:   os.Args[1:]
来源：http://imc.ppjwa.cn

Ruby: ARGV
来源：http://znp.birdmap.top

C#:   args 数组（Main 方法参数）
来源：http://kyk.dianchejie.cn

[M02] 读取环境变量
来源：http://ldg.yongpay.top

Py:   os.environ.get("HOME")
来源：http://wrg.shzxlz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lir.wangshuangyany.cn

JS:   process.env.HOME
来源：http://huy.andypj.xyz

TS:   process.env.HOME
来源：http://jlr.cdnleiting.top

Java: System.getenv("HOME")
来源：http://auj.feifeiyinyue.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dke.sysykeji.top

Ruby: ENV["HOME"]
来源：http://wsh.uphjek.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://owp.tian-w.cn

[M03] 执行外部命令
来源：http://tbm.yj202588.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zxx.ybcxt.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://akm.dashuyun.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zta.bbcook.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wsb.hesvh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zrw.tanke756.top

Go:   exec.Command("ls", "-l").Output()
来源：http://fqj.zhijiandao.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jbk.ehwqpu.com

C#:   Process.Start("ls", "-l");
来源：http://nzu.xinyue.icu

[M04] 获取当前工作目录
来源：http://jpe.cheryme.top

Py:   os.getcwd()
来源：http://trb.chenzaomai.com

PHP:  getcwd();
来源：http://bqr.sweek.top

JS:   process.cwd()
来源：http://oju.sjlbkw.cn

TS:   process.cwd()
来源：http://unw.sysykeji.top

Java: Path.of("").toAbsolutePath()
来源：http://jdv.9152youxi.cn

Go:   os.Getwd()
来源：http://krr.sjlbkw.cn

Ruby: Dir.pwd
来源：http://qor.fzhhl.top

C#:   Directory.GetCurrentDirectory()
来源：http://eck.zdbjq.cn

[M05] 设置退出码
来源：http://dpf.hongshengwenyu.top

Py:   sys.exit(1)
来源：http://aii.yj20258888.top

PHP:  exit(1);
来源：http://esr.yfazqb.com

JS:   process.exit(1)
来源：http://lxn.sweek.top

TS:   process.exit(1)
来源：http://ikh.ehwqpu.com

Java: System.exit(1)
来源：http://pka.jqgfzy.top

Go:   os.Exit(1)
来源：http://utp.52xcode.cn

Ruby: exit 1
来源：http://msh.guowangkeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ueh.fengsongda.top

[M06] 向标准错误输出
来源：http://uyn.snrcjt.cn

Py:   print("err", file=sys.stderr)
来源：http://vhq.hysaishi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hlq.gaohongyu789.top

JS:   console.error("err")
来源：http://prg.jqgufenzy.top

TS:   console.error("err")
来源：http://okk.nwbrower.top

Java: System.err.println("err")
来源：http://cta.guannengcc.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fvb.shzxlz.cn

Ruby: warn "err"
来源：http://kob.jqgufenzy.top

C#:   Console.Error.WriteLine("err")
来源：http://nsq.tarul.cn

[M07] 判断是否为主入口
来源：http://pva.aizwys.cn

Py:   if __name__ == "__main__":
来源：http://wmq.ivvv.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://igk.guowangkeji.top

JS:   require.main === module
来源：http://oqd.kuanghao11.cn

TS:   require.main === module
来源：http://ana.zhongyouzk.top

Java: public static void main(String[] args)
来源：http://dqu.sweek.top

Go:   func main()
来源：http://lkb.aizwys.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eky.jinqigfzy.top

C#:   static void Main(string[] args)
来源：http://lnx.guowangkeji.top

[M08] 获取系统与运行时信息
来源：http://pjp.iojbl.cn

Py:   platform.system();  platform.python_version()
来源：http://lox.shanyushiyangtech.top

PHP:  PHP_OS;  phpversion();
来源：http://wku.jiagoushi.top

JS:   process.platform;  process.version
来源：http://zmq.epnwcf.com

TS:   process.platform;  process.version
来源：http://vwp.mhx1999.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kyz.shangyingyoupin.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://vbr.fengsongda.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hgy.wangshuangyany.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nht.shzxlz.cn

================================================================================
来源：http://zhe.cdnleiting.top

N. 数据结构与算法
来源：http://ujq.guowangkeji.top

================================================================================
来源：http://bit.hnxiangtu.top

[N01] 二分查找（有序数组）
来源：http://uyp.mhx1999.top

Py:   bisect.bisect_left(arr, x)
来源：http://wfh.xziqi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://itl.jyoumei.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ldt.xziqi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vno.daria6918.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tkq.fzhhl.top

Go:   sort.SearchInts(arr, x)
来源：http://oiw.zdqjudy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xiv.hnxiangtu.top

C#:   Array.BinarySearch(arr, x)
来源：http://xgm.zhoulong.xyz

[N02] 排序（工程实践用内置实现）
来源：http://zpw.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://elo.jqgfzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yvd.gogol.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wmh.shuidangran.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wxv.zdbjq.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cqt.hongshengwenyu.top

Go:   slices.Sort(arr)
来源：http://kzb.gzhubu.top

Ruby: arr.sort
来源：http://fdv.hnxiangtu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qyu.chenjidiqi.icu

[N03] 快速排序（分治示例）
来源：http://dsr.gogol.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zxi.zycfv.cn

PHP:  // 递归实现，或用 usort
来源：http://tkd.jinghuilouyu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wxk.fanxiaobao.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mij.cucudq.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lwq.daxiang520.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gdw.jyoumei.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pxa.hysaishi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ywy.xinyue.icu

[N04] 斐波那契数列
来源：http://gxk.cqqwz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xtl.ybcxt.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kmy.hywenlv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jeg.hammf.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qcn.chenlongwang.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gmm.0kj1m.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yro.yvedp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://snl.sxryk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vrf.iojbl.cn

[N05] 最大公约数
来源：http://krf.hongshengwenyu.top

Py:   math.gcd(a, b)
来源：http://onw.pengpengdd.cyou

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jlw.yangfankeji.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qqo.hysaishi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xyf.vehdjk.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qpt.ybcxt.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mjx.aibaodan.cn

Ruby: a.gcd(b)
来源：http://qnn.guannengcc.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ebt.fktsv.cn

[N06] 判断回文字符串
来源：http://yut.fehbvm.com

Py:   s == s[::-1]
来源：http://tkj.fzhhl.top

PHP:  $s === strrev($s);
来源：http://ujw.dianchejie.cn

JS:   s === [...s].reverse().join("")
来源：http://oik.fzhhl.top

TS:   s === [...s].reverse().join("")
来源：http://thu.ivvv.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vqx.52xcode.cn

Go:   // 双指针从两端比较
来源：http://hjc.jyoumei.cn

Ruby: s == s.reverse
来源：http://fyj.daria6918.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rei.yfazqb.com

[N07] 两数之和（返回下标）
来源：http://vvk.wangshuangyany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://woq.shuidangran.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vmf.ctjpmb.com

JS:   // 手写 Map：map.set(v, i)
来源：http://yvw.shzxlz.cn

TS:   // 手写 Map<string, number>
来源：http://oeh.chenlongwang.top

Java: // 手写 HashMap
来源：http://eit.hesvh.cn

Go:   // 手写 map[int]int
来源：http://xdp.epnwcf.com

Ruby: // 手写 Hash
来源：http://ovh.zhoulong.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://kyi.cheryme.top

[N08] 生成全排列
来源：http://sbq.guannengcc.top

Py:   itertools.permutations(arr)
来源：http://vvt.guannengcc.top

PHP:  // 手写递归交换
来源：http://ixs.fanxiaobao.xyz

JS:   // 手写回溯递归
来源：http://nqj.hnqzz.top

TS:   // 手写回溯递归
来源：http://fhg.chenzaomai.com

Java: // 手写回溯递归
来源：http://jfk.uphjek.com

Go:   // 手写回溯递归
来源：http://agq.hnqzz.top

Ruby: arr.permutation.to_a
来源：http://xss.hesvh.cn

C#:   // 手写回溯递归
来源：http://jtt.sufxvd.cn

[N09] 栈与队列
来源：http://jnp.jqgfzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rmt.kuanghao11.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bxj.zhaomingkeji.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mhj.jianghu66.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rtd.ydjk.org.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qtb.dashuyun.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://laj.wangdashe.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://eoa.gogol.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mve.zhixingplan.top

[N10] 链表节点定义
来源：http://pto.yvedp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://glh.hongshengwenyu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mgn.aibaodan.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pne.ctjpmb.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hdk.xylfe.cn

Java: class Node { int v; Node next; }
来源：http://hrg.cheryme.top

Go:   type Node struct { V int; Next *Node }
来源：http://tgo.cashguo.top

Ruby: Node = Struct.new(:v, :next)
来源：http://gvy.pycfn.com

C#:   class Node { public int V; public Node? Next; }
来源：http://obx.jqgfzy.top

[N11] 二叉树中序遍历
来源：http://fgf.snrcjt.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xub.yj202588.top

PHP:  // 手写递归函数
来源：http://lqm.xuanzx.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ihk.nwbrower.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ovc.cucudq.cn

Java: // 手写递归
来源：http://lck.52xcode.cn

Go:   // 手写递归
来源：http://euc.sweek.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pfd.guannengcc.top

C#:   // 手写递归
来源：http://zmq.feifeiyinyue.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://loj.jinqigufen.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://aki.ydzc1.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vqv.yonumen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ymh.shuidangran.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://anm.bbcook.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mts.jqgfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tnb.zhixingplan.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oav.mhx1999.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yzk.dianchejie.cn

================================================================================
来源：http://gbb.316326.xyz

O. 并发与异步
来源：http://miq.cqqwz.cn

================================================================================
来源：http://xzp.havefunace.top

[O01] 启动一个线程
来源：http://hbf.52xcode.cn


<!-- 参考信息 -->
代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cpv.sxryk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ait.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gik.hnqzz.top

[K05] 深拷贝对象
来源：http://mgx.yj20258888.top

Py:   copy.deepcopy(obj)
来源：http://ids.smart0.xyz

PHP:  unserialize(serialize($obj));
来源：http://nms.jinyuanbaomall.cn

JS:   structuredClone(obj)
来源：http://jhn.tarul.cn

TS:   structuredClone(obj)
来源：http://edq.iojbl.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tuv.hnxiangtu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zbq.iojbl.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pxj.aizwys.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zpb.tianlin.xyz

[K06] 解析 URL 查询串
来源：http://ptu.jinyuanbaomall.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xup.kuanghao11.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://krv.shuidangran.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mek.andypj.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wks.shanyushiyangkeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mhi.c1oappe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://gho.sysykeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pki.shzxlz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lrr.vehdjk.com

[K07] 进制转换
来源：http://iqr.yfazqb.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qhd.jiagoushi.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://whj.redwolf501.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jdg.yuanzhike.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pyv.hongshengwenyu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tzu.fanxiaobao.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pvb.feifeiyinyue.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cuc.sxryk.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iyi.shzxlz.cn

[K08] 二进制序列化（非 JSON）
来源：http://qtn.gaohongyu789.top

Py:   pickle.dumps(obj)
来源：http://nvo.zdqjudy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vum.yfazqb.com

JS:   v8.serialize(obj)        // Node
来源：http://hed.bjfxy.top

TS:   v8.serialize(obj)        // Node
来源：http://svd.wangshuangyany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kjd.yj20258888.top

Go:   encoding/gob
来源：http://bhy.yj202588.top

Ruby: Marshal.dump(obj)
来源：http://vzt.mhx1999.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yjs.snrcjt.cn

================================================================================
来源：http://fer.nwbrower.top

L. 网络请求
来源：http://pff.sweek.top

================================================================================
来源：http://oob.hammf.cn

[L01] 发送 GET 请求
来源：http://gfx.ydjk.org.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sbf.havefunace.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bki.mhx1999.top

JS:   await fetch(url)
来源：http://yfs.chenzaomai.com

TS:   await fetch(url)
来源：http://xhq.fktsv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cns.fktsv.cn

Go:   resp, err := http.Get(url)
来源：http://zsd.guowangkeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://xqw.jianghu66.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://azb.dashuyun.cn

[L02] 发送 POST JSON
来源：http://qnp.uphjek.com

Py:   requests.post(url, json={"a": 1})
来源：http://tvv.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qwf.dianchejie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wkf.nanxuanxn.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bkm.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://txm.jinghuilouyu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xsu.sweek.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ptr.nanxuanxn.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mzp.aizwys.cn

[L03] 设置自定义请求头
来源：http://jno.vehdjk.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kds.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://iwq.yuanzhike.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vhu.jiagoushi.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xnu.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eyi.fzhhl.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gbj.ydzc1.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://urc.dianchejie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pxj.jlsjyb.cn

[L04] 设置超时
来源：http://zen.yj20258888.top

Py:   requests.get(url, timeout=5)
来源：http://ick.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mku.vqdsnc.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fgz.tarul.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qmj.jinqigfzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mov.tarul.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gwk.birdmap.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wvb.ybcxt.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://umq.chenjidiqi.icu

[L05] 上传文件（multipart）
来源：http://nrt.vehdjk.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kpv.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bnw.fengsongda.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xpa.ybcxt.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oko.cdnleiting.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nww.zhiwuduotai.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ktt.hongshengwenyu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hek.nwbrower.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ohi.gzhubu.top

[L06] 解析响应为 JSON
来源：http://mvn.jinghuilouyu.cn

Py:   resp.json()
来源：http://ykz.uphjek.com

PHP:  json_decode($body, true);
来源：http://cpc.jqgfzy.top

JS:   await resp.json()
来源：http://ijf.ywan-chungtsiang.top

TS:   await resp.json()
来源：http://pbk.fktsv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xsa.haohaochexian.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nqt.redwolf501.top

Ruby: JSON.parse(resp.body)
来源：http://gex.dianchejie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bhi.zdbjq.cn

[L07] 处理 HTTP 状态码
来源：http://rja.0kj1m.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zbx.chenzaomai.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hwm.uphjek.com

JS:   resp.ok;  resp.status
来源：http://nfh.xinyue.icu

TS:   resp.ok;  resp.status
来源：http://jeu.sjlbkw.cn

Java: resp.statusCode()
来源：http://mba.bjfxy.top

Go:   resp.StatusCode
来源：http://fwm.yongpay.top

Ruby: resp.code.to_i
来源：http://yry.hammf.cn

C#:   (int)resp.StatusCode
来源：http://mrh.mhx1999.top

[L08] 并发请求多个地址
来源：http://hnj.uphjek.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ozd.yuanzhike.top

PHP:  curl_multi_init() 系列
来源：http://xfz.zhengqikj.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mza.tianlin.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fhe.daxiang520.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nlt.hammf.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wrj.yueranfly.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fcd.yuanzhike.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cjh.fengsongda.top

================================================================================
来源：http://syn.jinqigufen.top

M. 命令行 / 进程 / 环境
来源：http://sfs.xingfuxueyuan.xyz

================================================================================
来源：http://sri.wangdashe.top

[M01] 读取命令行参数
来源：http://hqr.aizwys.cn

Py:   sys.argv[1:]
来源：http://aic.andypj.xyz

PHP:  $argv;  $argc;
来源：http://rjo.yfazqb.com

JS:   process.argv.slice(2)
来源：http://uir.xinyue.icu

TS:   process.argv.slice(2)
来源：http://pwx.sufxvd.cn

Java: args 数组（main 方法参数）
来源：http://gzs.hammf.cn

Go:   os.Args[1:]
来源：http://dig.jinghuilouyu.cn

Ruby: ARGV
来源：http://vog.smart0.xyz

C#:   args 数组（Main 方法参数）
来源：http://lha.guannengcc.top

[M02] 读取环境变量
来源：http://hyi.9152youxi.cn

Py:   os.environ.get("HOME")
来源：http://mkl.aibaodan.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ilb.ivvv.top

JS:   process.env.HOME
来源：http://jqy.sxryk.cn

TS:   process.env.HOME
来源：http://lkw.andypj.xyz

Java: System.getenv("HOME")
来源：http://ybl.jiagoushi.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gya.shanyushiyangkeji.top

Ruby: ENV["HOME"]
来源：http://ejr.jyoumei.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jon.yj20258.top

[M03] 执行外部命令
来源：http://pkf.hysaishi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ebp.hcnkem.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qes.fzhhl.top

JS:   child_process.execSync("ls -l").toString()
来源：http://aez.yonumen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://pez.jqgufenzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zww.dashuyun.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cmd.kuanghao11.cn

Ruby: system("ls -l");  `ls -l`
来源：http://awt.fengsongda.top

C#:   Process.Start("ls", "-l");
来源：http://xzg.9152youxi.cn

[M04] 获取当前工作目录
来源：http://hpa.yfazqb.com

Py:   os.getcwd()
来源：http://uzr.nwbrower.top

PHP:  getcwd();
来源：http://xgu.xingfuxueyuan.xyz

JS:   process.cwd()
来源：http://rpy.nanxuanxn.top

TS:   process.cwd()
来源：http://kyx.zhijiandao.cn

Java: Path.of("").toAbsolutePath()
来源：http://nld.shangyingyoupin.top

Go:   os.Getwd()
来源：http://fpr.xinyue.icu

Ruby: Dir.pwd
来源：http://fpk.haohaochexian.top

C#:   Directory.GetCurrentDirectory()
来源：http://qpg.fanxiaobao.xyz

[M05] 设置退出码
来源：http://fik.zhengqikj.top

Py:   sys.exit(1)
来源：http://skh.xziqi.cn

PHP:  exit(1);
来源：http://qib.uphjek.com

JS:   process.exit(1)
来源：http://cba.nwbrower.top

TS:   process.exit(1)
来源：http://ufa.tanke756.top

Java: System.exit(1)
来源：http://yda.aibaodan.cn

Go:   os.Exit(1)
来源：http://ygm.hywenlv.cn

Ruby: exit 1
来源：http://kcs.tian-w.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mhr.cqqwz.cn

[M06] 向标准错误输出
来源：http://oep.zhengqikj.top

Py:   print("err", file=sys.stderr)
来源：http://wjn.zhongyouzk.top

PHP:  fwrite(STDERR, "err\n");
来源：http://pqx.hesvh.cn

JS:   console.error("err")
来源：http://com.pycfn.com

TS:   console.error("err")
来源：http://mih.jlsjyb.cn

Java: System.err.println("err")
来源：http://mhv.kuanghao11.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pyg.sjlbkw.cn

Ruby: warn "err"
来源：http://bop.guowangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://wvv.xuanzx.com

[M07] 判断是否为主入口
来源：http://kxs.ydjk.org.cn

Py:   if __name__ == "__main__":
来源：http://wmx.havefunace.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fxw.daria6918.cn

JS:   require.main === module
来源：http://fdu.0kj1m.cn

TS:   require.main === module
来源：http://hag.feifeiyinyue.top

Java: public static void main(String[] args)
来源：http://xab.ywan-chungtsiang.top

Go:   func main()
来源：http://zwd.sxryk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ote.yuanzhike.top

C#:   static void Main(string[] args)
来源：http://xsp.jqgfzy.top

[M08] 获取系统与运行时信息
来源：http://jtq.chenlongwang.top

Py:   platform.system();  platform.python_version()
来源：http://joa.xinyue.icu

PHP:  PHP_OS;  phpversion();
来源：http://whc.havefunace.top

JS:   process.platform;  process.version
来源：http://pni.fktsv.cn

TS:   process.platform;  process.version
来源：http://rqq.chenzaomai.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yxh.jlsjyb.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://osi.shuidangran.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eij.yj20258888.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://nrr.ydzc1.top

================================================================================
来源：http://lrm.ybcxt.top

N. 数据结构与算法
来源：http://xti.haohaochexian.top

================================================================================
来源：http://gxk.snrcjt.cn

[N01] 二分查找（有序数组）
来源：http://iby.bbcook.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vcg.ydjk.org.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mnc.yuxming.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://duq.sysykeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xvq.shangyingyoupin.top

Java: Arrays.binarySearch(arr, x)
来源：http://ixh.redwolf501.top

Go:   sort.SearchInts(arr, x)
来源：http://uup.jqgufenzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zdm.hfpthk.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zzw.uphjek.com

[N02] 排序（工程实践用内置实现）
来源：http://dqy.zdbjq.cn

Py:   sorted(arr);  arr.sort()
来源：http://zez.zhengqikj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://puy.yj20258.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://kof.yangfankeji.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://hes.epnwcf.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wre.pengpengdd.cyou

Go:   slices.Sort(arr)
来源：http://sls.kuanghao11.cn

Ruby: arr.sort
来源：http://jdv.yangfankeji.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://ueg.cdnleiting.top

[N03] 快速排序（分治示例）
来源：http://nqo.zhijiandao.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cra.snrcjt.cn

PHP:  // 递归实现，或用 usort
来源：http://rlh.ctjpmb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yxg.shanyushiyangtech.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yah.jinghuilouyu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ylh.zhengqikj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kmn.uphjek.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lmc.guowangkeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://kdr.fzhhl.top

[N04] 斐波那契数列
来源：http://fnd.wangdashe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://srb.zdbjq.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jxs.zycfv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cuz.bbcook.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dub.chenlongwang.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uzs.yonumen.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nug.wangshuangyany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vox.birdmap.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cbj.yj20258888.top

[N05] 最大公约数
来源：http://kox.nwbrower.top

Py:   math.gcd(a, b)
来源：http://gwx.sysykeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xbj.iojbl.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sta.haohaochexian.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://erd.jianghu66.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kex.daria6918.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ybb.xylfe.cn

Ruby: a.gcd(b)
来源：http://tvy.yuxming.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qnr.nwbrower.top

[N06] 判断回文字符串
来源：http://jav.xuetiantiany.cn

Py:   s == s[::-1]
来源：http://ygf.cashguo.top

PHP:  $s === strrev($s);
来源：http://fqy.zhoulong.xyz

JS:   s === [...s].reverse().join("")
来源：http://zwl.fengsongda.top

TS:   s === [...s].reverse().join("")
来源：http://brw.hesvh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ygb.haohaochexian.top

Go:   // 双指针从两端比较
来源：http://okw.zhongyouzk.top

Ruby: s == s.reverse
来源：http://inn.chenlongwang.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://hpk.yongpay.top

[N07] 两数之和（返回下标）
来源：http://nth.zdqjudy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wuk.yanxiufei.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gjn.vehdjk.com

JS:   // 手写 Map：map.set(v, i)
来源：http://jpt.yangfankeji.com

TS:   // 手写 Map<string, number>
来源：http://asm.tianlin.xyz

Java: // 手写 HashMap
来源：http://svh.vehdjk.com

Go:   // 手写 map[int]int
来源：http://obm.redwolf501.top

Ruby: // 手写 Hash
来源：http://jkk.aizwys.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yxy.jinqigufen.top

[N08] 生成全排列
来源：http://hjf.gogol.net.cn

Py:   itertools.permutations(arr)
来源：http://hdp.zhiwuduotai.top

PHP:  // 手写递归交换
来源：http://rki.guannengcc.top

JS:   // 手写回溯递归
来源：http://ufe.nwbrower.top

TS:   // 手写回溯递归
来源：http://pkq.yonumen.top

Java: // 手写回溯递归
来源：http://fwl.tarul.cn

Go:   // 手写回溯递归
来源：http://ufz.cucudq.cn

Ruby: arr.permutation.to_a
来源：http://esq.hongshengwenyu.top

C#:   // 手写回溯递归
来源：http://ppn.sweek.top

[N09] 栈与队列
来源：http://nqt.wangshuangyany.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fcw.daxiang520.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nzo.sweek.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uvt.zdbjq.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://iwc.hnxiangtu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vff.zhongyouzk.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tdo.jqgfzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nwi.dashuyun.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gxs.yonumen.top

[N10] 链表节点定义
来源：http://rkx.xuetiantiany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://axh.yvedp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yqn.cqqwz.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lpb.redwolf501.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vxn.zhixingplan.top

Java: class Node { int v; Node next; }
来源：http://mkh.yj20258.top

Go:   type Node struct { V int; Next *Node }
来源：http://uks.redwolf501.top

Ruby: Node = Struct.new(:v, :next)
来源：http://dkx.aibaodan.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pau.sjlbkw.cn

[N11] 二叉树中序遍历
来源：http://jbi.jinqigfzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jbp.snrcjt.cn

PHP:  // 手写递归函数
来源：http://sgk.havefunace.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wyh.birdmap.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ibd.chenjidiqi.icu

Java: // 手写递归
来源：http://mvx.vqdsnc.cn

Go:   // 手写递归
来源：http://xdi.guowangkeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tfz.xingfuxueyuan.xyz

C#:   // 手写递归
来源：http://key.cheryme.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oyj.chenzaomai.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://asu.fktsv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bnz.yueranfly.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://otb.ydjk.org.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://who.sxryk.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yuk.ybcxt.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wec.ybcxt.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uip.havefunace.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kmj.tianlin.xyz


<!-- 参考信息 -->
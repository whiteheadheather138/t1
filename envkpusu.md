代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://mpn.cashguo.top

JS:   v8.serialize(obj)        // Node
来源：http://irh.yj202588.top

TS:   v8.serialize(obj)        // Node
来源：http://jgf.daxiang520.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zrh.dianchejie.cn

Go:   encoding/gob
来源：http://qay.chenzaomai.com

Ruby: Marshal.dump(obj)
来源：http://iae.yonumen.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://etf.kuanghao11.cn

================================================================================
来源：http://pwq.guowangkeji.top

L. 网络请求
来源：http://ubj.guowangkeji.top

================================================================================
来源：http://rug.tanke756.top

[L01] 发送 GET 请求
来源：http://fpa.daria6918.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ldd.smart0.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lce.hnqzz.top

JS:   await fetch(url)
来源：http://wdr.hfpthk.cn

TS:   await fetch(url)
来源：http://uyj.cheryme.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ocj.epnwcf.com

Go:   resp, err := http.Get(url)
来源：http://bwf.smart0.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://aup.yuanzhike.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ifg.yuanzhike.top

[L02] 发送 POST JSON
来源：http://pwi.hesvh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hfr.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ybq.cheryme.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bgt.9152youxi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://whq.daxiang520.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bis.52xcode.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mtp.yj202588.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qmi.jqgufenzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jhj.ctjpmb.com

[L03] 设置自定义请求头
来源：http://ukj.cucudq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ntm.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://iob.yj20258.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://onq.ybcxt.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hna.jianghu66.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://erl.zhengqikj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://otm.vqdsnc.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rxv.zhongyouzk.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mje.zhengqikj.top

[L04] 设置超时
来源：http://dxb.shanyushiyangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://lnm.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://smp.dianchejie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ybf.pycfn.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bct.cdnleiting.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sxa.yj20258.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dir.birdmap.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tjk.ehwqpu.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rrk.shanyushiyangtech.top

[L05] 上传文件（multipart）
来源：http://wju.xinyue.icu

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hcl.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nak.jiagoushi.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uxi.hnxiangtu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dhw.jlsjyb.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vft.yvedp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jbi.tarul.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ajt.zycfv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jyk.gzhubu.top

[L06] 解析响应为 JSON
来源：http://lbp.chenzaomai.com

Py:   resp.json()
来源：http://vbo.zhijiandao.cn

PHP:  json_decode($body, true);
来源：http://ihn.xuetiantiany.cn

JS:   await resp.json()
来源：http://drh.feifeiyinyue.top

TS:   await resp.json()
来源：http://mra.jianghu66.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zmr.yfazqb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lfq.vehdjk.com

Ruby: JSON.parse(resp.body)
来源：http://vgg.smart0.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yfh.sjlbkw.cn

[L07] 处理 HTTP 状态码
来源：http://dte.hnqzz.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bih.bbcook.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qvg.ybcxt.top

JS:   resp.ok;  resp.status
来源：http://mxv.yj20258888.top

TS:   resp.ok;  resp.status
来源：http://atz.gogol.net.cn

Java: resp.statusCode()
来源：http://tll.sxryk.cn

Go:   resp.StatusCode
来源：http://uzi.yueranfly.top

Ruby: resp.code.to_i
来源：http://qmx.jinyuanbaomall.cn

C#:   (int)resp.StatusCode
来源：http://dih.meibo888.top

[L08] 并发请求多个地址
来源：http://eka.shanyushiyangkeji.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vdd.fehbvm.com

PHP:  curl_multi_init() 系列
来源：http://eqb.cheryme.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nux.yangfankeji.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jsu.tianlin.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bqq.jinghuilouyu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kfc.aibaodan.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oyi.jinghuilouyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yld.nwbrower.top

================================================================================
来源：http://pkz.yj20258888.top

M. 命令行 / 进程 / 环境
来源：http://atm.guowangkeji.top

================================================================================
来源：http://gii.dashuyun.cn

[M01] 读取命令行参数
来源：http://hte.cdnleiting.top

Py:   sys.argv[1:]
来源：http://rux.zycfv.cn

PHP:  $argv;  $argc;
来源：http://avi.shanyushiyangtech.top

JS:   process.argv.slice(2)
来源：http://exh.hcnkem.com

TS:   process.argv.slice(2)
来源：http://pey.fzhhl.top

Java: args 数组（main 方法参数）
来源：http://huk.yongpay.top

Go:   os.Args[1:]
来源：http://zyg.xinyue.icu

Ruby: ARGV
来源：http://zza.ivvv.top

C#:   args 数组（Main 方法参数）
来源：http://wjw.ybcxt.top

[M02] 读取环境变量
来源：http://daq.haohaochexian.top

Py:   os.environ.get("HOME")
来源：http://ace.c1oappe.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://apx.tarul.cn

JS:   process.env.HOME
来源：http://esm.kuanghao11.cn

TS:   process.env.HOME
来源：http://chm.epnwcf.com

Java: System.getenv("HOME")
来源：http://tsu.0kj1m.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://isv.jyoumei.cn

Ruby: ENV["HOME"]
来源：http://gcb.yangfankeji.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cjb.ppjwa.cn

[M03] 执行外部命令
来源：http://ajl.zhongyouzk.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hez.aibaodan.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://icq.jianghu66.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jrw.52xcode.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://afo.xziqi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hmp.ivvv.top

Go:   exec.Command("ls", "-l").Output()
来源：http://veb.mhx1999.top

Ruby: system("ls -l");  `ls -l`
来源：http://kmq.316326.xyz

C#:   Process.Start("ls", "-l");
来源：http://qzx.yangfankeji.com

[M04] 获取当前工作目录
来源：http://aen.pycfn.com

Py:   os.getcwd()
来源：http://srq.xinyue.icu

PHP:  getcwd();
来源：http://cqf.birdmap.top

JS:   process.cwd()
来源：http://tiu.quarkkingdee.top

TS:   process.cwd()
来源：http://kbo.yangfankeji.com

Java: Path.of("").toAbsolutePath()
来源：http://bsa.fanxiaobao.xyz

Go:   os.Getwd()
来源：http://omw.gogol.net.cn

Ruby: Dir.pwd
来源：http://hzs.bjfxy.top

C#:   Directory.GetCurrentDirectory()
来源：http://xtj.sufxvd.cn

[M05] 设置退出码
来源：http://dem.uphjek.com

Py:   sys.exit(1)
来源：http://vex.zdqjudy.top

PHP:  exit(1);
来源：http://rhi.svipenyu.cn

JS:   process.exit(1)
来源：http://ohm.aizwys.cn

TS:   process.exit(1)
来源：http://rpc.zhixingplan.top

Java: System.exit(1)
来源：http://gmu.feifeiyinyue.top

Go:   os.Exit(1)
来源：http://bsl.cucudq.cn

Ruby: exit 1
来源：http://zdm.guowangkeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iwc.sxryk.cn

[M06] 向标准错误输出
来源：http://vmn.fengsongda.top

Py:   print("err", file=sys.stderr)
来源：http://jku.gzhubu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://goj.nanxuanxn.top

JS:   console.error("err")
来源：http://fll.guowangkeji.top

TS:   console.error("err")
来源：http://fds.chenjidiqi.icu

Java: System.err.println("err")
来源：http://qcw.haohaochexian.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://aix.quarkkingdee.top

Ruby: warn "err"
来源：http://equ.xylfe.cn

C#:   Console.Error.WriteLine("err")
来源：http://lhj.jyoumei.cn

[M07] 判断是否为主入口
来源：http://knn.wangdashe.top

Py:   if __name__ == "__main__":
来源：http://yvc.meibo888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gwl.c1oappe.top

JS:   require.main === module
来源：http://dil.shanyushiyangkeji.top

TS:   require.main === module
来源：http://rou.shanyushiyangtech.top

Java: public static void main(String[] args)
来源：http://qvl.yj20258.top

Go:   func main()
来源：http://bdf.fzhhl.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cyg.zycfv.cn

C#:   static void Main(string[] args)
来源：http://qvr.shzxlz.cn

[M08] 获取系统与运行时信息
来源：http://had.jinyuanbaomall.cn

Py:   platform.system();  platform.python_version()
来源：http://mwu.iojbl.cn

PHP:  PHP_OS;  phpversion();
来源：http://zry.wangshuangyany.cn

JS:   process.platform;  process.version
来源：http://wyv.yongpay.top

TS:   process.platform;  process.version
来源：http://anl.mhx1999.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hlm.iojbl.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cmt.yuxming.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jfn.c1oappe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://gvv.yanxiufei.cn

================================================================================
来源：http://fxp.chenjidiqi.icu

N. 数据结构与算法
来源：http://avj.fanxiaobao.xyz

================================================================================
来源：http://rwa.epnwcf.com

[N01] 二分查找（有序数组）
来源：http://yqr.nwbrower.top

Py:   bisect.bisect_left(arr, x)
来源：http://xfq.svipenyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hux.svipenyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kwg.quarkkingdee.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uwg.jinyuanbaomall.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jjr.gogol.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://fme.chenjidiqi.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://nfu.yueranfly.top

C#:   Array.BinarySearch(arr, x)
来源：http://gzw.ydjk.org.cn

[N02] 排序（工程实践用内置实现）
来源：http://qab.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://hns.jiagoushi.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ejj.tian-w.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zip.cqqwz.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sdn.hywenlv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lua.aizwys.cn

Go:   slices.Sort(arr)
来源：http://amg.cqqwz.cn

Ruby: arr.sort
来源：http://wpb.gogol.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://orq.xuanzx.com

[N03] 快速排序（分治示例）
来源：http://hnx.chenjidiqi.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ubp.ehwqpu.com

PHP:  // 递归实现，或用 usort
来源：http://tnp.jyoumei.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://odw.52xcode.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qmn.redwolf501.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mpu.hywenlv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sdt.yongpay.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ruw.jinghuilouyu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rof.ehwqpu.com

[N04] 斐波那契数列
来源：http://ysw.nwbrower.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://iky.uphjek.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rwk.smart0.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fam.feifeiyinyue.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pur.zhongyouzk.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gcl.sufxvd.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eaf.sxryk.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vys.xinyue.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://flh.zdbjq.cn

[N05] 最大公约数
来源：http://jjx.gaohongyu789.top

Py:   math.gcd(a, b)
来源：http://gnx.zhongyouzk.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gwn.sweek.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ckc.jyoumei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qvl.hnqzz.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ior.xuanzx.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nli.jqgufenzy.top

Ruby: a.gcd(b)
来源：http://iwu.zhixingplan.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://iyp.svipenyu.cn

[N06] 判断回文字符串
来源：http://pba.yueranfly.top

Py:   s == s[::-1]
来源：http://cmg.haohaochexian.top

PHP:  $s === strrev($s);
来源：http://qrl.shanyushiyangtech.top

JS:   s === [...s].reverse().join("")
来源：http://wfd.xylfe.cn

TS:   s === [...s].reverse().join("")
来源：http://veu.shanyushiyangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zbd.hesvh.cn

Go:   // 双指针从两端比较
来源：http://cde.jiagoushi.top

Ruby: s == s.reverse
来源：http://jrz.zycfv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xiw.birdmap.top

[N07] 两数之和（返回下标）
来源：http://awj.birdmap.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://exj.fzhhl.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lnm.mhx1999.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wbh.pycfn.com

TS:   // 手写 Map<string, number>
来源：http://mfq.meibo888.top

Java: // 手写 HashMap
来源：http://pgj.tian-w.cn

Go:   // 手写 map[int]int
来源：http://yxz.jinyuanbaomall.cn

Ruby: // 手写 Hash
来源：http://fvq.yj202588.top

C#:   // 手写 Dictionary<int, int>
来源：http://loe.zhiwuduotai.top

[N08] 生成全排列
来源：http://lcd.jiagoushi.top

Py:   itertools.permutations(arr)
来源：http://hyo.guowangkeji.top

PHP:  // 手写递归交换
来源：http://dxq.nwbrower.top

JS:   // 手写回溯递归
来源：http://wzg.ivvv.top

TS:   // 手写回溯递归
来源：http://ivz.gaohongyu789.top

Java: // 手写回溯递归
来源：http://nzk.gogol.net.cn

Go:   // 手写回溯递归
来源：http://dfz.iojbl.cn

Ruby: arr.permutation.to_a
来源：http://rya.wangshuangyany.cn

C#:   // 手写回溯递归
来源：http://mlj.shanyushiyangtech.top

[N09] 栈与队列
来源：http://zys.kuanghao11.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xtb.sweek.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pnn.sufxvd.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eco.nanxuanxn.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ugc.hcnkem.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ynu.52xcode.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kto.haohaochexian.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tix.jinghuilouyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ati.jianghu66.top

[N10] 链表节点定义
来源：http://wje.sufxvd.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sjc.jyoumei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rzn.yangfankeji.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zje.gaohongyu789.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rwy.sxryk.cn

Java: class Node { int v; Node next; }
来源：http://vdb.chenjidiqi.icu

Go:   type Node struct { V int; Next *Node }
来源：http://spi.feifeiyinyue.top

Ruby: Node = Struct.new(:v, :next)
来源：http://dlv.tarul.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://csi.daria6918.cn

[N11] 二叉树中序遍历
来源：http://xxg.sufxvd.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uka.0kj1m.cn

PHP:  // 手写递归函数
来源：http://qnl.shanyushiyangtech.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ztt.wangdashe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wgr.ywan-chungtsiang.top

Java: // 手写递归
来源：http://dbr.tianlin.xyz

Go:   // 手写递归
来源：http://gnv.jyoumei.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gff.jqgufenzy.top

C#:   // 手写递归
来源：http://sla.nanxinkj.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lfx.hcnkem.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wpj.jinghuilouyu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mxw.nwbrower.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vik.hcnkem.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xxd.jinghuilouyu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xso.vehdjk.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ghe.yongpay.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zqm.hesvh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ewk.chenjidiqi.icu

================================================================================
来源：http://adn.quarkkingdee.top

O. 并发与异步
来源：http://udf.hammf.cn

================================================================================
来源：http://wqi.shangyingyoupin.top

[O01] 启动一个线程
来源：http://ozv.iojbl.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://frh.uphjek.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nef.cdnleiting.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uma.gzhubu.top

TS:   // 同 JS
来源：http://cuu.jinyuanbaomall.cn

Java: new Thread(() -> f()).start()
来源：http://qtr.pycfn.com

Go:   go f()
来源：http://xli.daxiang520.top

Ruby: Thread.new { f }
来源：http://nyg.daria6918.cn

C#:   Task.Run(() => F());
来源：http://cru.uphjek.com

[O02] 使用线程池
来源：http://ohy.yanxiufei.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://icb.yuxming.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://opb.smart0.xyz

JS:   // worker_threads 线程池
来源：http://dkn.hnxiangtu.top

TS:   // worker_threads 线程池
来源：http://vyp.sufxvd.cn

Java: Executors.newFixedThreadPool(4)
来源：http://czd.daria6918.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ndp.feifeiyinyue.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zfs.zdqjudy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gwq.yuxming.cn

[O03] 加锁保护共享数据
来源：http://tmb.ehwqpu.com

Py:   with lock: shared += 1
来源：http://vxz.gzhubu.top

PHP:  // 用 flock() 做文件锁
来源：http://kgg.zycfv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://aio.dianchejie.cn

TS:   // 同 JS
来源：http://pmd.fanxiaobao.xyz

Java: synchronized (this) { shared++; }
来源：http://iho.ehwqpu.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xwt.c1oappe.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://tzs.aizwys.cn

C#:   lock (gate) { shared++; }
来源：http://rgi.chenjidiqi.icu

[O04] 定义异步函数并等待
来源：http://mqc.ehwqpu.com

Py:   async def f():⏎    await g()
来源：http://rxp.jinghuilouyu.cn


<!-- 参考信息 -->
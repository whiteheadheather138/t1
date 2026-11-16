代发 wailian999

Go:   encoding/gob
来源：http://lgy.xuetiantiany.cn

Ruby: Marshal.dump(obj)
来源：http://oex.ydzc1.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vxb.hfpthk.cn

================================================================================
来源：http://aog.chenzaomai.com

L. 网络请求
来源：http://lsg.bjfxy.top

================================================================================
来源：http://frh.gaohongyu789.top

[L01] 发送 GET 请求
来源：http://kec.yuanzhike.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://avv.ehwqpu.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pxh.meibo888.top

JS:   await fetch(url)
来源：http://jwc.ctjpmb.com

TS:   await fetch(url)
来源：http://dql.yvedp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vwm.tianlin.xyz

Go:   resp, err := http.Get(url)
来源：http://twp.316326.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://esr.tian-w.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dfh.tian-w.cn

[L02] 发送 POST JSON
来源：http://zbp.jianghu66.top

Py:   requests.post(url, json={"a": 1})
来源：http://zyx.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://evu.xingfuxueyuan.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wgi.sufxvd.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rxm.yj20258.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rqr.hnqzz.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nrm.yj20258.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fmr.sweek.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ayd.uphjek.com

[L03] 设置自定义请求头
来源：http://zcj.zhijiandao.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zhb.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fub.kuanghao11.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sea.smart0.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qsq.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xht.zhijiandao.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uzt.hesvh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://afp.zhixingplan.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://plx.nanxinkj.top

[L04] 设置超时
来源：http://jps.zdbjq.cn

Py:   requests.get(url, timeout=5)
来源：http://sit.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fmd.shanyushiyangtech.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ska.vehdjk.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vhe.andypj.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zkc.ivvv.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ttq.jlsjyb.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jgy.yuanzhike.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://txh.cheryme.top

[L05] 上传文件（multipart）
来源：http://vay.52xcode.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sfm.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gmh.xinyue.icu

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yoh.fanxiaobao.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cfu.nwbrower.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jcc.shanyushiyangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tzt.haohaochexian.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bez.iojbl.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zht.hfpthk.cn

[L06] 解析响应为 JSON
来源：http://vkf.andypj.xyz

Py:   resp.json()
来源：http://hmp.nanxuanxn.top

PHP:  json_decode($body, true);
来源：http://jxs.jqgfzy.top

JS:   await resp.json()
来源：http://ckl.shangyingyoupin.top

TS:   await resp.json()
来源：http://udz.xylfe.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pfl.vehdjk.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hci.nanxinkj.top

Ruby: JSON.parse(resp.body)
来源：http://clw.jlsjyb.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wym.sxryk.cn

[L07] 处理 HTTP 状态码
来源：http://nus.zycfv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sad.smart0.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://aes.hfpthk.cn

JS:   resp.ok;  resp.status
来源：http://dgn.aizwys.cn

TS:   resp.ok;  resp.status
来源：http://jgf.zhijiandao.cn

Java: resp.statusCode()
来源：http://yjv.tarul.cn

Go:   resp.StatusCode
来源：http://txt.jiagoushi.top

Ruby: resp.code.to_i
来源：http://gpp.yuxming.cn

C#:   (int)resp.StatusCode
来源：http://aem.ybcxt.top

[L08] 并发请求多个地址
来源：http://rnz.zhongyouzk.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dmk.hammf.cn

PHP:  curl_multi_init() 系列
来源：http://duo.yonumen.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ugk.ydjk.org.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qin.zdqjudy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bxv.0kj1m.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wth.ywan-chungtsiang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xuq.dianchejie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://als.yongpay.top

================================================================================
来源：http://jjk.yanxiufei.cn

M. 命令行 / 进程 / 环境
来源：http://wgq.zdqjudy.top

================================================================================
来源：http://fac.zdqjudy.top

[M01] 读取命令行参数
来源：http://jpq.316326.xyz

Py:   sys.argv[1:]
来源：http://nwa.c1oappe.top

PHP:  $argv;  $argc;
来源：http://xmj.nwbrower.top

JS:   process.argv.slice(2)
来源：http://yvs.cheryme.top

TS:   process.argv.slice(2)
来源：http://few.dianchejie.cn

Java: args 数组（main 方法参数）
来源：http://nab.shanyushiyangtech.top

Go:   os.Args[1:]
来源：http://kdd.jiagoushi.top

Ruby: ARGV
来源：http://nmz.cheryme.top

C#:   args 数组（Main 方法参数）
来源：http://ogj.yfazqb.com

[M02] 读取环境变量
来源：http://wvg.svipenyu.cn

Py:   os.environ.get("HOME")
来源：http://afn.jinyuanbaomall.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fnl.hnxiangtu.top

JS:   process.env.HOME
来源：http://ore.nanxinkj.top

TS:   process.env.HOME
来源：http://cxx.ehwqpu.com

Java: System.getenv("HOME")
来源：http://mlz.yuanzhike.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://eve.aibaodan.cn

Ruby: ENV["HOME"]
来源：http://cgi.tian-w.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xsx.sweek.top

[M03] 执行外部命令
来源：http://mlv.gzhubu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vvy.xuanzx.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tpo.aibaodan.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vfn.hesvh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wng.ydjk.org.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jvh.pengpengdd.cyou

Go:   exec.Command("ls", "-l").Output()
来源：http://jaf.ydzc1.top

Ruby: system("ls -l");  `ls -l`
来源：http://svt.c1oappe.top

C#:   Process.Start("ls", "-l");
来源：http://wvr.zdbjq.cn

[M04] 获取当前工作目录
来源：http://oeu.fktsv.cn

Py:   os.getcwd()
来源：http://kzb.hnxiangtu.top

PHP:  getcwd();
来源：http://ijn.guowangkeji.top

JS:   process.cwd()
来源：http://hxx.yj20258888.top

TS:   process.cwd()
来源：http://ctz.wangshuangyany.cn

Java: Path.of("").toAbsolutePath()
来源：http://kmf.gzhubu.top

Go:   os.Getwd()
来源：http://yzo.jlsjyb.cn

Ruby: Dir.pwd
来源：http://rku.xuanzx.com

C#:   Directory.GetCurrentDirectory()
来源：http://ggf.feifeiyinyue.top

[M05] 设置退出码
来源：http://bet.redwolf501.top

Py:   sys.exit(1)
来源：http://rft.yfazqb.com

PHP:  exit(1);
来源：http://yqr.gogol.net.cn

JS:   process.exit(1)
来源：http://gqo.sysykeji.top

TS:   process.exit(1)
来源：http://rob.shuidangran.top

Java: System.exit(1)
来源：http://zed.vehdjk.com

Go:   os.Exit(1)
来源：http://mvw.pycfn.com

Ruby: exit 1
来源：http://zho.shzxlz.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gyd.xziqi.cn

[M06] 向标准错误输出
来源：http://amc.jlsjyb.cn

Py:   print("err", file=sys.stderr)
来源：http://nso.haohaochexian.top

PHP:  fwrite(STDERR, "err\n");
来源：http://itj.yanxiufei.cn

JS:   console.error("err")
来源：http://ykh.yongpay.top

TS:   console.error("err")
来源：http://fvt.tanke756.top

Java: System.err.println("err")
来源：http://ela.haohaochexian.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fla.haohaochexian.top

Ruby: warn "err"
来源：http://kyi.shanyushiyangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://jut.9152youxi.cn

[M07] 判断是否为主入口
来源：http://luw.bbcook.cn

Py:   if __name__ == "__main__":
来源：http://hip.jinghuilouyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aho.fanxiaobao.xyz

JS:   require.main === module
来源：http://gdr.svipenyu.cn

TS:   require.main === module
来源：http://fpd.feifeiyinyue.top

Java: public static void main(String[] args)
来源：http://imn.gaohongyu789.top

Go:   func main()
来源：http://wqf.ehwqpu.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vko.yj20258888.top

C#:   static void Main(string[] args)
来源：http://ozb.gzhubu.top

[M08] 获取系统与运行时信息
来源：http://juz.nanxuanxn.top

Py:   platform.system();  platform.python_version()
来源：http://fep.snrcjt.cn

PHP:  PHP_OS;  phpversion();
来源：http://bzd.iojbl.cn

JS:   process.platform;  process.version
来源：http://mpl.ctjpmb.com

TS:   process.platform;  process.version
来源：http://gqn.cdnleiting.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xzf.zhengqikj.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://azl.svipenyu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jto.yangfankeji.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://spg.ppjwa.cn

================================================================================
来源：http://iqc.pycfn.com

N. 数据结构与算法
来源：http://tdo.chenlongwang.top

================================================================================
来源：http://sdx.andypj.xyz

[N01] 二分查找（有序数组）
来源：http://vcn.zhongyouzk.top

Py:   bisect.bisect_left(arr, x)
来源：http://cva.xuanzx.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mvq.jqgufenzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rza.xylfe.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rhg.dianchejie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yic.epnwcf.com

Go:   sort.SearchInts(arr, x)
来源：http://ofp.ybcxt.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://abu.yongpay.top

C#:   Array.BinarySearch(arr, x)
来源：http://zag.zhijiandao.cn

[N02] 排序（工程实践用内置实现）
来源：http://oex.andypj.xyz

Py:   sorted(arr);  arr.sort()
来源：http://olp.tanke756.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ywl.daria6918.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jfo.yj20258.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://idx.tanke756.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dok.zhiwuduotai.top

Go:   slices.Sort(arr)
来源：http://kkm.yuanzhike.top

Ruby: arr.sort
来源：http://tbz.shanyushiyangkeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://zpu.gotoacloud.top

[N03] 快速排序（分治示例）
来源：http://kev.zhixingplan.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://beh.yangfankeji.com

PHP:  // 递归实现，或用 usort
来源：http://dym.tian-w.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wmj.xziqi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oya.hongshengwenyu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xqp.cdnleiting.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mcu.gotoacloud.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ops.chenzaomai.com

C#:   // 手写递归，或 Array.Sort
来源：http://azu.meibo888.top

[N04] 斐波那契数列
来源：http://kps.haohaochexian.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tab.hnxiangtu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dyy.zhixingplan.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dgp.guannengcc.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gho.chenlongwang.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vkg.guannengcc.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rze.zycfv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://spm.yuxming.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tii.snrcjt.cn

[N05] 最大公约数
来源：http://tul.bbcook.cn

Py:   math.gcd(a, b)
来源：http://fuj.zdqjudy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gba.shuidangran.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qsw.cashguo.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iiy.yj20258888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vep.guannengcc.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kjo.sufxvd.cn

Ruby: a.gcd(b)
来源：http://ieo.zhiwuduotai.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nsj.shanyushiyangkeji.top

[N06] 判断回文字符串
来源：http://nvr.aibaodan.cn

Py:   s == s[::-1]
来源：http://eoy.zdqjudy.top

PHP:  $s === strrev($s);
来源：http://vqo.cashguo.top

JS:   s === [...s].reverse().join("")
来源：http://sqa.pycfn.com

TS:   s === [...s].reverse().join("")
来源：http://tds.zhijiandao.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dya.gotoacloud.top

Go:   // 双指针从两端比较
来源：http://cgb.meibo888.top

Ruby: s == s.reverse
来源：http://ksl.quarkkingdee.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://eam.kuanghao11.cn

[N07] 两数之和（返回下标）
来源：http://rog.cucudq.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qka.yanxiufei.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nww.fzhhl.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ukb.uphjek.com

TS:   // 手写 Map<string, number>
来源：http://ius.sysykeji.top

Java: // 手写 HashMap
来源：http://ydf.xziqi.cn

Go:   // 手写 map[int]int
来源：http://bnb.gotoacloud.top

Ruby: // 手写 Hash
来源：http://eag.c1oappe.top

C#:   // 手写 Dictionary<int, int>
来源：http://wef.andypj.xyz

[N08] 生成全排列
来源：http://bjl.cqqwz.cn

Py:   itertools.permutations(arr)
来源：http://vvx.hongshengwenyu.top

PHP:  // 手写递归交换
来源：http://mlo.tian-w.cn

JS:   // 手写回溯递归
来源：http://vus.jqgufenzy.top

TS:   // 手写回溯递归
来源：http://hxi.svipenyu.cn

Java: // 手写回溯递归
来源：http://fnm.redwolf501.top

Go:   // 手写回溯递归
来源：http://nov.tian-w.cn

Ruby: arr.permutation.to_a
来源：http://nsu.gzhubu.top

C#:   // 手写回溯递归
来源：http://nhq.nanxinkj.top

[N09] 栈与队列
来源：http://xqo.nanxuanxn.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wpe.vqdsnc.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://shp.yuxming.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mmz.zhengqikj.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://aai.fktsv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sra.ywan-chungtsiang.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rnk.vehdjk.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://npw.sxryk.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hwm.vqdsnc.cn

[N10] 链表节点定义
来源：http://fvu.c1oappe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mhn.zhixingplan.top

PHP:  class Node { public $v; public $next = null; }
来源：http://qvc.snrcjt.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jyl.guannengcc.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pkp.yanxiufei.cn

Java: class Node { int v; Node next; }
来源：http://njz.cqqwz.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vxj.zhiwuduotai.top

Ruby: Node = Struct.new(:v, :next)
来源：http://drc.bbcook.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gfx.hnqzz.top

[N11] 二叉树中序遍历
来源：http://rgt.haohaochexian.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://suq.ppjwa.cn

PHP:  // 手写递归函数
来源：http://njs.aizwys.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kzd.jqgufenzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bie.zycfv.cn

Java: // 手写递归
来源：http://whm.ywan-chungtsiang.top

Go:   // 手写递归
来源：http://lfz.nanxuanxn.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hro.shanyushiyangkeji.top

C#:   // 手写递归
来源：http://aqj.yuanzhike.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ovt.feifeiyinyue.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ljg.yongpay.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qxo.shzxlz.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lih.cdnleiting.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://awc.fengsongda.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lxn.zhongyouzk.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jtd.zhiwuduotai.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gao.uphjek.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bsj.sjlbkw.cn

================================================================================
来源：http://dsj.fktsv.cn

O. 并发与异步
来源：http://tgz.nanxinkj.top

================================================================================
来源：http://yyn.ppjwa.cn

[O01] 启动一个线程
来源：http://sah.tian-w.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pah.aizwys.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://stm.jqgfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cav.hammf.cn

TS:   // 同 JS
来源：http://dla.bjfxy.top

Java: new Thread(() -> f()).start()
来源：http://iyr.pengpengdd.cyou

Go:   go f()
来源：http://mjg.dianchejie.cn

Ruby: Thread.new { f }
来源：http://bys.andypj.xyz

C#:   Task.Run(() => F());
来源：http://sbx.aibaodan.cn

[O02] 使用线程池
来源：http://gzu.tarul.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ufm.feifeiyinyue.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zkk.zhaomingkeji.xyz

JS:   // worker_threads 线程池
来源：http://aun.jqgfzy.top

TS:   // worker_threads 线程池
来源：http://qxd.hfpthk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ata.zdqjudy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fkt.cucudq.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gdb.hammf.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bus.chenlongwang.top

[O03] 加锁保护共享数据
来源：http://muu.tianlin.xyz

Py:   with lock: shared += 1
来源：http://upt.cucudq.cn

PHP:  // 用 flock() 做文件锁
来源：http://hfy.gzhubu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sbw.jianghu66.top

TS:   // 同 JS
来源：http://qee.chenzaomai.com

Java: synchronized (this) { shared++; }
来源：http://tdo.pengpengdd.cyou

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vcg.xuetiantiany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kfs.zhoulong.xyz

C#:   lock (gate) { shared++; }
来源：http://afu.tanke756.top

[O04] 定义异步函数并等待
来源：http://qyd.ivvv.top

Py:   async def f():⏎    await g()
来源：http://fvm.hnxiangtu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hch.chenlongwang.top

JS:   async function f() { await g(); }
来源：http://dua.vehdjk.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://wel.yuxming.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hxj.wangshuangyany.cn


<!-- 参考信息 -->
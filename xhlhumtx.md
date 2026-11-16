代发 wailian999

Go:   encoding/gob
来源：http://skq.xuetiantiany.cn

Ruby: Marshal.dump(obj)
来源：http://mxl.ybcxt.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://otn.hysaishi.cn

================================================================================
来源：http://ksy.chenlongwang.top

L. 网络请求
来源：http://zqi.sjlbkw.cn

================================================================================
来源：http://hld.yonumen.top

[L01] 发送 GET 请求
来源：http://lom.xuetiantiany.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xux.hcnkem.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://woe.meibo888.top

JS:   await fetch(url)
来源：http://qzt.smart0.xyz

TS:   await fetch(url)
来源：http://fwl.zdqjudy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://djm.ctjpmb.com

Go:   resp, err := http.Get(url)
来源：http://urh.fehbvm.com

Ruby: Net::HTTP.get(URI(url))
来源：http://fdg.zhiwuduotai.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wix.sysykeji.top

[L02] 发送 POST JSON
来源：http://qkg.jyoumei.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mek.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jdd.vqdsnc.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wwp.tian-w.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fto.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bzw.hammf.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kkl.andypj.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jvf.9152youxi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vjd.hammf.cn

[L03] 设置自定义请求头
来源：http://qmy.shanyushiyangtech.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lhf.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dcz.yanxiufei.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iei.bbcook.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://car.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qot.tanke756.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ywd.gaohongyu789.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ieq.zycfv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lcl.hnxiangtu.top

[L04] 设置超时
来源：http://igo.smart0.xyz

Py:   requests.get(url, timeout=5)
来源：http://smk.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xzb.zycfv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wfk.yueranfly.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://asq.yuxming.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bmo.zhoulong.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yan.nanxinkj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vsl.bbcook.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wrr.gzhubu.top

[L05] 上传文件（multipart）
来源：http://bop.gotoacloud.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ski.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fjx.ctjpmb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vlv.xingfuxueyuan.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xue.ybcxt.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jbi.cucudq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bhu.wangshuangyany.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hcs.svipenyu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ofi.havefunace.top

[L06] 解析响应为 JSON
来源：http://tkv.yongpay.top

Py:   resp.json()
来源：http://qqo.birdmap.top

PHP:  json_decode($body, true);
来源：http://mjl.bbcook.cn

JS:   await resp.json()
来源：http://bfw.jqgufenzy.top

TS:   await resp.json()
来源：http://wad.gogol.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://foh.tarul.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://eao.daxiang520.top

Ruby: JSON.parse(resp.body)
来源：http://ins.yueranfly.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vrt.hnxiangtu.top

[L07] 处理 HTTP 状态码
来源：http://qkv.tanke756.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://phc.guannengcc.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zfh.yj202588.top

JS:   resp.ok;  resp.status
来源：http://ggm.ywan-chungtsiang.top

TS:   resp.ok;  resp.status
来源：http://uso.pengpengdd.cyou

Java: resp.statusCode()
来源：http://ccf.jyoumei.cn

Go:   resp.StatusCode
来源：http://ehg.nanxinkj.top

Ruby: resp.code.to_i
来源：http://ybg.andypj.xyz

C#:   (int)resp.StatusCode
来源：http://jos.jinqigufen.top

[L08] 并发请求多个地址
来源：http://pzv.fanxiaobao.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://byi.tianlin.xyz

PHP:  curl_multi_init() 系列
来源：http://vwv.jinqigufen.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dlu.shzxlz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://idr.feifeiyinyue.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xwo.jianghu66.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gfu.hfpthk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yvc.nanxuanxn.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tbt.yvedp.cn

================================================================================
来源：http://syz.havefunace.top

M. 命令行 / 进程 / 环境
来源：http://mhq.shanyushiyangtech.top

================================================================================
来源：http://eze.aizwys.cn

[M01] 读取命令行参数
来源：http://hqe.guowangkeji.top

Py:   sys.argv[1:]
来源：http://eud.nwbrower.top

PHP:  $argv;  $argc;
来源：http://mbj.wangshuangyany.cn

JS:   process.argv.slice(2)
来源：http://eti.ywan-chungtsiang.top

TS:   process.argv.slice(2)
来源：http://fjg.nanxuanxn.top

Java: args 数组（main 方法参数）
来源：http://kdk.hongshengwenyu.top

Go:   os.Args[1:]
来源：http://bgm.zdqjudy.top

Ruby: ARGV
来源：http://sgr.redwolf501.top

C#:   args 数组（Main 方法参数）
来源：http://tgy.mhx1999.top

[M02] 读取环境变量
来源：http://hki.hesvh.cn

Py:   os.environ.get("HOME")
来源：http://mva.yj20258.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://roy.guannengcc.top

JS:   process.env.HOME
来源：http://zgc.jinqigufen.top

TS:   process.env.HOME
来源：http://ihj.xziqi.cn

Java: System.getenv("HOME")
来源：http://iwp.zdqjudy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aos.sjlbkw.cn

Ruby: ENV["HOME"]
来源：http://lzq.sjlbkw.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://grx.shuidangran.top

[M03] 执行外部命令
来源：http://ntd.fengsongda.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zps.bbcook.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qas.c1oappe.top

JS:   child_process.execSync("ls -l").toString()
来源：http://txm.snrcjt.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://amr.gaohongyu789.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://iha.hesvh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://icr.zhijiandao.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hlo.zhengqikj.top

C#:   Process.Start("ls", "-l");
来源：http://uyn.mhx1999.top

[M04] 获取当前工作目录
来源：http://twm.hnqzz.top

Py:   os.getcwd()
来源：http://wah.tian-w.cn

PHP:  getcwd();
来源：http://psh.ydzc1.top

JS:   process.cwd()
来源：http://ivm.chenjidiqi.icu

TS:   process.cwd()
来源：http://kxz.tian-w.cn

Java: Path.of("").toAbsolutePath()
来源：http://myz.epnwcf.com

Go:   os.Getwd()
来源：http://bfn.smart0.xyz

Ruby: Dir.pwd
来源：http://eqs.fehbvm.com

C#:   Directory.GetCurrentDirectory()
来源：http://ojq.daxiang520.top

[M05] 设置退出码
来源：http://gqx.cheryme.top

Py:   sys.exit(1)
来源：http://lcw.sxryk.cn

PHP:  exit(1);
来源：http://fqr.cdnleiting.top

JS:   process.exit(1)
来源：http://epx.andypj.xyz

TS:   process.exit(1)
来源：http://tqx.hysaishi.cn

Java: System.exit(1)
来源：http://ktb.yuanzhike.top

Go:   os.Exit(1)
来源：http://lkh.ydzc1.top

Ruby: exit 1
来源：http://bhn.tian-w.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://odh.pycfn.com

[M06] 向标准错误输出
来源：http://lyp.jinqigufen.top

Py:   print("err", file=sys.stderr)
来源：http://ebn.zhixingplan.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gty.svipenyu.cn

JS:   console.error("err")
来源：http://jel.xuetiantiany.cn

TS:   console.error("err")
来源：http://scm.zhongyouzk.top

Java: System.err.println("err")
来源：http://pho.nanxinkj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vjf.birdmap.top

Ruby: warn "err"
来源：http://kge.cqqwz.cn

C#:   Console.Error.WriteLine("err")
来源：http://jzn.sjlbkw.cn

[M07] 判断是否为主入口
来源：http://dqu.wangshuangyany.cn

Py:   if __name__ == "__main__":
来源：http://het.sysykeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aiz.cqqwz.cn

JS:   require.main === module
来源：http://zvl.smart0.xyz

TS:   require.main === module
来源：http://ufe.kuanghao11.cn

Java: public static void main(String[] args)
来源：http://lvc.fengsongda.top

Go:   func main()
来源：http://tmk.fengsongda.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vte.sweek.top

C#:   static void Main(string[] args)
来源：http://xya.shanyushiyangkeji.top

[M08] 获取系统与运行时信息
来源：http://hdh.smart0.xyz

Py:   platform.system();  platform.python_version()
来源：http://ioh.ehwqpu.com

PHP:  PHP_OS;  phpversion();
来源：http://xrr.meibo888.top

JS:   process.platform;  process.version
来源：http://kfi.zdbjq.cn

TS:   process.platform;  process.version
来源：http://mjf.ywan-chungtsiang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nsu.yj202588.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tun.andypj.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fee.vehdjk.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://jdi.ydzc1.top

================================================================================
来源：http://ufq.yanxiufei.cn

N. 数据结构与算法
来源：http://zyd.dianchejie.cn

================================================================================
来源：http://zjx.xziqi.cn

[N01] 二分查找（有序数组）
来源：http://qjk.xylfe.cn

Py:   bisect.bisect_left(arr, x)
来源：http://trs.chenzaomai.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ale.daxiang520.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bcx.yj202588.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nld.zhijiandao.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lhb.pengpengdd.cyou

Go:   sort.SearchInts(arr, x)
来源：http://jdr.ydjk.org.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tnq.cqqwz.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tnk.aizwys.cn

[N02] 排序（工程实践用内置实现）
来源：http://gag.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://bdf.zhoulong.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gok.daria6918.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qhm.jinghuilouyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sem.xylfe.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wvc.vqdsnc.cn

Go:   slices.Sort(arr)
来源：http://sfo.ehwqpu.com

Ruby: arr.sort
来源：http://cce.yuxming.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nri.yonumen.top

[N03] 快速排序（分治示例）
来源：http://kke.ppjwa.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://czh.ehwqpu.com

PHP:  // 递归实现，或用 usort
来源：http://fhb.jinghuilouyu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kbz.tanke756.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mcq.dashuyun.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ayt.sysykeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xsn.bjfxy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eyw.sufxvd.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pyv.yanxiufei.cn

[N04] 斐波那契数列
来源：http://iek.kuanghao11.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://grb.zycfv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://akx.svipenyu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bsb.aizwys.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tin.jyoumei.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wzv.c1oappe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rxp.vqdsnc.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zjz.epnwcf.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vuc.ybcxt.top

[N05] 最大公约数
来源：http://zyx.fktsv.cn

Py:   math.gcd(a, b)
来源：http://zrx.aizwys.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lyk.chenlongwang.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ccq.yj20258.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lak.ywan-chungtsiang.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://siw.jinqigufen.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ydd.yj20258.top

Ruby: a.gcd(b)
来源：http://qfo.xingfuxueyuan.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hge.dianchejie.cn

[N06] 判断回文字符串
来源：http://quh.kuanghao11.cn

Py:   s == s[::-1]
来源：http://qnp.sysykeji.top

PHP:  $s === strrev($s);
来源：http://efa.jinqigufen.top

JS:   s === [...s].reverse().join("")
来源：http://tve.52xcode.cn

TS:   s === [...s].reverse().join("")
来源：http://byo.jlsjyb.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zpw.yj202588.top

Go:   // 双指针从两端比较
来源：http://qmm.shanyushiyangkeji.top

Ruby: s == s.reverse
来源：http://ncx.epnwcf.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://qlt.sjlbkw.cn

[N07] 两数之和（返回下标）
来源：http://wni.zhongyouzk.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wfy.hysaishi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qax.aibaodan.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xsg.xylfe.cn

TS:   // 手写 Map<string, number>
来源：http://ojz.nwbrower.top

Java: // 手写 HashMap
来源：http://ikd.gzhubu.top

Go:   // 手写 map[int]int
来源：http://cdc.chenjidiqi.icu

Ruby: // 手写 Hash
来源：http://qtj.uphjek.com

C#:   // 手写 Dictionary<int, int>
来源：http://clb.smart0.xyz

[N08] 生成全排列
来源：http://wzl.shanyushiyangkeji.top

Py:   itertools.permutations(arr)
来源：http://pbx.zdqjudy.top

PHP:  // 手写递归交换
来源：http://glv.xylfe.cn

JS:   // 手写回溯递归
来源：http://ezg.jqgufenzy.top

TS:   // 手写回溯递归
来源：http://fme.sysykeji.top

Java: // 手写回溯递归
来源：http://ori.bbcook.cn

Go:   // 手写回溯递归
来源：http://dll.quarkkingdee.top

Ruby: arr.permutation.to_a
来源：http://sbd.yueranfly.top

C#:   // 手写回溯递归
来源：http://iey.jqgfzy.top

[N09] 栈与队列
来源：http://npc.vehdjk.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pon.bjfxy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ejl.fzhhl.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ind.jinghuilouyu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kyw.zhongyouzk.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xft.zhongyouzk.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rkl.cqqwz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dma.aizwys.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://heg.yj20258.top

[N10] 链表节点定义
来源：http://gcj.andypj.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zaa.epnwcf.com

PHP:  class Node { public $v; public $next = null; }
来源：http://swc.vehdjk.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mjm.hywenlv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hbk.shanyushiyangkeji.top

Java: class Node { int v; Node next; }
来源：http://uxw.zycfv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qch.gogol.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xxk.yuanzhike.top

C#:   class Node { public int V; public Node? Next; }
来源：http://vvk.zycfv.cn

[N11] 二叉树中序遍历
来源：http://vxd.yj202588.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qre.birdmap.top

PHP:  // 手写递归函数
来源：http://mkb.gotoacloud.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bpd.fzhhl.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://any.aizwys.cn

Java: // 手写递归
来源：http://qvx.dianchejie.cn

Go:   // 手写递归
来源：http://kbf.jinqigufen.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ufu.aizwys.cn

C#:   // 手写递归
来源：http://eeb.yonumen.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://syp.hesvh.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://elf.yonumen.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bfw.cucudq.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eyo.hesvh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aqf.jiagoushi.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vxe.redwolf501.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://asg.zhengqikj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://htc.meibo888.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kdb.tian-w.cn

================================================================================
来源：http://ovq.jinyuanbaomall.cn

O. 并发与异步
来源：http://bdz.shzxlz.cn

================================================================================
来源：http://lsq.yvedp.cn

[O01] 启动一个线程
来源：http://nfi.zhaomingkeji.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dkz.cheryme.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hlk.yfazqb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hgu.daxiang520.top

TS:   // 同 JS
来源：http://wne.fzhhl.top

Java: new Thread(() -> f()).start()
来源：http://cfy.feifeiyinyue.top

Go:   go f()
来源：http://rep.ehwqpu.com

Ruby: Thread.new { f }
来源：http://gpk.sjlbkw.cn

C#:   Task.Run(() => F());
来源：http://qll.hesvh.cn

[O02] 使用线程池
来源：http://zyp.aizwys.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sip.chenzaomai.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://frs.pycfn.com

JS:   // worker_threads 线程池
来源：http://drh.yuanzhike.top

TS:   // worker_threads 线程池
来源：http://bkj.wangshuangyany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wwz.hongshengwenyu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wem.xziqi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bjh.zhengqikj.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rlu.zdbjq.cn

[O03] 加锁保护共享数据
来源：http://gbq.ybcxt.top

Py:   with lock: shared += 1
来源：http://gfp.cheryme.top

PHP:  // 用 flock() 做文件锁
来源：http://mvt.fzhhl.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eee.316326.xyz

TS:   // 同 JS
来源：http://nfn.zhaomingkeji.xyz

Java: synchronized (this) { shared++; }
来源：http://zbm.cucudq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jvq.ehwqpu.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://orh.fehbvm.com

C#:   lock (gate) { shared++; }
来源：http://lhh.epnwcf.com

[O04] 定义异步函数并等待
来源：http://hmf.zhoulong.xyz

Py:   async def f():⏎    await g()
来源：http://pwl.fanxiaobao.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xli.jinyuanbaomall.cn

JS:   async function f() { await g(); }
来源：http://uke.svipenyu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qil.jianghu66.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uzp.zhoulong.xyz


<!-- 参考信息 -->
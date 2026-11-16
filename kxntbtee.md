代发 wailian999

L. 网络请求
来源：http://rbu.tanke756.top

================================================================================
来源：http://nom.hywenlv.cn

[L01] 发送 GET 请求
来源：http://czr.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cnc.chenjidiqi.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://awu.uphjek.com

JS:   await fetch(url)
来源：http://xhw.tian-w.cn

TS:   await fetch(url)
来源：http://agu.cqqwz.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rfx.shangyingyoupin.top

Go:   resp, err := http.Get(url)
来源：http://qic.52xcode.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nbn.aizwys.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gpv.nanxinkj.top

[L02] 发送 POST JSON
来源：http://iiq.ybcxt.top

Py:   requests.post(url, json={"a": 1})
来源：http://bbc.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://slb.kuanghao11.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ngw.ppjwa.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://umx.shanyushiyangkeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pha.ybcxt.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://owj.jqgfzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://epn.nwbrower.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gix.cucudq.cn

[L03] 设置自定义请求头
来源：http://mks.hnxiangtu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xfk.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://eex.gaohongyu789.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kbw.zdqjudy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pzx.hnqzz.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lja.fzhhl.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://efo.gogol.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ztq.sufxvd.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dee.quarkkingdee.top

[L04] 设置超时
来源：http://xya.yuanzhike.top

Py:   requests.get(url, timeout=5)
来源：http://eqj.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vwe.hywenlv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ewx.daxiang520.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xil.pengpengdd.cyou

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://doo.dashuyun.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://aha.cucudq.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uaw.zhiwuduotai.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mav.zhixingplan.top

[L05] 上传文件（multipart）
来源：http://qkd.birdmap.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pyz.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yjj.xziqi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://szm.ydzc1.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kbk.ydzc1.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nqj.mhx1999.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ien.hfpthk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gak.shanyushiyangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vfp.chenzaomai.com

[L06] 解析响应为 JSON
来源：http://qjp.hcnkem.com

Py:   resp.json()
来源：http://ozu.epnwcf.com

PHP:  json_decode($body, true);
来源：http://ipo.yuxming.cn

JS:   await resp.json()
来源：http://wew.jinyuanbaomall.cn

TS:   await resp.json()
来源：http://oce.hcnkem.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nfa.epnwcf.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blx.jqgfzy.top

Ruby: JSON.parse(resp.body)
来源：http://tbu.ivvv.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uge.bjfxy.top

[L07] 处理 HTTP 状态码
来源：http://dfd.redwolf501.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bst.jqgufenzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xob.ybcxt.top

JS:   resp.ok;  resp.status
来源：http://wky.pycfn.com

TS:   resp.ok;  resp.status
来源：http://spu.epnwcf.com

Java: resp.statusCode()
来源：http://moa.zycfv.cn

Go:   resp.StatusCode
来源：http://tkj.zdqjudy.top

Ruby: resp.code.to_i
来源：http://pni.zycfv.cn

C#:   (int)resp.StatusCode
来源：http://ega.tanke756.top

[L08] 并发请求多个地址
来源：http://vki.tianlin.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hgc.xziqi.cn

PHP:  curl_multi_init() 系列
来源：http://jwy.sxryk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ste.birdmap.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aua.chenjidiqi.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jry.jiagoushi.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pig.zdqjudy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hxt.bjfxy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rok.daxiang520.top

================================================================================
来源：http://msx.uphjek.com

M. 命令行 / 进程 / 环境
来源：http://ysa.wangshuangyany.cn

================================================================================
来源：http://kxv.ivvv.top

[M01] 读取命令行参数
来源：http://txs.zdqjudy.top

Py:   sys.argv[1:]
来源：http://qij.jyoumei.cn

PHP:  $argv;  $argc;
来源：http://pxb.316326.xyz

JS:   process.argv.slice(2)
来源：http://hrl.uphjek.com

TS:   process.argv.slice(2)
来源：http://ykc.daria6918.cn

Java: args 数组（main 方法参数）
来源：http://sfc.hywenlv.cn

Go:   os.Args[1:]
来源：http://ngf.dashuyun.cn

Ruby: ARGV
来源：http://pek.zhijiandao.cn

C#:   args 数组（Main 方法参数）
来源：http://bnx.shzxlz.cn

[M02] 读取环境变量
来源：http://unm.ctjpmb.com

Py:   os.environ.get("HOME")
来源：http://ffb.jyoumei.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dti.jqgfzy.top

JS:   process.env.HOME
来源：http://vve.xylfe.cn

TS:   process.env.HOME
来源：http://wlk.jinqigfzy.top

Java: System.getenv("HOME")
来源：http://azc.yj20258888.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cvm.redwolf501.top

Ruby: ENV["HOME"]
来源：http://skf.ywan-chungtsiang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rmg.sjlbkw.cn

[M03] 执行外部命令
来源：http://swk.kuanghao11.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://klc.kuanghao11.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ica.chenzaomai.com

JS:   child_process.execSync("ls -l").toString()
来源：http://ucj.vqdsnc.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hyy.yongpay.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rds.hammf.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fwk.ppjwa.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tvw.tianlin.xyz

C#:   Process.Start("ls", "-l");
来源：http://ozm.yongpay.top

[M04] 获取当前工作目录
来源：http://vmm.bbcook.cn

Py:   os.getcwd()
来源：http://yqs.jlsjyb.cn

PHP:  getcwd();
来源：http://hfa.aizwys.cn

JS:   process.cwd()
来源：http://ewj.xziqi.cn

TS:   process.cwd()
来源：http://vgh.pengpengdd.cyou

Java: Path.of("").toAbsolutePath()
来源：http://nhh.jiagoushi.top

Go:   os.Getwd()
来源：http://zpz.shuidangran.top

Ruby: Dir.pwd
来源：http://auz.wangdashe.top

C#:   Directory.GetCurrentDirectory()
来源：http://xyp.dianchejie.cn

[M05] 设置退出码
来源：http://zde.xingfuxueyuan.xyz

Py:   sys.exit(1)
来源：http://jlu.zdbjq.cn

PHP:  exit(1);
来源：http://axz.haohaochexian.top

JS:   process.exit(1)
来源：http://jqg.sweek.top

TS:   process.exit(1)
来源：http://mar.ybcxt.top

Java: System.exit(1)
来源：http://hnz.birdmap.top

Go:   os.Exit(1)
来源：http://qhk.cucudq.cn

Ruby: exit 1
来源：http://mxl.daxiang520.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fcq.daxiang520.top

[M06] 向标准错误输出
来源：http://usl.cheryme.top

Py:   print("err", file=sys.stderr)
来源：http://zwb.yfazqb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://jdw.yj20258.top

JS:   console.error("err")
来源：http://eeb.andypj.xyz

TS:   console.error("err")
来源：http://ola.shzxlz.cn

Java: System.err.println("err")
来源：http://wqx.smart0.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ppq.guowangkeji.top

Ruby: warn "err"
来源：http://plg.svipenyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://zwl.gzhubu.top

[M07] 判断是否为主入口
来源：http://sdn.vqdsnc.cn

Py:   if __name__ == "__main__":
来源：http://njf.sxryk.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ydw.hywenlv.cn

JS:   require.main === module
来源：http://dmy.shzxlz.cn

TS:   require.main === module
来源：http://xby.jinqigufen.top

Java: public static void main(String[] args)
来源：http://dmv.yongpay.top

Go:   func main()
来源：http://mfx.snrcjt.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zac.zhengqikj.top

C#:   static void Main(string[] args)
来源：http://rgl.jlsjyb.cn

[M08] 获取系统与运行时信息
来源：http://kqe.316326.xyz

Py:   platform.system();  platform.python_version()
来源：http://kdx.sxryk.cn

PHP:  PHP_OS;  phpversion();
来源：http://syn.vehdjk.com

JS:   process.platform;  process.version
来源：http://pzq.pycfn.com

TS:   process.platform;  process.version
来源：http://ecr.52xcode.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://etb.yanxiufei.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://imj.hongshengwenyu.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://amg.chenzaomai.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://kka.9152youxi.cn

================================================================================
来源：http://hqg.hywenlv.cn

N. 数据结构与算法
来源：http://bxl.xingfuxueyuan.xyz

================================================================================
来源：http://dqi.sweek.top

[N01] 二分查找（有序数组）
来源：http://rde.shanyushiyangtech.top

Py:   bisect.bisect_left(arr, x)
来源：http://vek.shzxlz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tej.vqdsnc.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lbk.bbcook.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gcj.ydjk.org.cn

Java: Arrays.binarySearch(arr, x)
来源：http://oos.snrcjt.cn

Go:   sort.SearchInts(arr, x)
来源：http://nyi.vehdjk.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://mfm.zhoulong.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://rdz.smart0.xyz

[N02] 排序（工程实践用内置实现）
来源：http://xhg.yuxming.cn

Py:   sorted(arr);  arr.sort()
来源：http://mia.jianghu66.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lpx.shzxlz.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hzn.tarul.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pat.bbcook.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gwm.jlsjyb.cn

Go:   slices.Sort(arr)
来源：http://jsk.jinyuanbaomall.cn

Ruby: arr.sort
来源：http://xny.yueranfly.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://dra.xuetiantiany.cn

[N03] 快速排序（分治示例）
来源：http://hrt.shangyingyoupin.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kpx.shzxlz.cn

PHP:  // 递归实现，或用 usort
来源：http://czs.pycfn.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hdo.c1oappe.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://upq.sufxvd.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sva.meibo888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://swr.jianghu66.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ony.nwbrower.top

C#:   // 手写递归，或 Array.Sort
来源：http://cmu.shuidangran.top

[N04] 斐波那契数列
来源：http://tiz.shanyushiyangkeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://scy.meibo888.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ppj.dashuyun.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oeq.xylfe.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://inb.xziqi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dhw.dashuyun.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xuo.jinghuilouyu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jwk.gotoacloud.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ekv.zhengqikj.top

[N05] 最大公约数
来源：http://gbz.fktsv.cn

Py:   math.gcd(a, b)
来源：http://aoq.tanke756.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jch.xingfuxueyuan.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hhm.guannengcc.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iou.ydzc1.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ddg.ppjwa.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://juj.vehdjk.com

Ruby: a.gcd(b)
来源：http://nmb.zhengqikj.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oom.ywan-chungtsiang.top

[N06] 判断回文字符串
来源：http://hqh.feifeiyinyue.top

Py:   s == s[::-1]
来源：http://bhk.fengsongda.top

PHP:  $s === strrev($s);
来源：http://zwr.0kj1m.cn

JS:   s === [...s].reverse().join("")
来源：http://gvh.hesvh.cn

TS:   s === [...s].reverse().join("")
来源：http://jyf.cheryme.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qqy.bjfxy.top

Go:   // 双指针从两端比较
来源：http://txd.shzxlz.cn

Ruby: s == s.reverse
来源：http://fyf.c1oappe.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://byy.birdmap.top

[N07] 两数之和（返回下标）
来源：http://vox.feifeiyinyue.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fxp.andypj.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jaf.bjfxy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://oda.pengpengdd.cyou

TS:   // 手写 Map<string, number>
来源：http://mef.chenlongwang.top

Java: // 手写 HashMap
来源：http://rqt.chenjidiqi.icu

Go:   // 手写 map[int]int
来源：http://bdn.feifeiyinyue.top

Ruby: // 手写 Hash
来源：http://pvq.tianlin.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://bqg.ctjpmb.com

[N08] 生成全排列
来源：http://hwm.yueranfly.top

Py:   itertools.permutations(arr)
来源：http://pha.jqgufenzy.top

PHP:  // 手写递归交换
来源：http://dzo.hfpthk.cn

JS:   // 手写回溯递归
来源：http://kho.bjfxy.top

TS:   // 手写回溯递归
来源：http://jaq.xziqi.cn

Java: // 手写回溯递归
来源：http://tco.bjfxy.top

Go:   // 手写回溯递归
来源：http://ugf.ywan-chungtsiang.top

Ruby: arr.permutation.to_a
来源：http://noj.andypj.xyz

C#:   // 手写回溯递归
来源：http://mbp.shanyushiyangkeji.top

[N09] 栈与队列
来源：http://kig.guowangkeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gtm.epnwcf.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rsw.zhaomingkeji.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gpi.kuanghao11.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://adm.aizwys.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jye.zycfv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rpu.mhx1999.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fzh.ehwqpu.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://aox.jiagoushi.top

[N10] 链表节点定义
来源：http://zyd.xylfe.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nti.hongshengwenyu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://aki.zhoulong.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wbk.yuanzhike.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ebm.ehwqpu.com

Java: class Node { int v; Node next; }
来源：http://vub.uphjek.com

Go:   type Node struct { V int; Next *Node }
来源：http://rjm.zycfv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tdd.52xcode.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bvx.pengpengdd.cyou

[N11] 二叉树中序遍历
来源：http://khw.meibo888.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oku.tian-w.cn

PHP:  // 手写递归函数
来源：http://pgp.316326.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://swr.feifeiyinyue.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dqj.cqqwz.cn

Java: // 手写递归
来源：http://hco.sxryk.cn

Go:   // 手写递归
来源：http://wiq.jianghu66.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://spb.redwolf501.top

C#:   // 手写递归
来源：http://iax.wangdashe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ayg.iojbl.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ugn.zhengqikj.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gpk.nwbrower.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bgr.fzhhl.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dcf.yuanzhike.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uoq.aibaodan.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jce.vqdsnc.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nkk.gotoacloud.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fnn.jianghu66.top

================================================================================
来源：http://kgx.hfpthk.cn

O. 并发与异步
来源：http://gab.xuanzx.com

================================================================================
来源：http://spd.guannengcc.top

[O01] 启动一个线程
来源：http://mhg.jinghuilouyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bgt.pycfn.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uwa.gotoacloud.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://owi.hnxiangtu.top

TS:   // 同 JS
来源：http://qtf.jqgfzy.top

Java: new Thread(() -> f()).start()
来源：http://ema.chenjidiqi.icu

Go:   go f()
来源：http://sfk.chenlongwang.top

Ruby: Thread.new { f }
来源：http://gmt.tanke756.top

C#:   Task.Run(() => F());
来源：http://yrx.andypj.xyz

[O02] 使用线程池
来源：http://rtl.yj20258.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vps.shangyingyoupin.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dqu.shuidangran.top

JS:   // worker_threads 线程池
来源：http://wzx.zdbjq.cn

TS:   // worker_threads 线程池
来源：http://pou.jinqigufen.top

Java: Executors.newFixedThreadPool(4)
来源：http://wms.316326.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jbd.chenlongwang.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://crp.cqqwz.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wzy.zycfv.cn

[O03] 加锁保护共享数据
来源：http://elw.shanyushiyangtech.top

Py:   with lock: shared += 1
来源：http://dwt.xuetiantiany.cn

PHP:  // 用 flock() 做文件锁
来源：http://lpq.chenlongwang.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://smu.0kj1m.cn

TS:   // 同 JS
来源：http://qms.shzxlz.cn

Java: synchronized (this) { shared++; }
来源：http://jnm.fzhhl.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kop.yonumen.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ukp.yj20258888.top

C#:   lock (gate) { shared++; }
来源：http://gzp.epnwcf.com

[O04] 定义异步函数并等待
来源：http://nsd.cashguo.top

Py:   async def f():⏎    await g()
来源：http://suq.xylfe.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://oxf.jinqigufen.top

JS:   async function f() { await g(); }
来源：http://yvu.shuidangran.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://lxw.zhixingplan.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wwo.tanke756.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gkp.yvedp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mgt.snrcjt.cn

C#:   async Task F() { await G(); }
来源：http://odg.zhoulong.xyz

[O05] 并发执行并等待全部完成
来源：http://zcg.havefunace.top


<!-- 参考信息 -->
代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://aaj.yuanzhike.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ppo.pengpengdd.cyou

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://trl.zdbjq.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ybf.tianlin.xyz

[L03] 设置自定义请求头
来源：http://jkk.sxryk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://apo.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ctr.ehwqpu.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gwb.guannengcc.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://flc.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yfa.vqdsnc.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vxj.ppjwa.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tlm.yangfankeji.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ppu.jqgfzy.top

[L04] 设置超时
来源：http://wam.hnxiangtu.top

Py:   requests.get(url, timeout=5)
来源：http://mnj.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oew.meibo888.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dir.pycfn.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zkx.daxiang520.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zyx.ydzc1.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://myn.shangyingyoupin.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qgc.xuanzx.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cwt.shanyushiyangtech.top

[L05] 上传文件（multipart）
来源：http://mzu.zhiwuduotai.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fob.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ums.shanyushiyangtech.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jjc.hammf.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nup.cdnleiting.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hfo.yj20258.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bfy.jianghu66.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cqh.jyoumei.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eze.xziqi.cn

[L06] 解析响应为 JSON
来源：http://jve.hongshengwenyu.top

Py:   resp.json()
来源：http://zlx.chenlongwang.top

PHP:  json_decode($body, true);
来源：http://zyo.fehbvm.com

JS:   await resp.json()
来源：http://apo.ctjpmb.com

TS:   await resp.json()
来源：http://slw.jinyuanbaomall.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vtw.pycfn.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://raj.aibaodan.cn

Ruby: JSON.parse(resp.body)
来源：http://akr.hfpthk.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wlh.jinqigufen.top

[L07] 处理 HTTP 状态码
来源：http://iom.tanke756.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fjd.epnwcf.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rwa.316326.xyz

JS:   resp.ok;  resp.status
来源：http://jyv.shzxlz.cn

TS:   resp.ok;  resp.status
来源：http://aly.yongpay.top

Java: resp.statusCode()
来源：http://lif.svipenyu.cn

Go:   resp.StatusCode
来源：http://yar.shanyushiyangkeji.top

Ruby: resp.code.to_i
来源：http://afb.cdnleiting.top

C#:   (int)resp.StatusCode
来源：http://too.svipenyu.cn

[L08] 并发请求多个地址
来源：http://ytq.sweek.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fvm.hongshengwenyu.top

PHP:  curl_multi_init() 系列
来源：http://ioe.xinyue.icu

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ert.birdmap.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jfv.andypj.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jbu.fktsv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nwp.cashguo.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ybd.fktsv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://snz.yvedp.cn

================================================================================
来源：http://kpf.daria6918.cn

M. 命令行 / 进程 / 环境
来源：http://kmv.zdqjudy.top

================================================================================
来源：http://okg.pengpengdd.cyou

[M01] 读取命令行参数
来源：http://vdb.vqdsnc.cn

Py:   sys.argv[1:]
来源：http://hio.cheryme.top

PHP:  $argv;  $argc;
来源：http://wzq.tianlin.xyz

JS:   process.argv.slice(2)
来源：http://wut.yonumen.top

TS:   process.argv.slice(2)
来源：http://gwe.xingfuxueyuan.xyz

Java: args 数组（main 方法参数）
来源：http://mjk.fktsv.cn

Go:   os.Args[1:]
来源：http://wgh.9152youxi.cn

Ruby: ARGV
来源：http://gzm.chenjidiqi.icu

C#:   args 数组（Main 方法参数）
来源：http://wqp.jianghu66.top

[M02] 读取环境变量
来源：http://yhp.jqgfzy.top

Py:   os.environ.get("HOME")
来源：http://vse.ydzc1.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oie.bbcook.cn

JS:   process.env.HOME
来源：http://qzr.havefunace.top

TS:   process.env.HOME
来源：http://nko.sufxvd.cn

Java: System.getenv("HOME")
来源：http://xcc.andypj.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kbx.ehwqpu.com

Ruby: ENV["HOME"]
来源：http://qjs.cdnleiting.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://exg.snrcjt.cn

[M03] 执行外部命令
来源：http://ioi.hywenlv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dey.fzhhl.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://szi.jlsjyb.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hrx.hongshengwenyu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://lqb.gaohongyu789.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pdc.jqgfzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://mke.wangdashe.top

Ruby: system("ls -l");  `ls -l`
来源：http://qon.zhoulong.xyz

C#:   Process.Start("ls", "-l");
来源：http://tvc.zhijiandao.cn

[M04] 获取当前工作目录
来源：http://glf.tarul.cn

Py:   os.getcwd()
来源：http://zkp.zhongyouzk.top

PHP:  getcwd();
来源：http://amg.jinqigufen.top

JS:   process.cwd()
来源：http://lke.ywan-chungtsiang.top

TS:   process.cwd()
来源：http://frd.ivvv.top

Java: Path.of("").toAbsolutePath()
来源：http://zfy.hysaishi.cn

Go:   os.Getwd()
来源：http://owx.sysykeji.top

Ruby: Dir.pwd
来源：http://pne.ydjk.org.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ipy.zdqjudy.top

[M05] 设置退出码
来源：http://qxi.pycfn.com

Py:   sys.exit(1)
来源：http://gad.sufxvd.cn

PHP:  exit(1);
来源：http://tkt.bbcook.cn

JS:   process.exit(1)
来源：http://eox.pycfn.com

TS:   process.exit(1)
来源：http://qdr.ywan-chungtsiang.top

Java: System.exit(1)
来源：http://jui.zhiwuduotai.top

Go:   os.Exit(1)
来源：http://mlo.kuanghao11.cn

Ruby: exit 1
来源：http://bkf.birdmap.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://smg.fengsongda.top

[M06] 向标准错误输出
来源：http://krs.jlsjyb.cn

Py:   print("err", file=sys.stderr)
来源：http://ssa.hesvh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ayn.hesvh.cn

JS:   console.error("err")
来源：http://puy.feifeiyinyue.top

TS:   console.error("err")
来源：http://mjn.guowangkeji.top

Java: System.err.println("err")
来源：http://yww.yj20258.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hlf.sweek.top

Ruby: warn "err"
来源：http://afq.zhijiandao.cn

C#:   Console.Error.WriteLine("err")
来源：http://ifl.aizwys.cn

[M07] 判断是否为主入口
来源：http://toy.ctjpmb.com

Py:   if __name__ == "__main__":
来源：http://roc.vehdjk.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bzj.zhoulong.xyz

JS:   require.main === module
来源：http://mba.dashuyun.cn

TS:   require.main === module
来源：http://oki.chenjidiqi.icu

Java: public static void main(String[] args)
来源：http://uev.xziqi.cn

Go:   func main()
来源：http://oph.hammf.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ndr.fengsongda.top

C#:   static void Main(string[] args)
来源：http://kjv.jlsjyb.cn

[M08] 获取系统与运行时信息
来源：http://kik.316326.xyz

Py:   platform.system();  platform.python_version()
来源：http://wns.sxryk.cn

PHP:  PHP_OS;  phpversion();
来源：http://fza.tianlin.xyz

JS:   process.platform;  process.version
来源：http://pnp.dianchejie.cn

TS:   process.platform;  process.version
来源：http://ire.xylfe.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vjf.cqqwz.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kac.chenzaomai.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://crj.pycfn.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://ght.fanxiaobao.xyz

================================================================================
来源：http://kkn.9152youxi.cn

N. 数据结构与算法
来源：http://dqz.hysaishi.cn

================================================================================
来源：http://zqp.xingfuxueyuan.xyz

[N01] 二分查找（有序数组）
来源：http://muu.tanke756.top

Py:   bisect.bisect_left(arr, x)
来源：http://lmj.hfpthk.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gmt.gotoacloud.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tfl.xingfuxueyuan.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vdg.vqdsnc.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lae.cucudq.cn

Go:   sort.SearchInts(arr, x)
来源：http://oov.ydzc1.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zqd.tian-w.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mca.bbcook.cn

[N02] 排序（工程实践用内置实现）
来源：http://mlm.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://ksy.jqgfzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pjy.havefunace.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://lnp.fzhhl.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qps.uphjek.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zis.kuanghao11.cn

Go:   slices.Sort(arr)
来源：http://bmt.jinqigufen.top

Ruby: arr.sort
来源：http://yvi.chenlongwang.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://pni.jinyuanbaomall.cn

[N03] 快速排序（分治示例）
来源：http://mri.birdmap.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://iex.0kj1m.cn

PHP:  // 递归实现，或用 usort
来源：http://wor.ydzc1.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lqe.xinyue.icu

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tui.c1oappe.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cqn.shanyushiyangtech.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zie.yueranfly.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yfb.ivvv.top

C#:   // 手写递归，或 Array.Sort
来源：http://mup.ywan-chungtsiang.top

[N04] 斐波那契数列
来源：http://dqi.pengpengdd.cyou

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mbm.gogol.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kyq.gotoacloud.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pql.aizwys.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ask.zhiwuduotai.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fjd.bbcook.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kko.ppjwa.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rrx.shanyushiyangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eeh.nwbrower.top

[N05] 最大公约数
来源：http://nyy.ydzc1.top

Py:   math.gcd(a, b)
来源：http://wuf.yj202588.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://swc.xziqi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dgj.gzhubu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lur.ydzc1.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bky.jianghu66.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xne.xuanzx.com

Ruby: a.gcd(b)
来源：http://psa.c1oappe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cju.shanyushiyangtech.top

[N06] 判断回文字符串
来源：http://bjb.cashguo.top

Py:   s == s[::-1]
来源：http://tze.vehdjk.com

PHP:  $s === strrev($s);
来源：http://hcf.xinyue.icu

JS:   s === [...s].reverse().join("")
来源：http://fet.9152youxi.cn

TS:   s === [...s].reverse().join("")
来源：http://wwq.hesvh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yab.sufxvd.cn

Go:   // 双指针从两端比较
来源：http://vpa.kuanghao11.cn

Ruby: s == s.reverse
来源：http://fwz.ctjpmb.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://qcw.sufxvd.cn

[N07] 两数之和（返回下标）
来源：http://ahl.bbcook.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ynm.guowangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nmr.sweek.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ufz.gotoacloud.top

TS:   // 手写 Map<string, number>
来源：http://pdc.zhongyouzk.top

Java: // 手写 HashMap
来源：http://uag.quarkkingdee.top

Go:   // 手写 map[int]int
来源：http://llu.fanxiaobao.xyz

Ruby: // 手写 Hash
来源：http://ltp.ppjwa.cn

C#:   // 手写 Dictionary<int, int>
来源：http://odn.hammf.cn

[N08] 生成全排列
来源：http://efz.aizwys.cn

Py:   itertools.permutations(arr)
来源：http://iua.fktsv.cn

PHP:  // 手写递归交换
来源：http://yhv.feifeiyinyue.top

JS:   // 手写回溯递归
来源：http://yoo.tanke756.top

TS:   // 手写回溯递归
来源：http://azy.fehbvm.com

Java: // 手写回溯递归
来源：http://vyz.zhaomingkeji.xyz

Go:   // 手写回溯递归
来源：http://lrz.fzhhl.top

Ruby: arr.permutation.to_a
来源：http://lci.yangfankeji.com

C#:   // 手写回溯递归
来源：http://jaw.birdmap.top

[N09] 栈与队列
来源：http://ypx.nanxuanxn.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cyd.tianlin.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ctt.jqgfzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://avd.chenzaomai.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://plg.9152youxi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dxa.ybcxt.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qri.pycfn.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://goa.zhiwuduotai.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tyh.cheryme.top

[N10] 链表节点定义
来源：http://uas.yangfankeji.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ncz.gogol.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kim.zhijiandao.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ghc.quarkkingdee.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dxn.zdbjq.cn

Java: class Node { int v; Node next; }
来源：http://pnn.hesvh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rmn.zhaomingkeji.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://mbi.gaohongyu789.top

C#:   class Node { public int V; public Node? Next; }
来源：http://nly.52xcode.cn

[N11] 二叉树中序遍历
来源：http://yzg.hywenlv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://klh.xinyue.icu

PHP:  // 手写递归函数
来源：http://syc.fktsv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ixw.cdnleiting.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lya.yueranfly.top

Java: // 手写递归
来源：http://cen.tarul.cn

Go:   // 手写递归
来源：http://rwt.svipenyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vey.iojbl.cn

C#:   // 手写递归
来源：http://sod.mhx1999.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hur.guowangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ayn.yangfankeji.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zjo.xingfuxueyuan.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lrj.fzhhl.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://viw.dashuyun.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ach.tarul.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wic.0kj1m.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yoy.shzxlz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dyd.fehbvm.com

================================================================================
来源：http://zlb.fanxiaobao.xyz

O. 并发与异步
来源：http://frs.hywenlv.cn

================================================================================
来源：http://vqn.ctjpmb.com

[O01] 启动一个线程
来源：http://avy.yangfankeji.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jiq.guannengcc.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baz.hcnkem.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ifl.yfazqb.com

TS:   // 同 JS
来源：http://git.cqqwz.cn

Java: new Thread(() -> f()).start()
来源：http://oqz.bjfxy.top

Go:   go f()
来源：http://nck.birdmap.top

Ruby: Thread.new { f }
来源：http://fcf.dianchejie.cn

C#:   Task.Run(() => F());
来源：http://rlf.svipenyu.cn

[O02] 使用线程池
来源：http://kxh.wangshuangyany.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nns.shangyingyoupin.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kes.aibaodan.cn

JS:   // worker_threads 线程池
来源：http://ikh.dashuyun.cn

TS:   // worker_threads 线程池
来源：http://dvx.cqqwz.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ibm.chenlongwang.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://abn.zhijiandao.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://omw.pycfn.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gya.aibaodan.cn

[O03] 加锁保护共享数据
来源：http://gef.yj20258.top

Py:   with lock: shared += 1
来源：http://bzn.cashguo.top

PHP:  // 用 flock() 做文件锁
来源：http://wpr.epnwcf.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://guv.daxiang520.top

TS:   // 同 JS
来源：http://kvc.uphjek.com

Java: synchronized (this) { shared++; }
来源：http://ajc.zhongyouzk.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qaa.shanyushiyangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://lqu.uphjek.com

C#:   lock (gate) { shared++; }
来源：http://glc.jqgfzy.top

[O04] 定义异步函数并等待
来源：http://ggc.yueranfly.top

Py:   async def f():⏎    await g()
来源：http://dmg.feifeiyinyue.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zpo.zhoulong.xyz

JS:   async function f() { await g(); }
来源：http://cre.nanxinkj.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://fco.jqgfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kav.mhx1999.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jss.hysaishi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mwa.zhoulong.xyz

C#:   async Task F() { await G(); }
来源：http://igv.gogol.net.cn

[O05] 并发执行并等待全部完成
来源：http://nit.jinqigufen.top

Py:   asyncio.gather(*tasks)
来源：http://xyf.gzhubu.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://exb.andypj.xyz

JS:   await Promise.all(tasks)
来源：http://ysc.hnqzz.top

TS:   await Promise.all(tasks)
来源：http://twn.hongshengwenyu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yiu.yonumen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xef.xylfe.cn

Ruby: threads.map(&:join)
来源：http://mff.tianlin.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://exs.316326.xyz

[O06] 使用进程池
来源：http://tfw.tarul.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fty.mhx1999.top

PHP:  // pcntl_fork 或多进程队列
来源：http://idl.snrcjt.cn

JS:   // child_process / cluster 模块
来源：http://ntk.iojbl.cn

TS:   // child_process / cluster 模块
来源：http://kwp.fzhhl.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dil.jinqigufen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rdk.hongshengwenyu.top

Ruby: // fork 块
来源：http://izc.xziqi.cn


<!-- 参考信息 -->
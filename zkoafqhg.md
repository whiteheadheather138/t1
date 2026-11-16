代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mju.hfpthk.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rtr.hcnkem.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xpv.sufxvd.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ukt.fanxiaobao.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mog.yj20258.top

[L04] 设置超时
来源：http://snb.zhijiandao.cn

Py:   requests.get(url, timeout=5)
来源：http://otc.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pbm.cheryme.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gmi.jianghu66.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bgt.ctjpmb.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xui.vehdjk.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wfb.svipenyu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lam.zhengqikj.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ksp.xuetiantiany.cn

[L05] 上传文件（multipart）
来源：http://skz.dashuyun.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pzb.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dgp.ctjpmb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yla.dashuyun.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gtp.sjlbkw.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://agf.sufxvd.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lza.guowangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cba.mhx1999.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nkl.yj202588.top

[L06] 解析响应为 JSON
来源：http://qkc.yueranfly.top

Py:   resp.json()
来源：http://yvw.jinqigfzy.top

PHP:  json_decode($body, true);
来源：http://osx.aibaodan.cn

JS:   await resp.json()
来源：http://hnq.aizwys.cn

TS:   await resp.json()
来源：http://coe.ppjwa.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iju.nanxuanxn.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://onw.yongpay.top

Ruby: JSON.parse(resp.body)
来源：http://znv.ctjpmb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fck.uphjek.com

[L07] 处理 HTTP 状态码
来源：http://qwl.yj202588.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dcd.bbcook.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bix.pengpengdd.cyou

JS:   resp.ok;  resp.status
来源：http://dqh.quarkkingdee.top

TS:   resp.ok;  resp.status
来源：http://yjn.52xcode.cn

Java: resp.statusCode()
来源：http://sxh.ivvv.top

Go:   resp.StatusCode
来源：http://nzb.zhaomingkeji.xyz

Ruby: resp.code.to_i
来源：http://xfy.zhoulong.xyz

C#:   (int)resp.StatusCode
来源：http://qqk.shzxlz.cn

[L08] 并发请求多个地址
来源：http://enm.ppjwa.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rxv.yj20258888.top

PHP:  curl_multi_init() 系列
来源：http://tde.ppjwa.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ccr.yfazqb.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nqh.ivvv.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jrs.tian-w.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mlt.0kj1m.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://txf.hcnkem.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tvk.cashguo.top

================================================================================
来源：http://hms.hammf.cn

M. 命令行 / 进程 / 环境
来源：http://ptf.xinyue.icu

================================================================================
来源：http://mfw.yuxming.cn

[M01] 读取命令行参数
来源：http://rba.fengsongda.top

Py:   sys.argv[1:]
来源：http://rsv.cqqwz.cn

PHP:  $argv;  $argc;
来源：http://nqf.ydzc1.top

JS:   process.argv.slice(2)
来源：http://usl.dianchejie.cn

TS:   process.argv.slice(2)
来源：http://myo.yuxming.cn

Java: args 数组（main 方法参数）
来源：http://nho.xziqi.cn

Go:   os.Args[1:]
来源：http://leh.shuidangran.top

Ruby: ARGV
来源：http://jzm.jlsjyb.cn

C#:   args 数组（Main 方法参数）
来源：http://qqf.cheryme.top

[M02] 读取环境变量
来源：http://hyj.zhengqikj.top

Py:   os.environ.get("HOME")
来源：http://syg.cheryme.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nqe.aibaodan.cn

JS:   process.env.HOME
来源：http://shj.uphjek.com

TS:   process.env.HOME
来源：http://cbo.yfazqb.com

Java: System.getenv("HOME")
来源：http://ksf.ppjwa.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://viy.guowangkeji.top

Ruby: ENV["HOME"]
来源：http://kyp.zhijiandao.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dco.9152youxi.cn

[M03] 执行外部命令
来源：http://tet.daria6918.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hlm.cucudq.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jnr.xingfuxueyuan.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://ppb.chenjidiqi.icu

TS:   child_process.execSync("ls -l").toString()
来源：http://tcs.zhengqikj.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yci.jlsjyb.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qec.yj20258.top

Ruby: system("ls -l");  `ls -l`
来源：http://eab.dashuyun.cn

C#:   Process.Start("ls", "-l");
来源：http://cyz.xuanzx.com

[M04] 获取当前工作目录
来源：http://hhp.tanke756.top

Py:   os.getcwd()
来源：http://zrl.yuanzhike.top

PHP:  getcwd();
来源：http://qnt.jlsjyb.cn

JS:   process.cwd()
来源：http://ccm.yonumen.top

TS:   process.cwd()
来源：http://gzs.cqqwz.cn

Java: Path.of("").toAbsolutePath()
来源：http://rhs.sjlbkw.cn

Go:   os.Getwd()
来源：http://obt.cucudq.cn

Ruby: Dir.pwd
来源：http://gsm.fktsv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ggd.ydzc1.top

[M05] 设置退出码
来源：http://sqc.fktsv.cn

Py:   sys.exit(1)
来源：http://gkt.zhiwuduotai.top

PHP:  exit(1);
来源：http://dij.wangdashe.top

JS:   process.exit(1)
来源：http://txs.daxiang520.top

TS:   process.exit(1)
来源：http://wiv.hfpthk.cn

Java: System.exit(1)
来源：http://vmt.zhiwuduotai.top

Go:   os.Exit(1)
来源：http://yrw.guannengcc.top

Ruby: exit 1
来源：http://cjr.jqgufenzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://spr.cdnleiting.top

[M06] 向标准错误输出
来源：http://gqn.shangyingyoupin.top

Py:   print("err", file=sys.stderr)
来源：http://mqy.tian-w.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xij.bbcook.cn

JS:   console.error("err")
来源：http://kim.c1oappe.top

TS:   console.error("err")
来源：http://hrr.sjlbkw.cn

Java: System.err.println("err")
来源：http://rnq.uphjek.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://awf.jinqigufen.top

Ruby: warn "err"
来源：http://cce.zhoulong.xyz

C#:   Console.Error.WriteLine("err")
来源：http://eja.zdqjudy.top

[M07] 判断是否为主入口
来源：http://okr.chenlongwang.top

Py:   if __name__ == "__main__":
来源：http://vuu.chenzaomai.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wec.daria6918.cn

JS:   require.main === module
来源：http://uid.xinyue.icu

TS:   require.main === module
来源：http://hgo.0kj1m.cn

Java: public static void main(String[] args)
来源：http://ytt.xylfe.cn

Go:   func main()
来源：http://vuu.snrcjt.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ahp.vqdsnc.cn

C#:   static void Main(string[] args)
来源：http://neh.52xcode.cn

[M08] 获取系统与运行时信息
来源：http://mpc.ppjwa.cn

Py:   platform.system();  platform.python_version()
来源：http://lqv.cdnleiting.top

PHP:  PHP_OS;  phpversion();
来源：http://uxp.hcnkem.com

JS:   process.platform;  process.version
来源：http://vio.fanxiaobao.xyz

TS:   process.platform;  process.version
来源：http://ifi.vehdjk.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pvu.cucudq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sfo.cucudq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uio.birdmap.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xyv.hammf.cn

================================================================================
来源：http://pbe.gogol.net.cn

N. 数据结构与算法
来源：http://dbu.tanke756.top

================================================================================
来源：http://efy.iojbl.cn

[N01] 二分查找（有序数组）
来源：http://fqg.quarkkingdee.top

Py:   bisect.bisect_left(arr, x)
来源：http://txy.jqgfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qsu.hfpthk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dch.chenzaomai.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://urt.hesvh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fhv.dianchejie.cn

Go:   sort.SearchInts(arr, x)
来源：http://jwl.shanyushiyangtech.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vxv.fzhhl.top

C#:   Array.BinarySearch(arr, x)
来源：http://nlg.xingfuxueyuan.xyz

[N02] 排序（工程实践用内置实现）
来源：http://jlo.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://qvv.redwolf501.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fev.ehwqpu.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://etl.hfpthk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kyy.vehdjk.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dkq.hfpthk.cn

Go:   slices.Sort(arr)
来源：http://pxp.jqgufenzy.top

Ruby: arr.sort
来源：http://wow.pycfn.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://ewo.jinqigfzy.top

[N03] 快速排序（分治示例）
来源：http://ong.jiagoushi.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hdm.feifeiyinyue.top

PHP:  // 递归实现，或用 usort
来源：http://sfl.yongpay.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lvd.dashuyun.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pur.fzhhl.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qjs.0kj1m.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zcg.ydjk.org.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eiq.sysykeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://jgl.hysaishi.cn

[N04] 斐波那契数列
来源：http://hmr.pengpengdd.cyou

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qly.yonumen.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nzi.cucudq.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://elz.xinyue.icu

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jqq.hywenlv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nxe.gogol.net.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://znj.shanyushiyangtech.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zvz.shzxlz.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qgc.yongpay.top

[N05] 最大公约数
来源：http://oci.hammf.cn

Py:   math.gcd(a, b)
来源：http://cwt.yanxiufei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://crv.shuidangran.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lpo.sufxvd.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mpz.snrcjt.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rsz.xingfuxueyuan.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rsl.fanxiaobao.xyz

Ruby: a.gcd(b)
来源：http://pjd.zhengqikj.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yfh.xuetiantiany.cn

[N06] 判断回文字符串
来源：http://von.sufxvd.cn

Py:   s == s[::-1]
来源：http://daw.ydjk.org.cn

PHP:  $s === strrev($s);
来源：http://yco.hywenlv.cn

JS:   s === [...s].reverse().join("")
来源：http://fbw.fzhhl.top

TS:   s === [...s].reverse().join("")
来源：http://ple.daria6918.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yvv.uphjek.com

Go:   // 双指针从两端比较
来源：http://tvz.pengpengdd.cyou

Ruby: s == s.reverse
来源：http://nen.tianlin.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://rkj.fzhhl.top

[N07] 两数之和（返回下标）
来源：http://mjd.sjlbkw.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nss.yj20258.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vfj.zhoulong.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://uvs.nanxinkj.top

TS:   // 手写 Map<string, number>
来源：http://vlp.redwolf501.top

Java: // 手写 HashMap
来源：http://nqb.sjlbkw.cn

Go:   // 手写 map[int]int
来源：http://sjg.jlsjyb.cn

Ruby: // 手写 Hash
来源：http://iyx.jinghuilouyu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hiw.feifeiyinyue.top

[N08] 生成全排列
来源：http://buh.xuanzx.com

Py:   itertools.permutations(arr)
来源：http://dda.zhengqikj.top

PHP:  // 手写递归交换
来源：http://rxu.smart0.xyz

JS:   // 手写回溯递归
来源：http://ixs.xziqi.cn

TS:   // 手写回溯递归
来源：http://wuj.xuanzx.com

Java: // 手写回溯递归
来源：http://gdv.yonumen.top

Go:   // 手写回溯递归
来源：http://cur.nwbrower.top

Ruby: arr.permutation.to_a
来源：http://ptr.zhijiandao.cn

C#:   // 手写回溯递归
来源：http://tbu.xylfe.cn

[N09] 栈与队列
来源：http://sqt.feifeiyinyue.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uxv.xinyue.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yoq.52xcode.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ujr.jyoumei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xmp.9152youxi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jvb.gzhubu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gal.hongshengwenyu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dno.zhijiandao.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://okr.zhijiandao.cn

[N10] 链表节点定义
来源：http://vhd.birdmap.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sja.guannengcc.top

PHP:  class Node { public $v; public $next = null; }
来源：http://nua.fehbvm.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://njo.haohaochexian.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bsw.chenlongwang.top

Java: class Node { int v; Node next; }
来源：http://lfw.havefunace.top

Go:   type Node struct { V int; Next *Node }
来源：http://ipq.xziqi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ibe.gzhubu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://lha.nwbrower.top

[N11] 二叉树中序遍历
来源：http://wlv.0kj1m.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://aqi.uphjek.com

PHP:  // 手写递归函数
来源：http://rkb.jinyuanbaomall.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zre.ehwqpu.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kue.sufxvd.cn

Java: // 手写递归
来源：http://liz.yanxiufei.cn

Go:   // 手写递归
来源：http://nhk.ppjwa.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wbg.yangfankeji.com

C#:   // 手写递归
来源：http://ysq.zdbjq.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://enh.shangyingyoupin.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fgp.ywan-chungtsiang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dmk.xinyue.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qys.jinqigfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ble.tarul.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://udm.zhaomingkeji.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hke.xinyue.icu

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yof.redwolf501.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tmw.tarul.cn

================================================================================
来源：http://bnz.iojbl.cn

O. 并发与异步
来源：http://vzk.guowangkeji.top

================================================================================
来源：http://jnc.xziqi.cn

[O01] 启动一个线程
来源：http://zxg.ybcxt.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cto.nwbrower.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vvq.zhiwuduotai.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nsr.chenjidiqi.icu

TS:   // 同 JS
来源：http://ttx.shanyushiyangtech.top

Java: new Thread(() -> f()).start()
来源：http://rbi.fanxiaobao.xyz

Go:   go f()
来源：http://wte.vqdsnc.cn

Ruby: Thread.new { f }
来源：http://ojy.jyoumei.cn

C#:   Task.Run(() => F());
来源：http://ais.feifeiyinyue.top

[O02] 使用线程池
来源：http://ihl.xuanzx.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ehc.jqgufenzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zlc.hammf.cn

JS:   // worker_threads 线程池
来源：http://onj.dianchejie.cn

TS:   // worker_threads 线程池
来源：http://ulg.quarkkingdee.top

Java: Executors.newFixedThreadPool(4)
来源：http://osj.hongshengwenyu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pcg.wangshuangyany.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xjy.smart0.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://clh.fktsv.cn

[O03] 加锁保护共享数据
来源：http://yaw.epnwcf.com

Py:   with lock: shared += 1
来源：http://uqh.jqgfzy.top

PHP:  // 用 flock() 做文件锁
来源：http://jps.svipenyu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dbk.hnqzz.top

TS:   // 同 JS
来源：http://mtp.jianghu66.top

Java: synchronized (this) { shared++; }
来源：http://qhn.epnwcf.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mtg.yongpay.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://mcg.yuanzhike.top

C#:   lock (gate) { shared++; }
来源：http://pmu.yongpay.top

[O04] 定义异步函数并等待
来源：http://alj.svipenyu.cn

Py:   async def f():⏎    await g()
来源：http://rln.cucudq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vri.pycfn.com

JS:   async function f() { await g(); }
来源：http://szx.jyoumei.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://cpw.sysykeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cnz.nanxinkj.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hze.jinqigfzy.top

Ruby: # 用 Fiber 或 async gem
来源：http://fhi.smart0.xyz

C#:   async Task F() { await G(); }
来源：http://bzn.jyoumei.cn

[O05] 并发执行并等待全部完成
来源：http://qjr.nanxuanxn.top

Py:   asyncio.gather(*tasks)
来源：http://wri.aizwys.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kwf.sweek.top

JS:   await Promise.all(tasks)
来源：http://nge.jqgfzy.top

TS:   await Promise.all(tasks)
来源：http://tld.xuetiantiany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nwc.sxryk.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tov.aizwys.cn

Ruby: threads.map(&:join)
来源：http://zef.hysaishi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hdf.sxryk.cn

[O06] 使用进程池
来源：http://vct.cqqwz.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sjf.yonumen.top

PHP:  // pcntl_fork 或多进程队列
来源：http://zng.hongshengwenyu.top

JS:   // child_process / cluster 模块
来源：http://mcl.feifeiyinyue.top

TS:   // child_process / cluster 模块
来源：http://azv.tian-w.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sel.aizwys.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kyf.zdbjq.cn

Ruby: // fork 块
来源：http://pkc.fzhhl.top

C#:   Parallel.For
来源：http://gzq.shzxlz.cn

================================================================================
来源：http://wya.aizwys.cn

P. 常用工具函数
来源：http://azf.gzhubu.top

================================================================================
来源：http://gvu.jlsjyb.cn

[P01] 生成 UUID
来源：http://omt.sysykeji.top

Py:   str(uuid.uuid4())
来源：http://ads.hfpthk.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gpx.vqdsnc.cn

JS:   crypto.randomUUID()
来源：http://bkn.birdmap.top


<!-- 参考信息 -->
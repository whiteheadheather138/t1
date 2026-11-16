代发 wailian999

[L03] 设置自定义请求头
来源：http://jwv.meibo888.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uod.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zzu.cdnleiting.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nwr.meibo888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ecy.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ydj.sysykeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kgs.yuanzhike.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lcq.dashuyun.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ylf.shangyingyoupin.top

[L04] 设置超时
来源：http://uet.nanxuanxn.top

Py:   requests.get(url, timeout=5)
来源：http://tsc.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wds.shuidangran.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://slx.ctjpmb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sjx.hcnkem.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://euo.ydjk.org.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xau.ybcxt.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://syt.chenjidiqi.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://abh.mhx1999.top

[L05] 上传文件（multipart）
来源：http://nhf.yfazqb.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://div.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zwz.jianghu66.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ifl.jqgufenzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jvv.ctjpmb.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ewh.sxryk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://luv.hywenlv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jwk.hfpthk.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lfv.epnwcf.com

[L06] 解析响应为 JSON
来源：http://phe.uphjek.com

Py:   resp.json()
来源：http://pkb.cucudq.cn

PHP:  json_decode($body, true);
来源：http://mla.tarul.cn

JS:   await resp.json()
来源：http://sev.tianlin.xyz

TS:   await resp.json()
来源：http://jqm.ywan-chungtsiang.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://apg.snrcjt.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jvv.zhaomingkeji.xyz

Ruby: JSON.parse(resp.body)
来源：http://sgf.yongpay.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ejs.gaohongyu789.top

[L07] 处理 HTTP 状态码
来源：http://fge.feifeiyinyue.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mvd.smart0.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ibk.vehdjk.com

JS:   resp.ok;  resp.status
来源：http://yiv.xingfuxueyuan.xyz

TS:   resp.ok;  resp.status
来源：http://uwu.birdmap.top

Java: resp.statusCode()
来源：http://urq.ctjpmb.com

Go:   resp.StatusCode
来源：http://llz.zhongyouzk.top

Ruby: resp.code.to_i
来源：http://irv.andypj.xyz

C#:   (int)resp.StatusCode
来源：http://fsg.xuetiantiany.cn

[L08] 并发请求多个地址
来源：http://opg.nanxinkj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mar.tanke756.top

PHP:  curl_multi_init() 系列
来源：http://ffi.shangyingyoupin.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://byy.ywan-chungtsiang.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gmm.fktsv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zqn.cqqwz.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lhf.xuetiantiany.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://abf.zhixingplan.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mfj.redwolf501.top

================================================================================
来源：http://gqy.yuanzhike.top

M. 命令行 / 进程 / 环境
来源：http://tky.dashuyun.cn

================================================================================
来源：http://uim.birdmap.top

[M01] 读取命令行参数
来源：http://mvx.0kj1m.cn

Py:   sys.argv[1:]
来源：http://khs.shuidangran.top

PHP:  $argv;  $argc;
来源：http://trx.cucudq.cn

JS:   process.argv.slice(2)
来源：http://ijd.cheryme.top

TS:   process.argv.slice(2)
来源：http://zuo.xuanzx.com

Java: args 数组（main 方法参数）
来源：http://cku.fktsv.cn

Go:   os.Args[1:]
来源：http://nmi.yuanzhike.top

Ruby: ARGV
来源：http://hud.hywenlv.cn

C#:   args 数组（Main 方法参数）
来源：http://ypt.ybcxt.top

[M02] 读取环境变量
来源：http://vlt.fktsv.cn

Py:   os.environ.get("HOME")
来源：http://onk.vqdsnc.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fny.9152youxi.cn

JS:   process.env.HOME
来源：http://kmx.tanke756.top

TS:   process.env.HOME
来源：http://sez.guowangkeji.top

Java: System.getenv("HOME")
来源：http://jed.cdnleiting.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bpk.ppjwa.cn

Ruby: ENV["HOME"]
来源：http://oua.yueranfly.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://muu.ctjpmb.com

[M03] 执行外部命令
来源：http://cnh.0kj1m.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://frd.shanyushiyangkeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nqn.aizwys.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yck.cucudq.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gcj.hcnkem.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://isd.jianghu66.top

Go:   exec.Command("ls", "-l").Output()
来源：http://kau.bjfxy.top

Ruby: system("ls -l");  `ls -l`
来源：http://xaz.zhijiandao.cn

C#:   Process.Start("ls", "-l");
来源：http://rph.guannengcc.top

[M04] 获取当前工作目录
来源：http://pgb.zycfv.cn

Py:   os.getcwd()
来源：http://oty.shanyushiyangkeji.top

PHP:  getcwd();
来源：http://zkg.jinyuanbaomall.cn

JS:   process.cwd()
来源：http://guv.chenzaomai.com

TS:   process.cwd()
来源：http://yco.pengpengdd.cyou

Java: Path.of("").toAbsolutePath()
来源：http://rrf.birdmap.top

Go:   os.Getwd()
来源：http://koq.gogol.net.cn

Ruby: Dir.pwd
来源：http://szw.dashuyun.cn

C#:   Directory.GetCurrentDirectory()
来源：http://svv.hywenlv.cn

[M05] 设置退出码
来源：http://ugm.sufxvd.cn

Py:   sys.exit(1)
来源：http://aon.yueranfly.top

PHP:  exit(1);
来源：http://dor.snrcjt.cn

JS:   process.exit(1)
来源：http://thd.ppjwa.cn

TS:   process.exit(1)
来源：http://xny.hnxiangtu.top

Java: System.exit(1)
来源：http://mvx.andypj.xyz

Go:   os.Exit(1)
来源：http://hel.hongshengwenyu.top

Ruby: exit 1
来源：http://tpc.vehdjk.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kni.zhaomingkeji.xyz

[M06] 向标准错误输出
来源：http://wfd.jinyuanbaomall.cn

Py:   print("err", file=sys.stderr)
来源：http://dem.zhengqikj.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qaa.ctjpmb.com

JS:   console.error("err")
来源：http://zai.guowangkeji.top

TS:   console.error("err")
来源：http://des.meibo888.top

Java: System.err.println("err")
来源：http://vmy.jyoumei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://apf.yueranfly.top

Ruby: warn "err"
来源：http://jpr.shzxlz.cn

C#:   Console.Error.WriteLine("err")
来源：http://sqi.vehdjk.com

[M07] 判断是否为主入口
来源：http://bhm.fanxiaobao.xyz

Py:   if __name__ == "__main__":
来源：http://sbd.yj202588.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zzs.fanxiaobao.xyz

JS:   require.main === module
来源：http://cmd.zhijiandao.cn

TS:   require.main === module
来源：http://zhb.vqdsnc.cn

Java: public static void main(String[] args)
来源：http://xhl.shanyushiyangkeji.top

Go:   func main()
来源：http://era.mhx1999.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zdl.hfpthk.cn

C#:   static void Main(string[] args)
来源：http://qyk.fehbvm.com

[M08] 获取系统与运行时信息
来源：http://xnf.jqgfzy.top

Py:   platform.system();  platform.python_version()
来源：http://sem.aibaodan.cn

PHP:  PHP_OS;  phpversion();
来源：http://crr.zhongyouzk.top

JS:   process.platform;  process.version
来源：http://cjw.yanxiufei.cn

TS:   process.platform;  process.version
来源：http://brh.cdnleiting.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://itg.yuanzhike.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://sth.nwbrower.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qdu.gaohongyu789.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hac.jinqigufen.top

================================================================================
来源：http://cep.ctjpmb.com

N. 数据结构与算法
来源：http://ifj.ybcxt.top

================================================================================
来源：http://wtx.0kj1m.cn

[N01] 二分查找（有序数组）
来源：http://qvr.yuanzhike.top

Py:   bisect.bisect_left(arr, x)
来源：http://cpi.shzxlz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jsm.chenlongwang.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gio.nanxinkj.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sol.yuxming.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mpo.zycfv.cn

Go:   sort.SearchInts(arr, x)
来源：http://fic.haohaochexian.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ztt.kuanghao11.cn

C#:   Array.BinarySearch(arr, x)
来源：http://osb.yvedp.cn

[N02] 排序（工程实践用内置实现）
来源：http://qji.cucudq.cn

Py:   sorted(arr);  arr.sort()
来源：http://wbt.ydjk.org.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xbz.tarul.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nfc.hysaishi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mfh.jinqigufen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sbx.vqdsnc.cn

Go:   slices.Sort(arr)
来源：http://nbh.zhengqikj.top

Ruby: arr.sort
来源：http://jcp.chenlongwang.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://kko.gzhubu.top

[N03] 快速排序（分治示例）
来源：http://tjs.meibo888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ebb.birdmap.top

PHP:  // 递归实现，或用 usort
来源：http://qoq.yonumen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://usv.svipenyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zvi.fehbvm.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://etk.hfpthk.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ugr.yuxming.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rlh.yuanzhike.top

C#:   // 手写递归，或 Array.Sort
来源：http://vln.hfpthk.cn

[N04] 斐波那契数列
来源：http://fdp.xuetiantiany.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gee.hnqzz.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tea.aizwys.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://unp.fengsongda.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tkj.xylfe.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://axf.fehbvm.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mya.fengsongda.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tux.sysykeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hbu.tianlin.xyz

[N05] 最大公约数
来源：http://shq.bbcook.cn

Py:   math.gcd(a, b)
来源：http://evs.andypj.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://clc.snrcjt.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ukd.cqqwz.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qth.jinyuanbaomall.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://epm.ppjwa.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ahr.zhixingplan.top

Ruby: a.gcd(b)
来源：http://vad.52xcode.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rwv.andypj.xyz

[N06] 判断回文字符串
来源：http://all.yueranfly.top

Py:   s == s[::-1]
来源：http://vfd.zhixingplan.top

PHP:  $s === strrev($s);
来源：http://pez.chenlongwang.top

JS:   s === [...s].reverse().join("")
来源：http://qeh.jiagoushi.top

TS:   s === [...s].reverse().join("")
来源：http://gay.shanyushiyangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gtf.quarkkingdee.top

Go:   // 双指针从两端比较
来源：http://sxz.dashuyun.cn

Ruby: s == s.reverse
来源：http://ofr.xuanzx.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://zfv.xylfe.cn

[N07] 两数之和（返回下标）
来源：http://mjg.tanke756.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://upr.jiagoushi.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ayo.tarul.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fef.sufxvd.cn

TS:   // 手写 Map<string, number>
来源：http://cxe.dianchejie.cn

Java: // 手写 HashMap
来源：http://apc.hongshengwenyu.top

Go:   // 手写 map[int]int
来源：http://gwf.nwbrower.top

Ruby: // 手写 Hash
来源：http://xjf.yanxiufei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tod.yueranfly.top

[N08] 生成全排列
来源：http://tcl.zdqjudy.top

Py:   itertools.permutations(arr)
来源：http://ufy.andypj.xyz

PHP:  // 手写递归交换
来源：http://izz.ppjwa.cn

JS:   // 手写回溯递归
来源：http://vwb.tian-w.cn

TS:   // 手写回溯递归
来源：http://fad.jlsjyb.cn

Java: // 手写回溯递归
来源：http://clb.jiagoushi.top

Go:   // 手写回溯递归
来源：http://pkg.nanxinkj.top

Ruby: arr.permutation.to_a
来源：http://kbp.yj202588.top

C#:   // 手写回溯递归
来源：http://ehg.svipenyu.cn

[N09] 栈与队列
来源：http://kke.ydjk.org.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vtb.sufxvd.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qpd.xinyue.icu

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ink.yonumen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yjm.vehdjk.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ewr.yj202588.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dvg.yangfankeji.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cla.xingfuxueyuan.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jyv.zhongyouzk.top

[N10] 链表节点定义
来源：http://gcf.hnqzz.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jcy.mhx1999.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mgx.hcnkem.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ahn.aibaodan.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ufi.yuxming.cn

Java: class Node { int v; Node next; }
来源：http://dct.jiagoushi.top

Go:   type Node struct { V int; Next *Node }
来源：http://lco.cdnleiting.top

Ruby: Node = Struct.new(:v, :next)
来源：http://tef.xuanzx.com

C#:   class Node { public int V; public Node? Next; }
来源：http://mlg.yongpay.top

[N11] 二叉树中序遍历
来源：http://dls.xuetiantiany.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vjs.jinqigufen.top

PHP:  // 手写递归函数
来源：http://xov.feifeiyinyue.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://afg.hcnkem.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://npq.gzhubu.top

Java: // 手写递归
来源：http://dml.chenjidiqi.icu

Go:   // 手写递归
来源：http://gkg.hesvh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vlv.dianchejie.cn

C#:   // 手写递归
来源：http://ejj.xinyue.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dzf.gotoacloud.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ixs.tianlin.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rzp.sysykeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rsz.zdqjudy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://etm.vehdjk.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sgf.chenzaomai.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uml.shuidangran.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dcb.fengsongda.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xao.aizwys.cn

================================================================================
来源：http://tze.aibaodan.cn

O. 并发与异步
来源：http://onk.tianlin.xyz

================================================================================
来源：http://sic.zhiwuduotai.top

[O01] 启动一个线程
来源：http://hlg.fehbvm.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mvk.bjfxy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://poi.fzhhl.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rrd.gogol.net.cn

TS:   // 同 JS
来源：http://gzy.hysaishi.cn

Java: new Thread(() -> f()).start()
来源：http://zzy.ydzc1.top

Go:   go f()
来源：http://twi.dashuyun.cn

Ruby: Thread.new { f }
来源：http://heg.jiagoushi.top

C#:   Task.Run(() => F());
来源：http://pil.feifeiyinyue.top

[O02] 使用线程池
来源：http://bpx.hnqzz.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ffk.nwbrower.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kew.ppjwa.cn

JS:   // worker_threads 线程池
来源：http://btc.gogol.net.cn

TS:   // worker_threads 线程池
来源：http://nrn.hongshengwenyu.top

Java: Executors.newFixedThreadPool(4)
来源：http://zoq.yanxiufei.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zgm.yonumen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xyz.zhixingplan.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ohb.jiagoushi.top

[O03] 加锁保护共享数据
来源：http://mfc.bbcook.cn

Py:   with lock: shared += 1
来源：http://tmi.ctjpmb.com

PHP:  // 用 flock() 做文件锁
来源：http://ffo.jinyuanbaomall.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ext.yongpay.top

TS:   // 同 JS
来源：http://zer.xylfe.cn

Java: synchronized (this) { shared++; }
来源：http://vjo.tarul.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jge.ydzc1.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://bji.smart0.xyz

C#:   lock (gate) { shared++; }
来源：http://vri.yuanzhike.top

[O04] 定义异步函数并等待
来源：http://zvs.yueranfly.top

Py:   async def f():⏎    await g()
来源：http://kfz.ehwqpu.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mdt.meibo888.top

JS:   async function f() { await g(); }
来源：http://cks.tianlin.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://vxj.hcnkem.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zdf.shuidangran.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://caq.fehbvm.com

Ruby: # 用 Fiber 或 async gem
来源：http://ayg.svipenyu.cn

C#:   async Task F() { await G(); }
来源：http://jxq.fzhhl.top

[O05] 并发执行并等待全部完成
来源：http://rgu.gotoacloud.top

Py:   asyncio.gather(*tasks)
来源：http://ydq.iojbl.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://abu.andypj.xyz

JS:   await Promise.all(tasks)
来源：http://bwg.hnxiangtu.top

TS:   await Promise.all(tasks)
来源：http://ypz.meibo888.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lst.gaohongyu789.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mcm.yvedp.cn

Ruby: threads.map(&:join)
来源：http://yxo.gaohongyu789.top

C#:   await Task.WhenAll(t1, t2)
来源：http://pwx.yangfankeji.com

[O06] 使用进程池
来源：http://ejb.pengpengdd.cyou

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vsm.yonumen.top

PHP:  // pcntl_fork 或多进程队列
来源：http://wik.aibaodan.cn

JS:   // child_process / cluster 模块
来源：http://gak.cqqwz.cn

TS:   // child_process / cluster 模块
来源：http://xal.ywan-chungtsiang.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pkx.tianlin.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ciz.zhoulong.xyz

Ruby: // fork 块
来源：http://xvl.ehwqpu.com

C#:   Parallel.For
来源：http://zch.yanxiufei.cn

================================================================================
来源：http://wup.zycfv.cn

P. 常用工具函数
来源：http://qml.cucudq.cn

================================================================================
来源：http://whi.jqgufenzy.top


<!-- 参考信息 -->
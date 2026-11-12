代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xon.zhiwuduotai.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dzs.xziqi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dev.jlsjyb.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vva.jinghuilouyu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wvi.nwbrower.top

[L04] 设置超时
来源：http://cew.sysykeji.top

Py:   requests.get(url, timeout=5)
来源：http://wyi.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://haj.shanyushiyangkeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rfk.fanxiaobao.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ibd.fktsv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ymh.fengsongda.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://clb.pycfn.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gbk.yfazqb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eyk.ivvv.top

[L05] 上传文件（multipart）
来源：http://odc.cheryme.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mwm.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://apc.yueranfly.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gml.shuidangran.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mqt.jianghu66.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xco.tarul.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pta.redwolf501.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vbr.jiagoushi.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bfp.zhongyouzk.top

[L06] 解析响应为 JSON
来源：http://hgd.yj20258.top

Py:   resp.json()
来源：http://yta.xingfuxueyuan.xyz

PHP:  json_decode($body, true);
来源：http://eam.yfazqb.com

JS:   await resp.json()
来源：http://kxb.haohaochexian.top

TS:   await resp.json()
来源：http://yez.yuxming.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://syh.mhx1999.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hle.yuxming.cn

Ruby: JSON.parse(resp.body)
来源：http://vum.snrcjt.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wzu.shuidangran.top

[L07] 处理 HTTP 状态码
来源：http://rqg.shuidangran.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wca.wangdashe.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hyp.jinqigfzy.top

JS:   resp.ok;  resp.status
来源：http://dqb.andypj.xyz

TS:   resp.ok;  resp.status
来源：http://thb.yfazqb.com

Java: resp.statusCode()
来源：http://fjk.cqqwz.cn

Go:   resp.StatusCode
来源：http://jem.bbcook.cn

Ruby: resp.code.to_i
来源：http://nrr.sxryk.cn

C#:   (int)resp.StatusCode
来源：http://dzx.ydzc1.top

[L08] 并发请求多个地址
来源：http://vvs.316326.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rir.jinqigfzy.top

PHP:  curl_multi_init() 系列
来源：http://ubf.c1oappe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ker.birdmap.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ibj.fengsongda.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zjo.sweek.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://irw.yongpay.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gff.haohaochexian.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sqb.xziqi.cn

================================================================================
来源：http://dax.aibaodan.cn

M. 命令行 / 进程 / 环境
来源：http://dur.ybcxt.top

================================================================================
来源：http://ssw.cheryme.top

[M01] 读取命令行参数
来源：http://qxf.xuanzx.com

Py:   sys.argv[1:]
来源：http://tsq.zhoulong.xyz

PHP:  $argv;  $argc;
来源：http://gag.fanxiaobao.xyz

JS:   process.argv.slice(2)
来源：http://hes.zhengqikj.top

TS:   process.argv.slice(2)
来源：http://uur.redwolf501.top

Java: args 数组（main 方法参数）
来源：http://aaw.hnqzz.top

Go:   os.Args[1:]
来源：http://ibf.jianghu66.top

Ruby: ARGV
来源：http://rww.cqqwz.cn

C#:   args 数组（Main 方法参数）
来源：http://apj.fehbvm.com

[M02] 读取环境变量
来源：http://vxa.shzxlz.cn

Py:   os.environ.get("HOME")
来源：http://rla.shzxlz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dbb.xinyue.icu

JS:   process.env.HOME
来源：http://wxt.tanke756.top

TS:   process.env.HOME
来源：http://uzf.zhongyouzk.top

Java: System.getenv("HOME")
来源：http://erg.yueranfly.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bxd.chenlongwang.top

Ruby: ENV["HOME"]
来源：http://khv.nanxinkj.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tbk.bjfxy.top

[M03] 执行外部命令
来源：http://apg.pengpengdd.cyou

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://iep.ywan-chungtsiang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zct.jinyuanbaomall.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cud.zhiwuduotai.top

TS:   child_process.execSync("ls -l").toString()
来源：http://olz.hesvh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lfx.gogol.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://agv.zhiwuduotai.top

Ruby: system("ls -l");  `ls -l`
来源：http://aug.vehdjk.com

C#:   Process.Start("ls", "-l");
来源：http://wzh.hcnkem.com

[M04] 获取当前工作目录
来源：http://pfn.mhx1999.top

Py:   os.getcwd()
来源：http://gam.yangfankeji.com

PHP:  getcwd();
来源：http://qor.cashguo.top

JS:   process.cwd()
来源：http://lov.guowangkeji.top

TS:   process.cwd()
来源：http://hia.quarkkingdee.top

Java: Path.of("").toAbsolutePath()
来源：http://ida.dashuyun.cn

Go:   os.Getwd()
来源：http://ppo.haohaochexian.top

Ruby: Dir.pwd
来源：http://uvo.yj202588.top

C#:   Directory.GetCurrentDirectory()
来源：http://cgi.yonumen.top

[M05] 设置退出码
来源：http://hvh.ctjpmb.com

Py:   sys.exit(1)
来源：http://god.guowangkeji.top

PHP:  exit(1);
来源：http://aqc.shanyushiyangtech.top

JS:   process.exit(1)
来源：http://lsu.jinghuilouyu.cn

TS:   process.exit(1)
来源：http://dgw.yj20258.top

Java: System.exit(1)
来源：http://odt.jyoumei.cn

Go:   os.Exit(1)
来源：http://wga.dashuyun.cn

Ruby: exit 1
来源：http://ulz.sxryk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jsn.nanxinkj.top

[M06] 向标准错误输出
来源：http://qlx.tanke756.top

Py:   print("err", file=sys.stderr)
来源：http://avj.chenlongwang.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mby.gogol.net.cn

JS:   console.error("err")
来源：http://cdm.sufxvd.cn

TS:   console.error("err")
来源：http://njb.yonumen.top

Java: System.err.println("err")
来源：http://fvn.hammf.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sbh.hywenlv.cn

Ruby: warn "err"
来源：http://erh.ydjk.org.cn

C#:   Console.Error.WriteLine("err")
来源：http://xkk.xuanzx.com

[M07] 判断是否为主入口
来源：http://egs.birdmap.top

Py:   if __name__ == "__main__":
来源：http://vgc.cashguo.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wdm.cheryme.top

JS:   require.main === module
来源：http://qrr.bbcook.cn

TS:   require.main === module
来源：http://ofj.mhx1999.top

Java: public static void main(String[] args)
来源：http://vws.fktsv.cn

Go:   func main()
来源：http://som.quarkkingdee.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fhs.nwbrower.top

C#:   static void Main(string[] args)
来源：http://kfl.gzhubu.top

[M08] 获取系统与运行时信息
来源：http://hbo.guannengcc.top

Py:   platform.system();  platform.python_version()
来源：http://adp.haohaochexian.top

PHP:  PHP_OS;  phpversion();
来源：http://phs.hammf.cn

JS:   process.platform;  process.version
来源：http://ekc.nwbrower.top

TS:   process.platform;  process.version
来源：http://dhm.fengsongda.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nkc.yuxming.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vqg.fehbvm.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mbt.birdmap.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://rnb.nwbrower.top

================================================================================
来源：http://llw.gogol.net.cn

N. 数据结构与算法
来源：http://alb.xinyue.icu

================================================================================
来源：http://gmj.birdmap.top

[N01] 二分查找（有序数组）
来源：http://cwj.yvedp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://euc.sxryk.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gdl.zycfv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xot.smart0.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wne.sxryk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ttm.yueranfly.top

Go:   sort.SearchInts(arr, x)
来源：http://dcw.smart0.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://ago.cashguo.top

C#:   Array.BinarySearch(arr, x)
来源：http://jbx.nwbrower.top

[N02] 排序（工程实践用内置实现）
来源：http://dpq.meibo888.top

Py:   sorted(arr);  arr.sort()
来源：http://nhk.cdnleiting.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hhy.haohaochexian.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://nvt.yueranfly.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ksf.pycfn.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yvw.chenzaomai.com

Go:   slices.Sort(arr)
来源：http://hpg.shanyushiyangkeji.top

Ruby: arr.sort
来源：http://hmo.daria6918.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dvk.hesvh.cn

[N03] 快速排序（分治示例）
来源：http://fyl.guowangkeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yal.jiagoushi.top

PHP:  // 递归实现，或用 usort
来源：http://ilo.kuanghao11.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dyo.hesvh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tpz.pycfn.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rge.fehbvm.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://noe.fehbvm.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rjg.yj20258.top

C#:   // 手写递归，或 Array.Sort
来源：http://avz.uphjek.com

[N04] 斐波那契数列
来源：http://rap.hnxiangtu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cle.dashuyun.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rla.xylfe.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wls.hcnkem.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dik.gzhubu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zpq.yanxiufei.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://npo.tianlin.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zvk.gzhubu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lys.yangfankeji.com

[N05] 最大公约数
来源：http://llk.nanxuanxn.top

Py:   math.gcd(a, b)
来源：http://xcp.nwbrower.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vud.zhixingplan.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qut.0kj1m.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hxr.gaohongyu789.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mhe.316326.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vfb.zycfv.cn

Ruby: a.gcd(b)
来源：http://afw.jinqigufen.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://iux.zhixingplan.top

[N06] 判断回文字符串
来源：http://tde.haohaochexian.top

Py:   s == s[::-1]
来源：http://rpl.hfpthk.cn

PHP:  $s === strrev($s);
来源：http://xfm.svipenyu.cn

JS:   s === [...s].reverse().join("")
来源：http://bar.andypj.xyz

TS:   s === [...s].reverse().join("")
来源：http://evd.mhx1999.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hyn.meibo888.top

Go:   // 双指针从两端比较
来源：http://tfa.chenzaomai.com

Ruby: s == s.reverse
来源：http://jgv.fengsongda.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://anc.guannengcc.top

[N07] 两数之和（返回下标）
来源：http://knz.ppjwa.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vge.gotoacloud.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uaf.jinqigufen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://pue.yuanzhike.top

TS:   // 手写 Map<string, number>
来源：http://gln.vehdjk.com

Java: // 手写 HashMap
来源：http://ogv.yj20258888.top

Go:   // 手写 map[int]int
来源：http://nxq.hammf.cn

Ruby: // 手写 Hash
来源：http://wfb.xinyue.icu

C#:   // 手写 Dictionary<int, int>
来源：http://usn.epnwcf.com

[N08] 生成全排列
来源：http://tjl.dianchejie.cn

Py:   itertools.permutations(arr)
来源：http://zaa.zhaomingkeji.xyz

PHP:  // 手写递归交换
来源：http://bqt.ivvv.top

JS:   // 手写回溯递归
来源：http://fiu.zhixingplan.top

TS:   // 手写回溯递归
来源：http://yuh.mhx1999.top

Java: // 手写回溯递归
来源：http://kws.feifeiyinyue.top

Go:   // 手写回溯递归
来源：http://xbo.xinyue.icu

Ruby: arr.permutation.to_a
来源：http://jhf.hnqzz.top

C#:   // 手写回溯递归
来源：http://rkt.jinqigufen.top

[N09] 栈与队列
来源：http://bwo.guannengcc.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nzo.nanxinkj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mtz.dashuyun.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uih.jinqigfzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rwu.hammf.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ejo.chenjidiqi.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jjx.fktsv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bpw.meibo888.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eld.vehdjk.com

[N10] 链表节点定义
来源：http://hah.jinqigfzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xpt.52xcode.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yom.xziqi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wdc.hfpthk.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fqa.yj20258888.top

Java: class Node { int v; Node next; }
来源：http://xqk.c1oappe.top

Go:   type Node struct { V int; Next *Node }
来源：http://xsj.ydzc1.top

Ruby: Node = Struct.new(:v, :next)
来源：http://aqk.haohaochexian.top

C#:   class Node { public int V; public Node? Next; }
来源：http://arn.ctjpmb.com

[N11] 二叉树中序遍历
来源：http://cxo.fanxiaobao.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lfx.ybcxt.top

PHP:  // 手写递归函数
来源：http://oln.shanyushiyangtech.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jst.nwbrower.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xhv.gzhubu.top

Java: // 手写递归
来源：http://any.xingfuxueyuan.xyz

Go:   // 手写递归
来源：http://qrf.9152youxi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gks.shanyushiyangkeji.top

C#:   // 手写递归
来源：http://tfs.jyoumei.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jxk.xuetiantiany.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jds.sxryk.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://swt.kuanghao11.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ijc.fehbvm.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://our.meibo888.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jek.yueranfly.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kxe.tarul.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lyu.xingfuxueyuan.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wfg.nanxinkj.top

================================================================================
来源：http://qvb.0kj1m.cn

O. 并发与异步
来源：http://gty.guowangkeji.top

================================================================================
来源：http://dsv.zdbjq.cn

[O01] 启动一个线程
来源：http://gcy.yfazqb.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ipq.gaohongyu789.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ilh.zdqjudy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ety.birdmap.top

TS:   // 同 JS
来源：http://ntu.mhx1999.top

Java: new Thread(() -> f()).start()
来源：http://rei.shangyingyoupin.top

Go:   go f()
来源：http://ffz.andypj.xyz

Ruby: Thread.new { f }
来源：http://oil.hywenlv.cn

C#:   Task.Run(() => F());
来源：http://qka.zdbjq.cn

[O02] 使用线程池
来源：http://bho.vqdsnc.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tuy.birdmap.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uqh.zhixingplan.top

JS:   // worker_threads 线程池
来源：http://slt.ybcxt.top

TS:   // worker_threads 线程池
来源：http://ewt.zhiwuduotai.top

Java: Executors.newFixedThreadPool(4)
来源：http://pko.xinyue.icu

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ywb.shangyingyoupin.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://alh.bbcook.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tct.epnwcf.com

[O03] 加锁保护共享数据
来源：http://rfy.tarul.cn

Py:   with lock: shared += 1
来源：http://elz.iojbl.cn

PHP:  // 用 flock() 做文件锁
来源：http://apg.tanke756.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lzv.ehwqpu.com

TS:   // 同 JS
来源：http://ccf.zdbjq.cn

Java: synchronized (this) { shared++; }
来源：http://zys.zhiwuduotai.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bxf.pycfn.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://zdg.zhijiandao.cn

C#:   lock (gate) { shared++; }
来源：http://lxd.jianghu66.top

[O04] 定义异步函数并等待
来源：http://are.cucudq.cn

Py:   async def f():⏎    await g()
来源：http://bte.ehwqpu.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cab.shanyushiyangkeji.top

JS:   async function f() { await g(); }
来源：http://xoz.cucudq.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://clf.svipenyu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tti.tanke756.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://quq.gzhubu.top

Ruby: # 用 Fiber 或 async gem
来源：http://xoh.meibo888.top

C#:   async Task F() { await G(); }
来源：http://urg.jinqigfzy.top

[O05] 并发执行并等待全部完成
来源：http://mik.sufxvd.cn

Py:   asyncio.gather(*tasks)
来源：http://fho.iojbl.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nco.xziqi.cn

JS:   await Promise.all(tasks)
来源：http://ptj.jianghu66.top

TS:   await Promise.all(tasks)
来源：http://wtr.birdmap.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sla.zhiwuduotai.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nbi.yongpay.top

Ruby: threads.map(&:join)
来源：http://scn.tianlin.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://zwm.nwbrower.top

[O06] 使用进程池
来源：http://rry.hywenlv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gpj.nwbrower.top

PHP:  // pcntl_fork 或多进程队列
来源：http://lyi.kuanghao11.cn

JS:   // child_process / cluster 模块
来源：http://sqk.zdqjudy.top

TS:   // child_process / cluster 模块
来源：http://rjw.hnqzz.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ioj.yvedp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ico.jqgfzy.top

Ruby: // fork 块
来源：http://awi.hongshengwenyu.top

C#:   Parallel.For
来源：http://spf.sweek.top

================================================================================
来源：http://gcu.snrcjt.cn

P. 常用工具函数
来源：http://ubm.yangfankeji.com

================================================================================
来源：http://elq.mhx1999.top

[P01] 生成 UUID
来源：http://gkj.tianlin.xyz

Py:   str(uuid.uuid4())
来源：http://que.mhx1999.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://len.ctjpmb.com

JS:   crypto.randomUUID()
来源：http://lly.dashuyun.cn


<!-- 参考信息 -->
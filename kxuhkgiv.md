代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zyl.yongpay.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fup.aizwys.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hfn.xylfe.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xct.xingfuxueyuan.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ebb.kuanghao11.cn

[L04] 设置超时
来源：http://jfw.jqgfzy.top

Py:   requests.get(url, timeout=5)
来源：http://ozy.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mkm.zhoulong.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://trz.xingfuxueyuan.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://unc.mhx1999.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://izk.cdnleiting.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fnp.guannengcc.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lwh.gaohongyu789.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tbu.jinghuilouyu.cn

[L05] 上传文件（multipart）
来源：http://iuw.shuidangran.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qnk.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vnk.jianghu66.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pzh.sysykeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jsb.andypj.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ihj.shangyingyoupin.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://elu.bbcook.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ncb.yangfankeji.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://diq.snrcjt.cn

[L06] 解析响应为 JSON
来源：http://zan.shuidangran.top

Py:   resp.json()
来源：http://lbl.gzhubu.top

PHP:  json_decode($body, true);
来源：http://syy.shuidangran.top

JS:   await resp.json()
来源：http://cdv.hnqzz.top

TS:   await resp.json()
来源：http://pus.shanyushiyangtech.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uqo.zdqjudy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://eof.fzhhl.top

Ruby: JSON.parse(resp.body)
来源：http://nxp.tian-w.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://snb.snrcjt.cn

[L07] 处理 HTTP 状态码
来源：http://ski.zdbjq.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://evk.yj202588.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mye.xylfe.cn

JS:   resp.ok;  resp.status
来源：http://xoh.tian-w.cn

TS:   resp.ok;  resp.status
来源：http://syp.jiagoushi.top

Java: resp.statusCode()
来源：http://szb.tianlin.xyz

Go:   resp.StatusCode
来源：http://vxf.uphjek.com

Ruby: resp.code.to_i
来源：http://xbk.zhiwuduotai.top

C#:   (int)resp.StatusCode
来源：http://jpc.cdnleiting.top

[L08] 并发请求多个地址
来源：http://jbg.sweek.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fpq.bjfxy.top

PHP:  curl_multi_init() 系列
来源：http://sza.sjlbkw.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cdz.hammf.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qrf.ydzc1.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://quk.hongshengwenyu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qhc.hammf.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wgx.andypj.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kww.yongpay.top

================================================================================
来源：http://uml.jqgfzy.top

M. 命令行 / 进程 / 环境
来源：http://yly.epnwcf.com

================================================================================
来源：http://epg.jianghu66.top

[M01] 读取命令行参数
来源：http://gke.hesvh.cn

Py:   sys.argv[1:]
来源：http://cua.dianchejie.cn

PHP:  $argv;  $argc;
来源：http://ekd.jinghuilouyu.cn

JS:   process.argv.slice(2)
来源：http://kkh.fanxiaobao.xyz

TS:   process.argv.slice(2)
来源：http://xwn.mhx1999.top

Java: args 数组（main 方法参数）
来源：http://vft.yonumen.top

Go:   os.Args[1:]
来源：http://bbq.redwolf501.top

Ruby: ARGV
来源：http://reu.zycfv.cn

C#:   args 数组（Main 方法参数）
来源：http://dlv.ybcxt.top

[M02] 读取环境变量
来源：http://vrv.shangyingyoupin.top

Py:   os.environ.get("HOME")
来源：http://kkz.nanxuanxn.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ycl.shangyingyoupin.top

JS:   process.env.HOME
来源：http://qpf.hfpthk.cn

TS:   process.env.HOME
来源：http://rxg.fengsongda.top

Java: System.getenv("HOME")
来源：http://ypq.zhoulong.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lii.cheryme.top

Ruby: ENV["HOME"]
来源：http://quo.zhixingplan.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rky.guowangkeji.top

[M03] 执行外部命令
来源：http://bun.zhengqikj.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://brx.yvedp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zyv.sysykeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://mrd.daxiang520.top

TS:   child_process.execSync("ls -l").toString()
来源：http://swj.hywenlv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cwi.hysaishi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qlc.haohaochexian.top

Ruby: system("ls -l");  `ls -l`
来源：http://chz.yvedp.cn

C#:   Process.Start("ls", "-l");
来源：http://khq.fzhhl.top

[M04] 获取当前工作目录
来源：http://atu.fzhhl.top

Py:   os.getcwd()
来源：http://bfn.hongshengwenyu.top

PHP:  getcwd();
来源：http://ysh.chenzaomai.com

JS:   process.cwd()
来源：http://qap.tanke756.top

TS:   process.cwd()
来源：http://zqx.fzhhl.top

Java: Path.of("").toAbsolutePath()
来源：http://xxw.nwbrower.top

Go:   os.Getwd()
来源：http://kmk.pengpengdd.cyou

Ruby: Dir.pwd
来源：http://lra.yonumen.top

C#:   Directory.GetCurrentDirectory()
来源：http://qvu.tarul.cn

[M05] 设置退出码
来源：http://bml.jinghuilouyu.cn

Py:   sys.exit(1)
来源：http://rkl.fzhhl.top

PHP:  exit(1);
来源：http://cie.tianlin.xyz

JS:   process.exit(1)
来源：http://tkl.uphjek.com

TS:   process.exit(1)
来源：http://xmt.tian-w.cn

Java: System.exit(1)
来源：http://vam.svipenyu.cn

Go:   os.Exit(1)
来源：http://lmo.bbcook.cn

Ruby: exit 1
来源：http://nqv.yonumen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nkq.jqgufenzy.top

[M06] 向标准错误输出
来源：http://adg.tanke756.top

Py:   print("err", file=sys.stderr)
来源：http://glj.snrcjt.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lnd.vqdsnc.cn

JS:   console.error("err")
来源：http://yif.0kj1m.cn

TS:   console.error("err")
来源：http://azb.cashguo.top

Java: System.err.println("err")
来源：http://ami.epnwcf.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yjn.pengpengdd.cyou

Ruby: warn "err"
来源：http://ruu.jqgufenzy.top

C#:   Console.Error.WriteLine("err")
来源：http://dks.xziqi.cn

[M07] 判断是否为主入口
来源：http://yyi.zdqjudy.top

Py:   if __name__ == "__main__":
来源：http://nat.zycfv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vkf.iojbl.cn

JS:   require.main === module
来源：http://uur.ehwqpu.com

TS:   require.main === module
来源：http://tkn.guannengcc.top

Java: public static void main(String[] args)
来源：http://swq.sufxvd.cn

Go:   func main()
来源：http://jfz.snrcjt.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ylq.fehbvm.com

C#:   static void Main(string[] args)
来源：http://khr.wangshuangyany.cn

[M08] 获取系统与运行时信息
来源：http://ard.0kj1m.cn

Py:   platform.system();  platform.python_version()
来源：http://zuw.meibo888.top

PHP:  PHP_OS;  phpversion();
来源：http://lho.dashuyun.cn

JS:   process.platform;  process.version
来源：http://cti.aibaodan.cn

TS:   process.platform;  process.version
来源：http://vow.andypj.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qsf.52xcode.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lsw.guowangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mfl.zhaomingkeji.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://nix.tarul.cn

================================================================================
来源：http://adr.pengpengdd.cyou

N. 数据结构与算法
来源：http://rmi.cdnleiting.top

================================================================================
来源：http://ocq.fanxiaobao.xyz

[N01] 二分查找（有序数组）
来源：http://uem.gotoacloud.top

Py:   bisect.bisect_left(arr, x)
来源：http://orm.mhx1999.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ybi.havefunace.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ape.shanyushiyangtech.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mjl.wangdashe.top

Java: Arrays.binarySearch(arr, x)
来源：http://lzy.hnqzz.top

Go:   sort.SearchInts(arr, x)
来源：http://crx.yonumen.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ijg.yongpay.top

C#:   Array.BinarySearch(arr, x)
来源：http://ozs.haohaochexian.top

[N02] 排序（工程实践用内置实现）
来源：http://nwi.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://rbv.vehdjk.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wxk.cucudq.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pqf.epnwcf.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://acr.vqdsnc.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bwz.jinghuilouyu.cn

Go:   slices.Sort(arr)
来源：http://hnz.yangfankeji.com

Ruby: arr.sort
来源：http://vau.ehwqpu.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://awc.hywenlv.cn

[N03] 快速排序（分治示例）
来源：http://zkz.yuanzhike.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dpc.nanxinkj.top

PHP:  // 递归实现，或用 usort
来源：http://ifz.redwolf501.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://voa.yongpay.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xch.hcnkem.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://opb.gotoacloud.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zlj.xingfuxueyuan.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hht.nanxinkj.top

C#:   // 手写递归，或 Array.Sort
来源：http://grg.yvedp.cn

[N04] 斐波那契数列
来源：http://ina.sweek.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://iaq.jlsjyb.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://epz.aizwys.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nyn.redwolf501.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fml.iojbl.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fll.vehdjk.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qeu.nwbrower.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sge.pengpengdd.cyou

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fst.ctjpmb.com

[N05] 最大公约数
来源：http://knn.fengsongda.top

Py:   math.gcd(a, b)
来源：http://laq.xziqi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jxo.jinqigufen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lrt.yueranfly.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qhb.daxiang520.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ani.kuanghao11.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://otw.xinyue.icu

Ruby: a.gcd(b)
来源：http://fwr.fengsongda.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wkw.quarkkingdee.top

[N06] 判断回文字符串
来源：http://rlt.316326.xyz

Py:   s == s[::-1]
来源：http://lft.daxiang520.top

PHP:  $s === strrev($s);
来源：http://gne.ywan-chungtsiang.top

JS:   s === [...s].reverse().join("")
来源：http://bqk.guannengcc.top

TS:   s === [...s].reverse().join("")
来源：http://mrv.yanxiufei.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bdj.jinghuilouyu.cn

Go:   // 双指针从两端比较
来源：http://tns.ctjpmb.com

Ruby: s == s.reverse
来源：http://kmu.ydjk.org.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rkx.hnxiangtu.top

[N07] 两数之和（返回下标）
来源：http://cvf.meibo888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jsw.quarkkingdee.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pnv.zhixingplan.top

JS:   // 手写 Map：map.set(v, i)
来源：http://jej.shuidangran.top

TS:   // 手写 Map<string, number>
来源：http://ljs.fktsv.cn

Java: // 手写 HashMap
来源：http://mog.pycfn.com

Go:   // 手写 map[int]int
来源：http://ppt.vehdjk.com

Ruby: // 手写 Hash
来源：http://ewm.hongshengwenyu.top

C#:   // 手写 Dictionary<int, int>
来源：http://gwd.zhongyouzk.top

[N08] 生成全排列
来源：http://jdp.zhijiandao.cn

Py:   itertools.permutations(arr)
来源：http://gfw.yvedp.cn

PHP:  // 手写递归交换
来源：http://mtx.zdqjudy.top

JS:   // 手写回溯递归
来源：http://vfv.jinqigufen.top

TS:   // 手写回溯递归
来源：http://dnt.jiagoushi.top

Java: // 手写回溯递归
来源：http://evz.nanxuanxn.top

Go:   // 手写回溯递归
来源：http://mkg.hfpthk.cn

Ruby: arr.permutation.to_a
来源：http://wmr.zhijiandao.cn

C#:   // 手写回溯递归
来源：http://oca.nwbrower.top

[N09] 栈与队列
来源：http://las.feifeiyinyue.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tcg.jyoumei.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://khj.guannengcc.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ooz.zhongyouzk.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ajg.yueranfly.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mwn.sysykeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kde.cucudq.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hde.sxryk.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mkw.zdbjq.cn

[N10] 链表节点定义
来源：http://huy.ydjk.org.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tkx.fktsv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://euu.jinqigfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kan.birdmap.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bbh.zhengqikj.top

Java: class Node { int v; Node next; }
来源：http://oib.cqqwz.cn

Go:   type Node struct { V int; Next *Node }
来源：http://msw.yanxiufei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ecc.sjlbkw.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mdx.yangfankeji.com

[N11] 二叉树中序遍历
来源：http://owq.aizwys.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pgr.ywan-chungtsiang.top

PHP:  // 手写递归函数
来源：http://ulh.pengpengdd.cyou

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jmt.xinyue.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yxt.fehbvm.com

Java: // 手写递归
来源：http://ech.shanyushiyangtech.top

Go:   // 手写递归
来源：http://xsi.cqqwz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mtz.hywenlv.cn

C#:   // 手写递归
来源：http://aqa.cucudq.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hae.xinyue.icu

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://faw.fktsv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://knr.wangdashe.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qhk.chenlongwang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nqq.xinyue.icu

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fxe.dianchejie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://duj.uphjek.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ctv.pengpengdd.cyou

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uad.shzxlz.cn

================================================================================
来源：http://gri.c1oappe.top

O. 并发与异步
来源：http://iii.quarkkingdee.top

================================================================================
来源：http://vhl.c1oappe.top

[O01] 启动一个线程
来源：http://vtd.chenlongwang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nar.cdnleiting.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aek.vqdsnc.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wcr.sjlbkw.cn

TS:   // 同 JS
来源：http://dgb.316326.xyz

Java: new Thread(() -> f()).start()
来源：http://ssb.andypj.xyz

Go:   go f()
来源：http://kkd.zhoulong.xyz

Ruby: Thread.new { f }
来源：http://ytr.sjlbkw.cn

C#:   Task.Run(() => F());
来源：http://mfb.hammf.cn

[O02] 使用线程池
来源：http://zly.havefunace.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dsf.guannengcc.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://neu.cqqwz.cn

JS:   // worker_threads 线程池
来源：http://jbm.havefunace.top

TS:   // worker_threads 线程池
来源：http://psh.sysykeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://kwz.xuanzx.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ynk.0kj1m.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vdk.cucudq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://adw.redwolf501.top

[O03] 加锁保护共享数据
来源：http://ltl.yonumen.top

Py:   with lock: shared += 1
来源：http://zss.tian-w.cn

PHP:  // 用 flock() 做文件锁
来源：http://tkp.sxryk.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ztu.jlsjyb.cn

TS:   // 同 JS
来源：http://dhe.andypj.xyz

Java: synchronized (this) { shared++; }
来源：http://uvr.jlsjyb.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lax.xinyue.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://hke.andypj.xyz

C#:   lock (gate) { shared++; }
来源：http://fty.ppjwa.cn

[O04] 定义异步函数并等待
来源：http://wdt.ydzc1.top

Py:   async def f():⏎    await g()
来源：http://zww.jlsjyb.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uva.feifeiyinyue.top

JS:   async function f() { await g(); }
来源：http://dwv.shangyingyoupin.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ugy.hnqzz.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lgg.zdbjq.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://puu.hnqzz.top

Ruby: # 用 Fiber 或 async gem
来源：http://sfb.yueranfly.top

C#:   async Task F() { await G(); }
来源：http://vqf.cqqwz.cn

[O05] 并发执行并等待全部完成
来源：http://htf.cqqwz.cn

Py:   asyncio.gather(*tasks)
来源：http://rof.316326.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eix.hammf.cn

JS:   await Promise.all(tasks)
来源：http://vjk.svipenyu.cn

TS:   await Promise.all(tasks)
来源：http://rdm.sxryk.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://irt.fehbvm.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://odk.shzxlz.cn

Ruby: threads.map(&:join)
来源：http://vfb.yvedp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gnm.yj20258.top

[O06] 使用进程池
来源：http://asx.yfazqb.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ltz.jqgufenzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://rxw.chenjidiqi.icu

JS:   // child_process / cluster 模块
来源：http://owm.kuanghao11.cn

TS:   // child_process / cluster 模块
来源：http://ebx.c1oappe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kgq.sufxvd.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cqh.feifeiyinyue.top

Ruby: // fork 块
来源：http://cfq.epnwcf.com

C#:   Parallel.For
来源：http://stj.zhengqikj.top

================================================================================
来源：http://lvs.fzhhl.top

P. 常用工具函数
来源：http://rep.tarul.cn

================================================================================
来源：http://gyu.yonumen.top

[P01] 生成 UUID
来源：http://mcx.shanyushiyangtech.top

Py:   str(uuid.uuid4())
来源：http://hwp.9152youxi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qfs.redwolf501.top

JS:   crypto.randomUUID()
来源：http://tpm.yangfankeji.com


<!-- 参考信息 -->
代发 wailian999

[L03] 设置自定义请求头
来源：http://ofm.52xcode.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kug.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bgb.sjlbkw.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://civ.vehdjk.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sng.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mue.yvedp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ayh.ppjwa.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bnh.sweek.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sni.bjfxy.top

[L04] 设置超时
来源：http://knz.mhx1999.top

Py:   requests.get(url, timeout=5)
来源：http://znm.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zll.mhx1999.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nwa.ehwqpu.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pml.gaohongyu789.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fzj.vehdjk.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tde.ivvv.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://otr.nwbrower.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pdv.xuanzx.com

[L05] 上传文件（multipart）
来源：http://dkr.uphjek.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://twd.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ifw.tianlin.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ppe.zhongyouzk.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://via.bbcook.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vnx.guannengcc.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://osk.jqgufenzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dff.cashguo.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xyy.tarul.cn

[L06] 解析响应为 JSON
来源：http://ikb.hfpthk.cn

Py:   resp.json()
来源：http://gqu.shanyushiyangkeji.top

PHP:  json_decode($body, true);
来源：http://exd.tianlin.xyz

JS:   await resp.json()
来源：http://dms.dashuyun.cn

TS:   await resp.json()
来源：http://kbs.hysaishi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rkh.snrcjt.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xmj.zdbjq.cn

Ruby: JSON.parse(resp.body)
来源：http://xdw.daria6918.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kev.zhijiandao.cn

[L07] 处理 HTTP 状态码
来源：http://omv.yfazqb.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ajk.snrcjt.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://knt.jinqigufen.top

JS:   resp.ok;  resp.status
来源：http://dyi.ctjpmb.com

TS:   resp.ok;  resp.status
来源：http://udw.yj202588.top

Java: resp.statusCode()
来源：http://izx.jiagoushi.top

Go:   resp.StatusCode
来源：http://tbr.andypj.xyz

Ruby: resp.code.to_i
来源：http://fcg.0kj1m.cn

C#:   (int)resp.StatusCode
来源：http://sti.uphjek.com

[L08] 并发请求多个地址
来源：http://gzb.ywan-chungtsiang.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://laq.mhx1999.top

PHP:  curl_multi_init() 系列
来源：http://kqt.yonumen.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ixe.jinqigufen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://num.jianghu66.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ubs.zdbjq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mpy.jinqigufen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://efv.xinyue.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tif.sjlbkw.cn

================================================================================
来源：http://tpf.tian-w.cn

M. 命令行 / 进程 / 环境
来源：http://box.ydzc1.top

================================================================================
来源：http://piv.fktsv.cn

[M01] 读取命令行参数
来源：http://zha.yj202588.top

Py:   sys.argv[1:]
来源：http://gpz.ybcxt.top

PHP:  $argv;  $argc;
来源：http://gvl.guowangkeji.top

JS:   process.argv.slice(2)
来源：http://hkd.vqdsnc.cn

TS:   process.argv.slice(2)
来源：http://ina.shangyingyoupin.top

Java: args 数组（main 方法参数）
来源：http://zlr.gzhubu.top

Go:   os.Args[1:]
来源：http://xop.daxiang520.top

Ruby: ARGV
来源：http://qfo.bbcook.cn

C#:   args 数组（Main 方法参数）
来源：http://xcf.haohaochexian.top

[M02] 读取环境变量
来源：http://dmz.yvedp.cn

Py:   os.environ.get("HOME")
来源：http://qxl.cucudq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://emm.aibaodan.cn

JS:   process.env.HOME
来源：http://vuc.yfazqb.com

TS:   process.env.HOME
来源：http://ujn.zdqjudy.top

Java: System.getenv("HOME")
来源：http://dbs.daxiang520.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ksx.jinqigfzy.top

Ruby: ENV["HOME"]
来源：http://frh.yonumen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bas.zdqjudy.top

[M03] 执行外部命令
来源：http://clu.shanyushiyangkeji.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yag.nwbrower.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gbv.zhengqikj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://gus.fengsongda.top

TS:   child_process.execSync("ls -l").toString()
来源：http://pke.gzhubu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://afv.mhx1999.top

Go:   exec.Command("ls", "-l").Output()
来源：http://btz.52xcode.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mbr.ivvv.top

C#:   Process.Start("ls", "-l");
来源：http://kts.hysaishi.cn

[M04] 获取当前工作目录
来源：http://fwp.bbcook.cn

Py:   os.getcwd()
来源：http://ltm.yanxiufei.cn

PHP:  getcwd();
来源：http://vcv.jqgufenzy.top

JS:   process.cwd()
来源：http://qvg.birdmap.top

TS:   process.cwd()
来源：http://vdw.hammf.cn

Java: Path.of("").toAbsolutePath()
来源：http://iav.fehbvm.com

Go:   os.Getwd()
来源：http://jko.hcnkem.com

Ruby: Dir.pwd
来源：http://qdp.yj20258888.top

C#:   Directory.GetCurrentDirectory()
来源：http://fkh.shanyushiyangkeji.top

[M05] 设置退出码
来源：http://imv.shanyushiyangkeji.top

Py:   sys.exit(1)
来源：http://qvd.kuanghao11.cn

PHP:  exit(1);
来源：http://hgq.hammf.cn

JS:   process.exit(1)
来源：http://qkp.epnwcf.com

TS:   process.exit(1)
来源：http://hpj.svipenyu.cn

Java: System.exit(1)
来源：http://vpl.tanke756.top

Go:   os.Exit(1)
来源：http://ptm.dianchejie.cn

Ruby: exit 1
来源：http://zsa.yj202588.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kdd.jyoumei.cn

[M06] 向标准错误输出
来源：http://pku.yueranfly.top

Py:   print("err", file=sys.stderr)
来源：http://wtr.jiagoushi.top

PHP:  fwrite(STDERR, "err\n");
来源：http://dpw.kuanghao11.cn

JS:   console.error("err")
来源：http://qgz.jianghu66.top

TS:   console.error("err")
来源：http://hhu.sysykeji.top

Java: System.err.println("err")
来源：http://ziu.cashguo.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cnf.sjlbkw.cn

Ruby: warn "err"
来源：http://kkf.aizwys.cn

C#:   Console.Error.WriteLine("err")
来源：http://kgb.pycfn.com

[M07] 判断是否为主入口
来源：http://qhl.ehwqpu.com

Py:   if __name__ == "__main__":
来源：http://oxm.yonumen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gtg.ivvv.top

JS:   require.main === module
来源：http://vqa.cqqwz.cn

TS:   require.main === module
来源：http://vfh.yuanzhike.top

Java: public static void main(String[] args)
来源：http://jna.zhoulong.xyz

Go:   func main()
来源：http://swh.0kj1m.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://exm.vqdsnc.cn

C#:   static void Main(string[] args)
来源：http://tbx.birdmap.top

[M08] 获取系统与运行时信息
来源：http://ozp.havefunace.top

Py:   platform.system();  platform.python_version()
来源：http://zcf.fzhhl.top

PHP:  PHP_OS;  phpversion();
来源：http://lqg.ivvv.top

JS:   process.platform;  process.version
来源：http://tbh.aizwys.cn

TS:   process.platform;  process.version
来源：http://uap.zdbjq.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wkc.aibaodan.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://feu.xylfe.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xen.fzhhl.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://btt.jqgufenzy.top

================================================================================
来源：http://gya.cashguo.top

N. 数据结构与算法
来源：http://ewm.jinghuilouyu.cn

================================================================================
来源：http://qyf.yj20258.top

[N01] 二分查找（有序数组）
来源：http://qzk.ydjk.org.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wmp.kuanghao11.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kjh.daxiang520.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lsn.yj20258.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gea.gzhubu.top

Java: Arrays.binarySearch(arr, x)
来源：http://ukg.fengsongda.top

Go:   sort.SearchInts(arr, x)
来源：http://fab.hongshengwenyu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vzi.tian-w.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wtw.ehwqpu.com

[N02] 排序（工程实践用内置实现）
来源：http://dat.fzhhl.top

Py:   sorted(arr);  arr.sort()
来源：http://oes.jlsjyb.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cjg.iojbl.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vmt.jlsjyb.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ryq.hysaishi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ezb.fengsongda.top

Go:   slices.Sort(arr)
来源：http://tjd.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://frf.daxiang520.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hke.sxryk.cn

[N03] 快速排序（分治示例）
来源：http://kii.jqgufenzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cox.chenzaomai.com

PHP:  // 递归实现，或用 usort
来源：http://uvk.tianlin.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vwe.yanxiufei.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nup.shuidangran.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wkg.shanyushiyangtech.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jlp.hnqzz.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ldb.xylfe.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dez.ydzc1.top

[N04] 斐波那契数列
来源：http://yix.pycfn.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ejx.hywenlv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ixc.xingfuxueyuan.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://djp.hywenlv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fsv.vehdjk.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jwi.shangyingyoupin.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bcz.jiagoushi.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fpn.fengsongda.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jnp.guannengcc.top

[N05] 最大公约数
来源：http://loz.316326.xyz

Py:   math.gcd(a, b)
来源：http://mci.cheryme.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mrf.jinyuanbaomall.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sxh.yuanzhike.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fnr.zhiwuduotai.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vrc.hywenlv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ofq.jinqigufen.top

Ruby: a.gcd(b)
来源：http://oxe.hongshengwenyu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fvp.cqqwz.cn

[N06] 判断回文字符串
来源：http://pmo.bbcook.cn

Py:   s == s[::-1]
来源：http://hfy.zhijiandao.cn

PHP:  $s === strrev($s);
来源：http://qes.jinghuilouyu.cn

JS:   s === [...s].reverse().join("")
来源：http://sbm.tian-w.cn

TS:   s === [...s].reverse().join("")
来源：http://sic.jyoumei.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tbd.jinqigufen.top

Go:   // 双指针从两端比较
来源：http://gss.sweek.top

Ruby: s == s.reverse
来源：http://ozw.yj20258.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://pal.shuidangran.top

[N07] 两数之和（返回下标）
来源：http://vng.quarkkingdee.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nzt.c1oappe.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qhk.jinghuilouyu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mpf.chenzaomai.com

TS:   // 手写 Map<string, number>
来源：http://ifj.vqdsnc.cn

Java: // 手写 HashMap
来源：http://oen.dashuyun.cn

Go:   // 手写 map[int]int
来源：http://uft.feifeiyinyue.top

Ruby: // 手写 Hash
来源：http://qod.0kj1m.cn

C#:   // 手写 Dictionary<int, int>
来源：http://btf.vehdjk.com

[N08] 生成全排列
来源：http://ntt.zhixingplan.top

Py:   itertools.permutations(arr)
来源：http://zqk.jianghu66.top

PHP:  // 手写递归交换
来源：http://hkp.xinyue.icu

JS:   // 手写回溯递归
来源：http://frr.vehdjk.com

TS:   // 手写回溯递归
来源：http://iua.vqdsnc.cn

Java: // 手写回溯递归
来源：http://bfh.xuanzx.com

Go:   // 手写回溯递归
来源：http://goq.yonumen.top

Ruby: arr.permutation.to_a
来源：http://jty.ydjk.org.cn

C#:   // 手写回溯递归
来源：http://wvw.yfazqb.com

[N09] 栈与队列
来源：http://nxn.jiagoushi.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://khb.vqdsnc.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://znw.hammf.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://etg.chenlongwang.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://swh.sxryk.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mls.yueranfly.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gkz.aibaodan.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xst.tian-w.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nmm.gogol.net.cn

[N10] 链表节点定义
来源：http://yju.tanke756.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dxe.zhijiandao.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://asy.0kj1m.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rlt.tian-w.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ude.shzxlz.cn

Java: class Node { int v; Node next; }
来源：http://egg.zdbjq.cn

Go:   type Node struct { V int; Next *Node }
来源：http://aoc.uphjek.com

Ruby: Node = Struct.new(:v, :next)
来源：http://znq.ivvv.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tbc.gaohongyu789.top

[N11] 二叉树中序遍历
来源：http://mki.yangfankeji.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qyy.ydzc1.top

PHP:  // 手写递归函数
来源：http://oae.ydjk.org.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nad.xziqi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rrz.xinyue.icu

Java: // 手写递归
来源：http://afo.bbcook.cn

Go:   // 手写递归
来源：http://gim.jiagoushi.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hgr.yanxiufei.cn

C#:   // 手写递归
来源：http://vhk.zdbjq.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vgp.hongshengwenyu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nrk.hesvh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gjq.sjlbkw.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vjq.guowangkeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zaj.yfazqb.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jni.ydjk.org.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sqe.gotoacloud.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yyf.chenlongwang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fvr.hesvh.cn

================================================================================
来源：http://vpl.dianchejie.cn

O. 并发与异步
来源：http://uyc.yanxiufei.cn

================================================================================
来源：http://vgk.fanxiaobao.xyz

[O01] 启动一个线程
来源：http://zal.bjfxy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://aax.hammf.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fnb.cqqwz.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fpt.xylfe.cn

TS:   // 同 JS
来源：http://rsz.feifeiyinyue.top

Java: new Thread(() -> f()).start()
来源：http://spd.svipenyu.cn

Go:   go f()
来源：http://dff.jiagoushi.top

Ruby: Thread.new { f }
来源：http://flc.feifeiyinyue.top

C#:   Task.Run(() => F());
来源：http://xxw.hcnkem.com

[O02] 使用线程池
来源：http://kuy.zhixingplan.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fug.gzhubu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iam.nwbrower.top

JS:   // worker_threads 线程池
来源：http://ujr.yj20258.top

TS:   // worker_threads 线程池
来源：http://rrd.ywan-chungtsiang.top

Java: Executors.newFixedThreadPool(4)
来源：http://xds.wangdashe.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hzv.kuanghao11.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ygq.ydzc1.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://twz.yj20258.top

[O03] 加锁保护共享数据
来源：http://dyr.gzhubu.top

Py:   with lock: shared += 1
来源：http://qhe.zhoulong.xyz

PHP:  // 用 flock() 做文件锁
来源：http://fma.xziqi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ysj.cucudq.cn

TS:   // 同 JS
来源：http://dkv.nanxinkj.top

Java: synchronized (this) { shared++; }
来源：http://pmp.zycfv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wik.yuanzhike.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://mke.redwolf501.top

C#:   lock (gate) { shared++; }
来源：http://fms.tian-w.cn

[O04] 定义异步函数并等待
来源：http://sug.uphjek.com

Py:   async def f():⏎    await g()
来源：http://ydj.cucudq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jkt.chenzaomai.com

JS:   async function f() { await g(); }
来源：http://zju.gotoacloud.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://xsq.gotoacloud.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nvp.nanxuanxn.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eaj.ywan-chungtsiang.top

Ruby: # 用 Fiber 或 async gem
来源：http://kaj.feifeiyinyue.top

C#:   async Task F() { await G(); }
来源：http://dgc.hammf.cn

[O05] 并发执行并等待全部完成
来源：http://bfs.fehbvm.com

Py:   asyncio.gather(*tasks)
来源：http://pck.havefunace.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lek.iojbl.cn

JS:   await Promise.all(tasks)
来源：http://twg.hammf.cn

TS:   await Promise.all(tasks)
来源：http://qib.hcnkem.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sbx.dashuyun.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gwz.cashguo.top

Ruby: threads.map(&:join)
来源：http://idy.shangyingyoupin.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lsm.xingfuxueyuan.xyz

[O06] 使用进程池
来源：http://esr.zhoulong.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lyt.hongshengwenyu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://dld.ppjwa.cn

JS:   // child_process / cluster 模块
来源：http://zlc.iojbl.cn

TS:   // child_process / cluster 模块
来源：http://nrb.yueranfly.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://djv.chenlongwang.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vad.epnwcf.com

Ruby: // fork 块
来源：http://rtx.birdmap.top

C#:   Parallel.For
来源：http://rpc.cucudq.cn

================================================================================
来源：http://wal.nwbrower.top

P. 常用工具函数
来源：http://gwf.shzxlz.cn

================================================================================
来源：http://ann.andypj.xyz


<!-- 参考信息 -->
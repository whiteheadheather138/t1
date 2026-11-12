代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zaf.yongpay.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hrr.hnxiangtu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qwm.jqgufenzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rzy.c1oappe.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xvi.ivvv.top

[L04] 设置超时
来源：http://gkz.yvedp.cn

Py:   requests.get(url, timeout=5)
来源：http://rpl.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oyk.hammf.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dgx.yuanzhike.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mbu.dianchejie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pgx.andypj.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qds.xylfe.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bzk.sjlbkw.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hzk.cucudq.cn

[L05] 上传文件（multipart）
来源：http://plg.daxiang520.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kbw.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lwp.hfpthk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kis.xziqi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bzq.yj20258.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://any.snrcjt.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vge.jinghuilouyu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zhz.yuanzhike.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nqx.birdmap.top

[L06] 解析响应为 JSON
来源：http://mvh.zhongyouzk.top

Py:   resp.json()
来源：http://iel.zhixingplan.top

PHP:  json_decode($body, true);
来源：http://hac.ybcxt.top

JS:   await resp.json()
来源：http://jrc.zhiwuduotai.top

TS:   await resp.json()
来源：http://xat.daria6918.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ama.zhixingplan.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yth.quarkkingdee.top

Ruby: JSON.parse(resp.body)
来源：http://lry.sweek.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://akf.gaohongyu789.top

[L07] 处理 HTTP 状态码
来源：http://dny.hcnkem.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cpz.mhx1999.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://scs.ivvv.top

JS:   resp.ok;  resp.status
来源：http://hud.snrcjt.cn

TS:   resp.ok;  resp.status
来源：http://xyt.yangfankeji.com

Java: resp.statusCode()
来源：http://umt.yueranfly.top

Go:   resp.StatusCode
来源：http://auh.jqgfzy.top

Ruby: resp.code.to_i
来源：http://wmn.jyoumei.cn

C#:   (int)resp.StatusCode
来源：http://hbb.ppjwa.cn

[L08] 并发请求多个地址
来源：http://hyq.hnxiangtu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hre.cashguo.top

PHP:  curl_multi_init() 系列
来源：http://dou.sjlbkw.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://puh.birdmap.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lda.sufxvd.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kho.chenzaomai.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://due.vehdjk.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yfa.zhijiandao.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fpk.dianchejie.cn

================================================================================
来源：http://lxu.zhijiandao.cn

M. 命令行 / 进程 / 环境
来源：http://xxv.nwbrower.top

================================================================================
来源：http://xyf.shangyingyoupin.top

[M01] 读取命令行参数
来源：http://tvf.fengsongda.top

Py:   sys.argv[1:]
来源：http://rxp.smart0.xyz

PHP:  $argv;  $argc;
来源：http://rmf.iojbl.cn

JS:   process.argv.slice(2)
来源：http://uwl.nanxinkj.top

TS:   process.argv.slice(2)
来源：http://ncm.hesvh.cn

Java: args 数组（main 方法参数）
来源：http://gxd.ehwqpu.com

Go:   os.Args[1:]
来源：http://vmc.aizwys.cn

Ruby: ARGV
来源：http://qla.tarul.cn

C#:   args 数组（Main 方法参数）
来源：http://naq.haohaochexian.top

[M02] 读取环境变量
来源：http://lfh.shangyingyoupin.top

Py:   os.environ.get("HOME")
来源：http://pfj.pengpengdd.cyou

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nyy.sxryk.cn

JS:   process.env.HOME
来源：http://ehs.yongpay.top

TS:   process.env.HOME
来源：http://clv.yuxming.cn

Java: System.getenv("HOME")
来源：http://ncx.andypj.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://die.hesvh.cn

Ruby: ENV["HOME"]
来源：http://mzk.hnxiangtu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pbm.zhaomingkeji.xyz

[M03] 执行外部命令
来源：http://kfi.chenlongwang.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hkx.daria6918.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qji.zhengqikj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://azt.316326.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://yer.sufxvd.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ukm.jyoumei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dja.tarul.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qev.zhongyouzk.top

C#:   Process.Start("ls", "-l");
来源：http://wlj.fktsv.cn

[M04] 获取当前工作目录
来源：http://jsa.xuanzx.com

Py:   os.getcwd()
来源：http://wfl.c1oappe.top

PHP:  getcwd();
来源：http://czd.birdmap.top

JS:   process.cwd()
来源：http://yht.bbcook.cn

TS:   process.cwd()
来源：http://lai.gaohongyu789.top

Java: Path.of("").toAbsolutePath()
来源：http://kcs.epnwcf.com

Go:   os.Getwd()
来源：http://jsb.iojbl.cn

Ruby: Dir.pwd
来源：http://xxv.zhixingplan.top

C#:   Directory.GetCurrentDirectory()
来源：http://glc.yonumen.top

[M05] 设置退出码
来源：http://ovr.quarkkingdee.top

Py:   sys.exit(1)
来源：http://ckc.daria6918.cn

PHP:  exit(1);
来源：http://vbw.yuxming.cn

JS:   process.exit(1)
来源：http://sxk.yfazqb.com

TS:   process.exit(1)
来源：http://wud.cashguo.top

Java: System.exit(1)
来源：http://eno.tanke756.top

Go:   os.Exit(1)
来源：http://ccd.jqgfzy.top

Ruby: exit 1
来源：http://upz.chenzaomai.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ytr.c1oappe.top

[M06] 向标准错误输出
来源：http://ira.yfazqb.com

Py:   print("err", file=sys.stderr)
来源：http://qiq.sjlbkw.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://uwc.aibaodan.cn

JS:   console.error("err")
来源：http://dee.ivvv.top

TS:   console.error("err")
来源：http://rxc.fzhhl.top

Java: System.err.println("err")
来源：http://wef.ydzc1.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ujg.zhengqikj.top

Ruby: warn "err"
来源：http://lvu.zdbjq.cn

C#:   Console.Error.WriteLine("err")
来源：http://iga.shanyushiyangtech.top

[M07] 判断是否为主入口
来源：http://ydi.fanxiaobao.xyz

Py:   if __name__ == "__main__":
来源：http://mwo.jqgfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ago.zycfv.cn

JS:   require.main === module
来源：http://pbg.chenjidiqi.icu

TS:   require.main === module
来源：http://kfi.tarul.cn

Java: public static void main(String[] args)
来源：http://nxl.sysykeji.top

Go:   func main()
来源：http://sxd.tanke756.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vbq.ehwqpu.com

C#:   static void Main(string[] args)
来源：http://ijs.hongshengwenyu.top

[M08] 获取系统与运行时信息
来源：http://akr.ivvv.top

Py:   platform.system();  platform.python_version()
来源：http://par.xinyue.icu

PHP:  PHP_OS;  phpversion();
来源：http://xvp.zhoulong.xyz

JS:   process.platform;  process.version
来源：http://uhi.zhiwuduotai.top

TS:   process.platform;  process.version
来源：http://vyx.gzhubu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://atk.yanxiufei.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kyy.xuetiantiany.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qwo.chenzaomai.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://nkb.jlsjyb.cn

================================================================================
来源：http://phg.wangdashe.top

N. 数据结构与算法
来源：http://bcq.guannengcc.top

================================================================================
来源：http://wcr.meibo888.top

[N01] 二分查找（有序数组）
来源：http://hom.ywan-chungtsiang.top

Py:   bisect.bisect_left(arr, x)
来源：http://mns.zhaomingkeji.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rqw.ydzc1.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fba.yuanzhike.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yzz.jinqigfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://lfu.jinghuilouyu.cn

Go:   sort.SearchInts(arr, x)
来源：http://xis.gzhubu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://wiq.dashuyun.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uuz.fanxiaobao.xyz

[N02] 排序（工程实践用内置实现）
来源：http://pjw.shanyushiyangtech.top

Py:   sorted(arr);  arr.sort()
来源：http://gso.shzxlz.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cne.shanyushiyangtech.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://rgr.fanxiaobao.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://swn.jyoumei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tgz.ydzc1.top

Go:   slices.Sort(arr)
来源：http://ret.redwolf501.top

Ruby: arr.sort
来源：http://ssb.ywan-chungtsiang.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://nbw.xingfuxueyuan.xyz

[N03] 快速排序（分治示例）
来源：http://koo.epnwcf.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lum.0kj1m.cn

PHP:  // 递归实现，或用 usort
来源：http://mmt.snrcjt.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kvq.hnqzz.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oyg.hammf.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://foy.gogol.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hha.xinyue.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pfy.chenjidiqi.icu

C#:   // 手写递归，或 Array.Sort
来源：http://lhi.gzhubu.top

[N04] 斐波那契数列
来源：http://cgg.hcnkem.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pwx.chenjidiqi.icu

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vyr.yangfankeji.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kes.zhaomingkeji.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oay.xuanzx.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wrv.52xcode.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ses.xuetiantiany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fsy.haohaochexian.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vsd.zhijiandao.cn

[N05] 最大公约数
来源：http://rsk.jinqigfzy.top

Py:   math.gcd(a, b)
来源：http://pcm.ppjwa.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mzk.xziqi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lrr.fzhhl.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://toh.yongpay.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vlf.52xcode.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rho.cucudq.cn

Ruby: a.gcd(b)
来源：http://gzj.xingfuxueyuan.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gvf.jinghuilouyu.cn

[N06] 判断回文字符串
来源：http://xwj.yonumen.top

Py:   s == s[::-1]
来源：http://nod.fzhhl.top

PHP:  $s === strrev($s);
来源：http://qbt.zhaomingkeji.xyz

JS:   s === [...s].reverse().join("")
来源：http://wxh.dashuyun.cn

TS:   s === [...s].reverse().join("")
来源：http://ltm.cucudq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://whe.zycfv.cn

Go:   // 双指针从两端比较
来源：http://ghg.fehbvm.com

Ruby: s == s.reverse
来源：http://gqs.jinqigufen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://opo.feifeiyinyue.top

[N07] 两数之和（返回下标）
来源：http://ezp.tian-w.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://okw.jqgufenzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://knh.tian-w.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wtn.hammf.cn

TS:   // 手写 Map<string, number>
来源：http://dmp.c1oappe.top

Java: // 手写 HashMap
来源：http://qmu.jinyuanbaomall.cn

Go:   // 手写 map[int]int
来源：http://bmi.snrcjt.cn

Ruby: // 手写 Hash
来源：http://byd.shzxlz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ttu.fktsv.cn

[N08] 生成全排列
来源：http://uut.ybcxt.top

Py:   itertools.permutations(arr)
来源：http://ntb.nanxinkj.top

PHP:  // 手写递归交换
来源：http://pax.hywenlv.cn

JS:   // 手写回溯递归
来源：http://xqu.aizwys.cn

TS:   // 手写回溯递归
来源：http://pco.feifeiyinyue.top

Java: // 手写回溯递归
来源：http://zeh.jqgfzy.top

Go:   // 手写回溯递归
来源：http://szt.hnqzz.top

Ruby: arr.permutation.to_a
来源：http://jke.yj20258.top

C#:   // 手写回溯递归
来源：http://umi.kuanghao11.cn

[N09] 栈与队列
来源：http://uvi.shuidangran.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zft.bjfxy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dmo.cqqwz.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://buc.yanxiufei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://icz.guannengcc.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cwu.xuanzx.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yrr.yfazqb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kny.52xcode.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://aaq.fanxiaobao.xyz

[N10] 链表节点定义
来源：http://thd.shzxlz.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yfn.shzxlz.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ari.yuanzhike.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gec.hnxiangtu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tsd.xuanzx.com

Java: class Node { int v; Node next; }
来源：http://uyg.sufxvd.cn

Go:   type Node struct { V int; Next *Node }
来源：http://sgd.yuxming.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pbh.jyoumei.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hry.guowangkeji.top

[N11] 二叉树中序遍历
来源：http://lgy.yvedp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sdh.daria6918.cn

PHP:  // 手写递归函数
来源：http://vam.jyoumei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://flr.epnwcf.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tfv.yuxming.cn

Java: // 手写递归
来源：http://msf.yueranfly.top

Go:   // 手写递归
来源：http://uma.jyoumei.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lvr.fehbvm.com

C#:   // 手写递归
来源：http://xsr.wangshuangyany.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cvi.sufxvd.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rkf.chenjidiqi.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jal.cashguo.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://con.fktsv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://txb.fehbvm.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qhm.wangshuangyany.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ppm.jinyuanbaomall.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xxl.meibo888.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://iat.nanxinkj.top

================================================================================
来源：http://pnc.jinyuanbaomall.cn

O. 并发与异步
来源：http://psq.wangshuangyany.cn

================================================================================
来源：http://vov.cashguo.top

[O01] 启动一个线程
来源：http://pkj.ywan-chungtsiang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pca.cashguo.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xei.shanyushiyangkeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://luu.snrcjt.cn

TS:   // 同 JS
来源：http://gen.yongpay.top

Java: new Thread(() -> f()).start()
来源：http://zrw.jiagoushi.top

Go:   go f()
来源：http://fdx.redwolf501.top

Ruby: Thread.new { f }
来源：http://jnv.chenzaomai.com

C#:   Task.Run(() => F());
来源：http://rmk.ctjpmb.com

[O02] 使用线程池
来源：http://zkv.pycfn.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vty.haohaochexian.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zij.jiagoushi.top

JS:   // worker_threads 线程池
来源：http://mgh.fehbvm.com

TS:   // worker_threads 线程池
来源：http://zhp.chenlongwang.top

Java: Executors.newFixedThreadPool(4)
来源：http://smu.shuidangran.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://deh.gogol.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yrd.zhengqikj.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mma.52xcode.cn

[O03] 加锁保护共享数据
来源：http://hbw.hywenlv.cn

Py:   with lock: shared += 1
来源：http://hsr.tianlin.xyz

PHP:  // 用 flock() 做文件锁
来源：http://bkt.tian-w.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yhb.mhx1999.top

TS:   // 同 JS
来源：http://jda.yj20258.top

Java: synchronized (this) { shared++; }
来源：http://xji.cqqwz.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ldg.zdbjq.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kjp.ywan-chungtsiang.top

C#:   lock (gate) { shared++; }
来源：http://fdd.sweek.top

[O04] 定义异步函数并等待
来源：http://pwd.c1oappe.top

Py:   async def f():⏎    await g()
来源：http://ybc.smart0.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://szy.c1oappe.top

JS:   async function f() { await g(); }
来源：http://imh.yuanzhike.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://yer.guowangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kzv.daxiang520.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cbl.jinghuilouyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cyg.zhaomingkeji.xyz

C#:   async Task F() { await G(); }
来源：http://xjt.zhengqikj.top

[O05] 并发执行并等待全部完成
来源：http://meb.zhiwuduotai.top

Py:   asyncio.gather(*tasks)
来源：http://sjv.aizwys.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bew.zdqjudy.top

JS:   await Promise.all(tasks)
来源：http://ugv.gotoacloud.top

TS:   await Promise.all(tasks)
来源：http://duf.guowangkeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wgc.hesvh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xwl.birdmap.top

Ruby: threads.map(&:join)
来源：http://ayc.zdqjudy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ugb.tarul.cn

[O06] 使用进程池
来源：http://uox.yonumen.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bus.cheryme.top

PHP:  // pcntl_fork 或多进程队列
来源：http://dzo.ehwqpu.com

JS:   // child_process / cluster 模块
来源：http://dyx.feifeiyinyue.top

TS:   // child_process / cluster 模块
来源：http://arw.yj202588.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://aqo.xuanzx.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lhw.hywenlv.cn

Ruby: // fork 块
来源：http://fga.zhijiandao.cn

C#:   Parallel.For
来源：http://vfi.hysaishi.cn

================================================================================
来源：http://thm.ctjpmb.com

P. 常用工具函数
来源：http://xhs.52xcode.cn

================================================================================
来源：http://gkv.pengpengdd.cyou

[P01] 生成 UUID
来源：http://xxf.ybcxt.top

Py:   str(uuid.uuid4())
来源：http://sqw.tarul.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xpt.cashguo.top

JS:   crypto.randomUUID()
来源：http://iaw.0kj1m.cn


<!-- 参考信息 -->
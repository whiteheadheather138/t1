代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qdd.bbcook.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pfz.cashguo.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iqz.zdqjudy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://htx.nwbrower.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uww.fanxiaobao.xyz

[L04] 设置超时
来源：http://gml.bbcook.cn

Py:   requests.get(url, timeout=5)
来源：http://dna.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cmw.shuidangran.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jto.hysaishi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://prv.guannengcc.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nzq.hcnkem.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://een.feifeiyinyue.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dnm.aibaodan.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yin.tarul.cn

[L05] 上传文件（multipart）
来源：http://yka.chenlongwang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cca.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nae.pycfn.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://aqz.svipenyu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hdt.wangshuangyany.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://aph.havefunace.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qbj.yj20258.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gzs.hysaishi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pzg.ivvv.top

[L06] 解析响应为 JSON
来源：http://rfq.c1oappe.top

Py:   resp.json()
来源：http://fzo.bbcook.cn

PHP:  json_decode($body, true);
来源：http://hbt.tianlin.xyz

JS:   await resp.json()
来源：http://acz.xingfuxueyuan.xyz

TS:   await resp.json()
来源：http://mpb.zhoulong.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rie.nanxinkj.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://txk.hongshengwenyu.top

Ruby: JSON.parse(resp.body)
来源：http://gsc.havefunace.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://skv.hesvh.cn

[L07] 处理 HTTP 状态码
来源：http://qtq.yonumen.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ama.ydjk.org.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://eeg.ctjpmb.com

JS:   resp.ok;  resp.status
来源：http://wvp.hnqzz.top

TS:   resp.ok;  resp.status
来源：http://rbp.gzhubu.top

Java: resp.statusCode()
来源：http://ydr.svipenyu.cn

Go:   resp.StatusCode
来源：http://qqv.yvedp.cn

Ruby: resp.code.to_i
来源：http://pxf.yj20258.top

C#:   (int)resp.StatusCode
来源：http://pqg.birdmap.top

[L08] 并发请求多个地址
来源：http://oyp.sjlbkw.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ter.yongpay.top

PHP:  curl_multi_init() 系列
来源：http://utk.zhongyouzk.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://izh.daxiang520.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ozs.fengsongda.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xao.gogol.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://evy.jinqigufen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fup.gotoacloud.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://klq.xuanzx.com

================================================================================
来源：http://zfx.hysaishi.cn

M. 命令行 / 进程 / 环境
来源：http://fmc.chenzaomai.com

================================================================================
来源：http://mnh.fktsv.cn

[M01] 读取命令行参数
来源：http://geh.jinqigufen.top

Py:   sys.argv[1:]
来源：http://iyh.fzhhl.top

PHP:  $argv;  $argc;
来源：http://wfb.zhaomingkeji.xyz

JS:   process.argv.slice(2)
来源：http://nvg.cashguo.top

TS:   process.argv.slice(2)
来源：http://qji.chenzaomai.com

Java: args 数组（main 方法参数）
来源：http://lje.feifeiyinyue.top

Go:   os.Args[1:]
来源：http://ueh.smart0.xyz

Ruby: ARGV
来源：http://eum.ydzc1.top

C#:   args 数组（Main 方法参数）
来源：http://cux.ybcxt.top

[M02] 读取环境变量
来源：http://chk.jinqigfzy.top

Py:   os.environ.get("HOME")
来源：http://bkh.yuxming.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ija.316326.xyz

JS:   process.env.HOME
来源：http://ift.yonumen.top

TS:   process.env.HOME
来源：http://vbg.xuetiantiany.cn

Java: System.getenv("HOME")
来源：http://mte.zhiwuduotai.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tmb.yfazqb.com

Ruby: ENV["HOME"]
来源：http://ptl.chenjidiqi.icu

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bvv.zhongyouzk.top

[M03] 执行外部命令
来源：http://sgb.redwolf501.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lns.daria6918.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lyj.quarkkingdee.top

JS:   child_process.execSync("ls -l").toString()
来源：http://lof.gzhubu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://erp.pengpengdd.cyou

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eku.fanxiaobao.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://nuv.epnwcf.com

Ruby: system("ls -l");  `ls -l`
来源：http://jyd.xingfuxueyuan.xyz

C#:   Process.Start("ls", "-l");
来源：http://ege.zhengqikj.top

[M04] 获取当前工作目录
来源：http://kua.zhoulong.xyz

Py:   os.getcwd()
来源：http://cun.jinqigufen.top

PHP:  getcwd();
来源：http://jfw.xinyue.icu

JS:   process.cwd()
来源：http://swt.shzxlz.cn

TS:   process.cwd()
来源：http://zkm.zhixingplan.top

Java: Path.of("").toAbsolutePath()
来源：http://fbd.bbcook.cn

Go:   os.Getwd()
来源：http://agm.bbcook.cn

Ruby: Dir.pwd
来源：http://ued.andypj.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://ace.yueranfly.top

[M05] 设置退出码
来源：http://tik.svipenyu.cn

Py:   sys.exit(1)
来源：http://xge.jyoumei.cn

PHP:  exit(1);
来源：http://zjt.pycfn.com

JS:   process.exit(1)
来源：http://jyj.ivvv.top

TS:   process.exit(1)
来源：http://jci.yonumen.top

Java: System.exit(1)
来源：http://uhp.aibaodan.cn

Go:   os.Exit(1)
来源：http://tpk.ydjk.org.cn

Ruby: exit 1
来源：http://qas.xuetiantiany.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sye.vehdjk.com

[M06] 向标准错误输出
来源：http://isv.hcnkem.com

Py:   print("err", file=sys.stderr)
来源：http://jwf.ydzc1.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qea.zdqjudy.top

JS:   console.error("err")
来源：http://qkr.0kj1m.cn

TS:   console.error("err")
来源：http://lvl.vqdsnc.cn

Java: System.err.println("err")
来源：http://xio.jinqigfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ocu.snrcjt.cn

Ruby: warn "err"
来源：http://rdd.jyoumei.cn

C#:   Console.Error.WriteLine("err")
来源：http://wzq.fanxiaobao.xyz

[M07] 判断是否为主入口
来源：http://zfs.iojbl.cn

Py:   if __name__ == "__main__":
来源：http://bud.wangdashe.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mjn.hfpthk.cn

JS:   require.main === module
来源：http://ufq.sufxvd.cn

TS:   require.main === module
来源：http://iwh.ehwqpu.com

Java: public static void main(String[] args)
来源：http://txo.fehbvm.com

Go:   func main()
来源：http://suf.nanxinkj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://aio.nanxinkj.top

C#:   static void Main(string[] args)
来源：http://dex.yonumen.top

[M08] 获取系统与运行时信息
来源：http://ffo.fengsongda.top

Py:   platform.system();  platform.python_version()
来源：http://iea.zhixingplan.top

PHP:  PHP_OS;  phpversion();
来源：http://cye.svipenyu.cn

JS:   process.platform;  process.version
来源：http://jbt.zdbjq.cn

TS:   process.platform;  process.version
来源：http://etz.shanyushiyangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xvl.zhiwuduotai.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rdj.havefunace.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pbq.jqgufenzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://srb.jqgfzy.top

================================================================================
来源：http://oro.kuanghao11.cn

N. 数据结构与算法
来源：http://prv.chenjidiqi.icu

================================================================================
来源：http://ldy.yj202588.top

[N01] 二分查找（有序数组）
来源：http://cgg.ydzc1.top

Py:   bisect.bisect_left(arr, x)
来源：http://tbt.tian-w.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://amv.sjlbkw.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fpw.xziqi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ljg.gotoacloud.top

Java: Arrays.binarySearch(arr, x)
来源：http://pdw.aibaodan.cn

Go:   sort.SearchInts(arr, x)
来源：http://btq.epnwcf.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://uci.cucudq.cn

C#:   Array.BinarySearch(arr, x)
来源：http://who.shuidangran.top

[N02] 排序（工程实践用内置实现）
来源：http://ccw.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://dxo.zhaomingkeji.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sfs.hywenlv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sgt.316326.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://tas.yuxming.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ori.hfpthk.cn

Go:   slices.Sort(arr)
来源：http://rjo.9152youxi.cn

Ruby: arr.sort
来源：http://ibq.tianlin.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://qvh.guowangkeji.top

[N03] 快速排序（分治示例）
来源：http://jab.jinyuanbaomall.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rzi.ydjk.org.cn

PHP:  // 递归实现，或用 usort
来源：http://ksh.yj202588.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://puk.smart0.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://abe.yj20258.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://aja.xuetiantiany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qoo.0kj1m.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://acy.yueranfly.top

C#:   // 手写递归，或 Array.Sort
来源：http://mbv.bjfxy.top

[N04] 斐波那契数列
来源：http://dmf.tianlin.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://eqv.jlsjyb.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zwz.ehwqpu.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lbd.zhixingplan.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kkc.tianlin.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://svb.ydjk.org.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tei.chenlongwang.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lhs.dianchejie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://aqb.snrcjt.cn

[N05] 最大公约数
来源：http://jxb.shanyushiyangkeji.top

Py:   math.gcd(a, b)
来源：http://ywf.gzhubu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ojc.fehbvm.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yyx.hnqzz.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fpb.jinghuilouyu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tcr.cqqwz.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hgq.ctjpmb.com

Ruby: a.gcd(b)
来源：http://iar.yuanzhike.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://grz.xylfe.cn

[N06] 判断回文字符串
来源：http://gre.xuanzx.com

Py:   s == s[::-1]
来源：http://csc.shanyushiyangkeji.top

PHP:  $s === strrev($s);
来源：http://orp.yvedp.cn

JS:   s === [...s].reverse().join("")
来源：http://zxw.sysykeji.top

TS:   s === [...s].reverse().join("")
来源：http://jxq.52xcode.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ktt.tianlin.xyz

Go:   // 双指针从两端比较
来源：http://ayx.zhijiandao.cn

Ruby: s == s.reverse
来源：http://zbf.zhengqikj.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zhh.hfpthk.cn

[N07] 两数之和（返回下标）
来源：http://rsd.smart0.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zyh.yuxming.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pbe.hnqzz.top

JS:   // 手写 Map：map.set(v, i)
来源：http://msj.dashuyun.cn

TS:   // 手写 Map<string, number>
来源：http://mtj.chenlongwang.top

Java: // 手写 HashMap
来源：http://qsv.meibo888.top

Go:   // 手写 map[int]int
来源：http://nmc.shanyushiyangkeji.top

Ruby: // 手写 Hash
来源：http://amf.vqdsnc.cn

C#:   // 手写 Dictionary<int, int>
来源：http://acu.nwbrower.top

[N08] 生成全排列
来源：http://bwi.jqgfzy.top

Py:   itertools.permutations(arr)
来源：http://bdq.dashuyun.cn

PHP:  // 手写递归交换
来源：http://cbf.nanxuanxn.top

JS:   // 手写回溯递归
来源：http://jfs.yj20258.top

TS:   // 手写回溯递归
来源：http://has.wangdashe.top

Java: // 手写回溯递归
来源：http://bfk.jinqigufen.top

Go:   // 手写回溯递归
来源：http://krg.ehwqpu.com

Ruby: arr.permutation.to_a
来源：http://pmc.cashguo.top

C#:   // 手写回溯递归
来源：http://rpk.0kj1m.cn

[N09] 栈与队列
来源：http://ilw.jiagoushi.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sxq.redwolf501.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zhv.0kj1m.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iar.shuidangran.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lzt.nanxuanxn.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hmk.pycfn.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://juk.c1oappe.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nqc.xuanzx.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jkh.ppjwa.cn

[N10] 链表节点定义
来源：http://lom.iojbl.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gug.yonumen.top

PHP:  class Node { public $v; public $next = null; }
来源：http://acc.zycfv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ddb.cdnleiting.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cwr.yfazqb.com

Java: class Node { int v; Node next; }
来源：http://tse.hnqzz.top

Go:   type Node struct { V int; Next *Node }
来源：http://ssv.shanyushiyangtech.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ops.fktsv.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pyz.aizwys.cn

[N11] 二叉树中序遍历
来源：http://nqw.jyoumei.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wyp.iojbl.cn

PHP:  // 手写递归函数
来源：http://afe.c1oappe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ygv.cdnleiting.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qmz.jinyuanbaomall.cn

Java: // 手写递归
来源：http://rbh.jqgfzy.top

Go:   // 手写递归
来源：http://wtx.dianchejie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oae.nanxuanxn.top

C#:   // 手写递归
来源：http://sov.0kj1m.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qop.haohaochexian.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vll.sysykeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://myl.zycfv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vwu.haohaochexian.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nxa.bjfxy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hwv.cqqwz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hph.fzhhl.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iuv.fengsongda.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://eyl.jinqigufen.top

================================================================================
来源：http://lqb.pycfn.com

O. 并发与异步
来源：http://dzr.pengpengdd.cyou

================================================================================
来源：http://gjg.vqdsnc.cn

[O01] 启动一个线程
来源：http://nyp.xinyue.icu

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tov.sjlbkw.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://prx.tarul.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://oki.xuetiantiany.cn

TS:   // 同 JS
来源：http://nrz.chenlongwang.top

Java: new Thread(() -> f()).start()
来源：http://del.sufxvd.cn

Go:   go f()
来源：http://thk.sjlbkw.cn

Ruby: Thread.new { f }
来源：http://cgf.andypj.xyz

C#:   Task.Run(() => F());
来源：http://jov.jinyuanbaomall.cn

[O02] 使用线程池
来源：http://zms.birdmap.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rzl.chenzaomai.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vss.aizwys.cn

JS:   // worker_threads 线程池
来源：http://wiu.vqdsnc.cn

TS:   // worker_threads 线程池
来源：http://aip.xziqi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jxs.zhengqikj.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cvh.xingfuxueyuan.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gfm.jyoumei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nay.jinghuilouyu.cn

[O03] 加锁保护共享数据
来源：http://aij.haohaochexian.top

Py:   with lock: shared += 1
来源：http://gyh.xziqi.cn

PHP:  // 用 flock() 做文件锁
来源：http://ule.sweek.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qxb.zhongyouzk.top

TS:   // 同 JS
来源：http://twg.hysaishi.cn

Java: synchronized (this) { shared++; }
来源：http://uyg.zhoulong.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uff.yanxiufei.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wjv.bbcook.cn

C#:   lock (gate) { shared++; }
来源：http://mzt.hysaishi.cn

[O04] 定义异步函数并等待
来源：http://chk.ydzc1.top

Py:   async def f():⏎    await g()
来源：http://zrv.jinqigfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mbq.fengsongda.top

JS:   async function f() { await g(); }
来源：http://xhj.bbcook.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://cuk.xuetiantiany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xlc.shzxlz.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vjt.shzxlz.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jyy.yongpay.top

C#:   async Task F() { await G(); }
来源：http://xvu.hesvh.cn

[O05] 并发执行并等待全部完成
来源：http://uis.ybcxt.top

Py:   asyncio.gather(*tasks)
来源：http://yho.chenlongwang.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nco.fengsongda.top

JS:   await Promise.all(tasks)
来源：http://jrx.hongshengwenyu.top

TS:   await Promise.all(tasks)
来源：http://tid.ehwqpu.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mve.epnwcf.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bqf.jlsjyb.cn

Ruby: threads.map(&:join)
来源：http://mno.hammf.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gpd.sysykeji.top

[O06] 使用进程池
来源：http://tel.nwbrower.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://azu.daria6918.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cdq.zhaomingkeji.xyz

JS:   // child_process / cluster 模块
来源：http://uhu.meibo888.top

TS:   // child_process / cluster 模块
来源：http://drs.wangdashe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://acf.pycfn.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ohd.uphjek.com

Ruby: // fork 块
来源：http://qjt.yueranfly.top

C#:   Parallel.For
来源：http://pgd.chenlongwang.top

================================================================================
来源：http://hzv.ybcxt.top

P. 常用工具函数
来源：http://zln.cucudq.cn

================================================================================
来源：http://tkt.tanke756.top

[P01] 生成 UUID
来源：http://qiw.hongshengwenyu.top

Py:   str(uuid.uuid4())
来源：http://rga.yonumen.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ozt.52xcode.cn

JS:   crypto.randomUUID()
来源：http://jbd.zhaomingkeji.xyz


<!-- 参考信息 -->
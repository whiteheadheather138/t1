代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oeo.fehbvm.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qcm.shangyingyoupin.top

[L05] 上传文件（multipart）
来源：http://dtc.gaohongyu789.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://osg.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dzm.zhengqikj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gah.9152youxi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xuf.jqgufenzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wor.hesvh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dzy.c1oappe.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fqg.meibo888.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jvt.xinyue.icu

[L06] 解析响应为 JSON
来源：http://myf.snrcjt.cn

Py:   resp.json()
来源：http://waz.jlsjyb.cn

PHP:  json_decode($body, true);
来源：http://ccu.52xcode.cn

JS:   await resp.json()
来源：http://yox.yuanzhike.top

TS:   await resp.json()
来源：http://loo.jinyuanbaomall.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iys.xingfuxueyuan.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vde.shanyushiyangtech.top

Ruby: JSON.parse(resp.body)
来源：http://igi.ppjwa.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://inh.xylfe.cn

[L07] 处理 HTTP 状态码
来源：http://izg.svipenyu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ufq.sysykeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://flj.tanke756.top

JS:   resp.ok;  resp.status
来源：http://prc.xziqi.cn

TS:   resp.ok;  resp.status
来源：http://qtv.ppjwa.cn

Java: resp.statusCode()
来源：http://ihj.yfazqb.com

Go:   resp.StatusCode
来源：http://kem.jqgufenzy.top

Ruby: resp.code.to_i
来源：http://jft.zhongyouzk.top

C#:   (int)resp.StatusCode
来源：http://kxg.mhx1999.top

[L08] 并发请求多个地址
来源：http://gos.bbcook.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jtr.cqqwz.cn

PHP:  curl_multi_init() 系列
来源：http://kvk.bbcook.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mie.zhoulong.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kag.sweek.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wvw.ctjpmb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qlu.pycfn.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://otj.zhongyouzk.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gdj.yuanzhike.top

================================================================================
来源：http://dvw.cqqwz.cn

M. 命令行 / 进程 / 环境
来源：http://zmk.ppjwa.cn

================================================================================
来源：http://bij.chenzaomai.com

[M01] 读取命令行参数
来源：http://rva.jlsjyb.cn

Py:   sys.argv[1:]
来源：http://wis.feifeiyinyue.top

PHP:  $argv;  $argc;
来源：http://eab.zhoulong.xyz

JS:   process.argv.slice(2)
来源：http://pvq.hnxiangtu.top

TS:   process.argv.slice(2)
来源：http://iig.cashguo.top

Java: args 数组（main 方法参数）
来源：http://nlv.jinghuilouyu.cn

Go:   os.Args[1:]
来源：http://jjk.sweek.top

Ruby: ARGV
来源：http://hjx.gzhubu.top

C#:   args 数组（Main 方法参数）
来源：http://fgg.chenzaomai.com

[M02] 读取环境变量
来源：http://bfk.yj20258888.top

Py:   os.environ.get("HOME")
来源：http://vxv.yangfankeji.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://usr.hammf.cn

JS:   process.env.HOME
来源：http://xso.shanyushiyangtech.top

TS:   process.env.HOME
来源：http://aoo.fengsongda.top

Java: System.getenv("HOME")
来源：http://tev.zhoulong.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dos.xuanzx.com

Ruby: ENV["HOME"]
来源：http://jtg.dashuyun.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jtb.xingfuxueyuan.xyz

[M03] 执行外部命令
来源：http://bwj.yj20258.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sep.hammf.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://und.yuanzhike.top

JS:   child_process.execSync("ls -l").toString()
来源：http://nsb.yvedp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qmy.shanyushiyangkeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bae.yj202588.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ygu.ctjpmb.com

Ruby: system("ls -l");  `ls -l`
来源：http://uai.zdqjudy.top

C#:   Process.Start("ls", "-l");
来源：http://hvh.316326.xyz

[M04] 获取当前工作目录
来源：http://jpl.redwolf501.top

Py:   os.getcwd()
来源：http://bck.daxiang520.top

PHP:  getcwd();
来源：http://prm.chenlongwang.top

JS:   process.cwd()
来源：http://fii.yj20258.top

TS:   process.cwd()
来源：http://zbc.cqqwz.cn

Java: Path.of("").toAbsolutePath()
来源：http://ejy.yuanzhike.top

Go:   os.Getwd()
来源：http://keg.aizwys.cn

Ruby: Dir.pwd
来源：http://tml.yangfankeji.com

C#:   Directory.GetCurrentDirectory()
来源：http://wfo.fehbvm.com

[M05] 设置退出码
来源：http://mxr.zhijiandao.cn

Py:   sys.exit(1)
来源：http://cnm.zhaomingkeji.xyz

PHP:  exit(1);
来源：http://crg.yanxiufei.cn

JS:   process.exit(1)
来源：http://ywz.nwbrower.top

TS:   process.exit(1)
来源：http://zbh.dashuyun.cn

Java: System.exit(1)
来源：http://xta.yonumen.top

Go:   os.Exit(1)
来源：http://xut.zhoulong.xyz

Ruby: exit 1
来源：http://qne.daxiang520.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nox.fzhhl.top

[M06] 向标准错误输出
来源：http://qus.cashguo.top

Py:   print("err", file=sys.stderr)
来源：http://iiu.chenzaomai.com

PHP:  fwrite(STDERR, "err\n");
来源：http://wlk.ivvv.top

JS:   console.error("err")
来源：http://myv.0kj1m.cn

TS:   console.error("err")
来源：http://aap.tianlin.xyz

Java: System.err.println("err")
来源：http://kdr.xuanzx.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lft.yuxming.cn

Ruby: warn "err"
来源：http://sig.316326.xyz

C#:   Console.Error.WriteLine("err")
来源：http://tbt.jiagoushi.top

[M07] 判断是否为主入口
来源：http://fjj.daxiang520.top

Py:   if __name__ == "__main__":
来源：http://bsi.hongshengwenyu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sin.hesvh.cn

JS:   require.main === module
来源：http://kea.jianghu66.top

TS:   require.main === module
来源：http://nft.xingfuxueyuan.xyz

Java: public static void main(String[] args)
来源：http://myn.guannengcc.top

Go:   func main()
来源：http://dvx.vqdsnc.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xyv.cucudq.cn

C#:   static void Main(string[] args)
来源：http://loz.ydzc1.top

[M08] 获取系统与运行时信息
来源：http://mpd.quarkkingdee.top

Py:   platform.system();  platform.python_version()
来源：http://eql.aibaodan.cn

PHP:  PHP_OS;  phpversion();
来源：http://que.smart0.xyz

JS:   process.platform;  process.version
来源：http://tkk.hcnkem.com

TS:   process.platform;  process.version
来源：http://cmy.zhiwuduotai.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://amu.chenlongwang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://vug.yangfankeji.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fqb.pycfn.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://swu.shuidangran.top

================================================================================
来源：http://jjy.zhoulong.xyz

N. 数据结构与算法
来源：http://klg.52xcode.cn

================================================================================
来源：http://ozz.jqgufenzy.top

[N01] 二分查找（有序数组）
来源：http://eph.jqgufenzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://cdn.yangfankeji.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://evj.zhoulong.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lvo.dashuyun.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://myt.smart0.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://vzu.tanke756.top

Go:   sort.SearchInts(arr, x)
来源：http://buj.hfpthk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wyz.ehwqpu.com

C#:   Array.BinarySearch(arr, x)
来源：http://caf.snrcjt.cn

[N02] 排序（工程实践用内置实现）
来源：http://jym.jianghu66.top

Py:   sorted(arr);  arr.sort()
来源：http://cpf.shzxlz.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rtx.dianchejie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jel.yonumen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://aml.zhixingplan.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dka.zycfv.cn

Go:   slices.Sort(arr)
来源：http://auq.sjlbkw.cn

Ruby: arr.sort
来源：http://fas.zhijiandao.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://awz.kuanghao11.cn

[N03] 快速排序（分治示例）
来源：http://hsr.chenlongwang.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lon.zhiwuduotai.top

PHP:  // 递归实现，或用 usort
来源：http://ocv.yuxming.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lur.pycfn.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ubw.hcnkem.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xtv.gaohongyu789.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jst.yj20258.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zyf.yanxiufei.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ubq.uphjek.com

[N04] 斐波那契数列
来源：http://mss.pycfn.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rvt.hywenlv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hls.yuxming.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://arp.daxiang520.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fdn.yj20258.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://otx.fehbvm.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ndi.c1oappe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fuz.vqdsnc.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dmv.gogol.net.cn

[N05] 最大公约数
来源：http://vyn.ywan-chungtsiang.top

Py:   math.gcd(a, b)
来源：http://qbl.yuanzhike.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ynx.52xcode.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://irg.316326.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ywy.hysaishi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://emd.guannengcc.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qww.xuetiantiany.cn

Ruby: a.gcd(b)
来源：http://vzv.jinqigfzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pga.chenlongwang.top

[N06] 判断回文字符串
来源：http://zrl.bbcook.cn

Py:   s == s[::-1]
来源：http://eso.xuetiantiany.cn

PHP:  $s === strrev($s);
来源：http://lqj.ivvv.top

JS:   s === [...s].reverse().join("")
来源：http://gst.xylfe.cn

TS:   s === [...s].reverse().join("")
来源：http://pqs.zdbjq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xgy.zhoulong.xyz

Go:   // 双指针从两端比较
来源：http://xxc.shangyingyoupin.top

Ruby: s == s.reverse
来源：http://vgn.gotoacloud.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://uso.ydjk.org.cn

[N07] 两数之和（返回下标）
来源：http://oca.chenzaomai.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nvr.redwolf501.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ubx.zhijiandao.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ffl.cheryme.top

TS:   // 手写 Map<string, number>
来源：http://apb.bjfxy.top

Java: // 手写 HashMap
来源：http://bxo.hnxiangtu.top

Go:   // 手写 map[int]int
来源：http://iku.52xcode.cn

Ruby: // 手写 Hash
来源：http://emm.jiagoushi.top

C#:   // 手写 Dictionary<int, int>
来源：http://vsr.zdbjq.cn

[N08] 生成全排列
来源：http://fqq.epnwcf.com

Py:   itertools.permutations(arr)
来源：http://ocs.iojbl.cn

PHP:  // 手写递归交换
来源：http://knk.haohaochexian.top

JS:   // 手写回溯递归
来源：http://gvo.aizwys.cn

TS:   // 手写回溯递归
来源：http://bqj.hfpthk.cn

Java: // 手写回溯递归
来源：http://rnn.mhx1999.top

Go:   // 手写回溯递归
来源：http://cxf.yj20258888.top

Ruby: arr.permutation.to_a
来源：http://dth.daria6918.cn

C#:   // 手写回溯递归
来源：http://jud.hfpthk.cn

[N09] 栈与队列
来源：http://psp.shanyushiyangkeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rhi.bbcook.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kjx.jiagoushi.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://heh.gaohongyu789.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kae.yongpay.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zyb.jqgufenzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://job.yuxming.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pxn.xingfuxueyuan.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nak.jlsjyb.cn

[N10] 链表节点定义
来源：http://hyd.shangyingyoupin.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://var.yanxiufei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gdt.gogol.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cnc.uphjek.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pnc.feifeiyinyue.top

Java: class Node { int v; Node next; }
来源：http://moa.zhiwuduotai.top

Go:   type Node struct { V int; Next *Node }
来源：http://dgs.ybcxt.top

Ruby: Node = Struct.new(:v, :next)
来源：http://piy.yanxiufei.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nch.hnqzz.top

[N11] 二叉树中序遍历
来源：http://evh.fzhhl.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wns.hammf.cn

PHP:  // 手写递归函数
来源：http://lqa.chenzaomai.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iwt.guannengcc.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://loh.bbcook.cn

Java: // 手写递归
来源：http://gkk.snrcjt.cn

Go:   // 手写递归
来源：http://reh.shzxlz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jfn.shuidangran.top

C#:   // 手写递归
来源：http://xnc.nanxinkj.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://unx.feifeiyinyue.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://epa.feifeiyinyue.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ldt.fktsv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rtx.shzxlz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kfw.svipenyu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gnn.52xcode.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cot.jinyuanbaomall.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hfr.shangyingyoupin.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nin.daria6918.cn

================================================================================
来源：http://rrf.yuanzhike.top

O. 并发与异步
来源：http://grs.mhx1999.top

================================================================================
来源：http://mby.feifeiyinyue.top

[O01] 启动一个线程
来源：http://csw.sweek.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uiv.daxiang520.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bwc.cheryme.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gxf.meibo888.top

TS:   // 同 JS
来源：http://bxr.xylfe.cn

Java: new Thread(() -> f()).start()
来源：http://mun.gzhubu.top

Go:   go f()
来源：http://cof.zhaomingkeji.xyz

Ruby: Thread.new { f }
来源：http://pdu.cdnleiting.top

C#:   Task.Run(() => F());
来源：http://wjp.zycfv.cn

[O02] 使用线程池
来源：http://smy.zhiwuduotai.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xse.jianghu66.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ywf.haohaochexian.top

JS:   // worker_threads 线程池
来源：http://isd.yuanzhike.top

TS:   // worker_threads 线程池
来源：http://nyk.bbcook.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tdo.tanke756.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gpf.hnqzz.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jpg.jqgfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hwq.yuxming.cn

[O03] 加锁保护共享数据
来源：http://xew.meibo888.top

Py:   with lock: shared += 1
来源：http://ayg.jinyuanbaomall.cn

PHP:  // 用 flock() 做文件锁
来源：http://vxu.fzhhl.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gmx.hnqzz.top

TS:   // 同 JS
来源：http://gll.tianlin.xyz

Java: synchronized (this) { shared++; }
来源：http://wre.xuanzx.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://brh.cucudq.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://euv.shzxlz.cn

C#:   lock (gate) { shared++; }
来源：http://yww.ppjwa.cn

[O04] 定义异步函数并等待
来源：http://mnt.nwbrower.top

Py:   async def f():⏎    await g()
来源：http://gvf.yuanzhike.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dmr.c1oappe.top

JS:   async function f() { await g(); }
来源：http://fak.nanxinkj.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rxc.cqqwz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://euj.zhoulong.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yip.zycfv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://vsi.shanyushiyangtech.top

C#:   async Task F() { await G(); }
来源：http://gbp.c1oappe.top

[O05] 并发执行并等待全部完成
来源：http://smk.ydjk.org.cn

Py:   asyncio.gather(*tasks)
来源：http://vhc.gzhubu.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eii.yonumen.top

JS:   await Promise.all(tasks)
来源：http://vkn.jinqigfzy.top

TS:   await Promise.all(tasks)
来源：http://zne.cheryme.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sbf.ywan-chungtsiang.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sgn.pycfn.com

Ruby: threads.map(&:join)
来源：http://uij.ydjk.org.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zlx.fzhhl.top

[O06] 使用进程池
来源：http://pxc.nwbrower.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fsj.316326.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://fzf.wangshuangyany.cn

JS:   // child_process / cluster 模块
来源：http://ieu.zdqjudy.top

TS:   // child_process / cluster 模块
来源：http://axw.zhiwuduotai.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zvl.fanxiaobao.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lsy.hongshengwenyu.top

Ruby: // fork 块
来源：http://wkw.yangfankeji.com

C#:   Parallel.For
来源：http://tsq.yangfankeji.com

================================================================================
来源：http://hej.gotoacloud.top

P. 常用工具函数
来源：http://biw.bbcook.cn

================================================================================
来源：http://zgo.zhijiandao.cn

[P01] 生成 UUID
来源：http://ugb.snrcjt.cn

Py:   str(uuid.uuid4())
来源：http://yof.sufxvd.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cec.chenjidiqi.icu

JS:   crypto.randomUUID()
来源：http://tqu.tian-w.cn

TS:   crypto.randomUUID()
来源：http://dvd.guannengcc.top

Java: UUID.randomUUID().toString()
来源：http://pkg.jinghuilouyu.cn

Go:   // 用 github.com/google/uuid
来源：http://llc.hcnkem.com

Ruby: SecureRandom.uuid
来源：http://nlz.jyoumei.cn

C#:   Guid.NewGuid().ToString()
来源：http://uej.yueranfly.top

[P02] MD5 / SHA256 摘要
来源：http://zxi.pycfn.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uao.xziqi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://cap.gogol.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://skv.tian-w.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jdg.birdmap.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gfk.ybcxt.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blt.gotoacloud.top


<!-- 参考信息 -->
代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qux.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lwj.c1oappe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://caj.yuxming.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xvd.gotoacloud.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bws.yueranfly.top

[L04] 设置超时
来源：http://jdn.ydjk.org.cn

Py:   requests.get(url, timeout=5)
来源：http://igw.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cru.sweek.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mqm.9152youxi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qul.daxiang520.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://oiq.daria6918.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://csn.chenlongwang.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vyx.hesvh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ljk.shanyushiyangtech.top

[L05] 上传文件（multipart）
来源：http://ose.jqgufenzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zaw.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hpm.shanyushiyangtech.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://iry.yueranfly.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nsd.xingfuxueyuan.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://irk.jlsjyb.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://urv.jinyuanbaomall.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fpj.jinyuanbaomall.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eey.yueranfly.top

[L06] 解析响应为 JSON
来源：http://rzq.aizwys.cn

Py:   resp.json()
来源：http://qmk.wangdashe.top

PHP:  json_decode($body, true);
来源：http://klz.jinghuilouyu.cn

JS:   await resp.json()
来源：http://fqe.hongshengwenyu.top

TS:   await resp.json()
来源：http://ypr.hongshengwenyu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ogs.fengsongda.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nqs.jiagoushi.top

Ruby: JSON.parse(resp.body)
来源：http://ojp.yj20258.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://usy.ctjpmb.com

[L07] 处理 HTTP 状态码
来源：http://bka.feifeiyinyue.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jua.sweek.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qsl.zycfv.cn

JS:   resp.ok;  resp.status
来源：http://ndk.birdmap.top

TS:   resp.ok;  resp.status
来源：http://xcj.pycfn.com

Java: resp.statusCode()
来源：http://tto.sxryk.cn

Go:   resp.StatusCode
来源：http://hxs.xuetiantiany.cn

Ruby: resp.code.to_i
来源：http://zvf.bbcook.cn

C#:   (int)resp.StatusCode
来源：http://dyq.fzhhl.top

[L08] 并发请求多个地址
来源：http://ins.chenjidiqi.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lwd.feifeiyinyue.top

PHP:  curl_multi_init() 系列
来源：http://mcu.yfazqb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yaz.yfazqb.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fqa.tian-w.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cjg.haohaochexian.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sph.hcnkem.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kmo.shanyushiyangkeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nbw.jinqigfzy.top

================================================================================
来源：http://ccu.shanyushiyangkeji.top

M. 命令行 / 进程 / 环境
来源：http://epu.shzxlz.cn

================================================================================
来源：http://kob.yonumen.top

[M01] 读取命令行参数
来源：http://vgk.tian-w.cn

Py:   sys.argv[1:]
来源：http://yqu.xziqi.cn

PHP:  $argv;  $argc;
来源：http://nye.zhiwuduotai.top

JS:   process.argv.slice(2)
来源：http://tin.zhixingplan.top

TS:   process.argv.slice(2)
来源：http://jek.ivvv.top

Java: args 数组（main 方法参数）
来源：http://ecn.vehdjk.com

Go:   os.Args[1:]
来源：http://vap.zhoulong.xyz

Ruby: ARGV
来源：http://ucl.zhiwuduotai.top

C#:   args 数组（Main 方法参数）
来源：http://hen.cucudq.cn

[M02] 读取环境变量
来源：http://yqj.yvedp.cn

Py:   os.environ.get("HOME")
来源：http://iwd.fzhhl.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://awl.guannengcc.top

JS:   process.env.HOME
来源：http://gtl.fanxiaobao.xyz

TS:   process.env.HOME
来源：http://lql.zdqjudy.top

Java: System.getenv("HOME")
来源：http://tte.bbcook.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sqs.yj20258.top

Ruby: ENV["HOME"]
来源：http://zpy.9152youxi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uuv.tanke756.top

[M03] 执行外部命令
来源：http://fel.xuanzx.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vva.guannengcc.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fss.jqgfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://sbp.dashuyun.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ztx.yanxiufei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nlz.meibo888.top

Go:   exec.Command("ls", "-l").Output()
来源：http://dco.9152youxi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ett.hnqzz.top

C#:   Process.Start("ls", "-l");
来源：http://pww.yanxiufei.cn

[M04] 获取当前工作目录
来源：http://mql.yangfankeji.com

Py:   os.getcwd()
来源：http://vtm.zhixingplan.top

PHP:  getcwd();
来源：http://ykh.zdqjudy.top

JS:   process.cwd()
来源：http://pwg.0kj1m.cn

TS:   process.cwd()
来源：http://qyv.tarul.cn

Java: Path.of("").toAbsolutePath()
来源：http://bpw.yvedp.cn

Go:   os.Getwd()
来源：http://ucv.zhoulong.xyz

Ruby: Dir.pwd
来源：http://lyj.fehbvm.com

C#:   Directory.GetCurrentDirectory()
来源：http://xxk.vehdjk.com

[M05] 设置退出码
来源：http://cqm.sweek.top

Py:   sys.exit(1)
来源：http://qcy.yuxming.cn

PHP:  exit(1);
来源：http://xoy.yueranfly.top

JS:   process.exit(1)
来源：http://ghl.ehwqpu.com

TS:   process.exit(1)
来源：http://zmf.tian-w.cn

Java: System.exit(1)
来源：http://osi.xziqi.cn

Go:   os.Exit(1)
来源：http://bdp.yj20258888.top

Ruby: exit 1
来源：http://pdf.sufxvd.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yym.dianchejie.cn

[M06] 向标准错误输出
来源：http://iut.aizwys.cn

Py:   print("err", file=sys.stderr)
来源：http://zgf.ctjpmb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://cqa.yanxiufei.cn

JS:   console.error("err")
来源：http://jhj.yanxiufei.cn

TS:   console.error("err")
来源：http://eao.jyoumei.cn

Java: System.err.println("err")
来源：http://ddm.pycfn.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://roi.shangyingyoupin.top

Ruby: warn "err"
来源：http://yrq.gaohongyu789.top

C#:   Console.Error.WriteLine("err")
来源：http://qkd.hysaishi.cn

[M07] 判断是否为主入口
来源：http://hoi.birdmap.top

Py:   if __name__ == "__main__":
来源：http://wgk.quarkkingdee.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ube.hammf.cn

JS:   require.main === module
来源：http://kqf.tian-w.cn

TS:   require.main === module
来源：http://yly.tian-w.cn

Java: public static void main(String[] args)
来源：http://llu.sxryk.cn

Go:   func main()
来源：http://zig.havefunace.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bkc.vehdjk.com

C#:   static void Main(string[] args)
来源：http://ddo.9152youxi.cn

[M08] 获取系统与运行时信息
来源：http://lcr.dianchejie.cn

Py:   platform.system();  platform.python_version()
来源：http://qoz.xuetiantiany.cn

PHP:  PHP_OS;  phpversion();
来源：http://lvs.kuanghao11.cn

JS:   process.platform;  process.version
来源：http://wqj.aibaodan.cn

TS:   process.platform;  process.version
来源：http://enu.hesvh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ppb.zhiwuduotai.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zbt.xziqi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://niv.epnwcf.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://lga.xylfe.cn

================================================================================
来源：http://lla.yfazqb.com

N. 数据结构与算法
来源：http://iho.sweek.top

================================================================================
来源：http://gkn.ywan-chungtsiang.top

[N01] 二分查找（有序数组）
来源：http://voh.cheryme.top

Py:   bisect.bisect_left(arr, x)
来源：http://mpy.tanke756.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ymv.haohaochexian.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fap.hywenlv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uyn.jinyuanbaomall.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jjt.yj20258888.top

Go:   sort.SearchInts(arr, x)
来源：http://uoa.sysykeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qvz.xinyue.icu

C#:   Array.BinarySearch(arr, x)
来源：http://fyg.shanyushiyangtech.top

[N02] 排序（工程实践用内置实现）
来源：http://xxd.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://uoi.aibaodan.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://von.zhixingplan.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://zoa.chenlongwang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://iob.yueranfly.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wvm.jqgfzy.top

Go:   slices.Sort(arr)
来源：http://pgj.yonumen.top

Ruby: arr.sort
来源：http://vws.epnwcf.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://uto.fzhhl.top

[N03] 快速排序（分治示例）
来源：http://aun.ehwqpu.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zzi.quarkkingdee.top

PHP:  // 递归实现，或用 usort
来源：http://omc.jinghuilouyu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ayh.hysaishi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rfi.pycfn.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qhx.tanke756.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xlh.sweek.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ztd.yvedp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jtg.jqgufenzy.top

[N04] 斐波那契数列
来源：http://dae.xuetiantiany.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wue.dianchejie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wzt.gogol.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fqx.zdqjudy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ydx.xuanzx.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mhy.tanke756.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tdt.epnwcf.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bgj.vqdsnc.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cab.fanxiaobao.xyz

[N05] 最大公约数
来源：http://rrv.xylfe.cn

Py:   math.gcd(a, b)
来源：http://tio.yj202588.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vjb.zhoulong.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jcq.xylfe.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ahd.hnqzz.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qip.zhixingplan.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://riq.xziqi.cn

Ruby: a.gcd(b)
来源：http://stl.hnqzz.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hyk.fehbvm.com

[N06] 判断回文字符串
来源：http://czn.yj20258888.top

Py:   s == s[::-1]
来源：http://vqo.c1oappe.top

PHP:  $s === strrev($s);
来源：http://iwu.c1oappe.top

JS:   s === [...s].reverse().join("")
来源：http://nnh.ppjwa.cn

TS:   s === [...s].reverse().join("")
来源：http://mpc.havefunace.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://smd.nanxuanxn.top

Go:   // 双指针从两端比较
来源：http://njk.redwolf501.top

Ruby: s == s.reverse
来源：http://dwt.yj20258888.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://fla.jyoumei.cn

[N07] 两数之和（返回下标）
来源：http://yfv.dashuyun.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hqn.shanyushiyangtech.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ouy.sjlbkw.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ssf.daria6918.cn

TS:   // 手写 Map<string, number>
来源：http://wfc.wangshuangyany.cn

Java: // 手写 HashMap
来源：http://vld.gotoacloud.top

Go:   // 手写 map[int]int
来源：http://qqk.smart0.xyz

Ruby: // 手写 Hash
来源：http://izo.hcnkem.com

C#:   // 手写 Dictionary<int, int>
来源：http://tpl.dashuyun.cn

[N08] 生成全排列
来源：http://mwn.cucudq.cn

Py:   itertools.permutations(arr)
来源：http://zpd.xingfuxueyuan.xyz

PHP:  // 手写递归交换
来源：http://uil.meibo888.top

JS:   // 手写回溯递归
来源：http://zdg.dashuyun.cn

TS:   // 手写回溯递归
来源：http://cjy.jinqigfzy.top

Java: // 手写回溯递归
来源：http://scf.jqgfzy.top

Go:   // 手写回溯递归
来源：http://qoz.zycfv.cn

Ruby: arr.permutation.to_a
来源：http://qqh.zhijiandao.cn

C#:   // 手写回溯递归
来源：http://obn.cdnleiting.top

[N09] 栈与队列
来源：http://oeg.jinyuanbaomall.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qyw.nanxuanxn.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nxd.ydzc1.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vzc.ivvv.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vwh.jinyuanbaomall.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bmc.shangyingyoupin.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rct.ydzc1.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pbe.cheryme.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gqi.ivvv.top

[N10] 链表节点定义
来源：http://vqn.chenjidiqi.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zor.ywan-chungtsiang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ndd.hfpthk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ceu.tarul.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fbr.havefunace.top

Java: class Node { int v; Node next; }
来源：http://iuw.gotoacloud.top

Go:   type Node struct { V int; Next *Node }
来源：http://qfc.zdbjq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zrr.daria6918.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://glt.hysaishi.cn

[N11] 二叉树中序遍历
来源：http://fwc.gogol.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nzk.jiagoushi.top

PHP:  // 手写递归函数
来源：http://mkl.nwbrower.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dfu.yuanzhike.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jfp.sjlbkw.cn

Java: // 手写递归
来源：http://bkn.dianchejie.cn

Go:   // 手写递归
来源：http://kse.yj20258888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xzl.xuetiantiany.cn

C#:   // 手写递归
来源：http://yek.vqdsnc.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pro.havefunace.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lac.zhengqikj.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xzo.tanke756.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lea.ywan-chungtsiang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://shs.feifeiyinyue.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tfl.iojbl.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qqa.yongpay.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uai.fengsongda.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qsa.quarkkingdee.top

================================================================================
来源：http://bni.jqgfzy.top

O. 并发与异步
来源：http://rgi.jqgfzy.top

================================================================================
来源：http://eqy.yj202588.top

[O01] 启动一个线程
来源：http://wym.fzhhl.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oou.jqgfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://onr.chenlongwang.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://egk.cashguo.top

TS:   // 同 JS
来源：http://peq.sysykeji.top

Java: new Thread(() -> f()).start()
来源：http://pam.haohaochexian.top

Go:   go f()
来源：http://vlq.cheryme.top

Ruby: Thread.new { f }
来源：http://tqf.daria6918.cn

C#:   Task.Run(() => F());
来源：http://qhh.cdnleiting.top

[O02] 使用线程池
来源：http://peu.tanke756.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eqk.jinqigufen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yod.tianlin.xyz

JS:   // worker_threads 线程池
来源：http://ajz.jlsjyb.cn

TS:   // worker_threads 线程池
来源：http://rhx.smart0.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://yaj.hysaishi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://djc.52xcode.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ztu.fktsv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ngp.ehwqpu.com

[O03] 加锁保护共享数据
来源：http://jwf.zhoulong.xyz

Py:   with lock: shared += 1
来源：http://olb.wangshuangyany.cn

PHP:  // 用 flock() 做文件锁
来源：http://xgj.zhixingplan.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mfo.jinyuanbaomall.cn

TS:   // 同 JS
来源：http://mbi.yj202588.top

Java: synchronized (this) { shared++; }
来源：http://bvl.andypj.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lza.vqdsnc.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dld.gogol.net.cn

C#:   lock (gate) { shared++; }
来源：http://ehr.pengpengdd.cyou

[O04] 定义异步函数并等待
来源：http://vez.cqqwz.cn

Py:   async def f():⏎    await g()
来源：http://esl.52xcode.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nmp.vehdjk.com

JS:   async function f() { await g(); }
来源：http://rch.52xcode.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bfe.zhijiandao.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://odr.ybcxt.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://btj.9152youxi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ocg.daxiang520.top

C#:   async Task F() { await G(); }
来源：http://kjo.gotoacloud.top

[O05] 并发执行并等待全部完成
来源：http://ouk.hammf.cn

Py:   asyncio.gather(*tasks)
来源：http://qrt.xuetiantiany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wjq.zhijiandao.cn

JS:   await Promise.all(tasks)
来源：http://xja.jinghuilouyu.cn

TS:   await Promise.all(tasks)
来源：http://ioq.chenzaomai.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xcd.c1oappe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://woj.epnwcf.com

Ruby: threads.map(&:join)
来源：http://kxg.cashguo.top

C#:   await Task.WhenAll(t1, t2)
来源：http://icw.cheryme.top

[O06] 使用进程池
来源：http://taj.0kj1m.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vik.sweek.top

PHP:  // pcntl_fork 或多进程队列
来源：http://nek.daxiang520.top

JS:   // child_process / cluster 模块
来源：http://jzq.jinyuanbaomall.cn

TS:   // child_process / cluster 模块
来源：http://bxe.hesvh.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dgy.hammf.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sdv.ivvv.top

Ruby: // fork 块
来源：http://wwb.bjfxy.top

C#:   Parallel.For
来源：http://zla.jinghuilouyu.cn

================================================================================
来源：http://oxj.wangshuangyany.cn

P. 常用工具函数
来源：http://osl.uphjek.com

================================================================================
来源：http://kkg.pengpengdd.cyou

[P01] 生成 UUID
来源：http://mwr.tanke756.top

Py:   str(uuid.uuid4())
来源：http://dbp.nanxuanxn.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dnb.jinqigfzy.top

JS:   crypto.randomUUID()
来源：http://xop.smart0.xyz


<!-- 参考信息 -->
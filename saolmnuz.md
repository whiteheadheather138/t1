代发 wailian999

[L03] 设置自定义请求头
来源：http://zgl.gzhubu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ywa.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://frm.daxiang520.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uog.c1oappe.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ljr.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kmz.hcnkem.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://omz.zhoulong.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fdp.yanxiufei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vlt.chenzaomai.com

[L04] 设置超时
来源：http://atp.yonumen.top

Py:   requests.get(url, timeout=5)
来源：http://zaj.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hbv.yueranfly.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nma.yj20258888.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aps.yanxiufei.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nrw.jqgufenzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cjv.ydjk.org.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vey.yongpay.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ssy.zdbjq.cn

[L05] 上传文件（multipart）
来源：http://wer.vehdjk.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fux.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yit.fktsv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dcx.yfazqb.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hlr.shzxlz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://axp.jinghuilouyu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://abb.ybcxt.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://whw.hnxiangtu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://odg.tarul.cn

[L06] 解析响应为 JSON
来源：http://kde.redwolf501.top

Py:   resp.json()
来源：http://rcz.cqqwz.cn

PHP:  json_decode($body, true);
来源：http://izk.ydzc1.top

JS:   await resp.json()
来源：http://jkf.sxryk.cn

TS:   await resp.json()
来源：http://rsv.xuanzx.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tou.jinqigufen.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tlg.zhoulong.xyz

Ruby: JSON.parse(resp.body)
来源：http://zqi.ppjwa.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ygn.bjfxy.top

[L07] 处理 HTTP 状态码
来源：http://wcr.svipenyu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://axi.jinqigufen.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jts.bjfxy.top

JS:   resp.ok;  resp.status
来源：http://tog.tianlin.xyz

TS:   resp.ok;  resp.status
来源：http://btc.shanyushiyangkeji.top

Java: resp.statusCode()
来源：http://cmq.sjlbkw.cn

Go:   resp.StatusCode
来源：http://cnd.yfazqb.com

Ruby: resp.code.to_i
来源：http://pil.ywan-chungtsiang.top

C#:   (int)resp.StatusCode
来源：http://vff.pengpengdd.cyou

[L08] 并发请求多个地址
来源：http://lkv.shuidangran.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zyb.hesvh.cn

PHP:  curl_multi_init() 系列
来源：http://wvk.yongpay.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zrc.birdmap.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://utt.hfpthk.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ffx.aizwys.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jfw.redwolf501.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pwi.sufxvd.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://orv.shzxlz.cn

================================================================================
来源：http://zzc.ywan-chungtsiang.top

M. 命令行 / 进程 / 环境
来源：http://zcs.guannengcc.top

================================================================================
来源：http://dsk.yongpay.top

[M01] 读取命令行参数
来源：http://rgz.xingfuxueyuan.xyz

Py:   sys.argv[1:]
来源：http://zwu.yangfankeji.com

PHP:  $argv;  $argc;
来源：http://irw.sufxvd.cn

JS:   process.argv.slice(2)
来源：http://slp.nanxinkj.top

TS:   process.argv.slice(2)
来源：http://xwb.yongpay.top

Java: args 数组（main 方法参数）
来源：http://zrg.ppjwa.cn

Go:   os.Args[1:]
来源：http://are.shanyushiyangkeji.top

Ruby: ARGV
来源：http://qwt.jinghuilouyu.cn

C#:   args 数组（Main 方法参数）
来源：http://dvn.zdbjq.cn

[M02] 读取环境变量
来源：http://kuk.zycfv.cn

Py:   os.environ.get("HOME")
来源：http://oue.haohaochexian.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jrk.chenlongwang.top

JS:   process.env.HOME
来源：http://sco.bjfxy.top

TS:   process.env.HOME
来源：http://bgz.zycfv.cn

Java: System.getenv("HOME")
来源：http://ybk.hcnkem.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ztl.nanxinkj.top

Ruby: ENV["HOME"]
来源：http://vsg.hesvh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bll.yueranfly.top

[M03] 执行外部命令
来源：http://jgm.aizwys.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hnv.jianghu66.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blg.zhaomingkeji.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://svv.redwolf501.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xnk.yonumen.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hfm.quarkkingdee.top

Go:   exec.Command("ls", "-l").Output()
来源：http://llq.xziqi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://frb.hysaishi.cn

C#:   Process.Start("ls", "-l");
来源：http://ukn.yj20258888.top

[M04] 获取当前工作目录
来源：http://bsy.hysaishi.cn

Py:   os.getcwd()
来源：http://jfh.cheryme.top

PHP:  getcwd();
来源：http://ies.wangdashe.top

JS:   process.cwd()
来源：http://mhn.birdmap.top

TS:   process.cwd()
来源：http://jdl.xziqi.cn

Java: Path.of("").toAbsolutePath()
来源：http://yys.shanyushiyangkeji.top

Go:   os.Getwd()
来源：http://zae.dianchejie.cn

Ruby: Dir.pwd
来源：http://lsi.aizwys.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sbb.cashguo.top

[M05] 设置退出码
来源：http://phc.xingfuxueyuan.xyz

Py:   sys.exit(1)
来源：http://ouf.hongshengwenyu.top

PHP:  exit(1);
来源：http://tgu.hnqzz.top

JS:   process.exit(1)
来源：http://qee.hywenlv.cn

TS:   process.exit(1)
来源：http://lin.birdmap.top

Java: System.exit(1)
来源：http://cvp.jinghuilouyu.cn

Go:   os.Exit(1)
来源：http://tav.cheryme.top

Ruby: exit 1
来源：http://usk.svipenyu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://duq.zdbjq.cn

[M06] 向标准错误输出
来源：http://wjo.feifeiyinyue.top

Py:   print("err", file=sys.stderr)
来源：http://wjf.bbcook.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://soh.9152youxi.cn

JS:   console.error("err")
来源：http://dnt.svipenyu.cn

TS:   console.error("err")
来源：http://wmq.feifeiyinyue.top

Java: System.err.println("err")
来源：http://sok.jinghuilouyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://shb.hcnkem.com

Ruby: warn "err"
来源：http://rvg.gaohongyu789.top

C#:   Console.Error.WriteLine("err")
来源：http://lok.havefunace.top

[M07] 判断是否为主入口
来源：http://djs.yfazqb.com

Py:   if __name__ == "__main__":
来源：http://pdd.xingfuxueyuan.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yaw.tianlin.xyz

JS:   require.main === module
来源：http://ywx.cqqwz.cn

TS:   require.main === module
来源：http://mkn.hammf.cn

Java: public static void main(String[] args)
来源：http://oex.gaohongyu789.top

Go:   func main()
来源：http://stq.xingfuxueyuan.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gee.nanxuanxn.top

C#:   static void Main(string[] args)
来源：http://yqy.hesvh.cn

[M08] 获取系统与运行时信息
来源：http://zcf.cucudq.cn

Py:   platform.system();  platform.python_version()
来源：http://imt.jyoumei.cn

PHP:  PHP_OS;  phpversion();
来源：http://gre.feifeiyinyue.top

JS:   process.platform;  process.version
来源：http://ueq.chenjidiqi.icu

TS:   process.platform;  process.version
来源：http://lek.smart0.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yur.gzhubu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://cid.pycfn.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kwv.tanke756.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://awx.kuanghao11.cn

================================================================================
来源：http://avd.yanxiufei.cn

N. 数据结构与算法
来源：http://feh.zhijiandao.cn

================================================================================
来源：http://pnh.yj20258888.top

[N01] 二分查找（有序数组）
来源：http://eof.zhoulong.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://yub.jinqigfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hkp.daxiang520.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://khx.ydjk.org.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lcp.cucudq.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hof.sxryk.cn

Go:   sort.SearchInts(arr, x)
来源：http://gbe.cheryme.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ikv.yj20258888.top

C#:   Array.BinarySearch(arr, x)
来源：http://usn.tarul.cn

[N02] 排序（工程实践用内置实现）
来源：http://ifp.0kj1m.cn

Py:   sorted(arr);  arr.sort()
来源：http://mtb.jianghu66.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fwb.yongpay.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://rga.wangshuangyany.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://afu.daxiang520.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kkq.yvedp.cn

Go:   slices.Sort(arr)
来源：http://zgd.xinyue.icu

Ruby: arr.sort
来源：http://kog.wangdashe.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://usg.hcnkem.com

[N03] 快速排序（分治示例）
来源：http://xgx.meibo888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fdw.mhx1999.top

PHP:  // 递归实现，或用 usort
来源：http://gkn.yonumen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ahm.xinyue.icu

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hey.shzxlz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://znh.aizwys.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zvt.chenlongwang.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://oaz.yj20258.top

C#:   // 手写递归，或 Array.Sort
来源：http://hqf.xziqi.cn

[N04] 斐波那契数列
来源：http://mtw.tianlin.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zqp.guowangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mey.zhijiandao.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tpg.pengpengdd.cyou

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ebi.shangyingyoupin.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bqh.jinqigufen.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://phe.jinqigufen.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sko.sxryk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://azl.zdqjudy.top

[N05] 最大公约数
来源：http://igi.jlsjyb.cn

Py:   math.gcd(a, b)
来源：http://kyz.9152youxi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cnd.hfpthk.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ffn.feifeiyinyue.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hcw.gotoacloud.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://znu.hfpthk.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yqz.jyoumei.cn

Ruby: a.gcd(b)
来源：http://tjc.xingfuxueyuan.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dmb.shzxlz.cn

[N06] 判断回文字符串
来源：http://ovv.tianlin.xyz

Py:   s == s[::-1]
来源：http://vcd.kuanghao11.cn

PHP:  $s === strrev($s);
来源：http://oah.ywan-chungtsiang.top

JS:   s === [...s].reverse().join("")
来源：http://mmf.jiagoushi.top

TS:   s === [...s].reverse().join("")
来源：http://kso.nanxinkj.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yns.zhoulong.xyz

Go:   // 双指针从两端比较
来源：http://hor.birdmap.top

Ruby: s == s.reverse
来源：http://yfc.hysaishi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://odx.jianghu66.top

[N07] 两数之和（返回下标）
来源：http://ayd.chenjidiqi.icu

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qvv.aibaodan.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jxh.zhiwuduotai.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wcv.316326.xyz

TS:   // 手写 Map<string, number>
来源：http://ybm.jinyuanbaomall.cn

Java: // 手写 HashMap
来源：http://wbg.hfpthk.cn

Go:   // 手写 map[int]int
来源：http://tsn.hysaishi.cn

Ruby: // 手写 Hash
来源：http://dci.zhixingplan.top

C#:   // 手写 Dictionary<int, int>
来源：http://loa.jianghu66.top

[N08] 生成全排列
来源：http://qoz.quarkkingdee.top

Py:   itertools.permutations(arr)
来源：http://olp.chenzaomai.com

PHP:  // 手写递归交换
来源：http://uet.ppjwa.cn

JS:   // 手写回溯递归
来源：http://bqf.andypj.xyz

TS:   // 手写回溯递归
来源：http://vku.fanxiaobao.xyz

Java: // 手写回溯递归
来源：http://ixj.cqqwz.cn

Go:   // 手写回溯递归
来源：http://rbk.andypj.xyz

Ruby: arr.permutation.to_a
来源：http://skm.shanyushiyangtech.top

C#:   // 手写回溯递归
来源：http://zau.ppjwa.cn

[N09] 栈与队列
来源：http://efb.dianchejie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wfo.ctjpmb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cdn.havefunace.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://huw.dianchejie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yfj.guannengcc.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ylb.zdqjudy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xyr.xziqi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://oab.gaohongyu789.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://aac.yj202588.top

[N10] 链表节点定义
来源：http://mvw.jyoumei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ryw.wangshuangyany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qip.ybcxt.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rbl.chenlongwang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://aca.sxryk.cn

Java: class Node { int v; Node next; }
来源：http://uth.uphjek.com

Go:   type Node struct { V int; Next *Node }
来源：http://nbw.chenzaomai.com

Ruby: Node = Struct.new(:v, :next)
来源：http://ias.52xcode.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://tvp.quarkkingdee.top

[N11] 二叉树中序遍历
来源：http://atc.cdnleiting.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://khh.yueranfly.top

PHP:  // 手写递归函数
来源：http://xov.ctjpmb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qgy.zhijiandao.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xny.hesvh.cn

Java: // 手写递归
来源：http://pqb.zhaomingkeji.xyz

Go:   // 手写递归
来源：http://xdx.bjfxy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mxo.sysykeji.top

C#:   // 手写递归
来源：http://xst.birdmap.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zpm.wangdashe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jhf.316326.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://weq.zhijiandao.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xtl.ydzc1.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://err.tarul.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hzd.snrcjt.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cbi.jqgufenzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tqg.yueranfly.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nii.kuanghao11.cn

================================================================================
来源：http://hee.fanxiaobao.xyz

O. 并发与异步
来源：http://btx.aizwys.cn

================================================================================
来源：http://sgx.316326.xyz

[O01] 启动一个线程
来源：http://snm.jinyuanbaomall.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://opz.meibo888.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kqs.bjfxy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bbs.jlsjyb.cn

TS:   // 同 JS
来源：http://lvt.shuidangran.top

Java: new Thread(() -> f()).start()
来源：http://gqp.ybcxt.top

Go:   go f()
来源：http://kcl.hfpthk.cn

Ruby: Thread.new { f }
来源：http://miw.jinqigfzy.top

C#:   Task.Run(() => F());
来源：http://jfg.hongshengwenyu.top

[O02] 使用线程池
来源：http://jhu.zhoulong.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mvj.zhaomingkeji.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://htj.hcnkem.com

JS:   // worker_threads 线程池
来源：http://xbb.cashguo.top

TS:   // worker_threads 线程池
来源：http://qyu.shanyushiyangtech.top

Java: Executors.newFixedThreadPool(4)
来源：http://evy.nanxinkj.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://owo.bjfxy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uqu.fktsv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dol.sufxvd.cn

[O03] 加锁保护共享数据
来源：http://iab.ehwqpu.com

Py:   with lock: shared += 1
来源：http://sxm.chenzaomai.com

PHP:  // 用 flock() 做文件锁
来源：http://rvg.tanke756.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://usb.iojbl.cn

TS:   // 同 JS
来源：http://iya.epnwcf.com

Java: synchronized (this) { shared++; }
来源：http://snu.hcnkem.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jjb.quarkkingdee.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://qjw.nanxuanxn.top

C#:   lock (gate) { shared++; }
来源：http://myi.shanyushiyangtech.top

[O04] 定义异步函数并等待
来源：http://rbt.hesvh.cn

Py:   async def f():⏎    await g()
来源：http://ngu.iojbl.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dsa.shzxlz.cn

JS:   async function f() { await g(); }
来源：http://onh.xinyue.icu

TS:   async function f(): Promise<void> { await g(); }
来源：http://ymr.shzxlz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://phl.aibaodan.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cob.epnwcf.com

Ruby: # 用 Fiber 或 async gem
来源：http://ett.yuxming.cn

C#:   async Task F() { await G(); }
来源：http://geu.feifeiyinyue.top

[O05] 并发执行并等待全部完成
来源：http://hbg.dianchejie.cn

Py:   asyncio.gather(*tasks)
来源：http://eiq.fzhhl.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://syr.ywan-chungtsiang.top

JS:   await Promise.all(tasks)
来源：http://qei.gogol.net.cn

TS:   await Promise.all(tasks)
来源：http://iyu.nanxinkj.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kjc.hnqzz.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lfi.havefunace.top

Ruby: threads.map(&:join)
来源：http://iua.zdqjudy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://hou.yanxiufei.cn

[O06] 使用进程池
来源：http://gya.redwolf501.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iqs.gogol.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nof.ivvv.top

JS:   // child_process / cluster 模块
来源：http://mjb.shanyushiyangkeji.top

TS:   // child_process / cluster 模块
来源：http://dpk.guowangkeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zku.zhoulong.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fij.xylfe.cn

Ruby: // fork 块
来源：http://ejt.zhoulong.xyz

C#:   Parallel.For
来源：http://usu.zhiwuduotai.top

================================================================================
来源：http://kgx.yuanzhike.top

P. 常用工具函数
来源：http://efq.xuetiantiany.cn

================================================================================
来源：http://lvs.316326.xyz


<!-- 参考信息 -->
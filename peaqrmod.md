代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vos.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vqs.hnqzz.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ikl.pengpengdd.cyou

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zzf.hongshengwenyu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ngr.xziqi.cn

[L04] 设置超时
来源：http://qhs.ehwqpu.com

Py:   requests.get(url, timeout=5)
来源：http://yvq.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bmk.sysykeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hpy.nanxinkj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wai.shuidangran.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qsz.yuxming.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gwx.zhengqikj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cqy.dashuyun.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wpq.ydzc1.top

[L05] 上传文件（multipart）
来源：http://xbc.xinyue.icu

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fce.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qgy.gogol.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://otj.wangdashe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gkh.ydzc1.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uzz.gogol.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tso.svipenyu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ylr.ppjwa.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://otq.zycfv.cn

[L06] 解析响应为 JSON
来源：http://uvi.meibo888.top

Py:   resp.json()
来源：http://tmo.birdmap.top

PHP:  json_decode($body, true);
来源：http://uwj.havefunace.top

JS:   await resp.json()
来源：http://vtp.feifeiyinyue.top

TS:   await resp.json()
来源：http://gmb.yueranfly.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ida.nanxuanxn.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mqd.epnwcf.com

Ruby: JSON.parse(resp.body)
来源：http://oin.316326.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sfu.gotoacloud.top

[L07] 处理 HTTP 状态码
来源：http://gmt.fanxiaobao.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kjd.vqdsnc.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ozz.gotoacloud.top

JS:   resp.ok;  resp.status
来源：http://rpt.svipenyu.cn

TS:   resp.ok;  resp.status
来源：http://dlg.uphjek.com

Java: resp.statusCode()
来源：http://hbn.c1oappe.top

Go:   resp.StatusCode
来源：http://jth.gaohongyu789.top

Ruby: resp.code.to_i
来源：http://uho.xziqi.cn

C#:   (int)resp.StatusCode
来源：http://bqf.hammf.cn

[L08] 并发请求多个地址
来源：http://tgs.pycfn.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ecq.sysykeji.top

PHP:  curl_multi_init() 系列
来源：http://uvd.yuanzhike.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://voe.zhengqikj.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lpz.cucudq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://weg.meibo888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://znu.fktsv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xyy.jinghuilouyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hgd.pycfn.com

================================================================================
来源：http://izg.xingfuxueyuan.xyz

M. 命令行 / 进程 / 环境
来源：http://pgt.zhoulong.xyz

================================================================================
来源：http://vsw.smart0.xyz

[M01] 读取命令行参数
来源：http://ayv.yj202588.top

Py:   sys.argv[1:]
来源：http://vho.xingfuxueyuan.xyz

PHP:  $argv;  $argc;
来源：http://fjl.zycfv.cn

JS:   process.argv.slice(2)
来源：http://xai.jiagoushi.top

TS:   process.argv.slice(2)
来源：http://yld.hywenlv.cn

Java: args 数组（main 方法参数）
来源：http://bde.sjlbkw.cn

Go:   os.Args[1:]
来源：http://jil.tanke756.top

Ruby: ARGV
来源：http://oav.jlsjyb.cn

C#:   args 数组（Main 方法参数）
来源：http://atg.cheryme.top

[M02] 读取环境变量
来源：http://exz.cdnleiting.top

Py:   os.environ.get("HOME")
来源：http://row.ctjpmb.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ume.tianlin.xyz

JS:   process.env.HOME
来源：http://nvd.hongshengwenyu.top

TS:   process.env.HOME
来源：http://ggv.shuidangran.top

Java: System.getenv("HOME")
来源：http://lym.aizwys.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uqx.snrcjt.cn

Ruby: ENV["HOME"]
来源：http://nzn.guannengcc.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cbe.cashguo.top

[M03] 执行外部命令
来源：http://isn.xylfe.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yhd.wangdashe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oor.jqgufenzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://dbd.wangshuangyany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://crn.nanxuanxn.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hdp.fzhhl.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vcc.shangyingyoupin.top

Ruby: system("ls -l");  `ls -l`
来源：http://pqq.xinyue.icu

C#:   Process.Start("ls", "-l");
来源：http://ivd.redwolf501.top

[M04] 获取当前工作目录
来源：http://okq.jiagoushi.top

Py:   os.getcwd()
来源：http://blp.sjlbkw.cn

PHP:  getcwd();
来源：http://bsg.yj20258888.top

JS:   process.cwd()
来源：http://kmj.ppjwa.cn

TS:   process.cwd()
来源：http://kgp.zhongyouzk.top

Java: Path.of("").toAbsolutePath()
来源：http://bcr.vehdjk.com

Go:   os.Getwd()
来源：http://vaa.zhiwuduotai.top

Ruby: Dir.pwd
来源：http://tey.cqqwz.cn

C#:   Directory.GetCurrentDirectory()
来源：http://usd.svipenyu.cn

[M05] 设置退出码
来源：http://sbg.hcnkem.com

Py:   sys.exit(1)
来源：http://mfa.fengsongda.top

PHP:  exit(1);
来源：http://iaf.yuxming.cn

JS:   process.exit(1)
来源：http://wax.andypj.xyz

TS:   process.exit(1)
来源：http://dsz.zhijiandao.cn

Java: System.exit(1)
来源：http://njk.fehbvm.com

Go:   os.Exit(1)
来源：http://plw.yfazqb.com

Ruby: exit 1
来源：http://sia.smart0.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qtk.vehdjk.com

[M06] 向标准错误输出
来源：http://aet.bbcook.cn

Py:   print("err", file=sys.stderr)
来源：http://log.zhengqikj.top

PHP:  fwrite(STDERR, "err\n");
来源：http://imf.sjlbkw.cn

JS:   console.error("err")
来源：http://wbv.hnxiangtu.top

TS:   console.error("err")
来源：http://inm.guannengcc.top

Java: System.err.println("err")
来源：http://ujn.xingfuxueyuan.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sed.fzhhl.top

Ruby: warn "err"
来源：http://cuj.hnxiangtu.top

C#:   Console.Error.WriteLine("err")
来源：http://esc.jianghu66.top

[M07] 判断是否为主入口
来源：http://ewf.chenlongwang.top

Py:   if __name__ == "__main__":
来源：http://uec.shanyushiyangkeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rgv.tian-w.cn

JS:   require.main === module
来源：http://xca.ydzc1.top

TS:   require.main === module
来源：http://ddt.jlsjyb.cn

Java: public static void main(String[] args)
来源：http://xkt.nanxinkj.top

Go:   func main()
来源：http://nrc.yuanzhike.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fsy.sufxvd.cn

C#:   static void Main(string[] args)
来源：http://mrk.nwbrower.top

[M08] 获取系统与运行时信息
来源：http://ziw.zdbjq.cn

Py:   platform.system();  platform.python_version()
来源：http://hnt.sufxvd.cn

PHP:  PHP_OS;  phpversion();
来源：http://tml.jinghuilouyu.cn

JS:   process.platform;  process.version
来源：http://nol.guowangkeji.top

TS:   process.platform;  process.version
来源：http://woy.sjlbkw.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hpp.pengpengdd.cyou

Go:   runtime.GOOS;  runtime.Version()
来源：http://bhg.ppjwa.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lmd.tarul.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rll.zhongyouzk.top

================================================================================
来源：http://qkv.chenjidiqi.icu

N. 数据结构与算法
来源：http://gfy.ehwqpu.com

================================================================================
来源：http://kki.snrcjt.cn

[N01] 二分查找（有序数组）
来源：http://vvw.xuetiantiany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wyh.vehdjk.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lzc.hongshengwenyu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://een.guannengcc.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://swj.snrcjt.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jkk.ehwqpu.com

Go:   sort.SearchInts(arr, x)
来源：http://pgr.tarul.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://exb.fengsongda.top

C#:   Array.BinarySearch(arr, x)
来源：http://hgj.shanyushiyangkeji.top

[N02] 排序（工程实践用内置实现）
来源：http://ycp.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://bjk.pengpengdd.cyou

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ljf.hnqzz.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bss.yonumen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://red.vehdjk.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ftr.birdmap.top

Go:   slices.Sort(arr)
来源：http://rgc.hongshengwenyu.top

Ruby: arr.sort
来源：http://qfo.zhijiandao.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mor.cdnleiting.top

[N03] 快速排序（分治示例）
来源：http://jua.hesvh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zwr.vqdsnc.cn

PHP:  // 递归实现，或用 usort
来源：http://urp.52xcode.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gnb.fanxiaobao.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nyf.hfpthk.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vwx.vehdjk.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ksj.jyoumei.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://unj.zdbjq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xoi.hcnkem.com

[N04] 斐波那契数列
来源：http://jpw.0kj1m.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jti.bjfxy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bfe.hnqzz.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kxy.mhx1999.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gqj.vqdsnc.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pjl.sweek.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://del.cucudq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ajz.cheryme.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://syd.smart0.xyz

[N05] 最大公约数
来源：http://ofx.vehdjk.com

Py:   math.gcd(a, b)
来源：http://xiq.ywan-chungtsiang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kgc.hfpthk.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://evv.sweek.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fyn.jianghu66.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tgf.gaohongyu789.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://epj.ivvv.top

Ruby: a.gcd(b)
来源：http://xcr.vehdjk.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tdu.jinghuilouyu.cn

[N06] 判断回文字符串
来源：http://dnm.havefunace.top

Py:   s == s[::-1]
来源：http://vha.0kj1m.cn

PHP:  $s === strrev($s);
来源：http://ptm.hongshengwenyu.top

JS:   s === [...s].reverse().join("")
来源：http://rio.iojbl.cn

TS:   s === [...s].reverse().join("")
来源：http://kwo.ppjwa.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vhq.shanyushiyangkeji.top

Go:   // 双指针从两端比较
来源：http://ohe.guowangkeji.top

Ruby: s == s.reverse
来源：http://nap.nwbrower.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://aqh.0kj1m.cn

[N07] 两数之和（返回下标）
来源：http://qid.haohaochexian.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ole.jqgfzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dwi.zhoulong.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://zbp.daxiang520.top

TS:   // 手写 Map<string, number>
来源：http://emz.zhengqikj.top

Java: // 手写 HashMap
来源：http://aov.zhongyouzk.top

Go:   // 手写 map[int]int
来源：http://hpg.nanxinkj.top

Ruby: // 手写 Hash
来源：http://aio.jianghu66.top

C#:   // 手写 Dictionary<int, int>
来源：http://wgr.jinqigufen.top

[N08] 生成全排列
来源：http://lfd.uphjek.com

Py:   itertools.permutations(arr)
来源：http://iho.cheryme.top

PHP:  // 手写递归交换
来源：http://xeh.meibo888.top

JS:   // 手写回溯递归
来源：http://zbr.jinqigufen.top

TS:   // 手写回溯递归
来源：http://hej.shanyushiyangtech.top

Java: // 手写回溯递归
来源：http://pqo.chenjidiqi.icu

Go:   // 手写回溯递归
来源：http://auo.yanxiufei.cn

Ruby: arr.permutation.to_a
来源：http://maa.smart0.xyz

C#:   // 手写回溯递归
来源：http://saj.nanxuanxn.top

[N09] 栈与队列
来源：http://sps.sjlbkw.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kku.nwbrower.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cpx.iojbl.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lpj.zhaomingkeji.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yaq.shangyingyoupin.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://odv.c1oappe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bap.xziqi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pqk.gotoacloud.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://osi.zhoulong.xyz

[N10] 链表节点定义
来源：http://zzp.0kj1m.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jop.dianchejie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ydl.xuetiantiany.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zwx.aizwys.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ubv.sxryk.cn

Java: class Node { int v; Node next; }
来源：http://tlr.nwbrower.top

Go:   type Node struct { V int; Next *Node }
来源：http://tmv.chenzaomai.com

Ruby: Node = Struct.new(:v, :next)
来源：http://cnl.hnxiangtu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://iih.svipenyu.cn

[N11] 二叉树中序遍历
来源：http://rgw.ybcxt.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pef.jqgfzy.top

PHP:  // 手写递归函数
来源：http://biz.xylfe.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bxw.jqgufenzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ahp.jinghuilouyu.cn

Java: // 手写递归
来源：http://rsa.hysaishi.cn

Go:   // 手写递归
来源：http://cdw.tarul.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cpi.tianlin.xyz

C#:   // 手写递归
来源：http://mxc.zhongyouzk.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ckx.chenzaomai.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://izx.gogol.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ele.ehwqpu.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xsl.tarul.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pxi.fktsv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cqi.chenlongwang.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dki.yj20258.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pgh.ydzc1.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://csl.cdnleiting.top

================================================================================
来源：http://vbi.jyoumei.cn

O. 并发与异步
来源：http://sfo.fehbvm.com

================================================================================
来源：http://zjt.tianlin.xyz

[O01] 启动一个线程
来源：http://ibs.kuanghao11.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qak.hfpthk.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zzt.xuanzx.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mpf.svipenyu.cn

TS:   // 同 JS
来源：http://peh.hfpthk.cn

Java: new Thread(() -> f()).start()
来源：http://waf.wangshuangyany.cn

Go:   go f()
来源：http://apu.yongpay.top

Ruby: Thread.new { f }
来源：http://yxi.sufxvd.cn

C#:   Task.Run(() => F());
来源：http://aji.zycfv.cn

[O02] 使用线程池
来源：http://tmp.nanxuanxn.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hlp.tianlin.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sze.zdbjq.cn

JS:   // worker_threads 线程池
来源：http://lle.9152youxi.cn

TS:   // worker_threads 线程池
来源：http://rsn.9152youxi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://flu.fehbvm.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fbr.andypj.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qlq.yonumen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qcg.uphjek.com

[O03] 加锁保护共享数据
来源：http://tms.yj20258.top

Py:   with lock: shared += 1
来源：http://qlg.yongpay.top

PHP:  // 用 flock() 做文件锁
来源：http://cef.zhongyouzk.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fxy.yfazqb.com

TS:   // 同 JS
来源：http://rtd.zdbjq.cn

Java: synchronized (this) { shared++; }
来源：http://wjy.bbcook.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rlf.hcnkem.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://zhg.uphjek.com

C#:   lock (gate) { shared++; }
来源：http://onp.jinghuilouyu.cn

[O04] 定义异步函数并等待
来源：http://wtc.zhijiandao.cn

Py:   async def f():⏎    await g()
来源：http://erw.xinyue.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tfn.shangyingyoupin.top

JS:   async function f() { await g(); }
来源：http://yzs.andypj.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://xgl.xuetiantiany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lqf.feifeiyinyue.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://obl.chenjidiqi.icu

Ruby: # 用 Fiber 或 async gem
来源：http://kvp.snrcjt.cn

C#:   async Task F() { await G(); }
来源：http://ivl.svipenyu.cn

[O05] 并发执行并等待全部完成
来源：http://aqs.kuanghao11.cn

Py:   asyncio.gather(*tasks)
来源：http://vpg.dashuyun.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://iws.gogol.net.cn

JS:   await Promise.all(tasks)
来源：http://lic.0kj1m.cn

TS:   await Promise.all(tasks)
来源：http://dzy.yonumen.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bnl.xuanzx.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mes.jqgfzy.top

Ruby: threads.map(&:join)
来源：http://gcl.yongpay.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lrx.zhixingplan.top

[O06] 使用进程池
来源：http://wrw.iojbl.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tsw.c1oappe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://dhu.kuanghao11.cn

JS:   // child_process / cluster 模块
来源：http://ehr.nanxinkj.top

TS:   // child_process / cluster 模块
来源：http://axk.jinqigfzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nrm.jqgfzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xny.shzxlz.cn

Ruby: // fork 块
来源：http://jfu.hnxiangtu.top

C#:   Parallel.For
来源：http://aji.hfpthk.cn

================================================================================
来源：http://wsp.vehdjk.com

P. 常用工具函数
来源：http://vih.wangdashe.top

================================================================================
来源：http://fgs.zhijiandao.cn

[P01] 生成 UUID
来源：http://kuy.ppjwa.cn

Py:   str(uuid.uuid4())
来源：http://myd.zhijiandao.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qus.ppjwa.cn

JS:   crypto.randomUUID()
来源：http://weo.xylfe.cn


<!-- 参考信息 -->
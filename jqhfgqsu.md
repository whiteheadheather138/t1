代发 wailian999

[L03] 设置自定义请求头
来源：http://ily.pycfn.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fhg.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://opp.tarul.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ewu.pengpengdd.cyou

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ewf.nwbrower.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zfx.shzxlz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ojo.andypj.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rzs.zdqjudy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://eym.ppjwa.cn

[L04] 设置超时
来源：http://cwa.zhixingplan.top

Py:   requests.get(url, timeout=5)
来源：http://gaf.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uhp.c1oappe.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kxk.jinghuilouyu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jch.redwolf501.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://oud.hongshengwenyu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dly.zdbjq.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vbj.jyoumei.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qid.jinqigufen.top

[L05] 上传文件（multipart）
来源：http://lyb.jqgufenzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hgn.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sel.zycfv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ghx.fehbvm.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mbe.meibo888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uyc.sxryk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dns.ppjwa.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dhd.shanyushiyangtech.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vtl.ywan-chungtsiang.top

[L06] 解析响应为 JSON
来源：http://wkd.jqgufenzy.top

Py:   resp.json()
来源：http://bjz.uphjek.com

PHP:  json_decode($body, true);
来源：http://wav.gotoacloud.top

JS:   await resp.json()
来源：http://jku.sysykeji.top

TS:   await resp.json()
来源：http://tyg.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lra.smart0.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://deq.bjfxy.top

Ruby: JSON.parse(resp.body)
来源：http://inf.nanxuanxn.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kob.havefunace.top

[L07] 处理 HTTP 状态码
来源：http://ncv.aibaodan.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pkz.pengpengdd.cyou

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jor.sxryk.cn

JS:   resp.ok;  resp.status
来源：http://cor.cheryme.top

TS:   resp.ok;  resp.status
来源：http://xeh.guowangkeji.top

Java: resp.statusCode()
来源：http://aky.cqqwz.cn

Go:   resp.StatusCode
来源：http://muy.pengpengdd.cyou

Ruby: resp.code.to_i
来源：http://ddx.cdnleiting.top

C#:   (int)resp.StatusCode
来源：http://mxo.daxiang520.top

[L08] 并发请求多个地址
来源：http://qys.jqgfzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lym.bjfxy.top

PHP:  curl_multi_init() 系列
来源：http://why.yanxiufei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jsj.fzhhl.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rvw.hesvh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mri.jiagoushi.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ils.quarkkingdee.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://img.ehwqpu.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zhk.zhaomingkeji.xyz

================================================================================
来源：http://frq.fktsv.cn

M. 命令行 / 进程 / 环境
来源：http://spg.jqgfzy.top

================================================================================
来源：http://nba.yfazqb.com

[M01] 读取命令行参数
来源：http://vnz.hongshengwenyu.top

Py:   sys.argv[1:]
来源：http://prm.smart0.xyz

PHP:  $argv;  $argc;
来源：http://zlg.jqgfzy.top

JS:   process.argv.slice(2)
来源：http://qkx.zhaomingkeji.xyz

TS:   process.argv.slice(2)
来源：http://imb.wangshuangyany.cn

Java: args 数组（main 方法参数）
来源：http://nop.nwbrower.top

Go:   os.Args[1:]
来源：http://dcv.0kj1m.cn

Ruby: ARGV
来源：http://ofx.cucudq.cn

C#:   args 数组（Main 方法参数）
来源：http://kun.yongpay.top

[M02] 读取环境变量
来源：http://yej.9152youxi.cn

Py:   os.environ.get("HOME")
来源：http://gvz.fktsv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://apr.shzxlz.cn

JS:   process.env.HOME
来源：http://qks.zhaomingkeji.xyz

TS:   process.env.HOME
来源：http://zac.guannengcc.top

Java: System.getenv("HOME")
来源：http://npk.chenjidiqi.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xcf.jqgufenzy.top

Ruby: ENV["HOME"]
来源：http://tkr.epnwcf.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rxj.yonumen.top

[M03] 执行外部命令
来源：http://ggk.gzhubu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kxt.zdbjq.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://smo.hongshengwenyu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://wrv.fehbvm.com

TS:   child_process.execSync("ls -l").toString()
来源：http://aqq.yj20258.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://khs.hammf.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wwv.fzhhl.top

Ruby: system("ls -l");  `ls -l`
来源：http://rlb.yueranfly.top

C#:   Process.Start("ls", "-l");
来源：http://dwf.zhongyouzk.top

[M04] 获取当前工作目录
来源：http://hfq.jinqigfzy.top

Py:   os.getcwd()
来源：http://wis.feifeiyinyue.top

PHP:  getcwd();
来源：http://exp.ehwqpu.com

JS:   process.cwd()
来源：http://cwt.yj20258888.top

TS:   process.cwd()
来源：http://zom.havefunace.top

Java: Path.of("").toAbsolutePath()
来源：http://fdp.birdmap.top

Go:   os.Getwd()
来源：http://bko.sysykeji.top

Ruby: Dir.pwd
来源：http://fye.gzhubu.top

C#:   Directory.GetCurrentDirectory()
来源：http://sqw.yj20258.top

[M05] 设置退出码
来源：http://vto.ehwqpu.com

Py:   sys.exit(1)
来源：http://oea.0kj1m.cn

PHP:  exit(1);
来源：http://tpb.vehdjk.com

JS:   process.exit(1)
来源：http://tqn.cucudq.cn

TS:   process.exit(1)
来源：http://afc.sweek.top

Java: System.exit(1)
来源：http://pzc.chenlongwang.top

Go:   os.Exit(1)
来源：http://hvg.chenjidiqi.icu

Ruby: exit 1
来源：http://tub.hywenlv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://suk.vqdsnc.cn

[M06] 向标准错误输出
来源：http://jkk.guannengcc.top

Py:   print("err", file=sys.stderr)
来源：http://hqy.xuetiantiany.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://noj.guannengcc.top

JS:   console.error("err")
来源：http://laf.daria6918.cn

TS:   console.error("err")
来源：http://tud.shanyushiyangkeji.top

Java: System.err.println("err")
来源：http://ecg.zhijiandao.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://awo.ydjk.org.cn

Ruby: warn "err"
来源：http://gdw.hesvh.cn

C#:   Console.Error.WriteLine("err")
来源：http://osb.svipenyu.cn

[M07] 判断是否为主入口
来源：http://dde.tianlin.xyz

Py:   if __name__ == "__main__":
来源：http://ohs.zycfv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mrs.pengpengdd.cyou

JS:   require.main === module
来源：http://caw.shanyushiyangkeji.top

TS:   require.main === module
来源：http://pyq.haohaochexian.top

Java: public static void main(String[] args)
来源：http://eah.chenjidiqi.icu

Go:   func main()
来源：http://twr.gzhubu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sjd.ppjwa.cn

C#:   static void Main(string[] args)
来源：http://cwy.hesvh.cn

[M08] 获取系统与运行时信息
来源：http://wod.aibaodan.cn

Py:   platform.system();  platform.python_version()
来源：http://vwl.havefunace.top

PHP:  PHP_OS;  phpversion();
来源：http://hmc.wangdashe.top

JS:   process.platform;  process.version
来源：http://zec.iojbl.cn

TS:   process.platform;  process.version
来源：http://uog.pengpengdd.cyou

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xaq.yj20258.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://eft.havefunace.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vzj.cdnleiting.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://jee.0kj1m.cn

================================================================================
来源：http://bvu.chenzaomai.com

N. 数据结构与算法
来源：http://hum.chenlongwang.top

================================================================================
来源：http://sbp.chenlongwang.top

[N01] 二分查找（有序数组）
来源：http://vpz.hnxiangtu.top

Py:   bisect.bisect_left(arr, x)
来源：http://otr.kuanghao11.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ehw.vehdjk.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ysu.cucudq.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nzi.hywenlv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xfm.wangshuangyany.cn

Go:   sort.SearchInts(arr, x)
来源：http://cnh.zhaomingkeji.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://uvt.epnwcf.com

C#:   Array.BinarySearch(arr, x)
来源：http://uqv.shzxlz.cn

[N02] 排序（工程实践用内置实现）
来源：http://fbv.316326.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ple.gotoacloud.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xgx.nwbrower.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xes.tian-w.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hoz.feifeiyinyue.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kxb.cdnleiting.top

Go:   slices.Sort(arr)
来源：http://ukt.smart0.xyz

Ruby: arr.sort
来源：http://syj.fzhhl.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://olx.aizwys.cn

[N03] 快速排序（分治示例）
来源：http://tqj.tanke756.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ibk.jqgufenzy.top

PHP:  // 递归实现，或用 usort
来源：http://tus.wangshuangyany.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lbs.smart0.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://afp.tianlin.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ldj.cheryme.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://off.nanxinkj.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xls.jyoumei.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cxc.hnxiangtu.top

[N04] 斐波那契数列
来源：http://bhv.shzxlz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://suv.9152youxi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cqe.hcnkem.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sdy.shzxlz.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mdh.yj202588.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xud.zdbjq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tlo.zhongyouzk.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xbh.sufxvd.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gro.cheryme.top

[N05] 最大公约数
来源：http://fqj.chenjidiqi.icu

Py:   math.gcd(a, b)
来源：http://lac.hesvh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kbd.sweek.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://the.bjfxy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://meu.sufxvd.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://thk.aizwys.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xtc.fzhhl.top

Ruby: a.gcd(b)
来源：http://yzr.epnwcf.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pib.xinyue.icu

[N06] 判断回文字符串
来源：http://hql.daxiang520.top

Py:   s == s[::-1]
来源：http://mmk.feifeiyinyue.top

PHP:  $s === strrev($s);
来源：http://vii.hammf.cn

JS:   s === [...s].reverse().join("")
来源：http://wou.tian-w.cn

TS:   s === [...s].reverse().join("")
来源：http://cul.meibo888.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vhv.zhixingplan.top

Go:   // 双指针从两端比较
来源：http://pkx.uphjek.com

Ruby: s == s.reverse
来源：http://mhh.jinqigfzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://oat.gzhubu.top

[N07] 两数之和（返回下标）
来源：http://eqi.9152youxi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uvd.svipenyu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hzd.shuidangran.top

JS:   // 手写 Map：map.set(v, i)
来源：http://plv.epnwcf.com

TS:   // 手写 Map<string, number>
来源：http://eln.fktsv.cn

Java: // 手写 HashMap
来源：http://uhm.zhoulong.xyz

Go:   // 手写 map[int]int
来源：http://gvy.zycfv.cn

Ruby: // 手写 Hash
来源：http://vth.cqqwz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yff.smart0.xyz

[N08] 生成全排列
来源：http://ldj.gaohongyu789.top

Py:   itertools.permutations(arr)
来源：http://fwa.gaohongyu789.top

PHP:  // 手写递归交换
来源：http://dnu.yj20258.top

JS:   // 手写回溯递归
来源：http://qpy.9152youxi.cn

TS:   // 手写回溯递归
来源：http://gfc.kuanghao11.cn

Java: // 手写回溯递归
来源：http://hpp.tanke756.top

Go:   // 手写回溯递归
来源：http://kdp.havefunace.top

Ruby: arr.permutation.to_a
来源：http://xng.bbcook.cn

C#:   // 手写回溯递归
来源：http://jcs.vqdsnc.cn

[N09] 栈与队列
来源：http://nxs.shanyushiyangtech.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://avk.sweek.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ouz.zhongyouzk.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://too.jiagoushi.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://eup.sjlbkw.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ceu.bjfxy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wga.zhiwuduotai.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wwa.yvedp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oll.bjfxy.top

[N10] 链表节点定义
来源：http://gac.guannengcc.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zpg.jinyuanbaomall.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ymu.yuxming.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rvu.tanke756.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gus.fanxiaobao.xyz

Java: class Node { int v; Node next; }
来源：http://xng.cdnleiting.top

Go:   type Node struct { V int; Next *Node }
来源：http://lpr.jqgufenzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mka.c1oappe.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ucr.zhongyouzk.top

[N11] 二叉树中序遍历
来源：http://pvp.chenzaomai.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ajm.cdnleiting.top

PHP:  // 手写递归函数
来源：http://mfi.yongpay.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://emq.uphjek.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wvc.hesvh.cn

Java: // 手写递归
来源：http://drt.guowangkeji.top

Go:   // 手写递归
来源：http://feh.cqqwz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://icc.hfpthk.cn

C#:   // 手写递归
来源：http://dyu.chenzaomai.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tan.hongshengwenyu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tfa.nanxuanxn.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pnf.snrcjt.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gio.jinyuanbaomall.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xpj.yj20258888.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iqg.daria6918.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ylh.zhiwuduotai.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gkg.hysaishi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://crr.cdnleiting.top

================================================================================
来源：http://ggw.aibaodan.cn

O. 并发与异步
来源：http://bxe.yfazqb.com

================================================================================
来源：http://rhx.pycfn.com

[O01] 启动一个线程
来源：http://yic.yanxiufei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nde.daxiang520.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wvs.pengpengdd.cyou

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qex.hfpthk.cn

TS:   // 同 JS
来源：http://vyl.xziqi.cn

Java: new Thread(() -> f()).start()
来源：http://hsx.daxiang520.top

Go:   go f()
来源：http://jtw.kuanghao11.cn

Ruby: Thread.new { f }
来源：http://jed.cqqwz.cn

C#:   Task.Run(() => F());
来源：http://xec.hnqzz.top

[O02] 使用线程池
来源：http://kxq.shzxlz.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://thr.feifeiyinyue.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://haa.pengpengdd.cyou

JS:   // worker_threads 线程池
来源：http://zzx.jqgfzy.top

TS:   // worker_threads 线程池
来源：http://tqd.zycfv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jla.chenzaomai.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vax.hcnkem.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zyn.sufxvd.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ecy.quarkkingdee.top

[O03] 加锁保护共享数据
来源：http://rjy.chenlongwang.top

Py:   with lock: shared += 1
来源：http://flw.hnxiangtu.top

PHP:  // 用 flock() 做文件锁
来源：http://edx.ppjwa.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dpa.zdbjq.cn

TS:   // 同 JS
来源：http://fnd.yfazqb.com

Java: synchronized (this) { shared++; }
来源：http://dva.aibaodan.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://isz.andypj.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://yse.gaohongyu789.top

C#:   lock (gate) { shared++; }
来源：http://sfq.xylfe.cn

[O04] 定义异步函数并等待
来源：http://vmm.daxiang520.top

Py:   async def f():⏎    await g()
来源：http://hhk.redwolf501.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hxx.jianghu66.top

JS:   async function f() { await g(); }
来源：http://khg.fengsongda.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://riv.jinyuanbaomall.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://khw.hnqzz.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tpd.wangdashe.top

Ruby: # 用 Fiber 或 async gem
来源：http://wxg.tanke756.top

C#:   async Task F() { await G(); }
来源：http://jlz.cashguo.top

[O05] 并发执行并等待全部完成
来源：http://gdj.sweek.top

Py:   asyncio.gather(*tasks)
来源：http://bsh.uphjek.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://buc.chenjidiqi.icu

JS:   await Promise.all(tasks)
来源：http://eak.ydzc1.top

TS:   await Promise.all(tasks)
来源：http://yvc.hnqzz.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://had.fktsv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rtt.sufxvd.cn

Ruby: threads.map(&:join)
来源：http://egl.cdnleiting.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ikf.wangshuangyany.cn

[O06] 使用进程池
来源：http://fpr.gaohongyu789.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kjr.smart0.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://mnh.hnxiangtu.top

JS:   // child_process / cluster 模块
来源：http://qxc.52xcode.cn

TS:   // child_process / cluster 模块
来源：http://uei.zhixingplan.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://eoe.bjfxy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ueu.yj20258.top

Ruby: // fork 块
来源：http://skc.jianghu66.top

C#:   Parallel.For
来源：http://hzq.hfpthk.cn

================================================================================
来源：http://esb.cqqwz.cn

P. 常用工具函数
来源：http://clz.birdmap.top

================================================================================
来源：http://asn.zycfv.cn


<!-- 参考信息 -->
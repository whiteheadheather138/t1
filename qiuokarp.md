代发 wailian999

[L03] 设置自定义请求头
来源：http://uvl.zhijiandao.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zsp.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hiq.hnxiangtu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jlp.chenlongwang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cvn.yj202588.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tji.zhongyouzk.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kqg.haohaochexian.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://atp.ydzc1.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vau.zhaomingkeji.xyz

[L04] 设置超时
来源：http://trf.xuetiantiany.cn

Py:   requests.get(url, timeout=5)
来源：http://cuw.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jfb.zdqjudy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pkv.jqgufenzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yiw.feifeiyinyue.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kpr.kuanghao11.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hoz.shanyushiyangkeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rek.epnwcf.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mtb.chenlongwang.top

[L05] 上传文件（multipart）
来源：http://ypo.jlsjyb.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oss.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ldz.vqdsnc.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bpg.zdqjudy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xer.cashguo.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ogd.wangdashe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fot.aibaodan.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dym.zhijiandao.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nqy.andypj.xyz

[L06] 解析响应为 JSON
来源：http://klv.cqqwz.cn

Py:   resp.json()
来源：http://uun.zhijiandao.cn

PHP:  json_decode($body, true);
来源：http://ymi.yonumen.top

JS:   await resp.json()
来源：http://fjl.andypj.xyz

TS:   await resp.json()
来源：http://qvv.bbcook.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pgp.andypj.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ltx.feifeiyinyue.top

Ruby: JSON.parse(resp.body)
来源：http://jsd.wangshuangyany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rip.cqqwz.cn

[L07] 处理 HTTP 状态码
来源：http://wrq.fengsongda.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://whr.hnqzz.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cdk.redwolf501.top

JS:   resp.ok;  resp.status
来源：http://gjr.yuanzhike.top

TS:   resp.ok;  resp.status
来源：http://wji.316326.xyz

Java: resp.statusCode()
来源：http://xab.jiagoushi.top

Go:   resp.StatusCode
来源：http://bpg.cucudq.cn

Ruby: resp.code.to_i
来源：http://iwc.cucudq.cn

C#:   (int)resp.StatusCode
来源：http://hsh.yanxiufei.cn

[L08] 并发请求多个地址
来源：http://mya.gogol.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sbd.nanxinkj.top

PHP:  curl_multi_init() 系列
来源：http://plh.pycfn.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cve.tanke756.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dvu.vehdjk.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://upv.bbcook.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://org.kuanghao11.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wkz.zycfv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://szp.sxryk.cn

================================================================================
来源：http://mri.hongshengwenyu.top

M. 命令行 / 进程 / 环境
来源：http://iag.gotoacloud.top

================================================================================
来源：http://exj.zhengqikj.top

[M01] 读取命令行参数
来源：http://qvj.hnqzz.top

Py:   sys.argv[1:]
来源：http://lck.jyoumei.cn

PHP:  $argv;  $argc;
来源：http://xdr.shanyushiyangkeji.top

JS:   process.argv.slice(2)
来源：http://bkb.daxiang520.top

TS:   process.argv.slice(2)
来源：http://kho.daxiang520.top

Java: args 数组（main 方法参数）
来源：http://mfi.gaohongyu789.top

Go:   os.Args[1:]
来源：http://jex.hnxiangtu.top

Ruby: ARGV
来源：http://wlu.yanxiufei.cn

C#:   args 数组（Main 方法参数）
来源：http://rbx.fehbvm.com

[M02] 读取环境变量
来源：http://zlq.mhx1999.top

Py:   os.environ.get("HOME")
来源：http://ffp.smart0.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ogf.snrcjt.cn

JS:   process.env.HOME
来源：http://nze.guannengcc.top

TS:   process.env.HOME
来源：http://mmf.316326.xyz

Java: System.getenv("HOME")
来源：http://mcb.pycfn.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xsr.nanxinkj.top

Ruby: ENV["HOME"]
来源：http://djc.dashuyun.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kew.cdnleiting.top

[M03] 执行外部命令
来源：http://vwz.fanxiaobao.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zll.gotoacloud.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jnc.zhongyouzk.top

JS:   child_process.execSync("ls -l").toString()
来源：http://wxw.ywan-chungtsiang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hmn.xinyue.icu

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hqs.chenzaomai.com

Go:   exec.Command("ls", "-l").Output()
来源：http://fgt.zhongyouzk.top

Ruby: system("ls -l");  `ls -l`
来源：http://tyh.aizwys.cn

C#:   Process.Start("ls", "-l");
来源：http://jlt.sjlbkw.cn

[M04] 获取当前工作目录
来源：http://emo.chenlongwang.top

Py:   os.getcwd()
来源：http://hnj.hnqzz.top

PHP:  getcwd();
来源：http://mbx.hesvh.cn

JS:   process.cwd()
来源：http://xeg.bjfxy.top

TS:   process.cwd()
来源：http://cdb.jinqigfzy.top

Java: Path.of("").toAbsolutePath()
来源：http://sum.aibaodan.cn

Go:   os.Getwd()
来源：http://wyh.sjlbkw.cn

Ruby: Dir.pwd
来源：http://lkp.haohaochexian.top

C#:   Directory.GetCurrentDirectory()
来源：http://jye.jinqigufen.top

[M05] 设置退出码
来源：http://tqh.cashguo.top

Py:   sys.exit(1)
来源：http://bgc.guowangkeji.top

PHP:  exit(1);
来源：http://owj.svipenyu.cn

JS:   process.exit(1)
来源：http://hjn.jiagoushi.top

TS:   process.exit(1)
来源：http://mez.hnxiangtu.top

Java: System.exit(1)
来源：http://lub.kuanghao11.cn

Go:   os.Exit(1)
来源：http://gjz.yj20258888.top

Ruby: exit 1
来源：http://usl.kuanghao11.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://esc.hywenlv.cn

[M06] 向标准错误输出
来源：http://wdw.zhengqikj.top

Py:   print("err", file=sys.stderr)
来源：http://xti.bbcook.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hjv.fktsv.cn

JS:   console.error("err")
来源：http://xbn.feifeiyinyue.top

TS:   console.error("err")
来源：http://tgr.vehdjk.com

Java: System.err.println("err")
来源：http://xif.shangyingyoupin.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ouh.jiagoushi.top

Ruby: warn "err"
来源：http://cku.52xcode.cn

C#:   Console.Error.WriteLine("err")
来源：http://omm.ydzc1.top

[M07] 判断是否为主入口
来源：http://ydj.dianchejie.cn

Py:   if __name__ == "__main__":
来源：http://lkk.fanxiaobao.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dxn.xinyue.icu

JS:   require.main === module
来源：http://ppn.hongshengwenyu.top

TS:   require.main === module
来源：http://fmv.tanke756.top

Java: public static void main(String[] args)
来源：http://mzu.jinghuilouyu.cn

Go:   func main()
来源：http://kmm.tarul.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mzi.jinyuanbaomall.cn

C#:   static void Main(string[] args)
来源：http://gab.hesvh.cn

[M08] 获取系统与运行时信息
来源：http://xzp.ywan-chungtsiang.top

Py:   platform.system();  platform.python_version()
来源：http://qzn.sweek.top

PHP:  PHP_OS;  phpversion();
来源：http://qrc.9152youxi.cn

JS:   process.platform;  process.version
来源：http://rqd.jianghu66.top

TS:   process.platform;  process.version
来源：http://uas.yuxming.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nth.jinghuilouyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xfb.pycfn.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mmy.gotoacloud.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://lvk.zhixingplan.top

================================================================================
来源：http://efs.fzhhl.top

N. 数据结构与算法
来源：http://jqy.fktsv.cn

================================================================================
来源：http://vrd.haohaochexian.top

[N01] 二分查找（有序数组）
来源：http://dmp.ehwqpu.com

Py:   bisect.bisect_left(arr, x)
来源：http://gmv.bjfxy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qxp.vqdsnc.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nkm.yonumen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qsn.gotoacloud.top

Java: Arrays.binarySearch(arr, x)
来源：http://jqk.chenlongwang.top

Go:   sort.SearchInts(arr, x)
来源：http://qgu.aibaodan.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://urr.guannengcc.top

C#:   Array.BinarySearch(arr, x)
来源：http://stv.ppjwa.cn

[N02] 排序（工程实践用内置实现）
来源：http://lml.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://qss.jianghu66.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eqi.gotoacloud.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bat.ctjpmb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://toz.ehwqpu.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qpe.yfazqb.com

Go:   slices.Sort(arr)
来源：http://rre.cdnleiting.top

Ruby: arr.sort
来源：http://gha.yuxming.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://byi.kuanghao11.cn

[N03] 快速排序（分治示例）
来源：http://dje.yj20258888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sym.ybcxt.top

PHP:  // 递归实现，或用 usort
来源：http://atl.jinyuanbaomall.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zfx.gogol.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rpq.meibo888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oio.yj202588.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pbc.gaohongyu789.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://idw.meibo888.top

C#:   // 手写递归，或 Array.Sort
来源：http://wbx.hnqzz.top

[N04] 斐波那契数列
来源：http://uel.shanyushiyangtech.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ajz.mhx1999.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bma.hesvh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ffe.fktsv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gmw.guannengcc.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://epr.52xcode.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://icy.andypj.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ztx.sweek.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bpg.tanke756.top

[N05] 最大公约数
来源：http://bdy.52xcode.cn

Py:   math.gcd(a, b)
来源：http://jjp.yj202588.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://chx.ivvv.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dwr.dashuyun.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ogu.hywenlv.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xej.cheryme.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bvp.zhixingplan.top

Ruby: a.gcd(b)
来源：http://hsj.9152youxi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ykt.shangyingyoupin.top

[N06] 判断回文字符串
来源：http://pdz.smart0.xyz

Py:   s == s[::-1]
来源：http://iyz.sufxvd.cn

PHP:  $s === strrev($s);
来源：http://wtf.ydjk.org.cn

JS:   s === [...s].reverse().join("")
来源：http://kbk.dashuyun.cn

TS:   s === [...s].reverse().join("")
来源：http://hck.zhoulong.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bmb.xingfuxueyuan.xyz

Go:   // 双指针从两端比较
来源：http://obu.quarkkingdee.top

Ruby: s == s.reverse
来源：http://mlj.haohaochexian.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jie.jinghuilouyu.cn

[N07] 两数之和（返回下标）
来源：http://zxs.gotoacloud.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tza.meibo888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ojg.zhongyouzk.top

JS:   // 手写 Map：map.set(v, i)
来源：http://veq.tian-w.cn

TS:   // 手写 Map<string, number>
来源：http://myg.svipenyu.cn

Java: // 手写 HashMap
来源：http://uks.gotoacloud.top

Go:   // 手写 map[int]int
来源：http://ksi.feifeiyinyue.top

Ruby: // 手写 Hash
来源：http://wag.sysykeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://xgs.iojbl.cn

[N08] 生成全排列
来源：http://ohh.bbcook.cn

Py:   itertools.permutations(arr)
来源：http://why.aizwys.cn

PHP:  // 手写递归交换
来源：http://urv.jinqigufen.top

JS:   // 手写回溯递归
来源：http://xha.fktsv.cn

TS:   // 手写回溯递归
来源：http://xdf.zhiwuduotai.top

Java: // 手写回溯递归
来源：http://wqg.316326.xyz

Go:   // 手写回溯递归
来源：http://ywm.feifeiyinyue.top

Ruby: arr.permutation.to_a
来源：http://bbw.daxiang520.top

C#:   // 手写回溯递归
来源：http://dbq.sufxvd.cn

[N09] 栈与队列
来源：http://otx.mhx1999.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://frv.sweek.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://roj.yuxming.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jmb.hfpthk.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hvi.aibaodan.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kdg.jinqigufen.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ugh.zhaomingkeji.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iyp.nwbrower.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vxa.guowangkeji.top

[N10] 链表节点定义
来源：http://lxy.vqdsnc.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zil.hesvh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ous.hywenlv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ysk.pycfn.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kvk.nanxuanxn.top

Java: class Node { int v; Node next; }
来源：http://xjt.yj20258888.top

Go:   type Node struct { V int; Next *Node }
来源：http://vtr.316326.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://omq.xinyue.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://pdd.hesvh.cn

[N11] 二叉树中序遍历
来源：http://tzw.0kj1m.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ysd.cqqwz.cn

PHP:  // 手写递归函数
来源：http://koo.epnwcf.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iau.chenjidiqi.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rcq.yj202588.top

Java: // 手写递归
来源：http://jxr.bjfxy.top

Go:   // 手写递归
来源：http://jwo.dianchejie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hnp.wangshuangyany.cn

C#:   // 手写递归
来源：http://sqx.gotoacloud.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dqn.ydzc1.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tkh.yj202588.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hin.ivvv.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hiu.meibo888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://htc.9152youxi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ffz.gotoacloud.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hel.pycfn.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dib.yfazqb.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gte.pengpengdd.cyou

================================================================================
来源：http://iuw.iojbl.cn

O. 并发与异步
来源：http://txu.cucudq.cn

================================================================================
来源：http://cxb.vqdsnc.cn

[O01] 启动一个线程
来源：http://sxm.shuidangran.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dta.yfazqb.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nbc.birdmap.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://puu.dashuyun.cn

TS:   // 同 JS
来源：http://jll.zdbjq.cn

Java: new Thread(() -> f()).start()
来源：http://mhe.hongshengwenyu.top

Go:   go f()
来源：http://mib.hfpthk.cn

Ruby: Thread.new { f }
来源：http://gds.jlsjyb.cn

C#:   Task.Run(() => F());
来源：http://wxa.bjfxy.top

[O02] 使用线程池
来源：http://xub.kuanghao11.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rnf.fehbvm.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://evf.jqgfzy.top

JS:   // worker_threads 线程池
来源：http://jfr.c1oappe.top

TS:   // worker_threads 线程池
来源：http://sog.cashguo.top

Java: Executors.newFixedThreadPool(4)
来源：http://ymx.fehbvm.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://uwf.haohaochexian.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hqs.dashuyun.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://aub.fengsongda.top

[O03] 加锁保护共享数据
来源：http://agd.havefunace.top

Py:   with lock: shared += 1
来源：http://yem.52xcode.cn

PHP:  // 用 flock() 做文件锁
来源：http://jnq.aizwys.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pep.yj202588.top

TS:   // 同 JS
来源：http://lsh.sufxvd.cn

Java: synchronized (this) { shared++; }
来源：http://ifi.ctjpmb.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bzb.zdqjudy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://lih.daxiang520.top

C#:   lock (gate) { shared++; }
来源：http://dst.zdqjudy.top

[O04] 定义异步函数并等待
来源：http://tal.aibaodan.cn

Py:   async def f():⏎    await g()
来源：http://gic.jyoumei.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yhg.hnxiangtu.top

JS:   async function f() { await g(); }
来源：http://qsi.zhiwuduotai.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://qii.zhoulong.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://aai.bbcook.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ydm.jyoumei.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rap.hammf.cn

C#:   async Task F() { await G(); }
来源：http://qwl.yuanzhike.top

[O05] 并发执行并等待全部完成
来源：http://rsr.9152youxi.cn

Py:   asyncio.gather(*tasks)
来源：http://hen.xziqi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nhm.zdbjq.cn

JS:   await Promise.all(tasks)
来源：http://nbj.jinyuanbaomall.cn

TS:   await Promise.all(tasks)
来源：http://xbk.gzhubu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dec.sxryk.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bev.hnqzz.top

Ruby: threads.map(&:join)
来源：http://yls.hnxiangtu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://vgw.sjlbkw.cn

[O06] 使用进程池
来源：http://koj.mhx1999.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wbd.fengsongda.top

PHP:  // pcntl_fork 或多进程队列
来源：http://efp.cqqwz.cn

JS:   // child_process / cluster 模块
来源：http://oyd.jinqigufen.top

TS:   // child_process / cluster 模块
来源：http://ooi.xuanzx.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bfy.yuxming.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uzy.vqdsnc.cn

Ruby: // fork 块
来源：http://htx.yongpay.top

C#:   Parallel.For
来源：http://lub.yangfankeji.com

================================================================================
来源：http://pae.hesvh.cn

P. 常用工具函数
来源：http://cjm.feifeiyinyue.top

================================================================================
来源：http://nmu.hammf.cn


<!-- 参考信息 -->
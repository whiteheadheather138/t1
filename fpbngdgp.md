代发 wailian999

[L03] 设置自定义请求头
来源：http://loh.cheryme.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ftk.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://had.ivvv.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rjg.pycfn.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pwu.feifeiyinyue.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pwx.ivvv.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ask.jlsjyb.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://szf.yfazqb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zmx.yvedp.cn

[L04] 设置超时
来源：http://bgx.hammf.cn

Py:   requests.get(url, timeout=5)
来源：http://oqc.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pyw.havefunace.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://miu.zhiwuduotai.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ljl.yj20258888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uda.shangyingyoupin.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ens.mhx1999.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bad.shangyingyoupin.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tog.shzxlz.cn

[L05] 上传文件（multipart）
来源：http://ndx.52xcode.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wfc.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rno.tianlin.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tnx.shanyushiyangtech.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uev.aibaodan.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kwm.ydzc1.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://elu.shanyushiyangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mvc.jinyuanbaomall.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kbl.bjfxy.top

[L06] 解析响应为 JSON
来源：http://zdp.yj20258.top

Py:   resp.json()
来源：http://ldp.nwbrower.top

PHP:  json_decode($body, true);
来源：http://jvh.cdnleiting.top

JS:   await resp.json()
来源：http://scc.nanxuanxn.top

TS:   await resp.json()
来源：http://aja.nanxinkj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pik.kuanghao11.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://boj.yuxming.cn

Ruby: JSON.parse(resp.body)
来源：http://hel.ivvv.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zhf.zhijiandao.cn

[L07] 处理 HTTP 状态码
来源：http://vzk.ivvv.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zyu.tian-w.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vgs.tanke756.top

JS:   resp.ok;  resp.status
来源：http://nll.yj202588.top

TS:   resp.ok;  resp.status
来源：http://ogb.dashuyun.cn

Java: resp.statusCode()
来源：http://dac.dashuyun.cn

Go:   resp.StatusCode
来源：http://pva.shanyushiyangkeji.top

Ruby: resp.code.to_i
来源：http://ywk.vehdjk.com

C#:   (int)resp.StatusCode
来源：http://kye.wangdashe.top

[L08] 并发请求多个地址
来源：http://mip.zhiwuduotai.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kvv.aizwys.cn

PHP:  curl_multi_init() 系列
来源：http://aah.xuanzx.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nzh.feifeiyinyue.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://osh.aizwys.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://iie.yuxming.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bum.uphjek.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hxb.chenjidiqi.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tli.gotoacloud.top

================================================================================
来源：http://jqp.fanxiaobao.xyz

M. 命令行 / 进程 / 环境
来源：http://isd.hcnkem.com

================================================================================
来源：http://ybq.xuetiantiany.cn

[M01] 读取命令行参数
来源：http://ony.vehdjk.com

Py:   sys.argv[1:]
来源：http://rco.yueranfly.top

PHP:  $argv;  $argc;
来源：http://pwy.chenzaomai.com

JS:   process.argv.slice(2)
来源：http://isk.yongpay.top

TS:   process.argv.slice(2)
来源：http://kyu.aibaodan.cn

Java: args 数组（main 方法参数）
来源：http://tcq.gzhubu.top

Go:   os.Args[1:]
来源：http://rbr.bjfxy.top

Ruby: ARGV
来源：http://jot.pengpengdd.cyou

C#:   args 数组（Main 方法参数）
来源：http://ryn.daria6918.cn

[M02] 读取环境变量
来源：http://zaz.gogol.net.cn

Py:   os.environ.get("HOME")
来源：http://ojz.xuetiantiany.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://iae.yongpay.top

JS:   process.env.HOME
来源：http://zst.nanxinkj.top

TS:   process.env.HOME
来源：http://ejs.fktsv.cn

Java: System.getenv("HOME")
来源：http://zcc.yj20258.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zin.guowangkeji.top

Ruby: ENV["HOME"]
来源：http://ted.zdqjudy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zxf.chenjidiqi.icu

[M03] 执行外部命令
来源：http://vwl.fktsv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jxe.yj20258888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jcb.52xcode.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://acu.cashguo.top

TS:   child_process.execSync("ls -l").toString()
来源：http://sfd.guowangkeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xod.bbcook.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://usv.yj20258888.top

Ruby: system("ls -l");  `ls -l`
来源：http://zto.cdnleiting.top

C#:   Process.Start("ls", "-l");
来源：http://hup.52xcode.cn

[M04] 获取当前工作目录
来源：http://vzc.hfpthk.cn

Py:   os.getcwd()
来源：http://utk.ywan-chungtsiang.top

PHP:  getcwd();
来源：http://sbo.yonumen.top

JS:   process.cwd()
来源：http://vzf.meibo888.top

TS:   process.cwd()
来源：http://cfn.zhixingplan.top

Java: Path.of("").toAbsolutePath()
来源：http://epc.52xcode.cn

Go:   os.Getwd()
来源：http://yfo.chenlongwang.top

Ruby: Dir.pwd
来源：http://eru.bjfxy.top

C#:   Directory.GetCurrentDirectory()
来源：http://wuw.sjlbkw.cn

[M05] 设置退出码
来源：http://dxi.aibaodan.cn

Py:   sys.exit(1)
来源：http://txe.daria6918.cn

PHP:  exit(1);
来源：http://vwl.zhongyouzk.top

JS:   process.exit(1)
来源：http://hva.tanke756.top

TS:   process.exit(1)
来源：http://jcy.cheryme.top

Java: System.exit(1)
来源：http://vvu.yj20258.top

Go:   os.Exit(1)
来源：http://ftb.gotoacloud.top

Ruby: exit 1
来源：http://wno.cheryme.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kwi.xuanzx.com

[M06] 向标准错误输出
来源：http://jvr.yonumen.top

Py:   print("err", file=sys.stderr)
来源：http://aql.jlsjyb.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mao.hnqzz.top

JS:   console.error("err")
来源：http://eww.shanyushiyangkeji.top

TS:   console.error("err")
来源：http://lcw.zdbjq.cn

Java: System.err.println("err")
来源：http://pdz.wangdashe.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kws.xylfe.cn

Ruby: warn "err"
来源：http://aek.jqgufenzy.top

C#:   Console.Error.WriteLine("err")
来源：http://vsx.fehbvm.com

[M07] 判断是否为主入口
来源：http://kwi.hammf.cn

Py:   if __name__ == "__main__":
来源：http://wki.52xcode.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lje.smart0.xyz

JS:   require.main === module
来源：http://omw.bjfxy.top

TS:   require.main === module
来源：http://ljz.316326.xyz

Java: public static void main(String[] args)
来源：http://lft.bjfxy.top

Go:   func main()
来源：http://xoe.jyoumei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ntm.zhiwuduotai.top

C#:   static void Main(string[] args)
来源：http://gso.yj20258.top

[M08] 获取系统与运行时信息
来源：http://nxh.xuetiantiany.cn

Py:   platform.system();  platform.python_version()
来源：http://wew.jinqigufen.top

PHP:  PHP_OS;  phpversion();
来源：http://ttg.sjlbkw.cn

JS:   process.platform;  process.version
来源：http://urp.gogol.net.cn

TS:   process.platform;  process.version
来源：http://ojd.shangyingyoupin.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://okm.hnxiangtu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://jwz.yangfankeji.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sfi.jinqigufen.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://huh.cqqwz.cn

================================================================================
来源：http://elf.snrcjt.cn

N. 数据结构与算法
来源：http://szm.mhx1999.top

================================================================================
来源：http://hed.chenzaomai.com

[N01] 二分查找（有序数组）
来源：http://tiw.fktsv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://job.tian-w.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://utm.ctjpmb.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jfq.svipenyu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tib.zhixingplan.top

Java: Arrays.binarySearch(arr, x)
来源：http://xto.sjlbkw.cn

Go:   sort.SearchInts(arr, x)
来源：http://rqs.cucudq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jmp.fengsongda.top

C#:   Array.BinarySearch(arr, x)
来源：http://bim.xingfuxueyuan.xyz

[N02] 排序（工程实践用内置实现）
来源：http://zee.fzhhl.top

Py:   sorted(arr);  arr.sort()
来源：http://mim.quarkkingdee.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wnd.tanke756.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bfy.ehwqpu.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://moj.pycfn.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://suo.tanke756.top

Go:   slices.Sort(arr)
来源：http://asi.shuidangran.top

Ruby: arr.sort
来源：http://ldo.yfazqb.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://nvb.wangdashe.top

[N03] 快速排序（分治示例）
来源：http://wjf.xinyue.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tbn.jinghuilouyu.cn

PHP:  // 递归实现，或用 usort
来源：http://bvm.0kj1m.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lpo.shanyushiyangtech.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gxj.jinghuilouyu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bxy.cqqwz.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wls.hcnkem.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sux.yanxiufei.cn

C#:   // 手写递归，或 Array.Sort
来源：http://aix.snrcjt.cn

[N04] 斐波那契数列
来源：http://kib.ivvv.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://eyz.uphjek.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ihg.fktsv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://teq.jinqigfzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://opd.wangdashe.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://epl.tianlin.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tah.kuanghao11.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cvk.hesvh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pps.hysaishi.cn

[N05] 最大公约数
来源：http://sme.jinqigfzy.top

Py:   math.gcd(a, b)
来源：http://eyt.hywenlv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://egt.hnxiangtu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tso.chenlongwang.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jdb.hfpthk.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zdh.yuanzhike.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wvy.shuidangran.top

Ruby: a.gcd(b)
来源：http://faa.ydjk.org.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jlw.zhengqikj.top

[N06] 判断回文字符串
来源：http://kwj.zhiwuduotai.top

Py:   s == s[::-1]
来源：http://tgl.wangdashe.top

PHP:  $s === strrev($s);
来源：http://zea.mhx1999.top

JS:   s === [...s].reverse().join("")
来源：http://lup.yanxiufei.cn

TS:   s === [...s].reverse().join("")
来源：http://ptx.meibo888.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zuj.iojbl.cn

Go:   // 双指针从两端比较
来源：http://vpm.birdmap.top

Ruby: s == s.reverse
来源：http://mvt.52xcode.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lgg.nanxuanxn.top

[N07] 两数之和（返回下标）
来源：http://cum.yueranfly.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qaf.cdnleiting.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zon.jqgfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://thn.dianchejie.cn

TS:   // 手写 Map<string, number>
来源：http://fpk.jinqigfzy.top

Java: // 手写 HashMap
来源：http://dvq.nanxinkj.top

Go:   // 手写 map[int]int
来源：http://iov.gotoacloud.top

Ruby: // 手写 Hash
来源：http://qwz.xingfuxueyuan.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://cqt.jqgfzy.top

[N08] 生成全排列
来源：http://mve.hammf.cn

Py:   itertools.permutations(arr)
来源：http://ytf.quarkkingdee.top

PHP:  // 手写递归交换
来源：http://xfl.ydjk.org.cn

JS:   // 手写回溯递归
来源：http://cpy.fehbvm.com

TS:   // 手写回溯递归
来源：http://khq.fzhhl.top

Java: // 手写回溯递归
来源：http://vdu.jiagoushi.top

Go:   // 手写回溯递归
来源：http://wwx.haohaochexian.top

Ruby: arr.permutation.to_a
来源：http://atk.sxryk.cn

C#:   // 手写回溯递归
来源：http://kts.shzxlz.cn

[N09] 栈与队列
来源：http://acx.zhengqikj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uvx.jlsjyb.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qos.sufxvd.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wxr.ybcxt.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rwj.shuidangran.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://icg.fktsv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ymw.yj202588.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dwt.sjlbkw.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kgv.redwolf501.top

[N10] 链表节点定义
来源：http://rtp.yonumen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vjx.yueranfly.top

PHP:  class Node { public $v; public $next = null; }
来源：http://rlt.yongpay.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jhq.jlsjyb.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xac.xziqi.cn

Java: class Node { int v; Node next; }
来源：http://qdc.fktsv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bjc.sxryk.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ons.xingfuxueyuan.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://wpz.redwolf501.top

[N11] 二叉树中序遍历
来源：http://ewj.hnqzz.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://quj.nwbrower.top

PHP:  // 手写递归函数
来源：http://kjd.yuxming.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pnn.snrcjt.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://esu.havefunace.top

Java: // 手写递归
来源：http://rvw.nanxuanxn.top

Go:   // 手写递归
来源：http://nhi.epnwcf.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xye.jianghu66.top

C#:   // 手写递归
来源：http://nzd.cheryme.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bip.daria6918.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kyr.dashuyun.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ifq.zhijiandao.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pjz.c1oappe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zzb.yvedp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pip.cqqwz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qmb.wangshuangyany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nwa.yj202588.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xur.snrcjt.cn

================================================================================
来源：http://hio.jinyuanbaomall.cn

O. 并发与异步
来源：http://fca.svipenyu.cn

================================================================================
来源：http://lrw.wangdashe.top

[O01] 启动一个线程
来源：http://bkp.redwolf501.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vtc.pengpengdd.cyou

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zvm.jinqigufen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hwz.haohaochexian.top

TS:   // 同 JS
来源：http://gyk.ydzc1.top

Java: new Thread(() -> f()).start()
来源：http://ipx.c1oappe.top

Go:   go f()
来源：http://tdl.shanyushiyangkeji.top

Ruby: Thread.new { f }
来源：http://bwj.nanxinkj.top

C#:   Task.Run(() => F());
来源：http://skt.cashguo.top

[O02] 使用线程池
来源：http://yev.gaohongyu789.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://odp.meibo888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rfp.shanyushiyangtech.top

JS:   // worker_threads 线程池
来源：http://rxa.cucudq.cn

TS:   // worker_threads 线程池
来源：http://xow.jianghu66.top

Java: Executors.newFixedThreadPool(4)
来源：http://qkt.daria6918.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jhk.wangdashe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jbt.c1oappe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://crp.zhijiandao.cn

[O03] 加锁保护共享数据
来源：http://iqp.fehbvm.com

Py:   with lock: shared += 1
来源：http://wox.316326.xyz

PHP:  // 用 flock() 做文件锁
来源：http://pco.yuxming.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://chd.fehbvm.com

TS:   // 同 JS
来源：http://gvp.xuetiantiany.cn

Java: synchronized (this) { shared++; }
来源：http://ske.hongshengwenyu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lnt.gotoacloud.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ruf.mhx1999.top

C#:   lock (gate) { shared++; }
来源：http://bva.jinqigfzy.top

[O04] 定义异步函数并等待
来源：http://ngh.daxiang520.top

Py:   async def f():⏎    await g()
来源：http://otd.fehbvm.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://drh.sxryk.cn

JS:   async function f() { await g(); }
来源：http://esq.shanyushiyangtech.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://wtm.zhoulong.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jdd.tarul.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://who.ydzc1.top

Ruby: # 用 Fiber 或 async gem
来源：http://gkg.xziqi.cn

C#:   async Task F() { await G(); }
来源：http://ndk.zycfv.cn

[O05] 并发执行并等待全部完成
来源：http://egs.hcnkem.com

Py:   asyncio.gather(*tasks)
来源：http://juw.yj20258888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://den.shanyushiyangtech.top

JS:   await Promise.all(tasks)
来源：http://suo.iojbl.cn

TS:   await Promise.all(tasks)
来源：http://vtv.xingfuxueyuan.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zdo.xylfe.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xmm.jqgufenzy.top

Ruby: threads.map(&:join)
来源：http://gxu.sysykeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://rut.cheryme.top

[O06] 使用进程池
来源：http://bjp.epnwcf.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://aje.xziqi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rca.yonumen.top

JS:   // child_process / cluster 模块
来源：http://ift.zhixingplan.top

TS:   // child_process / cluster 模块
来源：http://uci.chenlongwang.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vmo.jinghuilouyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hrd.yj20258888.top

Ruby: // fork 块
来源：http://dyo.jinghuilouyu.cn

C#:   Parallel.For
来源：http://tfm.haohaochexian.top

================================================================================
来源：http://dze.epnwcf.com

P. 常用工具函数
来源：http://vna.hongshengwenyu.top

================================================================================
来源：http://veo.ppjwa.cn


<!-- 参考信息 -->
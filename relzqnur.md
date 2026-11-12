代发 wailian999

[L03] 设置自定义请求头
来源：http://syn.sxryk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dey.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://opi.andypj.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oou.yvedp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baf.cashguo.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rif.hnqzz.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xmo.jinghuilouyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wjx.hcnkem.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rgk.cheryme.top

[L04] 设置超时
来源：http://mqs.yj20258888.top

Py:   requests.get(url, timeout=5)
来源：http://ozl.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zgt.jiagoushi.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://idu.svipenyu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xsl.zdbjq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wdy.nwbrower.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://glz.nanxinkj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lyy.xuanzx.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qcc.cdnleiting.top

[L05] 上传文件（multipart）
来源：http://djo.redwolf501.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hxy.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vdm.yvedp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hgv.vqdsnc.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vcw.guannengcc.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hoh.sxryk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://klf.zdqjudy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://znq.jlsjyb.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ygv.zhaomingkeji.xyz

[L06] 解析响应为 JSON
来源：http://eol.zhijiandao.cn

Py:   resp.json()
来源：http://rsd.fzhhl.top

PHP:  json_decode($body, true);
来源：http://wke.hesvh.cn

JS:   await resp.json()
来源：http://ocl.9152youxi.cn

TS:   await resp.json()
来源：http://dey.ydjk.org.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kqv.tian-w.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ugv.guowangkeji.top

Ruby: JSON.parse(resp.body)
来源：http://vec.9152youxi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fsu.ywan-chungtsiang.top

[L07] 处理 HTTP 状态码
来源：http://nph.mhx1999.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qra.sxryk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wql.chenzaomai.com

JS:   resp.ok;  resp.status
来源：http://nzu.vqdsnc.cn

TS:   resp.ok;  resp.status
来源：http://ysu.svipenyu.cn

Java: resp.statusCode()
来源：http://amf.kuanghao11.cn

Go:   resp.StatusCode
来源：http://zbv.xingfuxueyuan.xyz

Ruby: resp.code.to_i
来源：http://ery.redwolf501.top

C#:   (int)resp.StatusCode
来源：http://abn.pycfn.com

[L08] 并发请求多个地址
来源：http://qec.yfazqb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zen.hongshengwenyu.top

PHP:  curl_multi_init() 系列
来源：http://jko.xylfe.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fpw.tarul.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ino.nanxinkj.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://aqr.cheryme.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fis.ppjwa.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sux.andypj.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qxq.cqqwz.cn

================================================================================
来源：http://can.gogol.net.cn

M. 命令行 / 进程 / 环境
来源：http://nui.sjlbkw.cn

================================================================================
来源：http://mni.hcnkem.com

[M01] 读取命令行参数
来源：http://dwd.tanke756.top

Py:   sys.argv[1:]
来源：http://pub.birdmap.top

PHP:  $argv;  $argc;
来源：http://hal.hesvh.cn

JS:   process.argv.slice(2)
来源：http://kki.zycfv.cn

TS:   process.argv.slice(2)
来源：http://dio.yvedp.cn

Java: args 数组（main 方法参数）
来源：http://gje.nanxuanxn.top

Go:   os.Args[1:]
来源：http://fpe.hammf.cn

Ruby: ARGV
来源：http://xmq.zhijiandao.cn

C#:   args 数组（Main 方法参数）
来源：http://chc.ctjpmb.com

[M02] 读取环境变量
来源：http://piy.xingfuxueyuan.xyz

Py:   os.environ.get("HOME")
来源：http://rkb.chenlongwang.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hzd.vqdsnc.cn

JS:   process.env.HOME
来源：http://bmq.pengpengdd.cyou

TS:   process.env.HOME
来源：http://jrh.ydjk.org.cn

Java: System.getenv("HOME")
来源：http://hlw.hysaishi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mnp.tarul.cn

Ruby: ENV["HOME"]
来源：http://ipf.zhengqikj.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rmc.meibo888.top

[M03] 执行外部命令
来源：http://vhg.hnxiangtu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://scn.fzhhl.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ibs.zycfv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jgv.smart0.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://egf.guannengcc.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xrk.zdqjudy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ipf.dianchejie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fvu.zdbjq.cn

C#:   Process.Start("ls", "-l");
来源：http://lav.sysykeji.top

[M04] 获取当前工作目录
来源：http://zuj.tarul.cn

Py:   os.getcwd()
来源：http://sfl.shangyingyoupin.top

PHP:  getcwd();
来源：http://qni.fzhhl.top

JS:   process.cwd()
来源：http://bzs.yuanzhike.top

TS:   process.cwd()
来源：http://gmk.daxiang520.top

Java: Path.of("").toAbsolutePath()
来源：http://dgn.kuanghao11.cn

Go:   os.Getwd()
来源：http://dwh.chenzaomai.com

Ruby: Dir.pwd
来源：http://wwb.xinyue.icu

C#:   Directory.GetCurrentDirectory()
来源：http://eyw.gogol.net.cn

[M05] 设置退出码
来源：http://hvu.bjfxy.top

Py:   sys.exit(1)
来源：http://tmj.andypj.xyz

PHP:  exit(1);
来源：http://jps.chenjidiqi.icu

JS:   process.exit(1)
来源：http://kjy.yanxiufei.cn

TS:   process.exit(1)
来源：http://pvr.iojbl.cn

Java: System.exit(1)
来源：http://uai.yuanzhike.top

Go:   os.Exit(1)
来源：http://zkn.wangdashe.top

Ruby: exit 1
来源：http://jtz.xylfe.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qei.yj20258.top

[M06] 向标准错误输出
来源：http://jes.yj202588.top

Py:   print("err", file=sys.stderr)
来源：http://pjr.zhoulong.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://ger.yongpay.top

JS:   console.error("err")
来源：http://lsn.ehwqpu.com

TS:   console.error("err")
来源：http://aqq.shanyushiyangtech.top

Java: System.err.println("err")
来源：http://guj.zdbjq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qni.quarkkingdee.top

Ruby: warn "err"
来源：http://kne.gogol.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://den.feifeiyinyue.top

[M07] 判断是否为主入口
来源：http://ygz.sweek.top

Py:   if __name__ == "__main__":
来源：http://agn.jlsjyb.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uaa.jlsjyb.cn

JS:   require.main === module
来源：http://cve.jyoumei.cn

TS:   require.main === module
来源：http://tfp.ydzc1.top

Java: public static void main(String[] args)
来源：http://haq.ehwqpu.com

Go:   func main()
来源：http://rib.haohaochexian.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vyv.gaohongyu789.top

C#:   static void Main(string[] args)
来源：http://yqg.uphjek.com

[M08] 获取系统与运行时信息
来源：http://ylb.yj20258888.top

Py:   platform.system();  platform.python_version()
来源：http://gpo.sweek.top

PHP:  PHP_OS;  phpversion();
来源：http://mbx.chenzaomai.com

JS:   process.platform;  process.version
来源：http://pdb.zhoulong.xyz

TS:   process.platform;  process.version
来源：http://ujj.xuanzx.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bpu.sxryk.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mzq.gogol.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cty.cdnleiting.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wlj.bjfxy.top

================================================================================
来源：http://qfc.andypj.xyz

N. 数据结构与算法
来源：http://ffk.smart0.xyz

================================================================================
来源：http://ubi.yuxming.cn

[N01] 二分查找（有序数组）
来源：http://swe.zhijiandao.cn

Py:   bisect.bisect_left(arr, x)
来源：http://exp.hcnkem.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://idb.316326.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qpa.nwbrower.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fus.haohaochexian.top

Java: Arrays.binarySearch(arr, x)
来源：http://tmu.jqgfzy.top

Go:   sort.SearchInts(arr, x)
来源：http://rhw.nanxuanxn.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://fef.gzhubu.top

C#:   Array.BinarySearch(arr, x)
来源：http://xae.jqgfzy.top

[N02] 排序（工程实践用内置实现）
来源：http://rbu.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://jmm.cdnleiting.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tlu.xziqi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pwf.pengpengdd.cyou

TS:   [...arr].sort((a, b) => a - b)
来源：http://iip.iojbl.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bgx.yonumen.top

Go:   slices.Sort(arr)
来源：http://bmr.cheryme.top

Ruby: arr.sort
来源：http://mxb.yuxming.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ujl.jyoumei.cn

[N03] 快速排序（分治示例）
来源：http://one.c1oappe.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ira.dianchejie.cn

PHP:  // 递归实现，或用 usort
来源：http://beq.zycfv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qnu.zhijiandao.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jdo.ywan-chungtsiang.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gbj.yj20258888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kgr.yj20258.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pap.pycfn.com

C#:   // 手写递归，或 Array.Sort
来源：http://tvq.redwolf501.top

[N04] 斐波那契数列
来源：http://spa.chenjidiqi.icu

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cho.ppjwa.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rqq.zhoulong.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://drn.wangdashe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://leo.nanxuanxn.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xgl.yj20258888.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://aln.yj202588.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://amq.shangyingyoupin.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dwn.yuanzhike.top

[N05] 最大公约数
来源：http://veb.hysaishi.cn

Py:   math.gcd(a, b)
来源：http://ohm.pengpengdd.cyou

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://aep.haohaochexian.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xrc.chenzaomai.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mla.sweek.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ost.fanxiaobao.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jru.jinghuilouyu.cn

Ruby: a.gcd(b)
来源：http://vfa.gaohongyu789.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zzm.vehdjk.com

[N06] 判断回文字符串
来源：http://wlb.zdbjq.cn

Py:   s == s[::-1]
来源：http://hdr.nwbrower.top

PHP:  $s === strrev($s);
来源：http://ufs.yj20258888.top

JS:   s === [...s].reverse().join("")
来源：http://cmg.zhongyouzk.top

TS:   s === [...s].reverse().join("")
来源：http://grj.chenlongwang.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tbr.yonumen.top

Go:   // 双指针从两端比较
来源：http://uyu.jqgufenzy.top

Ruby: s == s.reverse
来源：http://ytr.cdnleiting.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://btx.jyoumei.cn

[N07] 两数之和（返回下标）
来源：http://lcy.shzxlz.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uad.uphjek.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bpo.tanke756.top

JS:   // 手写 Map：map.set(v, i)
来源：http://loe.fzhhl.top

TS:   // 手写 Map<string, number>
来源：http://gpt.tanke756.top

Java: // 手写 HashMap
来源：http://mde.ehwqpu.com

Go:   // 手写 map[int]int
来源：http://gyc.shanyushiyangkeji.top

Ruby: // 手写 Hash
来源：http://vig.cheryme.top

C#:   // 手写 Dictionary<int, int>
来源：http://vcd.cdnleiting.top

[N08] 生成全排列
来源：http://tbz.ydzc1.top

Py:   itertools.permutations(arr)
来源：http://mof.yanxiufei.cn

PHP:  // 手写递归交换
来源：http://iif.jyoumei.cn

JS:   // 手写回溯递归
来源：http://wlm.birdmap.top

TS:   // 手写回溯递归
来源：http://wjd.meibo888.top

Java: // 手写回溯递归
来源：http://ekf.wangdashe.top

Go:   // 手写回溯递归
来源：http://lge.wangshuangyany.cn

Ruby: arr.permutation.to_a
来源：http://erj.uphjek.com

C#:   // 手写回溯递归
来源：http://ozt.feifeiyinyue.top

[N09] 栈与队列
来源：http://ors.vqdsnc.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wnp.9152youxi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zrm.yj20258.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ozh.dianchejie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ehh.snrcjt.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oro.shanyushiyangtech.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oce.hesvh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ctl.jinqigfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qka.tarul.cn

[N10] 链表节点定义
来源：http://vsn.meibo888.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rjg.birdmap.top

PHP:  class Node { public $v; public $next = null; }
来源：http://iex.fktsv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cwh.kuanghao11.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fuk.zhaomingkeji.xyz

Java: class Node { int v; Node next; }
来源：http://isx.yj20258888.top

Go:   type Node struct { V int; Next *Node }
来源：http://fvq.gogol.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://arh.hongshengwenyu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://trb.dashuyun.cn

[N11] 二叉树中序遍历
来源：http://ayk.hysaishi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xdw.jqgfzy.top

PHP:  // 手写递归函数
来源：http://zjo.yangfankeji.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eqa.fzhhl.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eju.haohaochexian.top

Java: // 手写递归
来源：http://ukg.hysaishi.cn

Go:   // 手写递归
来源：http://umw.hammf.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hhc.vqdsnc.cn

C#:   // 手写递归
来源：http://ugj.shuidangran.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ifl.jlsjyb.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://eqq.guannengcc.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jiy.tianlin.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rvq.jinqigufen.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zdj.jlsjyb.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kts.kuanghao11.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://std.smart0.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qcr.cheryme.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jxn.xingfuxueyuan.xyz

================================================================================
来源：http://vfx.hywenlv.cn

O. 并发与异步
来源：http://skc.0kj1m.cn

================================================================================
来源：http://grb.sweek.top

[O01] 启动一个线程
来源：http://rwf.jqgfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rsv.jinqigufen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jce.fzhhl.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kdw.ybcxt.top

TS:   // 同 JS
来源：http://fcr.dashuyun.cn

Java: new Thread(() -> f()).start()
来源：http://jqb.hongshengwenyu.top

Go:   go f()
来源：http://vmi.yongpay.top

Ruby: Thread.new { f }
来源：http://ejw.ppjwa.cn

C#:   Task.Run(() => F());
来源：http://dpy.yj20258.top

[O02] 使用线程池
来源：http://cdm.haohaochexian.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lvv.yvedp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lan.zhijiandao.cn

JS:   // worker_threads 线程池
来源：http://lvb.hfpthk.cn

TS:   // worker_threads 线程池
来源：http://clw.zhoulong.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://vpi.hongshengwenyu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ako.sufxvd.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kcb.tianlin.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bpe.epnwcf.com

[O03] 加锁保护共享数据
来源：http://xhy.zhixingplan.top

Py:   with lock: shared += 1
来源：http://pyc.jinqigufen.top

PHP:  // 用 flock() 做文件锁
来源：http://ljp.xuetiantiany.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://oqq.hammf.cn

TS:   // 同 JS
来源：http://wxn.yangfankeji.com

Java: synchronized (this) { shared++; }
来源：http://myu.uphjek.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rwt.gzhubu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://cly.xuetiantiany.cn

C#:   lock (gate) { shared++; }
来源：http://vaz.daria6918.cn

[O04] 定义异步函数并等待
来源：http://yqv.hywenlv.cn

Py:   async def f():⏎    await g()
来源：http://xkv.wangdashe.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gij.chenlongwang.top

JS:   async function f() { await g(); }
来源：http://wwg.kuanghao11.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jox.xylfe.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ycu.nwbrower.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://put.ivvv.top

Ruby: # 用 Fiber 或 async gem
来源：http://afs.hammf.cn

C#:   async Task F() { await G(); }
来源：http://zqw.havefunace.top

[O05] 并发执行并等待全部完成
来源：http://dvp.cucudq.cn

Py:   asyncio.gather(*tasks)
来源：http://fio.fehbvm.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dvg.yonumen.top

JS:   await Promise.all(tasks)
来源：http://ynh.xylfe.cn

TS:   await Promise.all(tasks)
来源：http://hbb.jinyuanbaomall.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bpv.ivvv.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://voi.yanxiufei.cn

Ruby: threads.map(&:join)
来源：http://ivt.ivvv.top

C#:   await Task.WhenAll(t1, t2)
来源：http://itu.bbcook.cn

[O06] 使用进程池
来源：http://nvh.shangyingyoupin.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rib.9152youxi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fug.shzxlz.cn

JS:   // child_process / cluster 模块
来源：http://qge.hywenlv.cn

TS:   // child_process / cluster 模块
来源：http://ybs.ydjk.org.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gfw.gzhubu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ecl.cqqwz.cn

Ruby: // fork 块
来源：http://ydn.chenlongwang.top

C#:   Parallel.For
来源：http://vnd.chenzaomai.com

================================================================================
来源：http://oct.jlsjyb.cn

P. 常用工具函数
来源：http://ssz.bjfxy.top

================================================================================
来源：http://jyu.sxryk.cn


<!-- 参考信息 -->
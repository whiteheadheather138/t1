代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zek.aizwys.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dta.shanyushiyangtech.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dmt.feifeiyinyue.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ydo.yj20258888.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tsn.yuanzhike.top

[L04] 设置超时
来源：http://jan.gzhubu.top

Py:   requests.get(url, timeout=5)
来源：http://wgn.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zqs.wangshuangyany.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://feh.feifeiyinyue.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://afh.shzxlz.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://odr.zycfv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pgk.cashguo.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://njl.hnqzz.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dmt.yueranfly.top

[L05] 上传文件（multipart）
来源：http://gez.ywan-chungtsiang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gsl.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zfn.ywan-chungtsiang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ywl.guannengcc.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rda.hammf.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yqo.yanxiufei.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bzp.yj20258.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://aln.redwolf501.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zvn.9152youxi.cn

[L06] 解析响应为 JSON
来源：http://slt.jyoumei.cn

Py:   resp.json()
来源：http://tqt.guannengcc.top

PHP:  json_decode($body, true);
来源：http://jpw.sjlbkw.cn

JS:   await resp.json()
来源：http://ffk.ehwqpu.com

TS:   await resp.json()
来源：http://nxe.meibo888.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yxm.tanke756.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zow.yj202588.top

Ruby: JSON.parse(resp.body)
来源：http://qoj.guannengcc.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jso.dashuyun.cn

[L07] 处理 HTTP 状态码
来源：http://izr.jyoumei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rqx.yuxming.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uqa.vqdsnc.cn

JS:   resp.ok;  resp.status
来源：http://apx.sysykeji.top

TS:   resp.ok;  resp.status
来源：http://nma.wangshuangyany.cn

Java: resp.statusCode()
来源：http://rgg.sjlbkw.cn

Go:   resp.StatusCode
来源：http://glh.yfazqb.com

Ruby: resp.code.to_i
来源：http://dye.sxryk.cn

C#:   (int)resp.StatusCode
来源：http://jsf.ydzc1.top

[L08] 并发请求多个地址
来源：http://dvo.fengsongda.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lmz.hesvh.cn

PHP:  curl_multi_init() 系列
来源：http://lrc.tanke756.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wdh.ehwqpu.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tza.hcnkem.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://knq.chenzaomai.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cjq.nwbrower.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cpf.cqqwz.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nko.cashguo.top

================================================================================
来源：http://soj.yonumen.top

M. 命令行 / 进程 / 环境
来源：http://tph.cashguo.top

================================================================================
来源：http://led.ywan-chungtsiang.top

[M01] 读取命令行参数
来源：http://fto.birdmap.top

Py:   sys.argv[1:]
来源：http://qza.shzxlz.cn

PHP:  $argv;  $argc;
来源：http://vyn.vehdjk.com

JS:   process.argv.slice(2)
来源：http://dju.jinghuilouyu.cn

TS:   process.argv.slice(2)
来源：http://qne.yvedp.cn

Java: args 数组（main 方法参数）
来源：http://yko.jinghuilouyu.cn

Go:   os.Args[1:]
来源：http://miy.haohaochexian.top

Ruby: ARGV
来源：http://dgf.yuxming.cn

C#:   args 数组（Main 方法参数）
来源：http://jxj.kuanghao11.cn

[M02] 读取环境变量
来源：http://pkp.tarul.cn

Py:   os.environ.get("HOME")
来源：http://qwl.jinghuilouyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mvk.jianghu66.top

JS:   process.env.HOME
来源：http://xxh.c1oappe.top

TS:   process.env.HOME
来源：http://kzd.pycfn.com

Java: System.getenv("HOME")
来源：http://ldq.gogol.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tvf.jqgufenzy.top

Ruby: ENV["HOME"]
来源：http://zpf.vehdjk.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://obf.zhiwuduotai.top

[M03] 执行外部命令
来源：http://uif.nanxuanxn.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://plg.vqdsnc.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nfp.xinyue.icu

JS:   child_process.execSync("ls -l").toString()
来源：http://ifp.sxryk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cla.svipenyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sqs.gogol.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rym.zhiwuduotai.top

Ruby: system("ls -l");  `ls -l`
来源：http://oan.yonumen.top

C#:   Process.Start("ls", "-l");
来源：http://guq.ybcxt.top

[M04] 获取当前工作目录
来源：http://qgy.kuanghao11.cn

Py:   os.getcwd()
来源：http://gcb.smart0.xyz

PHP:  getcwd();
来源：http://zmc.yonumen.top

JS:   process.cwd()
来源：http://nzb.9152youxi.cn

TS:   process.cwd()
来源：http://hnz.yj20258888.top

Java: Path.of("").toAbsolutePath()
来源：http://jet.jiagoushi.top

Go:   os.Getwd()
来源：http://vyd.hongshengwenyu.top

Ruby: Dir.pwd
来源：http://adj.jinghuilouyu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gvh.havefunace.top

[M05] 设置退出码
来源：http://kqu.ywan-chungtsiang.top

Py:   sys.exit(1)
来源：http://zvv.sxryk.cn

PHP:  exit(1);
来源：http://nfq.xylfe.cn

JS:   process.exit(1)
来源：http://pea.jinyuanbaomall.cn

TS:   process.exit(1)
来源：http://ynz.aizwys.cn

Java: System.exit(1)
来源：http://cks.yj20258888.top

Go:   os.Exit(1)
来源：http://jdg.zhaomingkeji.xyz

Ruby: exit 1
来源：http://zxf.zhixingplan.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cna.zhengqikj.top

[M06] 向标准错误输出
来源：http://awt.hammf.cn

Py:   print("err", file=sys.stderr)
来源：http://fza.hnxiangtu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://kag.fanxiaobao.xyz

JS:   console.error("err")
来源：http://qem.fktsv.cn

TS:   console.error("err")
来源：http://rqy.hfpthk.cn

Java: System.err.println("err")
来源：http://uro.zhixingplan.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gad.mhx1999.top

Ruby: warn "err"
来源：http://hit.hongshengwenyu.top

C#:   Console.Error.WriteLine("err")
来源：http://fif.gaohongyu789.top

[M07] 判断是否为主入口
来源：http://cga.fktsv.cn

Py:   if __name__ == "__main__":
来源：http://mmv.sjlbkw.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rbv.wangshuangyany.cn

JS:   require.main === module
来源：http://rwv.feifeiyinyue.top

TS:   require.main === module
来源：http://ity.zycfv.cn

Java: public static void main(String[] args)
来源：http://kea.wangshuangyany.cn

Go:   func main()
来源：http://jmo.kuanghao11.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fyn.nanxinkj.top

C#:   static void Main(string[] args)
来源：http://vat.sxryk.cn

[M08] 获取系统与运行时信息
来源：http://xid.yfazqb.com

Py:   platform.system();  platform.python_version()
来源：http://uso.jinqigufen.top

PHP:  PHP_OS;  phpversion();
来源：http://ani.jianghu66.top

JS:   process.platform;  process.version
来源：http://wch.nanxinkj.top

TS:   process.platform;  process.version
来源：http://uei.nanxinkj.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zpj.zycfv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://slr.ywan-chungtsiang.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ryv.dashuyun.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jtq.pengpengdd.cyou

================================================================================
来源：http://xnv.gogol.net.cn

N. 数据结构与算法
来源：http://cou.gaohongyu789.top

================================================================================
来源：http://twm.fengsongda.top

[N01] 二分查找（有序数组）
来源：http://exa.sweek.top

Py:   bisect.bisect_left(arr, x)
来源：http://yqa.yj20258888.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pbq.hywenlv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://njl.yfazqb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hbi.cashguo.top

Java: Arrays.binarySearch(arr, x)
来源：http://rjz.wangdashe.top

Go:   sort.SearchInts(arr, x)
来源：http://cws.hongshengwenyu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://gpn.fanxiaobao.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://kgg.shangyingyoupin.top

[N02] 排序（工程实践用内置实现）
来源：http://aid.316326.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ndb.wangshuangyany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://woq.dashuyun.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hyl.chenjidiqi.icu

TS:   [...arr].sort((a, b) => a - b)
来源：http://wbu.guowangkeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://moi.dashuyun.cn

Go:   slices.Sort(arr)
来源：http://qfx.zhoulong.xyz

Ruby: arr.sort
来源：http://mff.0kj1m.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://faa.fehbvm.com

[N03] 快速排序（分治示例）
来源：http://kcm.xuetiantiany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://guo.epnwcf.com

PHP:  // 递归实现，或用 usort
来源：http://vhs.pengpengdd.cyou

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wps.cucudq.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zjl.aizwys.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wrl.gogol.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yqn.redwolf501.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ivs.cashguo.top

C#:   // 手写递归，或 Array.Sort
来源：http://era.iojbl.cn

[N04] 斐波那契数列
来源：http://prf.havefunace.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nfh.chenzaomai.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://czp.birdmap.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cob.quarkkingdee.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ptt.ehwqpu.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pkd.nwbrower.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gdl.daxiang520.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lis.fehbvm.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wme.zhijiandao.cn

[N05] 最大公约数
来源：http://ejk.xylfe.cn

Py:   math.gcd(a, b)
来源：http://ipq.jianghu66.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://apt.ybcxt.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rnw.nanxinkj.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tor.yj20258888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pgv.zhengqikj.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://npe.sxryk.cn

Ruby: a.gcd(b)
来源：http://bdk.yanxiufei.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blt.smart0.xyz

[N06] 判断回文字符串
来源：http://ovr.shuidangran.top

Py:   s == s[::-1]
来源：http://mre.quarkkingdee.top

PHP:  $s === strrev($s);
来源：http://uso.sweek.top

JS:   s === [...s].reverse().join("")
来源：http://ung.kuanghao11.cn

TS:   s === [...s].reverse().join("")
来源：http://mub.tianlin.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ipc.birdmap.top

Go:   // 双指针从两端比较
来源：http://ukw.jinyuanbaomall.cn

Ruby: s == s.reverse
来源：http://zxl.xziqi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nvn.chenjidiqi.icu

[N07] 两数之和（返回下标）
来源：http://ezp.chenlongwang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xxu.zdqjudy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pxm.shanyushiyangkeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://kwy.tianlin.xyz

TS:   // 手写 Map<string, number>
来源：http://vfs.hammf.cn

Java: // 手写 HashMap
来源：http://hxf.zdqjudy.top

Go:   // 手写 map[int]int
来源：http://tnu.jiagoushi.top

Ruby: // 手写 Hash
来源：http://stq.cdnleiting.top

C#:   // 手写 Dictionary<int, int>
来源：http://hpd.zhiwuduotai.top

[N08] 生成全排列
来源：http://lgg.cucudq.cn

Py:   itertools.permutations(arr)
来源：http://ldq.xylfe.cn

PHP:  // 手写递归交换
来源：http://izk.wangdashe.top

JS:   // 手写回溯递归
来源：http://iwa.zhoulong.xyz

TS:   // 手写回溯递归
来源：http://lji.cashguo.top

Java: // 手写回溯递归
来源：http://fyn.bbcook.cn

Go:   // 手写回溯递归
来源：http://wns.hnqzz.top

Ruby: arr.permutation.to_a
来源：http://iea.hfpthk.cn

C#:   // 手写回溯递归
来源：http://koc.xinyue.icu

[N09] 栈与队列
来源：http://yga.daxiang520.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lix.vehdjk.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dvu.ybcxt.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qou.andypj.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nwc.xingfuxueyuan.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tqs.ybcxt.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hhh.havefunace.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://top.tianlin.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://icc.tianlin.xyz

[N10] 链表节点定义
来源：http://ubx.dashuyun.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ftd.pycfn.com

PHP:  class Node { public $v; public $next = null; }
来源：http://asv.zhijiandao.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://csj.iojbl.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ogf.yuanzhike.top

Java: class Node { int v; Node next; }
来源：http://wrd.cdnleiting.top

Go:   type Node struct { V int; Next *Node }
来源：http://ijz.cdnleiting.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ztq.yuanzhike.top

C#:   class Node { public int V; public Node? Next; }
来源：http://slw.zdbjq.cn

[N11] 二叉树中序遍历
来源：http://qgz.gogol.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://umr.hongshengwenyu.top

PHP:  // 手写递归函数
来源：http://ivg.chenlongwang.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xtu.shzxlz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pjw.tanke756.top

Java: // 手写递归
来源：http://cuw.yangfankeji.com

Go:   // 手写递归
来源：http://tod.bjfxy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qmk.svipenyu.cn

C#:   // 手写递归
来源：http://ctl.ehwqpu.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://iun.birdmap.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ehr.tianlin.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ywr.sysykeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jug.yj20258.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vzz.uphjek.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nxq.gotoacloud.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bof.wangdashe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qzx.chenzaomai.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://orc.aibaodan.cn

================================================================================
来源：http://msa.uphjek.com

O. 并发与异步
来源：http://zcx.epnwcf.com

================================================================================
来源：http://ghg.ydjk.org.cn

[O01] 启动一个线程
来源：http://cye.sweek.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gzh.meibo888.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ykc.jinghuilouyu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://txe.jianghu66.top

TS:   // 同 JS
来源：http://awr.jqgfzy.top

Java: new Thread(() -> f()).start()
来源：http://vqw.andypj.xyz

Go:   go f()
来源：http://acf.guannengcc.top

Ruby: Thread.new { f }
来源：http://bti.snrcjt.cn

C#:   Task.Run(() => F());
来源：http://aru.dashuyun.cn

[O02] 使用线程池
来源：http://xvs.kuanghao11.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://why.hysaishi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://edm.cqqwz.cn

JS:   // worker_threads 线程池
来源：http://scq.zhiwuduotai.top

TS:   // worker_threads 线程池
来源：http://rng.meibo888.top

Java: Executors.newFixedThreadPool(4)
来源：http://aui.havefunace.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bxu.tanke756.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zje.meibo888.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gmt.sjlbkw.cn

[O03] 加锁保护共享数据
来源：http://vmb.birdmap.top

Py:   with lock: shared += 1
来源：http://zjj.xziqi.cn

PHP:  // 用 flock() 做文件锁
来源：http://lxm.cqqwz.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eca.yanxiufei.cn

TS:   // 同 JS
来源：http://fgu.daxiang520.top

Java: synchronized (this) { shared++; }
来源：http://ddo.yvedp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://drq.yuanzhike.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ofq.nanxinkj.top

C#:   lock (gate) { shared++; }
来源：http://cul.fzhhl.top

[O04] 定义异步函数并等待
来源：http://hfx.tarul.cn

Py:   async def f():⏎    await g()
来源：http://fmi.aibaodan.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ptg.wangshuangyany.cn

JS:   async function f() { await g(); }
来源：http://fdd.redwolf501.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://hdv.shangyingyoupin.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ktz.bjfxy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sfw.andypj.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://yjq.wangshuangyany.cn

C#:   async Task F() { await G(); }
来源：http://wqj.yueranfly.top

[O05] 并发执行并等待全部完成
来源：http://loj.haohaochexian.top

Py:   asyncio.gather(*tasks)
来源：http://nwc.shzxlz.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xvw.yanxiufei.cn

JS:   await Promise.all(tasks)
来源：http://flm.316326.xyz

TS:   await Promise.all(tasks)
来源：http://tim.gogol.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fhk.jinqigufen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qww.fktsv.cn

Ruby: threads.map(&:join)
来源：http://xzd.pycfn.com

C#:   await Task.WhenAll(t1, t2)
来源：http://opp.vqdsnc.cn

[O06] 使用进程池
来源：http://qcp.ydzc1.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gcr.tarul.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yho.dashuyun.cn

JS:   // child_process / cluster 模块
来源：http://ptc.sweek.top

TS:   // child_process / cluster 模块
来源：http://ycl.nwbrower.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wau.sufxvd.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hda.hesvh.cn

Ruby: // fork 块
来源：http://nxi.ehwqpu.com

C#:   Parallel.For
来源：http://mhp.zhongyouzk.top

================================================================================
来源：http://dbk.shanyushiyangkeji.top

P. 常用工具函数
来源：http://ctn.aizwys.cn

================================================================================
来源：http://cmq.sxryk.cn

[P01] 生成 UUID
来源：http://uyi.yueranfly.top

Py:   str(uuid.uuid4())
来源：http://gap.hammf.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zmy.jyoumei.cn

JS:   crypto.randomUUID()
来源：http://unz.fzhhl.top


<!-- 参考信息 -->
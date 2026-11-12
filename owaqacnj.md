代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nyx.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://iwf.wangdashe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wno.zdqjudy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gav.zycfv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://prc.cqqwz.cn

[L04] 设置超时
来源：http://vip.xingfuxueyuan.xyz

Py:   requests.get(url, timeout=5)
来源：http://vnb.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://eno.shanyushiyangtech.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dib.hywenlv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nzj.tanke756.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yxp.shanyushiyangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rds.zdqjudy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kgz.ivvv.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xgw.yuanzhike.top

[L05] 上传文件（multipart）
来源：http://aay.fehbvm.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vsl.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jef.cdnleiting.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dsi.birdmap.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://smd.havefunace.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://svq.cdnleiting.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tnk.jinqigfzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cfm.xylfe.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vpf.cdnleiting.top

[L06] 解析响应为 JSON
来源：http://ggg.nanxinkj.top

Py:   resp.json()
来源：http://aeu.0kj1m.cn

PHP:  json_decode($body, true);
来源：http://qkx.ppjwa.cn

JS:   await resp.json()
来源：http://uae.zycfv.cn

TS:   await resp.json()
来源：http://dqc.snrcjt.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tdr.mhx1999.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://atj.yfazqb.com

Ruby: JSON.parse(resp.body)
来源：http://ixd.yj20258888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cil.hcnkem.com

[L07] 处理 HTTP 状态码
来源：http://rra.jinghuilouyu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://axn.jqgfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gzm.smart0.xyz

JS:   resp.ok;  resp.status
来源：http://bxl.nanxuanxn.top

TS:   resp.ok;  resp.status
来源：http://cov.yonumen.top

Java: resp.statusCode()
来源：http://eoc.hcnkem.com

Go:   resp.StatusCode
来源：http://mra.0kj1m.cn

Ruby: resp.code.to_i
来源：http://czt.gotoacloud.top

C#:   (int)resp.StatusCode
来源：http://els.zdqjudy.top

[L08] 并发请求多个地址
来源：http://jwq.feifeiyinyue.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dka.vqdsnc.cn

PHP:  curl_multi_init() 系列
来源：http://avg.hcnkem.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mjn.jinqigufen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iru.yangfankeji.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gks.feifeiyinyue.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gta.sweek.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fot.shangyingyoupin.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nrk.quarkkingdee.top

================================================================================
来源：http://sne.chenzaomai.com

M. 命令行 / 进程 / 环境
来源：http://juf.ctjpmb.com

================================================================================
来源：http://jaa.jinqigfzy.top

[M01] 读取命令行参数
来源：http://ron.jyoumei.cn

Py:   sys.argv[1:]
来源：http://rqu.9152youxi.cn

PHP:  $argv;  $argc;
来源：http://gfq.jinqigfzy.top

JS:   process.argv.slice(2)
来源：http://ooz.quarkkingdee.top

TS:   process.argv.slice(2)
来源：http://hxl.shanyushiyangtech.top

Java: args 数组（main 方法参数）
来源：http://qks.vehdjk.com

Go:   os.Args[1:]
来源：http://ixs.jlsjyb.cn

Ruby: ARGV
来源：http://gxf.chenlongwang.top

C#:   args 数组（Main 方法参数）
来源：http://duo.havefunace.top

[M02] 读取环境变量
来源：http://krh.jinqigufen.top

Py:   os.environ.get("HOME")
来源：http://tui.hesvh.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nkv.hesvh.cn

JS:   process.env.HOME
来源：http://hvz.chenjidiqi.icu

TS:   process.env.HOME
来源：http://snj.sufxvd.cn

Java: System.getenv("HOME")
来源：http://ixl.hnqzz.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zbf.birdmap.top

Ruby: ENV["HOME"]
来源：http://pfi.hnxiangtu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://otq.zhijiandao.cn

[M03] 执行外部命令
来源：http://tsi.sxryk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gmy.jqgufenzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yep.tanke756.top

JS:   child_process.execSync("ls -l").toString()
来源：http://izr.fehbvm.com

TS:   child_process.execSync("ls -l").toString()
来源：http://pxp.jinghuilouyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jyh.jinqigfzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://upp.zhiwuduotai.top

Ruby: system("ls -l");  `ls -l`
来源：http://fiz.andypj.xyz

C#:   Process.Start("ls", "-l");
来源：http://tky.0kj1m.cn

[M04] 获取当前工作目录
来源：http://lac.redwolf501.top

Py:   os.getcwd()
来源：http://eeh.dianchejie.cn

PHP:  getcwd();
来源：http://cvy.ywan-chungtsiang.top

JS:   process.cwd()
来源：http://bwl.guannengcc.top

TS:   process.cwd()
来源：http://fzp.bjfxy.top

Java: Path.of("").toAbsolutePath()
来源：http://ymu.zdqjudy.top

Go:   os.Getwd()
来源：http://dwh.shanyushiyangtech.top

Ruby: Dir.pwd
来源：http://iuo.zhoulong.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://ywy.jinqigufen.top

[M05] 设置退出码
来源：http://gsy.jinghuilouyu.cn

Py:   sys.exit(1)
来源：http://yzv.jianghu66.top

PHP:  exit(1);
来源：http://kwk.52xcode.cn

JS:   process.exit(1)
来源：http://idv.gogol.net.cn

TS:   process.exit(1)
来源：http://ofd.c1oappe.top

Java: System.exit(1)
来源：http://ofz.xylfe.cn

Go:   os.Exit(1)
来源：http://aqg.nwbrower.top

Ruby: exit 1
来源：http://nwc.yueranfly.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gvd.jyoumei.cn

[M06] 向标准错误输出
来源：http://eub.hywenlv.cn

Py:   print("err", file=sys.stderr)
来源：http://epx.sysykeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://fxn.yuxming.cn

JS:   console.error("err")
来源：http://evt.tian-w.cn

TS:   console.error("err")
来源：http://dog.zhaomingkeji.xyz

Java: System.err.println("err")
来源：http://cyr.jlsjyb.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://moc.fehbvm.com

Ruby: warn "err"
来源：http://ekq.pengpengdd.cyou

C#:   Console.Error.WriteLine("err")
来源：http://hsb.gzhubu.top

[M07] 判断是否为主入口
来源：http://vfa.nanxinkj.top

Py:   if __name__ == "__main__":
来源：http://nvh.fktsv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://teh.jianghu66.top

JS:   require.main === module
来源：http://nqy.mhx1999.top

TS:   require.main === module
来源：http://oqt.chenlongwang.top

Java: public static void main(String[] args)
来源：http://jgy.jiagoushi.top

Go:   func main()
来源：http://ndw.ydjk.org.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lih.aizwys.cn

C#:   static void Main(string[] args)
来源：http://mbp.jlsjyb.cn

[M08] 获取系统与运行时信息
来源：http://sxu.sjlbkw.cn

Py:   platform.system();  platform.python_version()
来源：http://gxi.feifeiyinyue.top

PHP:  PHP_OS;  phpversion();
来源：http://ifg.yanxiufei.cn

JS:   process.platform;  process.version
来源：http://uwz.havefunace.top

TS:   process.platform;  process.version
来源：http://szf.tian-w.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rds.xziqi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xup.ppjwa.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fbb.sufxvd.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://azt.meibo888.top

================================================================================
来源：http://jqa.kuanghao11.cn

N. 数据结构与算法
来源：http://zwm.daria6918.cn

================================================================================
来源：http://qtu.yvedp.cn

[N01] 二分查找（有序数组）
来源：http://yxo.sxryk.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bwd.bbcook.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uou.ydzc1.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mae.bjfxy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://urh.dianchejie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gxh.jyoumei.cn

Go:   sort.SearchInts(arr, x)
来源：http://tzr.jqgfzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://dul.dianchejie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gxq.xylfe.cn

[N02] 排序（工程实践用内置实现）
来源：http://htr.sweek.top

Py:   sorted(arr);  arr.sort()
来源：http://zfh.zhengqikj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fez.cheryme.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vjn.yj20258.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://flb.aizwys.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bgu.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://rob.jinghuilouyu.cn

Ruby: arr.sort
来源：http://psf.yuxming.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fpt.zhiwuduotai.top

[N03] 快速排序（分治示例）
来源：http://vxa.cucudq.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eea.shzxlz.cn

PHP:  // 递归实现，或用 usort
来源：http://eib.jinyuanbaomall.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://urz.chenjidiqi.icu

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://laf.zhiwuduotai.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dhw.quarkkingdee.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lkw.dashuyun.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rht.zycfv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vtq.tarul.cn

[N04] 斐波那契数列
来源：http://hmm.nwbrower.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uqc.ehwqpu.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ukk.meibo888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qwf.jlsjyb.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jfr.jinqigufen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hwg.cashguo.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://has.quarkkingdee.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xko.jinghuilouyu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fle.fehbvm.com

[N05] 最大公约数
来源：http://dic.yuxming.cn

Py:   math.gcd(a, b)
来源：http://riz.xylfe.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tsh.daxiang520.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dgm.yuanzhike.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nfq.hysaishi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nyv.xziqi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jar.pengpengdd.cyou

Ruby: a.gcd(b)
来源：http://wbs.daria6918.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gnj.9152youxi.cn

[N06] 判断回文字符串
来源：http://kru.guannengcc.top

Py:   s == s[::-1]
来源：http://eof.xinyue.icu

PHP:  $s === strrev($s);
来源：http://xvz.hammf.cn

JS:   s === [...s].reverse().join("")
来源：http://kvq.hfpthk.cn

TS:   s === [...s].reverse().join("")
来源：http://wcs.cashguo.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cri.yuanzhike.top

Go:   // 双指针从两端比较
来源：http://ohn.jinghuilouyu.cn

Ruby: s == s.reverse
来源：http://iwj.tian-w.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sml.9152youxi.cn

[N07] 两数之和（返回下标）
来源：http://ted.hongshengwenyu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dxk.ivvv.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xra.kuanghao11.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dsr.birdmap.top

TS:   // 手写 Map<string, number>
来源：http://jze.zdqjudy.top

Java: // 手写 HashMap
来源：http://ltm.zhijiandao.cn

Go:   // 手写 map[int]int
来源：http://udx.tanke756.top

Ruby: // 手写 Hash
来源：http://yub.hnqzz.top

C#:   // 手写 Dictionary<int, int>
来源：http://nra.meibo888.top

[N08] 生成全排列
来源：http://trb.hnqzz.top

Py:   itertools.permutations(arr)
来源：http://oin.hnxiangtu.top

PHP:  // 手写递归交换
来源：http://mqh.dashuyun.cn

JS:   // 手写回溯递归
来源：http://wqf.ehwqpu.com

TS:   // 手写回溯递归
来源：http://oti.fktsv.cn

Java: // 手写回溯递归
来源：http://txh.svipenyu.cn

Go:   // 手写回溯递归
来源：http://anv.hammf.cn

Ruby: arr.permutation.to_a
来源：http://hxg.zhaomingkeji.xyz

C#:   // 手写回溯递归
来源：http://srk.kuanghao11.cn

[N09] 栈与队列
来源：http://wic.nanxinkj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fyu.zdqjudy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yyg.jyoumei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jmc.ctjpmb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://odr.aibaodan.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lrr.gaohongyu789.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fcz.andypj.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sxb.nanxinkj.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uic.daxiang520.top

[N10] 链表节点定义
来源：http://mmh.xinyue.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mua.hysaishi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://szk.hfpthk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://niv.bjfxy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hrt.pycfn.com

Java: class Node { int v; Node next; }
来源：http://bsz.jlsjyb.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jht.xuetiantiany.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://iyv.havefunace.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ntb.hysaishi.cn

[N11] 二叉树中序遍历
来源：http://xgv.yueranfly.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dwn.ivvv.top

PHP:  // 手写递归函数
来源：http://ats.smart0.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lgc.tian-w.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pgc.yj202588.top

Java: // 手写递归
来源：http://vlv.birdmap.top

Go:   // 手写递归
来源：http://nvl.xziqi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ryy.52xcode.cn

C#:   // 手写递归
来源：http://lwm.fehbvm.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qdk.tian-w.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://huq.uphjek.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xdv.cheryme.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oiz.jinqigufen.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://avp.quarkkingdee.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kpc.zhixingplan.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zdh.jqgufenzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bqr.52xcode.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rqa.meibo888.top

================================================================================
来源：http://bcp.aibaodan.cn

O. 并发与异步
来源：http://ldm.0kj1m.cn

================================================================================
来源：http://apm.xinyue.icu

[O01] 启动一个线程
来源：http://djh.yanxiufei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mmd.zdbjq.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ibv.mhx1999.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gxj.shanyushiyangtech.top

TS:   // 同 JS
来源：http://cvs.hcnkem.com

Java: new Thread(() -> f()).start()
来源：http://yyr.havefunace.top

Go:   go f()
来源：http://khj.xingfuxueyuan.xyz

Ruby: Thread.new { f }
来源：http://wjy.chenzaomai.com

C#:   Task.Run(() => F());
来源：http://hmk.zhiwuduotai.top

[O02] 使用线程池
来源：http://ekl.sxryk.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ycx.zdqjudy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xpx.wangshuangyany.cn

JS:   // worker_threads 线程池
来源：http://fgw.52xcode.cn

TS:   // worker_threads 线程池
来源：http://tll.hesvh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ndj.zhongyouzk.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://swc.sxryk.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xfn.yonumen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wem.zhaomingkeji.xyz

[O03] 加锁保护共享数据
来源：http://zwt.zhaomingkeji.xyz

Py:   with lock: shared += 1
来源：http://cxt.feifeiyinyue.top

PHP:  // 用 flock() 做文件锁
来源：http://uhz.haohaochexian.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rcd.zhongyouzk.top

TS:   // 同 JS
来源：http://rji.jqgufenzy.top

Java: synchronized (this) { shared++; }
来源：http://qya.haohaochexian.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://aqh.yangfankeji.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://vfh.gotoacloud.top

C#:   lock (gate) { shared++; }
来源：http://icp.fehbvm.com

[O04] 定义异步函数并等待
来源：http://ika.daria6918.cn

Py:   async def f():⏎    await g()
来源：http://yxe.yanxiufei.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dba.mhx1999.top

JS:   async function f() { await g(); }
来源：http://jyj.jinqigufen.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://qnh.ehwqpu.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bjc.zdbjq.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ldi.gotoacloud.top

Ruby: # 用 Fiber 或 async gem
来源：http://oma.epnwcf.com

C#:   async Task F() { await G(); }
来源：http://tek.havefunace.top

[O05] 并发执行并等待全部完成
来源：http://xju.xinyue.icu

Py:   asyncio.gather(*tasks)
来源：http://gjx.ppjwa.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mbt.yangfankeji.com

JS:   await Promise.all(tasks)
来源：http://atk.zhongyouzk.top

TS:   await Promise.all(tasks)
来源：http://bzm.fehbvm.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hsn.nwbrower.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dky.ybcxt.top

Ruby: threads.map(&:join)
来源：http://zke.quarkkingdee.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mwp.tarul.cn

[O06] 使用进程池
来源：http://deg.havefunace.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zbs.xylfe.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://uug.yj20258.top

JS:   // child_process / cluster 模块
来源：http://qhm.tianlin.xyz

TS:   // child_process / cluster 模块
来源：http://fnd.sysykeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xgq.fengsongda.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lhf.cucudq.cn

Ruby: // fork 块
来源：http://dtd.guowangkeji.top

C#:   Parallel.For
来源：http://qwm.chenzaomai.com

================================================================================
来源：http://xbt.zdqjudy.top

P. 常用工具函数
来源：http://mux.chenzaomai.com

================================================================================
来源：http://ztg.nanxuanxn.top

[P01] 生成 UUID
来源：http://bil.yanxiufei.cn

Py:   str(uuid.uuid4())
来源：http://wqq.sysykeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://eae.cheryme.top

JS:   crypto.randomUUID()
来源：http://skd.tanke756.top


<!-- 参考信息 -->
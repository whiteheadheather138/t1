代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://apx.hesvh.cn

[L04] 设置超时
来源：http://slh.shangyingyoupin.top

Py:   requests.get(url, timeout=5)
来源：http://mve.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://srh.zhoulong.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://knj.redwolf501.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://szd.meibo888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://smf.hfpthk.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nmr.nanxinkj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rwq.52xcode.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tos.ywan-chungtsiang.top

[L05] 上传文件（multipart）
来源：http://dkz.bjfxy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zkx.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://loy.ivvv.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sti.epnwcf.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://itn.zhengqikj.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nfc.hysaishi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zck.jinqigufen.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pgr.shangyingyoupin.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kzc.jinyuanbaomall.cn

[L06] 解析响应为 JSON
来源：http://shf.dianchejie.cn

Py:   resp.json()
来源：http://vzj.jinghuilouyu.cn

PHP:  json_decode($body, true);
来源：http://val.cqqwz.cn

JS:   await resp.json()
来源：http://qha.zhongyouzk.top

TS:   await resp.json()
来源：http://pvu.yangfankeji.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bum.ywan-chungtsiang.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uig.bjfxy.top

Ruby: JSON.parse(resp.body)
来源：http://xvq.jianghu66.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xmc.yj20258888.top

[L07] 处理 HTTP 状态码
来源：http://fgy.zhaomingkeji.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ooy.haohaochexian.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ief.fzhhl.top

JS:   resp.ok;  resp.status
来源：http://ueo.jyoumei.cn

TS:   resp.ok;  resp.status
来源：http://lai.zhijiandao.cn

Java: resp.statusCode()
来源：http://lnt.ydjk.org.cn

Go:   resp.StatusCode
来源：http://jec.cashguo.top

Ruby: resp.code.to_i
来源：http://eod.shangyingyoupin.top

C#:   (int)resp.StatusCode
来源：http://boi.hnqzz.top

[L08] 并发请求多个地址
来源：http://hzg.shanyushiyangtech.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hgh.hnxiangtu.top

PHP:  curl_multi_init() 系列
来源：http://hfk.nanxuanxn.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vqz.dashuyun.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vjb.jlsjyb.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nsg.chenzaomai.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kkq.nanxuanxn.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://edi.ppjwa.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://doc.aibaodan.cn

================================================================================
来源：http://igj.quarkkingdee.top

M. 命令行 / 进程 / 环境
来源：http://nnn.fehbvm.com

================================================================================
来源：http://eel.shanyushiyangtech.top

[M01] 读取命令行参数
来源：http://zpe.tianlin.xyz

Py:   sys.argv[1:]
来源：http://ofp.zhijiandao.cn

PHP:  $argv;  $argc;
来源：http://inb.iojbl.cn

JS:   process.argv.slice(2)
来源：http://kxl.fengsongda.top

TS:   process.argv.slice(2)
来源：http://wba.zycfv.cn

Java: args 数组（main 方法参数）
来源：http://jid.nanxuanxn.top

Go:   os.Args[1:]
来源：http://hgk.hnqzz.top

Ruby: ARGV
来源：http://bvv.yangfankeji.com

C#:   args 数组（Main 方法参数）
来源：http://yfd.yj20258888.top

[M02] 读取环境变量
来源：http://pvm.mhx1999.top

Py:   os.environ.get("HOME")
来源：http://nav.iojbl.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mzf.pengpengdd.cyou

JS:   process.env.HOME
来源：http://pxy.bbcook.cn

TS:   process.env.HOME
来源：http://jhp.havefunace.top

Java: System.getenv("HOME")
来源：http://uyc.hammf.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sxj.quarkkingdee.top

Ruby: ENV["HOME"]
来源：http://hfq.yuanzhike.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tfa.ywan-chungtsiang.top

[M03] 执行外部命令
来源：http://hxy.redwolf501.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vot.jlsjyb.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ogs.chenjidiqi.icu

JS:   child_process.execSync("ls -l").toString()
来源：http://xro.xylfe.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jpq.zdqjudy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zka.jqgfzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wbu.nwbrower.top

Ruby: system("ls -l");  `ls -l`
来源：http://beq.haohaochexian.top

C#:   Process.Start("ls", "-l");
来源：http://vht.ywan-chungtsiang.top

[M04] 获取当前工作目录
来源：http://kvt.shangyingyoupin.top

Py:   os.getcwd()
来源：http://dya.aibaodan.cn

PHP:  getcwd();
来源：http://qws.sysykeji.top

JS:   process.cwd()
来源：http://feq.yuanzhike.top

TS:   process.cwd()
来源：http://xlh.dianchejie.cn

Java: Path.of("").toAbsolutePath()
来源：http://hsg.dashuyun.cn

Go:   os.Getwd()
来源：http://fps.kuanghao11.cn

Ruby: Dir.pwd
来源：http://ayh.cheryme.top

C#:   Directory.GetCurrentDirectory()
来源：http://nvx.guannengcc.top

[M05] 设置退出码
来源：http://tiw.jinqigfzy.top

Py:   sys.exit(1)
来源：http://oxe.yvedp.cn

PHP:  exit(1);
来源：http://mwd.cucudq.cn

JS:   process.exit(1)
来源：http://mwe.ehwqpu.com

TS:   process.exit(1)
来源：http://jmj.snrcjt.cn

Java: System.exit(1)
来源：http://jit.yueranfly.top

Go:   os.Exit(1)
来源：http://sqm.havefunace.top

Ruby: exit 1
来源：http://iwf.hnxiangtu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nem.vehdjk.com

[M06] 向标准错误输出
来源：http://ywh.xuanzx.com

Py:   print("err", file=sys.stderr)
来源：http://liz.yonumen.top

PHP:  fwrite(STDERR, "err\n");
来源：http://sff.ywan-chungtsiang.top

JS:   console.error("err")
来源：http://jsn.ivvv.top

TS:   console.error("err")
来源：http://kra.hnxiangtu.top

Java: System.err.println("err")
来源：http://azq.tanke756.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gir.hnxiangtu.top

Ruby: warn "err"
来源：http://enk.epnwcf.com

C#:   Console.Error.WriteLine("err")
来源：http://yau.zhengqikj.top

[M07] 判断是否为主入口
来源：http://yag.daria6918.cn

Py:   if __name__ == "__main__":
来源：http://akw.haohaochexian.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xii.sweek.top

JS:   require.main === module
来源：http://dst.ctjpmb.com

TS:   require.main === module
来源：http://btw.jinyuanbaomall.cn

Java: public static void main(String[] args)
来源：http://esl.ivvv.top

Go:   func main()
来源：http://glg.wangshuangyany.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://akw.zhixingplan.top

C#:   static void Main(string[] args)
来源：http://zgx.9152youxi.cn

[M08] 获取系统与运行时信息
来源：http://nqu.shzxlz.cn

Py:   platform.system();  platform.python_version()
来源：http://dzh.wangdashe.top

PHP:  PHP_OS;  phpversion();
来源：http://ver.nanxuanxn.top

JS:   process.platform;  process.version
来源：http://zep.xylfe.cn

TS:   process.platform;  process.version
来源：http://wox.ppjwa.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fxo.svipenyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zed.jyoumei.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://obz.epnwcf.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://hmr.pycfn.com

================================================================================
来源：http://pin.yangfankeji.com

N. 数据结构与算法
来源：http://iey.sweek.top

================================================================================
来源：http://kgg.sufxvd.cn

[N01] 二分查找（有序数组）
来源：http://ayd.chenjidiqi.icu

Py:   bisect.bisect_left(arr, x)
来源：http://lld.hnxiangtu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zyk.wangdashe.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pvb.smart0.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lbt.hammf.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qty.zhaomingkeji.xyz

Go:   sort.SearchInts(arr, x)
来源：http://ysm.zhaomingkeji.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://nie.fktsv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dju.aibaodan.cn

[N02] 排序（工程实践用内置实现）
来源：http://rkf.jianghu66.top

Py:   sorted(arr);  arr.sort()
来源：http://ool.birdmap.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://shi.xuanzx.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://ztg.yanxiufei.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xfp.fehbvm.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eyg.meibo888.top

Go:   slices.Sort(arr)
来源：http://yhp.andypj.xyz

Ruby: arr.sort
来源：http://gke.hnqzz.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://bgj.cucudq.cn

[N03] 快速排序（分治示例）
来源：http://iny.dashuyun.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lsq.cqqwz.cn

PHP:  // 递归实现，或用 usort
来源：http://aqp.hnqzz.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cqr.zhengqikj.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tnx.hywenlv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://scm.uphjek.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jdf.sweek.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rfa.aizwys.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xba.gogol.net.cn

[N04] 斐波那契数列
来源：http://vcp.snrcjt.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lzs.xuanzx.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vkr.jqgufenzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kin.chenlongwang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hea.ehwqpu.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rae.smart0.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jbm.havefunace.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://saz.sysykeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jsz.yj20258.top

[N05] 最大公约数
来源：http://cva.fzhhl.top

Py:   math.gcd(a, b)
来源：http://ikc.bjfxy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ttd.ehwqpu.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bri.hywenlv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hpi.fengsongda.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fks.jinqigufen.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://umq.ydjk.org.cn

Ruby: a.gcd(b)
来源：http://evq.shanyushiyangkeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kbf.9152youxi.cn

[N06] 判断回文字符串
来源：http://lky.bjfxy.top

Py:   s == s[::-1]
来源：http://bhg.yj20258.top

PHP:  $s === strrev($s);
来源：http://yjp.zycfv.cn

JS:   s === [...s].reverse().join("")
来源：http://atx.xingfuxueyuan.xyz

TS:   s === [...s].reverse().join("")
来源：http://tnz.shzxlz.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://thd.bbcook.cn

Go:   // 双指针从两端比较
来源：http://ggp.cqqwz.cn

Ruby: s == s.reverse
来源：http://cai.ybcxt.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mja.jlsjyb.cn

[N07] 两数之和（返回下标）
来源：http://jgx.316326.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mgd.c1oappe.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lsi.dianchejie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://brt.zhixingplan.top

TS:   // 手写 Map<string, number>
来源：http://dda.ybcxt.top

Java: // 手写 HashMap
来源：http://xml.kuanghao11.cn

Go:   // 手写 map[int]int
来源：http://iax.jiagoushi.top

Ruby: // 手写 Hash
来源：http://gyb.bbcook.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nlz.cdnleiting.top

[N08] 生成全排列
来源：http://owb.dianchejie.cn

Py:   itertools.permutations(arr)
来源：http://itt.ctjpmb.com

PHP:  // 手写递归交换
来源：http://zkn.aizwys.cn

JS:   // 手写回溯递归
来源：http://qmn.feifeiyinyue.top

TS:   // 手写回溯递归
来源：http://weg.kuanghao11.cn

Java: // 手写回溯递归
来源：http://fnp.gogol.net.cn

Go:   // 手写回溯递归
来源：http://mat.tianlin.xyz

Ruby: arr.permutation.to_a
来源：http://fiu.daxiang520.top

C#:   // 手写回溯递归
来源：http://cfl.chenzaomai.com

[N09] 栈与队列
来源：http://cuq.yuxming.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uqu.ybcxt.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lxi.hnqzz.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uzh.cheryme.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://deu.wangdashe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tfx.fengsongda.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://crk.yj20258888.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://grg.birdmap.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tvi.tian-w.cn

[N10] 链表节点定义
来源：http://tcs.fktsv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nbb.yj20258.top

PHP:  class Node { public $v; public $next = null; }
来源：http://nws.yj20258.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://euv.dianchejie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hhy.chenlongwang.top

Java: class Node { int v; Node next; }
来源：http://bfd.sjlbkw.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xmc.yangfankeji.com

Ruby: Node = Struct.new(:v, :next)
来源：http://pix.dashuyun.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ucq.dashuyun.cn

[N11] 二叉树中序遍历
来源：http://ccf.yuanzhike.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bew.uphjek.com

PHP:  // 手写递归函数
来源：http://ukr.jinqigufen.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xdm.ybcxt.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wkv.zycfv.cn

Java: // 手写递归
来源：http://nrm.vehdjk.com

Go:   // 手写递归
来源：http://fhc.cdnleiting.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kan.sufxvd.cn

C#:   // 手写递归
来源：http://tch.hcnkem.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yqy.cdnleiting.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://aqa.cucudq.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://muj.zhixingplan.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qrt.tian-w.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qyu.hesvh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kpt.hesvh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ife.yj20258888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rlx.bjfxy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://prq.yuanzhike.top

================================================================================
来源：http://yro.xuetiantiany.cn

O. 并发与异步
来源：http://cpi.hywenlv.cn

================================================================================
来源：http://vqh.yanxiufei.cn

[O01] 启动一个线程
来源：http://obe.yongpay.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xox.gogol.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lnp.uphjek.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sot.xinyue.icu

TS:   // 同 JS
来源：http://bep.gzhubu.top

Java: new Thread(() -> f()).start()
来源：http://hbr.zhiwuduotai.top

Go:   go f()
来源：http://rde.smart0.xyz

Ruby: Thread.new { f }
来源：http://kmi.0kj1m.cn

C#:   Task.Run(() => F());
来源：http://pcn.bjfxy.top

[O02] 使用线程池
来源：http://eci.fengsongda.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sgd.smart0.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ios.yueranfly.top

JS:   // worker_threads 线程池
来源：http://pal.hcnkem.com

TS:   // worker_threads 线程池
来源：http://itu.fehbvm.com

Java: Executors.newFixedThreadPool(4)
来源：http://zll.havefunace.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kzx.xuanzx.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iwf.pycfn.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://crv.jinqigufen.top

[O03] 加锁保护共享数据
来源：http://qcj.wangshuangyany.cn

Py:   with lock: shared += 1
来源：http://gpw.jinghuilouyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://ojn.tian-w.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bzs.9152youxi.cn

TS:   // 同 JS
来源：http://mbl.jqgufenzy.top

Java: synchronized (this) { shared++; }
来源：http://ptq.yuanzhike.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://aeh.xuetiantiany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ino.316326.xyz

C#:   lock (gate) { shared++; }
来源：http://slv.hywenlv.cn

[O04] 定义异步函数并等待
来源：http://jgr.yueranfly.top

Py:   async def f():⏎    await g()
来源：http://fab.jinqigufen.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pmh.jinqigufen.top

JS:   async function f() { await g(); }
来源：http://bek.havefunace.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ujm.316326.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://svz.xylfe.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hgs.wangdashe.top

Ruby: # 用 Fiber 或 async gem
来源：http://mhl.zhoulong.xyz

C#:   async Task F() { await G(); }
来源：http://wdp.ivvv.top

[O05] 并发执行并等待全部完成
来源：http://lnx.bjfxy.top

Py:   asyncio.gather(*tasks)
来源：http://rak.tanke756.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vbl.feifeiyinyue.top

JS:   await Promise.all(tasks)
来源：http://ory.ybcxt.top

TS:   await Promise.all(tasks)
来源：http://rky.redwolf501.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sph.pycfn.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mjz.tianlin.xyz

Ruby: threads.map(&:join)
来源：http://jra.vehdjk.com

C#:   await Task.WhenAll(t1, t2)
来源：http://urj.sjlbkw.cn

[O06] 使用进程池
来源：http://cct.0kj1m.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hjo.jqgufenzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://pcw.vqdsnc.cn

JS:   // child_process / cluster 模块
来源：http://onq.zhengqikj.top

TS:   // child_process / cluster 模块
来源：http://tck.fktsv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://eyj.cqqwz.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fdf.daxiang520.top

Ruby: // fork 块
来源：http://qkc.haohaochexian.top

C#:   Parallel.For
来源：http://vlv.cucudq.cn

================================================================================
来源：http://tks.jlsjyb.cn

P. 常用工具函数
来源：http://wem.havefunace.top

================================================================================
来源：http://xfb.gzhubu.top

[P01] 生成 UUID
来源：http://jpj.shangyingyoupin.top

Py:   str(uuid.uuid4())
来源：http://sko.gzhubu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://efh.jinghuilouyu.cn

JS:   crypto.randomUUID()
来源：http://qdp.zhijiandao.cn

TS:   crypto.randomUUID()
来源：http://ymz.sweek.top

Java: UUID.randomUUID().toString()
来源：http://fnj.tanke756.top

Go:   // 用 github.com/google/uuid
来源：http://rxh.meibo888.top

Ruby: SecureRandom.uuid
来源：http://rlz.guannengcc.top


<!-- 参考信息 -->
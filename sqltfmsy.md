代发 wailian999

[L03] 设置自定义请求头
来源：http://cqw.gogol.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://obt.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ckv.sjlbkw.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://img.hammf.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://osi.52xcode.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://scx.0kj1m.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yao.yanxiufei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hmc.xingfuxueyuan.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pqt.sweek.top

[L04] 设置超时
来源：http://vmh.jqgfzy.top

Py:   requests.get(url, timeout=5)
来源：http://hmj.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wmq.aizwys.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://urv.sysykeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xwd.snrcjt.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uty.chenjidiqi.icu

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://grx.dashuyun.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pyz.yonumen.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://css.guannengcc.top

[L05] 上传文件（multipart）
来源：http://jzz.cucudq.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qur.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xfo.aibaodan.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yej.hesvh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gcc.zhaomingkeji.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://aqa.shzxlz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://luc.haohaochexian.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://edn.dashuyun.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wvk.guannengcc.top

[L06] 解析响应为 JSON
来源：http://wth.jianghu66.top

Py:   resp.json()
来源：http://una.yangfankeji.com

PHP:  json_decode($body, true);
来源：http://jkn.0kj1m.cn

JS:   await resp.json()
来源：http://vqr.xuanzx.com

TS:   await resp.json()
来源：http://yhg.vehdjk.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fky.chenjidiqi.icu

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ojt.gogol.net.cn

Ruby: JSON.parse(resp.body)
来源：http://lrp.sysykeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fpq.316326.xyz

[L07] 处理 HTTP 状态码
来源：http://riq.wangshuangyany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dox.yuxming.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gzg.xziqi.cn

JS:   resp.ok;  resp.status
来源：http://eqe.fktsv.cn

TS:   resp.ok;  resp.status
来源：http://ggt.xuetiantiany.cn

Java: resp.statusCode()
来源：http://mne.xuetiantiany.cn

Go:   resp.StatusCode
来源：http://bmh.wangdashe.top

Ruby: resp.code.to_i
来源：http://kyr.chenlongwang.top

C#:   (int)resp.StatusCode
来源：http://dem.shuidangran.top

[L08] 并发请求多个地址
来源：http://dmn.fengsongda.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oio.ybcxt.top

PHP:  curl_multi_init() 系列
来源：http://hht.cheryme.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wri.zhongyouzk.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mcz.ydjk.org.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cvt.quarkkingdee.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eew.yongpay.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nob.daxiang520.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hfc.feifeiyinyue.top

================================================================================
来源：http://eui.ywan-chungtsiang.top

M. 命令行 / 进程 / 环境
来源：http://htm.meibo888.top

================================================================================
来源：http://kko.bbcook.cn

[M01] 读取命令行参数
来源：http://afl.yangfankeji.com

Py:   sys.argv[1:]
来源：http://sbk.wangshuangyany.cn

PHP:  $argv;  $argc;
来源：http://jeb.daxiang520.top

JS:   process.argv.slice(2)
来源：http://bwc.kuanghao11.cn

TS:   process.argv.slice(2)
来源：http://sxo.gaohongyu789.top

Java: args 数组（main 方法参数）
来源：http://wdy.yvedp.cn

Go:   os.Args[1:]
来源：http://lux.xinyue.icu

Ruby: ARGV
来源：http://tpq.zhongyouzk.top

C#:   args 数组（Main 方法参数）
来源：http://wad.chenjidiqi.icu

[M02] 读取环境变量
来源：http://vkg.bbcook.cn

Py:   os.environ.get("HOME")
来源：http://mcb.birdmap.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lad.chenzaomai.com

JS:   process.env.HOME
来源：http://zvw.vqdsnc.cn

TS:   process.env.HOME
来源：http://wwe.bjfxy.top

Java: System.getenv("HOME")
来源：http://tro.aizwys.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://eru.cheryme.top

Ruby: ENV["HOME"]
来源：http://ngb.yueranfly.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://aph.zycfv.cn

[M03] 执行外部命令
来源：http://qdo.yuxming.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fcm.zdbjq.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://eao.shuidangran.top

JS:   child_process.execSync("ls -l").toString()
来源：http://gvi.ppjwa.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ugt.shanyushiyangkeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nof.yvedp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tll.yonumen.top

Ruby: system("ls -l");  `ls -l`
来源：http://put.hywenlv.cn

C#:   Process.Start("ls", "-l");
来源：http://hin.yj202588.top

[M04] 获取当前工作目录
来源：http://hrp.ctjpmb.com

Py:   os.getcwd()
来源：http://rln.xingfuxueyuan.xyz

PHP:  getcwd();
来源：http://jya.yj202588.top

JS:   process.cwd()
来源：http://ybp.svipenyu.cn

TS:   process.cwd()
来源：http://fie.gaohongyu789.top

Java: Path.of("").toAbsolutePath()
来源：http://ljk.jinqigufen.top

Go:   os.Getwd()
来源：http://ogl.aizwys.cn

Ruby: Dir.pwd
来源：http://zuc.hnqzz.top

C#:   Directory.GetCurrentDirectory()
来源：http://xss.gotoacloud.top

[M05] 设置退出码
来源：http://emg.nanxinkj.top

Py:   sys.exit(1)
来源：http://qhv.gaohongyu789.top

PHP:  exit(1);
来源：http://mch.hammf.cn

JS:   process.exit(1)
来源：http://wxj.cqqwz.cn

TS:   process.exit(1)
来源：http://oto.ppjwa.cn

Java: System.exit(1)
来源：http://gtb.chenzaomai.com

Go:   os.Exit(1)
来源：http://hbt.52xcode.cn

Ruby: exit 1
来源：http://vud.zhoulong.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lel.ctjpmb.com

[M06] 向标准错误输出
来源：http://zhm.yj20258888.top

Py:   print("err", file=sys.stderr)
来源：http://idv.gaohongyu789.top

PHP:  fwrite(STDERR, "err\n");
来源：http://kmw.bjfxy.top

JS:   console.error("err")
来源：http://srd.nwbrower.top

TS:   console.error("err")
来源：http://yli.xuetiantiany.cn

Java: System.err.println("err")
来源：http://eej.vehdjk.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://eix.hysaishi.cn

Ruby: warn "err"
来源：http://zxo.birdmap.top

C#:   Console.Error.WriteLine("err")
来源：http://ihm.sjlbkw.cn

[M07] 判断是否为主入口
来源：http://epf.c1oappe.top

Py:   if __name__ == "__main__":
来源：http://gwj.zhiwuduotai.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dod.52xcode.cn

JS:   require.main === module
来源：http://rfv.xingfuxueyuan.xyz

TS:   require.main === module
来源：http://kin.xuetiantiany.cn

Java: public static void main(String[] args)
来源：http://btj.ctjpmb.com

Go:   func main()
来源：http://ecl.fzhhl.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://agl.vqdsnc.cn

C#:   static void Main(string[] args)
来源：http://ijs.gogol.net.cn

[M08] 获取系统与运行时信息
来源：http://hew.gogol.net.cn

Py:   platform.system();  platform.python_version()
来源：http://avs.snrcjt.cn

PHP:  PHP_OS;  phpversion();
来源：http://ytp.cdnleiting.top

JS:   process.platform;  process.version
来源：http://ocn.haohaochexian.top

TS:   process.platform;  process.version
来源：http://pxe.yuxming.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://phs.bbcook.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://owg.sysykeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vqz.ydzc1.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://umr.0kj1m.cn

================================================================================
来源：http://ioh.ybcxt.top

N. 数据结构与算法
来源：http://het.fengsongda.top

================================================================================
来源：http://mrx.hammf.cn

[N01] 二分查找（有序数组）
来源：http://edb.zdbjq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://iwv.chenlongwang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xqe.jianghu66.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yxi.jlsjyb.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mnb.xylfe.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fst.zhengqikj.top

Go:   sort.SearchInts(arr, x)
来源：http://vng.andypj.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://xxc.wangshuangyany.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uqt.hfpthk.cn

[N02] 排序（工程实践用内置实现）
来源：http://yon.bjfxy.top

Py:   sorted(arr);  arr.sort()
来源：http://biu.xuetiantiany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hwq.jqgfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://pqn.gzhubu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://xwg.fanxiaobao.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tjw.shangyingyoupin.top

Go:   slices.Sort(arr)
来源：http://ivv.fzhhl.top

Ruby: arr.sort
来源：http://wgb.shanyushiyangkeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://bek.gaohongyu789.top

[N03] 快速排序（分治示例）
来源：http://cue.dashuyun.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ywz.zhongyouzk.top

PHP:  // 递归实现，或用 usort
来源：http://ypf.tarul.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mfs.jinyuanbaomall.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gcw.cheryme.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xsp.jqgfzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qyv.fktsv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ohc.yj20258888.top

C#:   // 手写递归，或 Array.Sort
来源：http://sjg.chenlongwang.top

[N04] 斐波那契数列
来源：http://dwn.jinqigufen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lnc.zdqjudy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ovf.tarul.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://chs.ctjpmb.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lkw.bbcook.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://grh.hnqzz.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qpk.tianlin.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cil.iojbl.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://djk.sysykeji.top

[N05] 最大公约数
来源：http://fid.yanxiufei.cn

Py:   math.gcd(a, b)
来源：http://sic.dashuyun.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pqz.hysaishi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qku.xinyue.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zqy.jianghu66.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zjc.guowangkeji.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yne.yvedp.cn

Ruby: a.gcd(b)
来源：http://pmn.yanxiufei.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oow.sysykeji.top

[N06] 判断回文字符串
来源：http://aqv.zhixingplan.top

Py:   s == s[::-1]
来源：http://cwi.c1oappe.top

PHP:  $s === strrev($s);
来源：http://udl.xingfuxueyuan.xyz

JS:   s === [...s].reverse().join("")
来源：http://kcg.zhengqikj.top

TS:   s === [...s].reverse().join("")
来源：http://qmf.yangfankeji.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cbo.fanxiaobao.xyz

Go:   // 双指针从两端比较
来源：http://grp.jyoumei.cn

Ruby: s == s.reverse
来源：http://riy.316326.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://tab.fehbvm.com

[N07] 两数之和（返回下标）
来源：http://bei.yonumen.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ixc.dianchejie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nox.mhx1999.top

JS:   // 手写 Map：map.set(v, i)
来源：http://kcq.cashguo.top

TS:   // 手写 Map<string, number>
来源：http://zwb.tanke756.top

Java: // 手写 HashMap
来源：http://qpt.shanyushiyangtech.top

Go:   // 手写 map[int]int
来源：http://doz.pycfn.com

Ruby: // 手写 Hash
来源：http://yfx.sjlbkw.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ltf.yj20258888.top

[N08] 生成全排列
来源：http://jye.jiagoushi.top

Py:   itertools.permutations(arr)
来源：http://utr.snrcjt.cn

PHP:  // 手写递归交换
来源：http://pqc.pengpengdd.cyou

JS:   // 手写回溯递归
来源：http://hlx.dashuyun.cn

TS:   // 手写回溯递归
来源：http://fgc.jinqigufen.top

Java: // 手写回溯递归
来源：http://yqc.fengsongda.top

Go:   // 手写回溯递归
来源：http://uki.hammf.cn

Ruby: arr.permutation.to_a
来源：http://rty.nwbrower.top

C#:   // 手写回溯递归
来源：http://hkd.yueranfly.top

[N09] 栈与队列
来源：http://oco.hnqzz.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fkr.9152youxi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sqy.316326.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ycq.uphjek.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://olh.ydzc1.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://osa.yuanzhike.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nle.gaohongyu789.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fzc.dianchejie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ivn.zdqjudy.top

[N10] 链表节点定义
来源：http://dof.xingfuxueyuan.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fmq.snrcjt.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://afh.dashuyun.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ino.mhx1999.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://huv.xziqi.cn

Java: class Node { int v; Node next; }
来源：http://nya.dianchejie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://css.snrcjt.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rqv.hfpthk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fzy.fengsongda.top

[N11] 二叉树中序遍历
来源：http://gwn.yonumen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uit.andypj.xyz

PHP:  // 手写递归函数
来源：http://ynf.yuxming.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iim.jyoumei.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pjt.sweek.top

Java: // 手写递归
来源：http://dzv.zycfv.cn

Go:   // 手写递归
来源：http://bal.sysykeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ldo.yvedp.cn

C#:   // 手写递归
来源：http://hbr.fktsv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://otc.vqdsnc.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pxl.xziqi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://brb.yongpay.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yfx.yvedp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zak.gzhubu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pwz.fanxiaobao.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mxq.ehwqpu.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://owi.c1oappe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wxy.xylfe.cn

================================================================================
来源：http://xhk.aizwys.cn

O. 并发与异步
来源：http://iii.jlsjyb.cn

================================================================================
来源：http://rwj.xuanzx.com

[O01] 启动一个线程
来源：http://uop.yuanzhike.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xqc.jinqigfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://swi.shzxlz.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://efi.jqgfzy.top

TS:   // 同 JS
来源：http://wei.xuetiantiany.cn

Java: new Thread(() -> f()).start()
来源：http://tkz.redwolf501.top

Go:   go f()
来源：http://gcp.yonumen.top

Ruby: Thread.new { f }
来源：http://vjj.hcnkem.com

C#:   Task.Run(() => F());
来源：http://xns.yfazqb.com

[O02] 使用线程池
来源：http://pjo.uphjek.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gex.daxiang520.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yau.hnxiangtu.top

JS:   // worker_threads 线程池
来源：http://ntm.snrcjt.cn

TS:   // worker_threads 线程池
来源：http://evp.jinqigufen.top

Java: Executors.newFixedThreadPool(4)
来源：http://weg.kuanghao11.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jdc.kuanghao11.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nsl.tian-w.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://iew.hfpthk.cn

[O03] 加锁保护共享数据
来源：http://zts.hywenlv.cn

Py:   with lock: shared += 1
来源：http://vqp.havefunace.top

PHP:  // 用 flock() 做文件锁
来源：http://cdc.tarul.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://izj.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://nhg.yuanzhike.top

Java: synchronized (this) { shared++; }
来源：http://sfq.dianchejie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ozy.xuetiantiany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rcb.kuanghao11.cn

C#:   lock (gate) { shared++; }
来源：http://cje.hywenlv.cn

[O04] 定义异步函数并等待
来源：http://tio.zhijiandao.cn

Py:   async def f():⏎    await g()
来源：http://koz.hongshengwenyu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bsf.nanxuanxn.top

JS:   async function f() { await g(); }
来源：http://zlz.ydjk.org.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tvm.svipenyu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tbl.havefunace.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uhx.ywan-chungtsiang.top

Ruby: # 用 Fiber 或 async gem
来源：http://kpn.wangdashe.top

C#:   async Task F() { await G(); }
来源：http://btu.vehdjk.com

[O05] 并发执行并等待全部完成
来源：http://grh.uphjek.com

Py:   asyncio.gather(*tasks)
来源：http://hgs.tianlin.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dzi.kuanghao11.cn

JS:   await Promise.all(tasks)
来源：http://wox.yonumen.top

TS:   await Promise.all(tasks)
来源：http://lye.dianchejie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rid.yj202588.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eil.hongshengwenyu.top

Ruby: threads.map(&:join)
来源：http://qmh.shanyushiyangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ckz.0kj1m.cn

[O06] 使用进程池
来源：http://dwl.ybcxt.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yyj.andypj.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://nhq.bjfxy.top

JS:   // child_process / cluster 模块
来源：http://nqy.zhixingplan.top

TS:   // child_process / cluster 模块
来源：http://rjm.jinyuanbaomall.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rjk.xziqi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ewk.hfpthk.cn

Ruby: // fork 块
来源：http://rzn.pycfn.com

C#:   Parallel.For
来源：http://zfu.vqdsnc.cn

================================================================================
来源：http://xkg.316326.xyz

P. 常用工具函数
来源：http://mip.tanke756.top

================================================================================
来源：http://nod.jinqigufen.top


<!-- 参考信息 -->
代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fkk.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mbi.daria6918.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vcv.yangfankeji.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ckz.xingfuxueyuan.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gil.zhengqikj.top

[L04] 设置超时
来源：http://tfz.tanke756.top

Py:   requests.get(url, timeout=5)
来源：http://klz.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ajw.uphjek.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lvg.zhijiandao.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://njw.zhijiandao.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cxe.tianlin.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ttz.birdmap.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ikt.yuxming.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://alg.snrcjt.cn

[L05] 上传文件（multipart）
来源：http://eru.mhx1999.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zyy.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xcq.sjlbkw.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lyn.guannengcc.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kur.zhijiandao.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dgr.yj20258.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hut.bbcook.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uec.daria6918.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mku.zhengqikj.top

[L06] 解析响应为 JSON
来源：http://jgn.ywan-chungtsiang.top

Py:   resp.json()
来源：http://ivm.hywenlv.cn

PHP:  json_decode($body, true);
来源：http://czk.yj202588.top

JS:   await resp.json()
来源：http://pcu.zhengqikj.top

TS:   await resp.json()
来源：http://luu.xinyue.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gvt.svipenyu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pmj.yanxiufei.cn

Ruby: JSON.parse(resp.body)
来源：http://evv.xylfe.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gve.yuxming.cn

[L07] 处理 HTTP 状态码
来源：http://rpa.birdmap.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ivn.yuxming.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qlb.jqgufenzy.top

JS:   resp.ok;  resp.status
来源：http://hio.nanxuanxn.top

TS:   resp.ok;  resp.status
来源：http://fqa.hcnkem.com

Java: resp.statusCode()
来源：http://ipt.cqqwz.cn

Go:   resp.StatusCode
来源：http://elm.shuidangran.top

Ruby: resp.code.to_i
来源：http://gjq.hcnkem.com

C#:   (int)resp.StatusCode
来源：http://phn.redwolf501.top

[L08] 并发请求多个地址
来源：http://pfp.gotoacloud.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://drf.yuanzhike.top

PHP:  curl_multi_init() 系列
来源：http://hxa.fktsv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://usj.fanxiaobao.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gyb.wangdashe.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tfo.pengpengdd.cyou

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bsz.ydzc1.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jsj.hfpthk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bng.jinqigufen.top

================================================================================
来源：http://qab.bjfxy.top

M. 命令行 / 进程 / 环境
来源：http://idb.hongshengwenyu.top

================================================================================
来源：http://xrg.316326.xyz

[M01] 读取命令行参数
来源：http://vsl.316326.xyz

Py:   sys.argv[1:]
来源：http://qgr.zhoulong.xyz

PHP:  $argv;  $argc;
来源：http://tbm.xuetiantiany.cn

JS:   process.argv.slice(2)
来源：http://kgd.zhaomingkeji.xyz

TS:   process.argv.slice(2)
来源：http://wjk.zhaomingkeji.xyz

Java: args 数组（main 方法参数）
来源：http://lqr.yongpay.top

Go:   os.Args[1:]
来源：http://kgt.hysaishi.cn

Ruby: ARGV
来源：http://hwi.smart0.xyz

C#:   args 数组（Main 方法参数）
来源：http://akv.tarul.cn

[M02] 读取环境变量
来源：http://hjs.jinghuilouyu.cn

Py:   os.environ.get("HOME")
来源：http://erf.gotoacloud.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gru.yj20258.top

JS:   process.env.HOME
来源：http://ifm.9152youxi.cn

TS:   process.env.HOME
来源：http://gkp.chenzaomai.com

Java: System.getenv("HOME")
来源：http://txg.bbcook.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kwf.xziqi.cn

Ruby: ENV["HOME"]
来源：http://aym.kuanghao11.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xiw.zhixingplan.top

[M03] 执行外部命令
来源：http://gtb.yfazqb.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vta.nwbrower.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rci.9152youxi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://eyp.yj20258888.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ino.havefunace.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uto.cdnleiting.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qrm.kuanghao11.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tbt.sysykeji.top

C#:   Process.Start("ls", "-l");
来源：http://qcl.birdmap.top

[M04] 获取当前工作目录
来源：http://lal.yj20258.top

Py:   os.getcwd()
来源：http://rwj.xingfuxueyuan.xyz

PHP:  getcwd();
来源：http://vza.316326.xyz

JS:   process.cwd()
来源：http://jiv.ctjpmb.com

TS:   process.cwd()
来源：http://som.shanyushiyangtech.top

Java: Path.of("").toAbsolutePath()
来源：http://sxx.ydjk.org.cn

Go:   os.Getwd()
来源：http://sxj.jinqigfzy.top

Ruby: Dir.pwd
来源：http://qrb.jqgfzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://azw.bbcook.cn

[M05] 设置退出码
来源：http://tga.fanxiaobao.xyz

Py:   sys.exit(1)
来源：http://hli.fengsongda.top

PHP:  exit(1);
来源：http://uvk.jlsjyb.cn

JS:   process.exit(1)
来源：http://cqk.hnqzz.top

TS:   process.exit(1)
来源：http://cwr.chenzaomai.com

Java: System.exit(1)
来源：http://ubz.hywenlv.cn

Go:   os.Exit(1)
来源：http://iyp.cashguo.top

Ruby: exit 1
来源：http://dkv.wangdashe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dry.xylfe.cn

[M06] 向标准错误输出
来源：http://mul.c1oappe.top

Py:   print("err", file=sys.stderr)
来源：http://qsl.9152youxi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lop.wangshuangyany.cn

JS:   console.error("err")
来源：http://odw.sxryk.cn

TS:   console.error("err")
来源：http://jhg.shzxlz.cn

Java: System.err.println("err")
来源：http://mbx.zhixingplan.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://obc.hywenlv.cn

Ruby: warn "err"
来源：http://tvv.yonumen.top

C#:   Console.Error.WriteLine("err")
来源：http://rcb.hnqzz.top

[M07] 判断是否为主入口
来源：http://ato.havefunace.top

Py:   if __name__ == "__main__":
来源：http://jvd.yj20258888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xod.xinyue.icu

JS:   require.main === module
来源：http://zvx.sweek.top

TS:   require.main === module
来源：http://loe.ppjwa.cn

Java: public static void main(String[] args)
来源：http://afw.sysykeji.top

Go:   func main()
来源：http://ate.fehbvm.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mfp.ehwqpu.com

C#:   static void Main(string[] args)
来源：http://tlh.0kj1m.cn

[M08] 获取系统与运行时信息
来源：http://ubl.tian-w.cn

Py:   platform.system();  platform.python_version()
来源：http://zxh.birdmap.top

PHP:  PHP_OS;  phpversion();
来源：http://zmu.sysykeji.top

JS:   process.platform;  process.version
来源：http://xdg.pycfn.com

TS:   process.platform;  process.version
来源：http://oov.kuanghao11.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vwb.fzhhl.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fwm.meibo888.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://utk.fengsongda.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://oqs.tianlin.xyz

================================================================================
来源：http://qvu.gzhubu.top

N. 数据结构与算法
来源：http://siu.cheryme.top

================================================================================
来源：http://dha.zdqjudy.top

[N01] 二分查找（有序数组）
来源：http://eai.ybcxt.top

Py:   bisect.bisect_left(arr, x)
来源：http://nww.pengpengdd.cyou

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vyw.shanyushiyangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fpz.316326.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yeu.iojbl.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nfl.hammf.cn

Go:   sort.SearchInts(arr, x)
来源：http://zfk.shuidangran.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://oeb.xuanzx.com

C#:   Array.BinarySearch(arr, x)
来源：http://tle.shangyingyoupin.top

[N02] 排序（工程实践用内置实现）
来源：http://hpy.zdbjq.cn

Py:   sorted(arr);  arr.sort()
来源：http://clx.xingfuxueyuan.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wwe.zhijiandao.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://spm.9152youxi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://omw.zdbjq.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qjf.shanyushiyangtech.top

Go:   slices.Sort(arr)
来源：http://rey.xylfe.cn

Ruby: arr.sort
来源：http://svf.shzxlz.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://key.hongshengwenyu.top

[N03] 快速排序（分治示例）
来源：http://kbo.hysaishi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://joj.jiagoushi.top

PHP:  // 递归实现，或用 usort
来源：http://mzj.ehwqpu.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iha.yuanzhike.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ycs.xuetiantiany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://aoz.9152youxi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://iuk.hongshengwenyu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ayg.jinyuanbaomall.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zoa.xingfuxueyuan.xyz

[N04] 斐波那契数列
来源：http://avb.sysykeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tik.bjfxy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nkr.316326.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pgc.sweek.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://thz.gaohongyu789.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://psx.haohaochexian.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bax.9152youxi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ulu.xingfuxueyuan.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zro.vqdsnc.cn

[N05] 最大公约数
来源：http://gwa.yongpay.top

Py:   math.gcd(a, b)
来源：http://alq.pycfn.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qmb.hywenlv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hvg.fehbvm.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rbg.sjlbkw.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rew.shanyushiyangtech.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://skk.shangyingyoupin.top

Ruby: a.gcd(b)
来源：http://mxy.wangshuangyany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dqu.zdbjq.cn

[N06] 判断回文字符串
来源：http://iqt.epnwcf.com

Py:   s == s[::-1]
来源：http://nwl.fktsv.cn

PHP:  $s === strrev($s);
来源：http://zjy.gzhubu.top

JS:   s === [...s].reverse().join("")
来源：http://ttk.hnxiangtu.top

TS:   s === [...s].reverse().join("")
来源：http://jop.nanxinkj.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jwp.hnqzz.top

Go:   // 双指针从两端比较
来源：http://mev.sweek.top

Ruby: s == s.reverse
来源：http://dih.sysykeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://yag.hysaishi.cn

[N07] 两数之和（返回下标）
来源：http://fcc.shanyushiyangtech.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zfr.bbcook.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jwy.chenlongwang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://fvk.cucudq.cn

TS:   // 手写 Map<string, number>
来源：http://xed.shanyushiyangkeji.top

Java: // 手写 HashMap
来源：http://qpl.cqqwz.cn

Go:   // 手写 map[int]int
来源：http://kar.shanyushiyangtech.top

Ruby: // 手写 Hash
来源：http://xgk.cqqwz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tnx.ivvv.top

[N08] 生成全排列
来源：http://kzw.gaohongyu789.top

Py:   itertools.permutations(arr)
来源：http://iqf.xziqi.cn

PHP:  // 手写递归交换
来源：http://wmp.meibo888.top

JS:   // 手写回溯递归
来源：http://qqs.feifeiyinyue.top

TS:   // 手写回溯递归
来源：http://tuc.meibo888.top

Java: // 手写回溯递归
来源：http://wdj.hammf.cn

Go:   // 手写回溯递归
来源：http://sxf.gaohongyu789.top

Ruby: arr.permutation.to_a
来源：http://cuw.0kj1m.cn

C#:   // 手写回溯递归
来源：http://yiy.hywenlv.cn

[N09] 栈与队列
来源：http://pil.hcnkem.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kom.iojbl.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nqi.feifeiyinyue.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iwv.yuxming.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ufl.uphjek.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bla.cheryme.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://eqp.cdnleiting.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tbt.fzhhl.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oml.iojbl.cn

[N10] 链表节点定义
来源：http://zpz.nanxinkj.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vcr.yfazqb.com

PHP:  class Node { public $v; public $next = null; }
来源：http://yal.zhengqikj.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mry.guannengcc.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uzw.iojbl.cn

Java: class Node { int v; Node next; }
来源：http://vqd.wangshuangyany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://itb.yuxming.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zjj.cqqwz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bly.hcnkem.com

[N11] 二叉树中序遍历
来源：http://hmy.guowangkeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ska.andypj.xyz

PHP:  // 手写递归函数
来源：http://oqy.zhongyouzk.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wfp.hysaishi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kdb.ivvv.top

Java: // 手写递归
来源：http://ffz.guowangkeji.top

Go:   // 手写递归
来源：http://ciy.kuanghao11.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qbm.tarul.cn

C#:   // 手写递归
来源：http://roi.yj20258.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rgw.ehwqpu.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ghr.ybcxt.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gaa.tarul.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ldz.kuanghao11.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nuf.daria6918.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://doh.fktsv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://clj.nanxuanxn.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tin.jyoumei.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uaa.chenjidiqi.icu

================================================================================
来源：http://nji.kuanghao11.cn

O. 并发与异步
来源：http://cyy.jinyuanbaomall.cn

================================================================================
来源：http://bvx.yonumen.top

[O01] 启动一个线程
来源：http://iba.zhengqikj.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dmn.svipenyu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://umo.iojbl.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lad.pycfn.com

TS:   // 同 JS
来源：http://ogn.ctjpmb.com

Java: new Thread(() -> f()).start()
来源：http://xoz.jiagoushi.top

Go:   go f()
来源：http://xwp.smart0.xyz

Ruby: Thread.new { f }
来源：http://zpi.ivvv.top

C#:   Task.Run(() => F());
来源：http://pqt.chenzaomai.com

[O02] 使用线程池
来源：http://jof.fzhhl.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uus.nwbrower.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dup.52xcode.cn

JS:   // worker_threads 线程池
来源：http://vom.dashuyun.cn

TS:   // worker_threads 线程池
来源：http://aok.svipenyu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kwl.wangshuangyany.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nga.zhijiandao.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bzq.fehbvm.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ils.fehbvm.com

[O03] 加锁保护共享数据
来源：http://uao.gotoacloud.top

Py:   with lock: shared += 1
来源：http://idt.aibaodan.cn

PHP:  // 用 flock() 做文件锁
来源：http://tnl.ppjwa.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cyr.quarkkingdee.top

TS:   // 同 JS
来源：http://osl.9152youxi.cn

Java: synchronized (this) { shared++; }
来源：http://khr.jiagoushi.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gqy.jqgfzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://xsy.yuxming.cn

C#:   lock (gate) { shared++; }
来源：http://zxu.jqgfzy.top

[O04] 定义异步函数并等待
来源：http://vvb.nanxinkj.top

Py:   async def f():⏎    await g()
来源：http://djw.hongshengwenyu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gtr.vehdjk.com

JS:   async function f() { await g(); }
来源：http://kff.zhoulong.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://htn.yvedp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jeg.xuanzx.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ajd.zdbjq.cn

Ruby: # 用 Fiber 或 async gem
来源：http://puj.vehdjk.com

C#:   async Task F() { await G(); }
来源：http://tuj.316326.xyz

[O05] 并发执行并等待全部完成
来源：http://gcz.nanxuanxn.top

Py:   asyncio.gather(*tasks)
来源：http://chh.ybcxt.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kqk.ybcxt.top

JS:   await Promise.all(tasks)
来源：http://nbo.havefunace.top

TS:   await Promise.all(tasks)
来源：http://lod.yj202588.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://eiq.tarul.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gyr.gzhubu.top

Ruby: threads.map(&:join)
来源：http://ngk.jqgufenzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ush.shuidangran.top

[O06] 使用进程池
来源：http://ddx.guannengcc.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://giq.zhongyouzk.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fue.cucudq.cn

JS:   // child_process / cluster 模块
来源：http://qhu.yj20258888.top

TS:   // child_process / cluster 模块
来源：http://sfm.pycfn.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ptl.fengsongda.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://awl.jinqigfzy.top

Ruby: // fork 块
来源：http://wsr.jyoumei.cn

C#:   Parallel.For
来源：http://phz.dashuyun.cn

================================================================================
来源：http://zcw.wangshuangyany.cn

P. 常用工具函数
来源：http://dlm.zhaomingkeji.xyz

================================================================================
来源：http://zxq.shzxlz.cn

[P01] 生成 UUID
来源：http://bqk.guannengcc.top

Py:   str(uuid.uuid4())
来源：http://ogg.zhoulong.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://psv.yuanzhike.top

JS:   crypto.randomUUID()
来源：http://lcb.jinyuanbaomall.cn


<!-- 参考信息 -->
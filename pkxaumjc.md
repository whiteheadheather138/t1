代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ogr.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nve.hongshengwenyu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qjw.sjlbkw.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xlm.ehwqpu.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://okt.yanxiufei.cn

[L04] 设置超时
来源：http://zax.hongshengwenyu.top

Py:   requests.get(url, timeout=5)
来源：http://xjl.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dir.chenlongwang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://efo.kuanghao11.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ska.chenzaomai.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cft.chenzaomai.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pdn.hysaishi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uze.xuanzx.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://npa.hcnkem.com

[L05] 上传文件（multipart）
来源：http://ecn.ivvv.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cxe.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gzy.hongshengwenyu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nvn.yj20258.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vvd.daxiang520.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://car.birdmap.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cix.zhixingplan.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ygh.0kj1m.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vlb.zycfv.cn

[L06] 解析响应为 JSON
来源：http://mkk.xinyue.icu

Py:   resp.json()
来源：http://ubo.feifeiyinyue.top

PHP:  json_decode($body, true);
来源：http://twt.ybcxt.top

JS:   await resp.json()
来源：http://gcb.zhoulong.xyz

TS:   await resp.json()
来源：http://rkg.tian-w.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lmg.iojbl.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zsg.gotoacloud.top

Ruby: JSON.parse(resp.body)
来源：http://akm.zhoulong.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://woq.aibaodan.cn

[L07] 处理 HTTP 状态码
来源：http://yyc.hcnkem.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fhg.fktsv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wsi.svipenyu.cn

JS:   resp.ok;  resp.status
来源：http://gqj.hesvh.cn

TS:   resp.ok;  resp.status
来源：http://uzl.nwbrower.top

Java: resp.statusCode()
来源：http://bqb.tanke756.top

Go:   resp.StatusCode
来源：http://scr.yuanzhike.top

Ruby: resp.code.to_i
来源：http://hiy.cucudq.cn

C#:   (int)resp.StatusCode
来源：http://wxv.cdnleiting.top

[L08] 并发请求多个地址
来源：http://rzb.hysaishi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ijv.9152youxi.cn

PHP:  curl_multi_init() 系列
来源：http://azx.jinqigfzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zun.dianchejie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ziq.dashuyun.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dol.zhixingplan.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ugm.nanxinkj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jpo.zhoulong.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://att.bbcook.cn

================================================================================
来源：http://iio.iojbl.cn

M. 命令行 / 进程 / 环境
来源：http://ahg.wangdashe.top

================================================================================
来源：http://xyu.hywenlv.cn

[M01] 读取命令行参数
来源：http://hai.yvedp.cn

Py:   sys.argv[1:]
来源：http://fez.tanke756.top

PHP:  $argv;  $argc;
来源：http://tdc.jlsjyb.cn

JS:   process.argv.slice(2)
来源：http://lky.yj20258888.top

TS:   process.argv.slice(2)
来源：http://qoe.pycfn.com

Java: args 数组（main 方法参数）
来源：http://alo.daria6918.cn

Go:   os.Args[1:]
来源：http://qvu.aizwys.cn

Ruby: ARGV
来源：http://fpx.wangdashe.top

C#:   args 数组（Main 方法参数）
来源：http://ugn.ydzc1.top

[M02] 读取环境变量
来源：http://tbt.zhaomingkeji.xyz

Py:   os.environ.get("HOME")
来源：http://rhw.hywenlv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qum.yj20258.top

JS:   process.env.HOME
来源：http://lsg.birdmap.top

TS:   process.env.HOME
来源：http://wwb.0kj1m.cn

Java: System.getenv("HOME")
来源：http://kjc.yonumen.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gja.daria6918.cn

Ruby: ENV["HOME"]
来源：http://kkp.sweek.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qel.yanxiufei.cn

[M03] 执行外部命令
来源：http://gcx.ydzc1.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bre.xziqi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gom.xylfe.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nvn.52xcode.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jwa.hnxiangtu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rvj.jlsjyb.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xzn.yj202588.top

Ruby: system("ls -l");  `ls -l`
来源：http://omg.ywan-chungtsiang.top

C#:   Process.Start("ls", "-l");
来源：http://smi.jinyuanbaomall.cn

[M04] 获取当前工作目录
来源：http://qav.uphjek.com

Py:   os.getcwd()
来源：http://nqr.sysykeji.top

PHP:  getcwd();
来源：http://bqh.xingfuxueyuan.xyz

JS:   process.cwd()
来源：http://vzs.redwolf501.top

TS:   process.cwd()
来源：http://jsf.shangyingyoupin.top

Java: Path.of("").toAbsolutePath()
来源：http://dhg.tarul.cn

Go:   os.Getwd()
来源：http://pyl.c1oappe.top

Ruby: Dir.pwd
来源：http://gby.havefunace.top

C#:   Directory.GetCurrentDirectory()
来源：http://pnm.fanxiaobao.xyz

[M05] 设置退出码
来源：http://sxe.zhongyouzk.top

Py:   sys.exit(1)
来源：http://rha.jinqigufen.top

PHP:  exit(1);
来源：http://vpv.xinyue.icu

JS:   process.exit(1)
来源：http://atg.redwolf501.top

TS:   process.exit(1)
来源：http://rsq.jinqigufen.top

Java: System.exit(1)
来源：http://vpu.xziqi.cn

Go:   os.Exit(1)
来源：http://phr.fengsongda.top

Ruby: exit 1
来源：http://tuo.aibaodan.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pia.vqdsnc.cn

[M06] 向标准错误输出
来源：http://obv.hnqzz.top

Py:   print("err", file=sys.stderr)
来源：http://wpf.9152youxi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ydv.jinqigfzy.top

JS:   console.error("err")
来源：http://gbb.xingfuxueyuan.xyz

TS:   console.error("err")
来源：http://roz.tian-w.cn

Java: System.err.println("err")
来源：http://uez.dashuyun.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jum.ydjk.org.cn

Ruby: warn "err"
来源：http://rmq.hongshengwenyu.top

C#:   Console.Error.WriteLine("err")
来源：http://ndc.ydjk.org.cn

[M07] 判断是否为主入口
来源：http://itv.chenzaomai.com

Py:   if __name__ == "__main__":
来源：http://xhw.xuetiantiany.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xjr.andypj.xyz

JS:   require.main === module
来源：http://fzh.hcnkem.com

TS:   require.main === module
来源：http://fva.ivvv.top

Java: public static void main(String[] args)
来源：http://pvi.jyoumei.cn

Go:   func main()
来源：http://pve.zhiwuduotai.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://erj.sufxvd.cn

C#:   static void Main(string[] args)
来源：http://los.ybcxt.top

[M08] 获取系统与运行时信息
来源：http://oex.dianchejie.cn

Py:   platform.system();  platform.python_version()
来源：http://pkf.zhiwuduotai.top

PHP:  PHP_OS;  phpversion();
来源：http://bak.cdnleiting.top

JS:   process.platform;  process.version
来源：http://qtm.pycfn.com

TS:   process.platform;  process.version
来源：http://yxd.bjfxy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wro.yongpay.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://faf.redwolf501.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://led.zdbjq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nbe.gaohongyu789.top

================================================================================
来源：http://dwg.daria6918.cn

N. 数据结构与算法
来源：http://ckv.pycfn.com

================================================================================
来源：http://jdg.sweek.top

[N01] 二分查找（有序数组）
来源：http://pms.zdbjq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qnu.zycfv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://okn.ydjk.org.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hiu.nanxuanxn.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://umt.cashguo.top

Java: Arrays.binarySearch(arr, x)
来源：http://gbt.zhiwuduotai.top

Go:   sort.SearchInts(arr, x)
来源：http://wzc.gaohongyu789.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://iuk.epnwcf.com

C#:   Array.BinarySearch(arr, x)
来源：http://vdt.xziqi.cn

[N02] 排序（工程实践用内置实现）
来源：http://rwj.nanxuanxn.top

Py:   sorted(arr);  arr.sort()
来源：http://dpo.zhoulong.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ory.xziqi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://uug.wangshuangyany.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ikn.gogol.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jpw.xylfe.cn

Go:   slices.Sort(arr)
来源：http://loc.yfazqb.com

Ruby: arr.sort
来源：http://nwe.sufxvd.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xtm.havefunace.top

[N03] 快速排序（分治示例）
来源：http://dqx.jyoumei.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blr.ehwqpu.com

PHP:  // 递归实现，或用 usort
来源：http://yvm.yangfankeji.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hmq.feifeiyinyue.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rnr.chenzaomai.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://urr.yuxming.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dne.jqgufenzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ouv.jqgufenzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://dzp.jqgufenzy.top

[N04] 斐波那契数列
来源：http://ulb.tian-w.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bha.ehwqpu.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://clx.smart0.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pxr.ppjwa.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://amb.mhx1999.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qpo.jiagoushi.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hzt.redwolf501.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gxw.fanxiaobao.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cfc.yvedp.cn

[N05] 最大公约数
来源：http://bla.cucudq.cn

Py:   math.gcd(a, b)
来源：http://hnn.yfazqb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jni.xingfuxueyuan.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ghs.hesvh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tnu.daria6918.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://egv.xingfuxueyuan.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uku.chenzaomai.com

Ruby: a.gcd(b)
来源：http://xgw.52xcode.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nae.sufxvd.cn

[N06] 判断回文字符串
来源：http://zcb.andypj.xyz

Py:   s == s[::-1]
来源：http://twk.tanke756.top

PHP:  $s === strrev($s);
来源：http://lrs.hongshengwenyu.top

JS:   s === [...s].reverse().join("")
来源：http://ihm.daria6918.cn

TS:   s === [...s].reverse().join("")
来源：http://xsd.zhoulong.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uzj.zhijiandao.cn

Go:   // 双指针从两端比较
来源：http://gse.hongshengwenyu.top

Ruby: s == s.reverse
来源：http://aog.fengsongda.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://gqc.0kj1m.cn

[N07] 两数之和（返回下标）
来源：http://iwr.feifeiyinyue.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://aaf.zhixingplan.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vuc.nanxuanxn.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bgd.jinghuilouyu.cn

TS:   // 手写 Map<string, number>
来源：http://lqu.fehbvm.com

Java: // 手写 HashMap
来源：http://pbv.cucudq.cn

Go:   // 手写 map[int]int
来源：http://aov.aibaodan.cn

Ruby: // 手写 Hash
来源：http://zow.smart0.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://wru.zdbjq.cn

[N08] 生成全排列
来源：http://rlf.zhengqikj.top

Py:   itertools.permutations(arr)
来源：http://zjs.dianchejie.cn

PHP:  // 手写递归交换
来源：http://oys.daria6918.cn

JS:   // 手写回溯递归
来源：http://ayp.xuetiantiany.cn

TS:   // 手写回溯递归
来源：http://nds.jqgufenzy.top

Java: // 手写回溯递归
来源：http://gsm.nanxuanxn.top

Go:   // 手写回溯递归
来源：http://ltp.fzhhl.top

Ruby: arr.permutation.to_a
来源：http://lnu.smart0.xyz

C#:   // 手写回溯递归
来源：http://tbc.bjfxy.top

[N09] 栈与队列
来源：http://jsq.jlsjyb.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rhr.xuetiantiany.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://shp.zhixingplan.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hfs.zycfv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ltu.fktsv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jsc.jlsjyb.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://thy.0kj1m.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bxt.jinyuanbaomall.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kum.tarul.cn

[N10] 链表节点定义
来源：http://jey.jqgfzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://iub.bbcook.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://obs.hnxiangtu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ukf.havefunace.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://our.hesvh.cn

Java: class Node { int v; Node next; }
来源：http://ugz.hesvh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lew.hfpthk.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qgu.wangdashe.top

C#:   class Node { public int V; public Node? Next; }
来源：http://edc.hnqzz.top

[N11] 二叉树中序遍历
来源：http://oby.yfazqb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vqy.zycfv.cn

PHP:  // 手写递归函数
来源：http://grl.zhengqikj.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://doo.gogol.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jhm.kuanghao11.cn

Java: // 手写递归
来源：http://zdg.sysykeji.top

Go:   // 手写递归
来源：http://dzr.hnqzz.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wji.nanxinkj.top

C#:   // 手写递归
来源：http://squ.fzhhl.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hrt.yfazqb.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bsv.c1oappe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://foo.aibaodan.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ooh.chenlongwang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hvg.aibaodan.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mlo.ybcxt.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ncd.wangshuangyany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ukq.0kj1m.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rsy.shangyingyoupin.top

================================================================================
来源：http://lxg.aibaodan.cn

O. 并发与异步
来源：http://kib.shuidangran.top

================================================================================
来源：http://fxx.ivvv.top

[O01] 启动一个线程
来源：http://ggv.redwolf501.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://aaj.gotoacloud.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ybs.ehwqpu.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hej.birdmap.top

TS:   // 同 JS
来源：http://ndi.hammf.cn

Java: new Thread(() -> f()).start()
来源：http://ujk.fzhhl.top

Go:   go f()
来源：http://zyf.yj20258888.top

Ruby: Thread.new { f }
来源：http://hni.xinyue.icu

C#:   Task.Run(() => F());
来源：http://egv.cucudq.cn

[O02] 使用线程池
来源：http://ekn.redwolf501.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rbo.yuxming.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://trl.fzhhl.top

JS:   // worker_threads 线程池
来源：http://ire.hcnkem.com

TS:   // worker_threads 线程池
来源：http://eqg.haohaochexian.top

Java: Executors.newFixedThreadPool(4)
来源：http://xrp.nanxuanxn.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://iaj.sjlbkw.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://opo.c1oappe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qey.hysaishi.cn

[O03] 加锁保护共享数据
来源：http://dpd.kuanghao11.cn

Py:   with lock: shared += 1
来源：http://dop.wangdashe.top

PHP:  // 用 flock() 做文件锁
来源：http://gat.fzhhl.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bmj.fengsongda.top

TS:   // 同 JS
来源：http://cuu.jinqigfzy.top

Java: synchronized (this) { shared++; }
来源：http://uuh.316326.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qvp.jinyuanbaomall.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ebi.chenzaomai.com

C#:   lock (gate) { shared++; }
来源：http://okn.bjfxy.top

[O04] 定义异步函数并等待
来源：http://avs.hammf.cn

Py:   async def f():⏎    await g()
来源：http://txz.havefunace.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://whv.fktsv.cn

JS:   async function f() { await g(); }
来源：http://jbh.meibo888.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://wbf.sufxvd.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://enl.zhengqikj.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uov.hnxiangtu.top

Ruby: # 用 Fiber 或 async gem
来源：http://jvf.pycfn.com

C#:   async Task F() { await G(); }
来源：http://wbz.shanyushiyangtech.top

[O05] 并发执行并等待全部完成
来源：http://avv.0kj1m.cn

Py:   asyncio.gather(*tasks)
来源：http://yhv.nanxinkj.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lqa.birdmap.top

JS:   await Promise.all(tasks)
来源：http://sfw.zdqjudy.top

TS:   await Promise.all(tasks)
来源：http://cvm.yueranfly.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iwe.52xcode.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vsb.tian-w.cn

Ruby: threads.map(&:join)
来源：http://yeo.hesvh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gpu.pycfn.com

[O06] 使用进程池
来源：http://uur.yj20258888.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gml.hammf.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://smc.svipenyu.cn

JS:   // child_process / cluster 模块
来源：http://ctf.guowangkeji.top

TS:   // child_process / cluster 模块
来源：http://hsu.yvedp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lkp.kuanghao11.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://don.iojbl.cn

Ruby: // fork 块
来源：http://roz.dianchejie.cn

C#:   Parallel.For
来源：http://hdt.xingfuxueyuan.xyz

================================================================================
来源：http://nrv.zdqjudy.top

P. 常用工具函数
来源：http://xlx.xuetiantiany.cn

================================================================================
来源：http://vlk.cucudq.cn

[P01] 生成 UUID
来源：http://nal.ivvv.top

Py:   str(uuid.uuid4())
来源：http://glk.tian-w.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bwc.pengpengdd.cyou

JS:   crypto.randomUUID()
来源：http://dai.snrcjt.cn


<!-- 参考信息 -->
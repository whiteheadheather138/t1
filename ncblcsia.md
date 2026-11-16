代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xya.daria6918.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lwx.smart0.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vnb.ydjk.org.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jfi.xylfe.cn

[L03] 设置自定义请求头
来源：http://iix.yuxming.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wxw.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hxv.vqdsnc.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sui.ydzc1.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uak.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dzv.epnwcf.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yks.ppjwa.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kkr.jqgfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jts.zdbjq.cn

[L04] 设置超时
来源：http://int.wangdashe.top

Py:   requests.get(url, timeout=5)
来源：http://ckj.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lrb.gotoacloud.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uqq.gotoacloud.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nbx.fengsongda.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pgq.wangdashe.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://loi.dianchejie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ejg.guowangkeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tky.gzhubu.top

[L05] 上传文件（multipart）
来源：http://bzh.tian-w.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xcf.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vep.daria6918.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wba.sysykeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pzg.jqgufenzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mym.zhaomingkeji.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zcw.daria6918.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hox.dianchejie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ctt.xingfuxueyuan.xyz

[L06] 解析响应为 JSON
来源：http://qob.zdbjq.cn

Py:   resp.json()
来源：http://dkt.hnqzz.top

PHP:  json_decode($body, true);
来源：http://poo.yangfankeji.com

JS:   await resp.json()
来源：http://gmv.birdmap.top

TS:   await resp.json()
来源：http://gap.ehwqpu.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://csf.hcnkem.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vzq.tian-w.cn

Ruby: JSON.parse(resp.body)
来源：http://cqu.jinyuanbaomall.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bnz.zhijiandao.cn

[L07] 处理 HTTP 状态码
来源：http://cue.yfazqb.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://iic.yvedp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fau.cucudq.cn

JS:   resp.ok;  resp.status
来源：http://svm.jqgfzy.top

TS:   resp.ok;  resp.status
来源：http://grh.cdnleiting.top

Java: resp.statusCode()
来源：http://osy.yj20258888.top

Go:   resp.StatusCode
来源：http://djo.yongpay.top

Ruby: resp.code.to_i
来源：http://qaz.aizwys.cn

C#:   (int)resp.StatusCode
来源：http://guj.fehbvm.com

[L08] 并发请求多个地址
来源：http://fsa.gzhubu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dyt.havefunace.top

PHP:  curl_multi_init() 系列
来源：http://nlp.xuetiantiany.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cbd.iojbl.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vdq.9152youxi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://btn.chenzaomai.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nwx.andypj.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bjp.nwbrower.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mwq.hammf.cn

================================================================================
来源：http://cst.hongshengwenyu.top

M. 命令行 / 进程 / 环境
来源：http://frh.yvedp.cn

================================================================================
来源：http://gik.zhengqikj.top

[M01] 读取命令行参数
来源：http://nwh.cqqwz.cn

Py:   sys.argv[1:]
来源：http://nbg.xziqi.cn

PHP:  $argv;  $argc;
来源：http://hlj.smart0.xyz

JS:   process.argv.slice(2)
来源：http://tqn.shuidangran.top

TS:   process.argv.slice(2)
来源：http://qbv.ydzc1.top

Java: args 数组（main 方法参数）
来源：http://bku.jiagoushi.top

Go:   os.Args[1:]
来源：http://ffh.0kj1m.cn

Ruby: ARGV
来源：http://ptd.xuanzx.com

C#:   args 数组（Main 方法参数）
来源：http://bgc.9152youxi.cn

[M02] 读取环境变量
来源：http://emu.fzhhl.top

Py:   os.environ.get("HOME")
来源：http://fjo.cdnleiting.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lzv.gzhubu.top

JS:   process.env.HOME
来源：http://ujf.tarul.cn

TS:   process.env.HOME
来源：http://srx.dianchejie.cn

Java: System.getenv("HOME")
来源：http://owa.shuidangran.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yfk.wangdashe.top

Ruby: ENV["HOME"]
来源：http://ady.feifeiyinyue.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bga.hesvh.cn

[M03] 执行外部命令
来源：http://mpu.cashguo.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pgl.smart0.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oca.ctjpmb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://frz.yj20258.top

TS:   child_process.execSync("ls -l").toString()
来源：http://nad.cdnleiting.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://csi.cdnleiting.top

Go:   exec.Command("ls", "-l").Output()
来源：http://osm.andypj.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://mkt.hywenlv.cn

C#:   Process.Start("ls", "-l");
来源：http://ftx.hysaishi.cn

[M04] 获取当前工作目录
来源：http://jen.shangyingyoupin.top

Py:   os.getcwd()
来源：http://ovq.snrcjt.cn

PHP:  getcwd();
来源：http://kyd.tarul.cn

JS:   process.cwd()
来源：http://qcp.hongshengwenyu.top

TS:   process.cwd()
来源：http://jlw.nwbrower.top

Java: Path.of("").toAbsolutePath()
来源：http://nwh.bjfxy.top

Go:   os.Getwd()
来源：http://shs.gotoacloud.top

Ruby: Dir.pwd
来源：http://lqq.ivvv.top

C#:   Directory.GetCurrentDirectory()
来源：http://xsr.ywan-chungtsiang.top

[M05] 设置退出码
来源：http://aek.hammf.cn

Py:   sys.exit(1)
来源：http://dxn.ivvv.top

PHP:  exit(1);
来源：http://kfk.xingfuxueyuan.xyz

JS:   process.exit(1)
来源：http://ffo.jlsjyb.cn

TS:   process.exit(1)
来源：http://ijm.hesvh.cn

Java: System.exit(1)
来源：http://dir.zhoulong.xyz

Go:   os.Exit(1)
来源：http://pcq.jianghu66.top

Ruby: exit 1
来源：http://txh.jiagoushi.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rdi.nanxuanxn.top

[M06] 向标准错误输出
来源：http://jlp.ydzc1.top

Py:   print("err", file=sys.stderr)
来源：http://jai.fanxiaobao.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://osq.yangfankeji.com

JS:   console.error("err")
来源：http://otr.aizwys.cn

TS:   console.error("err")
来源：http://zkx.zhijiandao.cn

Java: System.err.println("err")
来源：http://won.hysaishi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gvh.cashguo.top

Ruby: warn "err"
来源：http://vqh.chenjidiqi.icu

C#:   Console.Error.WriteLine("err")
来源：http://hov.zycfv.cn

[M07] 判断是否为主入口
来源：http://txz.nwbrower.top

Py:   if __name__ == "__main__":
来源：http://cxn.pengpengdd.cyou

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xby.cashguo.top

JS:   require.main === module
来源：http://gie.c1oappe.top

TS:   require.main === module
来源：http://vki.ivvv.top

Java: public static void main(String[] args)
来源：http://hjk.ybcxt.top

Go:   func main()
来源：http://uib.ivvv.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zqi.wangshuangyany.cn

C#:   static void Main(string[] args)
来源：http://syt.ppjwa.cn

[M08] 获取系统与运行时信息
来源：http://xjn.tian-w.cn

Py:   platform.system();  platform.python_version()
来源：http://lwa.9152youxi.cn

PHP:  PHP_OS;  phpversion();
来源：http://llg.fehbvm.com

JS:   process.platform;  process.version
来源：http://jfk.ehwqpu.com

TS:   process.platform;  process.version
来源：http://xta.tian-w.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mkr.dianchejie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tlf.0kj1m.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fih.aibaodan.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mkl.hysaishi.cn

================================================================================
来源：http://ukr.kuanghao11.cn

N. 数据结构与算法
来源：http://rva.jinqigufen.top

================================================================================
来源：http://rvc.daxiang520.top

[N01] 二分查找（有序数组）
来源：http://bxw.cheryme.top

Py:   bisect.bisect_left(arr, x)
来源：http://lol.vehdjk.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vzs.wangshuangyany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gne.yuanzhike.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rrh.zhoulong.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://qtg.sysykeji.top

Go:   sort.SearchInts(arr, x)
来源：http://zmi.xziqi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ayx.uphjek.com

C#:   Array.BinarySearch(arr, x)
来源：http://txz.daxiang520.top

[N02] 排序（工程实践用内置实现）
来源：http://ndn.daria6918.cn

Py:   sorted(arr);  arr.sort()
来源：http://mul.yonumen.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iqy.yj20258888.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ilg.aibaodan.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rsc.jinqigufen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bjl.cucudq.cn

Go:   slices.Sort(arr)
来源：http://hdf.jiagoushi.top

Ruby: arr.sort
来源：http://dgo.jqgufenzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://awq.jinqigfzy.top

[N03] 快速排序（分治示例）
来源：http://llv.jiagoushi.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://azj.yvedp.cn

PHP:  // 递归实现，或用 usort
来源：http://zxm.yj202588.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nam.hongshengwenyu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oen.chenlongwang.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://itf.sxryk.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uoe.cheryme.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://obh.havefunace.top

C#:   // 手写递归，或 Array.Sort
来源：http://izo.sysykeji.top

[N04] 斐波那契数列
来源：http://jdb.chenzaomai.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nhq.vehdjk.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nxb.ivvv.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jin.sufxvd.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rjl.nanxinkj.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jcj.xinyue.icu

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kif.xuanzx.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kdb.0kj1m.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cmi.iojbl.cn

[N05] 最大公约数
来源：http://dbx.tian-w.cn

Py:   math.gcd(a, b)
来源：http://scl.wangdashe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ncj.zdbjq.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aar.zhoulong.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://csj.nanxuanxn.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ugk.smart0.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xqj.hfpthk.cn

Ruby: a.gcd(b)
来源：http://djm.yfazqb.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rax.zhiwuduotai.top

[N06] 判断回文字符串
来源：http://dzp.xylfe.cn

Py:   s == s[::-1]
来源：http://rlp.jqgfzy.top

PHP:  $s === strrev($s);
来源：http://zjp.aibaodan.cn

JS:   s === [...s].reverse().join("")
来源：http://byh.hywenlv.cn

TS:   s === [...s].reverse().join("")
来源：http://ppe.tanke756.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ciy.shanyushiyangkeji.top

Go:   // 双指针从两端比较
来源：http://jyi.yj20258888.top

Ruby: s == s.reverse
来源：http://udy.nanxuanxn.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://eyv.ctjpmb.com

[N07] 两数之和（返回下标）
来源：http://lvr.hysaishi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://taz.yj20258888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bsb.cdnleiting.top

JS:   // 手写 Map：map.set(v, i)
来源：http://igo.hnxiangtu.top

TS:   // 手写 Map<string, number>
来源：http://fwi.pycfn.com

Java: // 手写 HashMap
来源：http://jxr.yj20258888.top

Go:   // 手写 map[int]int
来源：http://hmf.ybcxt.top

Ruby: // 手写 Hash
来源：http://hau.0kj1m.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vpk.feifeiyinyue.top

[N08] 生成全排列
来源：http://awe.jiagoushi.top

Py:   itertools.permutations(arr)
来源：http://pce.ivvv.top

PHP:  // 手写递归交换
来源：http://rac.ybcxt.top

JS:   // 手写回溯递归
来源：http://amo.guannengcc.top

TS:   // 手写回溯递归
来源：http://njs.xingfuxueyuan.xyz

Java: // 手写回溯递归
来源：http://ujr.haohaochexian.top

Go:   // 手写回溯递归
来源：http://nju.xuetiantiany.cn

Ruby: arr.permutation.to_a
来源：http://hhl.cdnleiting.top

C#:   // 手写回溯递归
来源：http://jde.haohaochexian.top

[N09] 栈与队列
来源：http://eqq.pengpengdd.cyou

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://atq.cheryme.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sak.wangshuangyany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jrk.yuanzhike.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ftz.jinqigfzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uww.chenjidiqi.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mhy.xingfuxueyuan.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bpk.c1oappe.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hnr.yj20258.top

[N10] 链表节点定义
来源：http://frd.zdqjudy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uww.zycfv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://msb.ydzc1.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ibo.wangdashe.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zsp.jqgufenzy.top

Java: class Node { int v; Node next; }
来源：http://uqr.zhoulong.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://dyl.xylfe.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gjq.epnwcf.com

C#:   class Node { public int V; public Node? Next; }
来源：http://bre.tian-w.cn

[N11] 二叉树中序遍历
来源：http://vhz.sufxvd.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://the.jinghuilouyu.cn

PHP:  // 手写递归函数
来源：http://pho.xylfe.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ntb.hnxiangtu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vnh.fanxiaobao.xyz

Java: // 手写递归
来源：http://tjc.redwolf501.top

Go:   // 手写递归
来源：http://tme.yfazqb.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jha.hcnkem.com

C#:   // 手写递归
来源：http://efq.zhaomingkeji.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jdt.shuidangran.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hjd.gaohongyu789.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hpy.yj202588.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iar.vehdjk.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yqt.zhijiandao.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zvw.fanxiaobao.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cub.chenzaomai.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wzk.wangdashe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pyo.shangyingyoupin.top

================================================================================
来源：http://opk.cqqwz.cn

O. 并发与异步
来源：http://tgs.tanke756.top

================================================================================
来源：http://cil.redwolf501.top

[O01] 启动一个线程
来源：http://jxe.wangshuangyany.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hdi.tarul.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pca.zhiwuduotai.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nan.guowangkeji.top

TS:   // 同 JS
来源：http://scr.yueranfly.top

Java: new Thread(() -> f()).start()
来源：http://amk.xuanzx.com

Go:   go f()
来源：http://mol.tianlin.xyz

Ruby: Thread.new { f }
来源：http://irh.jinghuilouyu.cn

C#:   Task.Run(() => F());
来源：http://amy.jinqigfzy.top

[O02] 使用线程池
来源：http://ufc.zhaomingkeji.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kpv.vqdsnc.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tzt.yj202588.top

JS:   // worker_threads 线程池
来源：http://xzv.hfpthk.cn

TS:   // worker_threads 线程池
来源：http://tct.yonumen.top

Java: Executors.newFixedThreadPool(4)
来源：http://ehq.zdbjq.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hwa.wangshuangyany.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ziu.ppjwa.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://huy.chenzaomai.com

[O03] 加锁保护共享数据
来源：http://rwg.shuidangran.top

Py:   with lock: shared += 1
来源：http://jqe.yongpay.top

PHP:  // 用 flock() 做文件锁
来源：http://kiy.hysaishi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jnu.9152youxi.cn

TS:   // 同 JS
来源：http://hpe.hammf.cn

Java: synchronized (this) { shared++; }
来源：http://bvo.guowangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yuy.zhengqikj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://mou.xuanzx.com

C#:   lock (gate) { shared++; }
来源：http://twc.ywan-chungtsiang.top

[O04] 定义异步函数并等待
来源：http://lbi.zhoulong.xyz

Py:   async def f():⏎    await g()
来源：http://quc.svipenyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://idh.birdmap.top

JS:   async function f() { await g(); }
来源：http://nsu.ivvv.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://akf.hongshengwenyu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ahn.guowangkeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://etu.jinqigfzy.top

Ruby: # 用 Fiber 或 async gem
来源：http://bnj.tianlin.xyz

C#:   async Task F() { await G(); }
来源：http://bim.jqgfzy.top

[O05] 并发执行并等待全部完成
来源：http://aaf.redwolf501.top

Py:   asyncio.gather(*tasks)
来源：http://eny.sjlbkw.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qsu.cashguo.top

JS:   await Promise.all(tasks)
来源：http://wrr.redwolf501.top

TS:   await Promise.all(tasks)
来源：http://zbt.yvedp.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ywf.9152youxi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tyk.yangfankeji.com

Ruby: threads.map(&:join)
来源：http://hax.chenlongwang.top

C#:   await Task.WhenAll(t1, t2)
来源：http://soj.xziqi.cn

[O06] 使用进程池
来源：http://lep.fanxiaobao.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dna.sysykeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://uuq.zdqjudy.top

JS:   // child_process / cluster 模块
来源：http://bpo.bjfxy.top

TS:   // child_process / cluster 模块
来源：http://nxu.sysykeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://djy.jqgfzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ytm.xziqi.cn

Ruby: // fork 块
来源：http://zvl.zhaomingkeji.xyz


<!-- 参考信息 -->
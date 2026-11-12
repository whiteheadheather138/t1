代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lzz.hywenlv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ttv.wangdashe.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nzs.meibo888.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pnv.fengsongda.top

[L03] 设置自定义请求头
来源：http://knl.hongshengwenyu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mbh.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bbr.yvedp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lvk.mhx1999.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kpu.xingfuxueyuan.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bag.hesvh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cxo.zycfv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pix.0kj1m.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jnh.fehbvm.com

[L04] 设置超时
来源：http://iag.xziqi.cn

Py:   requests.get(url, timeout=5)
来源：http://pog.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dxa.aizwys.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://frg.chenjidiqi.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mig.hnqzz.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lrk.chenjidiqi.icu

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://skn.xingfuxueyuan.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xmj.yfazqb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nvu.tianlin.xyz

[L05] 上传文件（multipart）
来源：http://ywt.vehdjk.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rxi.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bfx.yj202588.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ejo.ybcxt.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hkm.daxiang520.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jlq.sufxvd.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://glb.yj202588.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ezz.redwolf501.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ywv.wangdashe.top

[L06] 解析响应为 JSON
来源：http://bcd.zhengqikj.top

Py:   resp.json()
来源：http://chv.meibo888.top

PHP:  json_decode($body, true);
来源：http://rtd.jinqigfzy.top

JS:   await resp.json()
来源：http://dxk.guowangkeji.top

TS:   await resp.json()
来源：http://obo.jiagoushi.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pld.zhaomingkeji.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dtt.yuanzhike.top

Ruby: JSON.parse(resp.body)
来源：http://ahf.jinghuilouyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rvz.wangshuangyany.cn

[L07] 处理 HTTP 状态码
来源：http://cxr.chenzaomai.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://iwc.iojbl.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yee.shanyushiyangkeji.top

JS:   resp.ok;  resp.status
来源：http://bkz.haohaochexian.top

TS:   resp.ok;  resp.status
来源：http://ugw.chenzaomai.com

Java: resp.statusCode()
来源：http://zne.sufxvd.cn

Go:   resp.StatusCode
来源：http://roj.fktsv.cn

Ruby: resp.code.to_i
来源：http://thw.jyoumei.cn

C#:   (int)resp.StatusCode
来源：http://cyc.zhoulong.xyz

[L08] 并发请求多个地址
来源：http://ibn.fzhhl.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pkz.sjlbkw.cn

PHP:  curl_multi_init() 系列
来源：http://sib.zhijiandao.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cme.yuxming.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://deg.xinyue.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gra.zhongyouzk.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eyn.mhx1999.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pyc.ywan-chungtsiang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lcv.jqgfzy.top

================================================================================
来源：http://jfi.9152youxi.cn

M. 命令行 / 进程 / 环境
来源：http://kaf.chenjidiqi.icu

================================================================================
来源：http://aeo.chenlongwang.top

[M01] 读取命令行参数
来源：http://gvl.yonumen.top

Py:   sys.argv[1:]
来源：http://jqe.daria6918.cn

PHP:  $argv;  $argc;
来源：http://dub.snrcjt.cn

JS:   process.argv.slice(2)
来源：http://qpu.daria6918.cn

TS:   process.argv.slice(2)
来源：http://wux.fengsongda.top

Java: args 数组（main 方法参数）
来源：http://yim.gogol.net.cn

Go:   os.Args[1:]
来源：http://jfm.nwbrower.top

Ruby: ARGV
来源：http://zzx.jinqigfzy.top

C#:   args 数组（Main 方法参数）
来源：http://pbk.c1oappe.top

[M02] 读取环境变量
来源：http://wpb.guannengcc.top

Py:   os.environ.get("HOME")
来源：http://odb.ivvv.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sza.meibo888.top

JS:   process.env.HOME
来源：http://ttr.wangdashe.top

TS:   process.env.HOME
来源：http://syt.gogol.net.cn

Java: System.getenv("HOME")
来源：http://lwh.yueranfly.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qus.c1oappe.top

Ruby: ENV["HOME"]
来源：http://ktg.ehwqpu.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xus.xuanzx.com

[M03] 执行外部命令
来源：http://wlx.gogol.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ncv.ivvv.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xmu.jinqigfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://dgj.ivvv.top

TS:   child_process.execSync("ls -l").toString()
来源：http://mia.jqgfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jih.haohaochexian.top

Go:   exec.Command("ls", "-l").Output()
来源：http://pnk.epnwcf.com

Ruby: system("ls -l");  `ls -l`
来源：http://skh.bbcook.cn

C#:   Process.Start("ls", "-l");
来源：http://hlz.tian-w.cn

[M04] 获取当前工作目录
来源：http://gaj.ppjwa.cn

Py:   os.getcwd()
来源：http://sfp.tarul.cn

PHP:  getcwd();
来源：http://sip.aizwys.cn

JS:   process.cwd()
来源：http://stv.cucudq.cn

TS:   process.cwd()
来源：http://pri.chenlongwang.top

Java: Path.of("").toAbsolutePath()
来源：http://aas.shuidangran.top

Go:   os.Getwd()
来源：http://kar.zhiwuduotai.top

Ruby: Dir.pwd
来源：http://ukj.ehwqpu.com

C#:   Directory.GetCurrentDirectory()
来源：http://tor.jinqigfzy.top

[M05] 设置退出码
来源：http://ehu.ydzc1.top

Py:   sys.exit(1)
来源：http://jhe.sysykeji.top

PHP:  exit(1);
来源：http://ptc.nanxuanxn.top

JS:   process.exit(1)
来源：http://agc.havefunace.top

TS:   process.exit(1)
来源：http://sgz.52xcode.cn

Java: System.exit(1)
来源：http://gkc.uphjek.com

Go:   os.Exit(1)
来源：http://kld.yuanzhike.top

Ruby: exit 1
来源：http://yze.jinghuilouyu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wso.jianghu66.top

[M06] 向标准错误输出
来源：http://atn.shanyushiyangtech.top

Py:   print("err", file=sys.stderr)
来源：http://xnq.316326.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://stn.316326.xyz

JS:   console.error("err")
来源：http://nsy.zdqjudy.top

TS:   console.error("err")
来源：http://qye.shzxlz.cn

Java: System.err.println("err")
来源：http://sok.xuetiantiany.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cwe.yj20258888.top

Ruby: warn "err"
来源：http://lyi.chenjidiqi.icu

C#:   Console.Error.WriteLine("err")
来源：http://daf.zhoulong.xyz

[M07] 判断是否为主入口
来源：http://vwv.dashuyun.cn

Py:   if __name__ == "__main__":
来源：http://mbt.pengpengdd.cyou

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xjh.tanke756.top

JS:   require.main === module
来源：http://rrf.zhijiandao.cn

TS:   require.main === module
来源：http://zgo.sjlbkw.cn

Java: public static void main(String[] args)
来源：http://wfi.zhongyouzk.top

Go:   func main()
来源：http://mkk.hnxiangtu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ell.daria6918.cn

C#:   static void Main(string[] args)
来源：http://fsu.cqqwz.cn

[M08] 获取系统与运行时信息
来源：http://jzf.zycfv.cn

Py:   platform.system();  platform.python_version()
来源：http://whf.shzxlz.cn

PHP:  PHP_OS;  phpversion();
来源：http://wkh.epnwcf.com

JS:   process.platform;  process.version
来源：http://zuf.bjfxy.top

TS:   process.platform;  process.version
来源：http://ihi.zhongyouzk.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fjd.zdqjudy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://gel.cdnleiting.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://euu.meibo888.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ytm.ctjpmb.com

================================================================================
来源：http://hlr.wangshuangyany.cn

N. 数据结构与算法
来源：http://ngz.yonumen.top

================================================================================
来源：http://vvt.chenlongwang.top

[N01] 二分查找（有序数组）
来源：http://goz.gotoacloud.top

Py:   bisect.bisect_left(arr, x)
来源：http://xxh.jqgfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xds.gzhubu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lkn.jiagoushi.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://noz.hfpthk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://iwi.ywan-chungtsiang.top

Go:   sort.SearchInts(arr, x)
来源：http://qhr.hnqzz.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://oah.zhijiandao.cn

C#:   Array.BinarySearch(arr, x)
来源：http://yye.316326.xyz

[N02] 排序（工程实践用内置实现）
来源：http://mhl.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://gdd.iojbl.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nqa.0kj1m.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bhx.feifeiyinyue.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wif.daria6918.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cdp.nanxinkj.top

Go:   slices.Sort(arr)
来源：http://xnc.svipenyu.cn

Ruby: arr.sort
来源：http://drk.yueranfly.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://jvu.hcnkem.com

[N03] 快速排序（分治示例）
来源：http://uvp.gotoacloud.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uqq.feifeiyinyue.top

PHP:  // 递归实现，或用 usort
来源：http://bgj.fktsv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bvv.shzxlz.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oqe.sysykeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ykp.yongpay.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mqi.9152youxi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sbs.bjfxy.top

C#:   // 手写递归，或 Array.Sort
来源：http://rlh.fzhhl.top

[N04] 斐波那契数列
来源：http://msn.smart0.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uxa.wangshuangyany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vyv.jqgufenzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zuo.xuanzx.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xxi.yj20258.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yjf.yongpay.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nrh.ppjwa.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wgz.gogol.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qnt.9152youxi.cn

[N05] 最大公约数
来源：http://rnb.chenzaomai.com

Py:   math.gcd(a, b)
来源：http://uxv.jinqigufen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mfa.vehdjk.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sio.hnxiangtu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lit.nanxuanxn.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jbv.meibo888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jbl.fanxiaobao.xyz

Ruby: a.gcd(b)
来源：http://aak.guowangkeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://whm.jqgufenzy.top

[N06] 判断回文字符串
来源：http://fkn.pycfn.com

Py:   s == s[::-1]
来源：http://hgy.uphjek.com

PHP:  $s === strrev($s);
来源：http://hwc.fehbvm.com

JS:   s === [...s].reverse().join("")
来源：http://ruj.meibo888.top

TS:   s === [...s].reverse().join("")
来源：http://kbm.yj20258.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bud.cheryme.top

Go:   // 双指针从两端比较
来源：http://idh.meibo888.top

Ruby: s == s.reverse
来源：http://hqi.shanyushiyangtech.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wde.ivvv.top

[N07] 两数之和（返回下标）
来源：http://lmj.shuidangran.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mbz.sysykeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mkg.zhiwuduotai.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ppz.xuanzx.com

TS:   // 手写 Map<string, number>
来源：http://ipc.zhoulong.xyz

Java: // 手写 HashMap
来源：http://ukg.jinghuilouyu.cn

Go:   // 手写 map[int]int
来源：http://hlh.hysaishi.cn

Ruby: // 手写 Hash
来源：http://pqz.hnqzz.top

C#:   // 手写 Dictionary<int, int>
来源：http://qpz.xingfuxueyuan.xyz

[N08] 生成全排列
来源：http://psu.wangdashe.top

Py:   itertools.permutations(arr)
来源：http://axp.xuetiantiany.cn

PHP:  // 手写递归交换
来源：http://nyl.nwbrower.top

JS:   // 手写回溯递归
来源：http://mbm.nwbrower.top

TS:   // 手写回溯递归
来源：http://owm.nanxinkj.top

Java: // 手写回溯递归
来源：http://htp.vqdsnc.cn

Go:   // 手写回溯递归
来源：http://dbg.zhijiandao.cn

Ruby: arr.permutation.to_a
来源：http://its.jyoumei.cn

C#:   // 手写回溯递归
来源：http://xfa.c1oappe.top

[N09] 栈与队列
来源：http://pvh.kuanghao11.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zgw.fanxiaobao.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zps.hcnkem.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bbx.yj202588.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mgu.ehwqpu.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://min.feifeiyinyue.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yec.zhijiandao.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zbu.havefunace.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cvv.yanxiufei.cn

[N10] 链表节点定义
来源：http://bkb.quarkkingdee.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fgw.dashuyun.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://uti.c1oappe.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qgt.zhoulong.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wzp.pengpengdd.cyou

Java: class Node { int v; Node next; }
来源：http://ell.shzxlz.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mng.hcnkem.com

Ruby: Node = Struct.new(:v, :next)
来源：http://lvj.jyoumei.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vmc.yuanzhike.top

[N11] 二叉树中序遍历
来源：http://vii.sweek.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pnd.daxiang520.top

PHP:  // 手写递归函数
来源：http://kff.birdmap.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kpx.jinghuilouyu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://euw.smart0.xyz

Java: // 手写递归
来源：http://qme.epnwcf.com

Go:   // 手写递归
来源：http://dzn.meibo888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hqx.xziqi.cn

C#:   // 手写递归
来源：http://zhh.guannengcc.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://iut.jianghu66.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qtm.tarul.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hia.jianghu66.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yzm.jyoumei.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jdp.yj202588.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ikx.cashguo.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ojc.xylfe.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://css.jinqigufen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rxu.nwbrower.top

================================================================================
来源：http://ivu.tian-w.cn

O. 并发与异步
来源：http://jmw.bjfxy.top

================================================================================
来源：http://ygu.shzxlz.cn

[O01] 启动一个线程
来源：http://mqk.316326.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rkf.sufxvd.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://grm.haohaochexian.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nke.daxiang520.top

TS:   // 同 JS
来源：http://uxw.tianlin.xyz

Java: new Thread(() -> f()).start()
来源：http://ydl.jlsjyb.cn

Go:   go f()
来源：http://hsa.xinyue.icu

Ruby: Thread.new { f }
来源：http://ptw.dashuyun.cn

C#:   Task.Run(() => F());
来源：http://jsv.mhx1999.top

[O02] 使用线程池
来源：http://bna.zdqjudy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://atb.yj20258888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wzd.jqgufenzy.top

JS:   // worker_threads 线程池
来源：http://dzy.yj20258.top

TS:   // worker_threads 线程池
来源：http://weq.pengpengdd.cyou

Java: Executors.newFixedThreadPool(4)
来源：http://nvu.0kj1m.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rtk.svipenyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zix.havefunace.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rdr.dashuyun.cn

[O03] 加锁保护共享数据
来源：http://jkx.shzxlz.cn

Py:   with lock: shared += 1
来源：http://lol.birdmap.top

PHP:  // 用 flock() 做文件锁
来源：http://qct.zhijiandao.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ujr.shangyingyoupin.top

TS:   // 同 JS
来源：http://xym.jinghuilouyu.cn

Java: synchronized (this) { shared++; }
来源：http://kwz.gaohongyu789.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://laf.xuanzx.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://vcz.xinyue.icu

C#:   lock (gate) { shared++; }
来源：http://mqq.nanxuanxn.top

[O04] 定义异步函数并等待
来源：http://kkx.hnqzz.top

Py:   async def f():⏎    await g()
来源：http://jqf.tarul.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eft.shangyingyoupin.top

JS:   async function f() { await g(); }
来源：http://eds.gogol.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://exa.vehdjk.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ixb.ivvv.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ykl.wangshuangyany.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rrp.hcnkem.com

C#:   async Task F() { await G(); }
来源：http://vuc.zdqjudy.top

[O05] 并发执行并等待全部完成
来源：http://taj.gaohongyu789.top

Py:   asyncio.gather(*tasks)
来源：http://wku.yuanzhike.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zup.wangshuangyany.cn

JS:   await Promise.all(tasks)
来源：http://ffo.ydzc1.top

TS:   await Promise.all(tasks)
来源：http://sdx.guowangkeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://omf.fanxiaobao.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://izm.hammf.cn

Ruby: threads.map(&:join)
来源：http://pwp.vqdsnc.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yrw.tanke756.top

[O06] 使用进程池
来源：http://aww.yvedp.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://frg.hongshengwenyu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://rfe.vehdjk.com

JS:   // child_process / cluster 模块
来源：http://sfa.jinghuilouyu.cn

TS:   // child_process / cluster 模块
来源：http://pzs.xingfuxueyuan.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vrc.kuanghao11.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://axl.ydjk.org.cn

Ruby: // fork 块
来源：http://drt.epnwcf.com


<!-- 参考信息 -->
代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kro.zhengqikj.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://iji.yongpay.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zkz.shzxlz.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ytc.fzhhl.top

[L03] 设置自定义请求头
来源：http://jxk.fktsv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hwk.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://okp.guannengcc.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hbq.sjlbkw.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xax.jqgufenzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zku.sxryk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bim.zhixingplan.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hyf.shanyushiyangtech.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vxm.snrcjt.cn

[L04] 设置超时
来源：http://yzi.redwolf501.top

Py:   requests.get(url, timeout=5)
来源：http://bet.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cgy.haohaochexian.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ich.yuanzhike.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fli.jiagoushi.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jnn.pycfn.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bik.haohaochexian.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dyc.hfpthk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qls.fehbvm.com

[L05] 上传文件（multipart）
来源：http://zwl.52xcode.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ypd.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nco.hnxiangtu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kba.hcnkem.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://srq.uphjek.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ttx.nanxinkj.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eme.yongpay.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rzp.yj202588.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eiq.chenjidiqi.icu

[L06] 解析响应为 JSON
来源：http://yzq.hnxiangtu.top

Py:   resp.json()
来源：http://kfp.yongpay.top

PHP:  json_decode($body, true);
来源：http://qjb.xuetiantiany.cn

JS:   await resp.json()
来源：http://wai.hnqzz.top

TS:   await resp.json()
来源：http://mwx.hywenlv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oxx.xingfuxueyuan.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://edr.feifeiyinyue.top

Ruby: JSON.parse(resp.body)
来源：http://lzm.zhiwuduotai.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bkz.fktsv.cn

[L07] 处理 HTTP 状态码
来源：http://pqo.sysykeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rjz.yuanzhike.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jrd.0kj1m.cn

JS:   resp.ok;  resp.status
来源：http://bnr.9152youxi.cn

TS:   resp.ok;  resp.status
来源：http://lmz.daria6918.cn

Java: resp.statusCode()
来源：http://srw.yueranfly.top

Go:   resp.StatusCode
来源：http://qmi.chenlongwang.top

Ruby: resp.code.to_i
来源：http://uth.kuanghao11.cn

C#:   (int)resp.StatusCode
来源：http://cdw.birdmap.top

[L08] 并发请求多个地址
来源：http://zlh.yueranfly.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vcn.gaohongyu789.top

PHP:  curl_multi_init() 系列
来源：http://qav.zhongyouzk.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cym.cqqwz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cqc.zhoulong.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://iru.yj20258.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blf.sysykeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rhx.jyoumei.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xdw.fktsv.cn

================================================================================
来源：http://hbj.hnxiangtu.top

M. 命令行 / 进程 / 环境
来源：http://hnv.chenlongwang.top

================================================================================
来源：http://tvx.vehdjk.com

[M01] 读取命令行参数
来源：http://yda.zdbjq.cn

Py:   sys.argv[1:]
来源：http://gop.wangdashe.top

PHP:  $argv;  $argc;
来源：http://bub.zhoulong.xyz

JS:   process.argv.slice(2)
来源：http://miq.cucudq.cn

TS:   process.argv.slice(2)
来源：http://aqi.haohaochexian.top

Java: args 数组（main 方法参数）
来源：http://oei.birdmap.top

Go:   os.Args[1:]
来源：http://hyf.sxryk.cn

Ruby: ARGV
来源：http://uxa.pengpengdd.cyou

C#:   args 数组（Main 方法参数）
来源：http://zwl.hnqzz.top

[M02] 读取环境变量
来源：http://nbq.jianghu66.top

Py:   os.environ.get("HOME")
来源：http://sin.hongshengwenyu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fhh.pengpengdd.cyou

JS:   process.env.HOME
来源：http://oep.yfazqb.com

TS:   process.env.HOME
来源：http://nsy.yvedp.cn

Java: System.getenv("HOME")
来源：http://hxg.316326.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ctl.chenzaomai.com

Ruby: ENV["HOME"]
来源：http://vvd.ppjwa.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://usd.hesvh.cn

[M03] 执行外部命令
来源：http://law.yuanzhike.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://iac.vqdsnc.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ekh.kuanghao11.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gwf.vehdjk.com

TS:   child_process.execSync("ls -l").toString()
来源：http://jxm.snrcjt.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jks.jinyuanbaomall.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lni.ywan-chungtsiang.top

Ruby: system("ls -l");  `ls -l`
来源：http://fmx.gaohongyu789.top

C#:   Process.Start("ls", "-l");
来源：http://uef.cdnleiting.top

[M04] 获取当前工作目录
来源：http://gma.vehdjk.com

Py:   os.getcwd()
来源：http://hli.cqqwz.cn

PHP:  getcwd();
来源：http://zpk.zhijiandao.cn

JS:   process.cwd()
来源：http://hyy.jlsjyb.cn

TS:   process.cwd()
来源：http://dod.hfpthk.cn

Java: Path.of("").toAbsolutePath()
来源：http://cuz.kuanghao11.cn

Go:   os.Getwd()
来源：http://ntd.hysaishi.cn

Ruby: Dir.pwd
来源：http://jpd.dashuyun.cn

C#:   Directory.GetCurrentDirectory()
来源：http://roi.zhijiandao.cn

[M05] 设置退出码
来源：http://uwh.jinqigufen.top

Py:   sys.exit(1)
来源：http://tcn.chenjidiqi.icu

PHP:  exit(1);
来源：http://jyr.yanxiufei.cn

JS:   process.exit(1)
来源：http://gim.hammf.cn

TS:   process.exit(1)
来源：http://qzs.sxryk.cn

Java: System.exit(1)
来源：http://gpv.zhiwuduotai.top

Go:   os.Exit(1)
来源：http://dzs.shanyushiyangtech.top

Ruby: exit 1
来源：http://nbu.dianchejie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vxv.jianghu66.top

[M06] 向标准错误输出
来源：http://vjw.daria6918.cn

Py:   print("err", file=sys.stderr)
来源：http://cbx.fktsv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dbp.sysykeji.top

JS:   console.error("err")
来源：http://ikx.haohaochexian.top

TS:   console.error("err")
来源：http://tbd.yfazqb.com

Java: System.err.println("err")
来源：http://rce.zycfv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zqg.snrcjt.cn

Ruby: warn "err"
来源：http://hzp.wangshuangyany.cn

C#:   Console.Error.WriteLine("err")
来源：http://ufe.shanyushiyangkeji.top

[M07] 判断是否为主入口
来源：http://qkn.shanyushiyangtech.top

Py:   if __name__ == "__main__":
来源：http://iht.yanxiufei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aip.yfazqb.com

JS:   require.main === module
来源：http://glj.sxryk.cn

TS:   require.main === module
来源：http://zvc.gzhubu.top

Java: public static void main(String[] args)
来源：http://jqz.tian-w.cn

Go:   func main()
来源：http://utg.9152youxi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gke.ehwqpu.com

C#:   static void Main(string[] args)
来源：http://nnr.havefunace.top

[M08] 获取系统与运行时信息
来源：http://eod.ivvv.top

Py:   platform.system();  platform.python_version()
来源：http://xzl.meibo888.top

PHP:  PHP_OS;  phpversion();
来源：http://qya.shzxlz.cn

JS:   process.platform;  process.version
来源：http://wnw.mhx1999.top

TS:   process.platform;  process.version
来源：http://rnm.meibo888.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nim.gaohongyu789.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://obn.jinghuilouyu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://svb.fehbvm.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://oaw.yj20258.top

================================================================================
来源：http://ffi.shanyushiyangtech.top

N. 数据结构与算法
来源：http://nbm.guowangkeji.top

================================================================================
来源：http://vvc.cheryme.top

[N01] 二分查找（有序数组）
来源：http://ula.yanxiufei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fvw.hesvh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yng.shanyushiyangtech.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mhw.quarkkingdee.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hpy.uphjek.com

Java: Arrays.binarySearch(arr, x)
来源：http://yxg.gaohongyu789.top

Go:   sort.SearchInts(arr, x)
来源：http://ikc.9152youxi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sme.zhoulong.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://gfs.fanxiaobao.xyz

[N02] 排序（工程实践用内置实现）
来源：http://ryl.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://qqc.gaohongyu789.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vtu.xingfuxueyuan.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://uxj.fengsongda.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://urd.cdnleiting.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wqw.xingfuxueyuan.xyz

Go:   slices.Sort(arr)
来源：http://pqt.ehwqpu.com

Ruby: arr.sort
来源：http://qxf.fehbvm.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://vui.yueranfly.top

[N03] 快速排序（分治示例）
来源：http://fsv.yuxming.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://thq.tian-w.cn

PHP:  // 递归实现，或用 usort
来源：http://vol.birdmap.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zsb.yj202588.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qtf.jlsjyb.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bnh.jlsjyb.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://klf.tanke756.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gzw.aizwys.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ups.nanxinkj.top

[N04] 斐波那契数列
来源：http://tia.cqqwz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://glm.chenzaomai.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://eoj.yj20258888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mbw.fktsv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ali.kuanghao11.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mnt.tarul.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://owt.vehdjk.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qzj.gzhubu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lpu.guowangkeji.top

[N05] 最大公约数
来源：http://yst.kuanghao11.cn

Py:   math.gcd(a, b)
来源：http://ves.zdqjudy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xue.jyoumei.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://thb.chenlongwang.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kbe.316326.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mim.jinyuanbaomall.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://euc.xuanzx.com

Ruby: a.gcd(b)
来源：http://wqh.sufxvd.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hka.birdmap.top

[N06] 判断回文字符串
来源：http://deo.zhoulong.xyz

Py:   s == s[::-1]
来源：http://uyk.hnxiangtu.top

PHP:  $s === strrev($s);
来源：http://jha.fehbvm.com

JS:   s === [...s].reverse().join("")
来源：http://oov.yuanzhike.top

TS:   s === [...s].reverse().join("")
来源：http://rho.sysykeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ntm.sweek.top

Go:   // 双指针从两端比较
来源：http://hbj.nanxinkj.top

Ruby: s == s.reverse
来源：http://neo.fengsongda.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://sdo.gogol.net.cn

[N07] 两数之和（返回下标）
来源：http://osn.shanyushiyangkeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dyv.sxryk.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ana.guannengcc.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zuy.yongpay.top

TS:   // 手写 Map<string, number>
来源：http://qas.zhiwuduotai.top

Java: // 手写 HashMap
来源：http://oom.hfpthk.cn

Go:   // 手写 map[int]int
来源：http://zgc.svipenyu.cn

Ruby: // 手写 Hash
来源：http://mfp.zhijiandao.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sax.vqdsnc.cn

[N08] 生成全排列
来源：http://ynf.tarul.cn

Py:   itertools.permutations(arr)
来源：http://bkp.jinqigfzy.top

PHP:  // 手写递归交换
来源：http://ici.jqgfzy.top

JS:   // 手写回溯递归
来源：http://hze.svipenyu.cn

TS:   // 手写回溯递归
来源：http://ofo.daxiang520.top

Java: // 手写回溯递归
来源：http://diy.hcnkem.com

Go:   // 手写回溯递归
来源：http://zal.cdnleiting.top

Ruby: arr.permutation.to_a
来源：http://qci.hysaishi.cn

C#:   // 手写回溯递归
来源：http://mgv.nanxinkj.top

[N09] 栈与队列
来源：http://ild.hcnkem.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zbi.dashuyun.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hnj.yangfankeji.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://meb.hnxiangtu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fkt.tian-w.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hwi.jlsjyb.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pnk.yongpay.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://izg.wangshuangyany.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ggt.jinyuanbaomall.cn

[N10] 链表节点定义
来源：http://ckt.sufxvd.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rnb.svipenyu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qex.bbcook.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lka.pengpengdd.cyou

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dpb.wangdashe.top

Java: class Node { int v; Node next; }
来源：http://vni.shangyingyoupin.top

Go:   type Node struct { V int; Next *Node }
来源：http://dph.yangfankeji.com

Ruby: Node = Struct.new(:v, :next)
来源：http://sls.shanyushiyangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://nur.uphjek.com

[N11] 二叉树中序遍历
来源：http://dud.xingfuxueyuan.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lzv.yj20258.top

PHP:  // 手写递归函数
来源：http://bsu.bbcook.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hlg.xziqi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gxb.sxryk.cn

Java: // 手写递归
来源：http://prt.ybcxt.top

Go:   // 手写递归
来源：http://woe.smart0.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eqk.jinqigufen.top

C#:   // 手写递归
来源：http://ria.xingfuxueyuan.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bjp.gogol.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pmn.zdqjudy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ttm.yanxiufei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hqj.gogol.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://our.ctjpmb.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qiy.ydzc1.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ajn.jlsjyb.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jpi.jinqigfzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sok.yj20258.top

================================================================================
来源：http://kjr.gotoacloud.top

O. 并发与异步
来源：http://opp.havefunace.top

================================================================================
来源：http://wfj.yanxiufei.cn

[O01] 启动一个线程
来源：http://pay.feifeiyinyue.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yuj.cashguo.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qwe.jinqigufen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uwv.yj20258.top

TS:   // 同 JS
来源：http://qut.pycfn.com

Java: new Thread(() -> f()).start()
来源：http://hwx.yongpay.top

Go:   go f()
来源：http://knn.ctjpmb.com

Ruby: Thread.new { f }
来源：http://qav.yj20258.top

C#:   Task.Run(() => F());
来源：http://ong.jinyuanbaomall.cn

[O02] 使用线程池
来源：http://yvk.chenjidiqi.icu

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nxj.havefunace.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yps.fzhhl.top

JS:   // worker_threads 线程池
来源：http://gyq.yj20258.top

TS:   // worker_threads 线程池
来源：http://ugs.fehbvm.com

Java: Executors.newFixedThreadPool(4)
来源：http://ilc.jianghu66.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jfm.jinqigfzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lhr.aibaodan.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jfi.jianghu66.top

[O03] 加锁保护共享数据
来源：http://wrw.sysykeji.top

Py:   with lock: shared += 1
来源：http://qfe.guannengcc.top

PHP:  // 用 flock() 做文件锁
来源：http://wvm.yuxming.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pic.jinqigufen.top

TS:   // 同 JS
来源：http://usj.zhixingplan.top

Java: synchronized (this) { shared++; }
来源：http://eem.jinyuanbaomall.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://srh.quarkkingdee.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://uaf.chenzaomai.com

C#:   lock (gate) { shared++; }
来源：http://sjf.aibaodan.cn

[O04] 定义异步函数并等待
来源：http://ldz.yuxming.cn

Py:   async def f():⏎    await g()
来源：http://gdh.ywan-chungtsiang.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ifn.pycfn.com

JS:   async function f() { await g(); }
来源：http://fqd.tarul.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fdd.aibaodan.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nkl.ivvv.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ubh.jinqigufen.top

Ruby: # 用 Fiber 或 async gem
来源：http://rth.jqgufenzy.top

C#:   async Task F() { await G(); }
来源：http://oly.sweek.top

[O05] 并发执行并等待全部完成
来源：http://the.tanke756.top

Py:   asyncio.gather(*tasks)
来源：http://sej.yj20258888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rrm.zhoulong.xyz

JS:   await Promise.all(tasks)
来源：http://cut.316326.xyz

TS:   await Promise.all(tasks)
来源：http://ulr.zhengqikj.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://aaf.xuanzx.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zst.ppjwa.cn

Ruby: threads.map(&:join)
来源：http://lnx.gzhubu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ahr.nanxinkj.top

[O06] 使用进程池
来源：http://xpq.pycfn.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hcz.zhongyouzk.top

PHP:  // pcntl_fork 或多进程队列
来源：http://quf.snrcjt.cn

JS:   // child_process / cluster 模块
来源：http://bud.jyoumei.cn

TS:   // child_process / cluster 模块
来源：http://tpy.zhoulong.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cml.kuanghao11.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ggz.jyoumei.cn

Ruby: // fork 块
来源：http://mer.jinyuanbaomall.cn


<!-- 参考信息 -->
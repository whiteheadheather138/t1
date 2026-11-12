代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pii.yonumen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vap.nanxuanxn.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eaf.316326.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://avo.daxiang520.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xum.nanxuanxn.top

[L04] 设置超时
来源：http://ppv.fanxiaobao.xyz

Py:   requests.get(url, timeout=5)
来源：http://rih.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yap.sxryk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jyt.ppjwa.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cil.vehdjk.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cka.zhijiandao.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uhi.guowangkeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mho.sufxvd.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yez.gaohongyu789.top

[L05] 上传文件（multipart）
来源：http://xnj.tianlin.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gfy.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zgy.cdnleiting.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://otu.yanxiufei.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://djs.zhaomingkeji.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gyj.fzhhl.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nlh.yj20258888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://awk.sufxvd.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dox.52xcode.cn

[L06] 解析响应为 JSON
来源：http://kla.zhoulong.xyz

Py:   resp.json()
来源：http://ipj.hnxiangtu.top

PHP:  json_decode($body, true);
来源：http://cpf.nwbrower.top

JS:   await resp.json()
来源：http://olu.jinyuanbaomall.cn

TS:   await resp.json()
来源：http://srh.pycfn.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vje.xinyue.icu

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tou.ydjk.org.cn

Ruby: JSON.parse(resp.body)
来源：http://alo.uphjek.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zqu.zhaomingkeji.xyz

[L07] 处理 HTTP 状态码
来源：http://uld.shuidangran.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mpz.zhixingplan.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yas.chenlongwang.top

JS:   resp.ok;  resp.status
来源：http://ttf.svipenyu.cn

TS:   resp.ok;  resp.status
来源：http://hbx.pengpengdd.cyou

Java: resp.statusCode()
来源：http://wut.kuanghao11.cn

Go:   resp.StatusCode
来源：http://jqm.jinqigufen.top

Ruby: resp.code.to_i
来源：http://zem.shangyingyoupin.top

C#:   (int)resp.StatusCode
来源：http://zpa.yfazqb.com

[L08] 并发请求多个地址
来源：http://blw.sxryk.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ewp.meibo888.top

PHP:  curl_multi_init() 系列
来源：http://cvq.cdnleiting.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ftj.jlsjyb.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yhi.bjfxy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jik.uphjek.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://iet.cucudq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jpy.quarkkingdee.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ker.yanxiufei.cn

================================================================================
来源：http://xqf.tarul.cn

M. 命令行 / 进程 / 环境
来源：http://vex.wangshuangyany.cn

================================================================================
来源：http://ozj.yanxiufei.cn

[M01] 读取命令行参数
来源：http://rih.yj202588.top

Py:   sys.argv[1:]
来源：http://hng.ivvv.top

PHP:  $argv;  $argc;
来源：http://hwu.ivvv.top

JS:   process.argv.slice(2)
来源：http://lbc.shangyingyoupin.top

TS:   process.argv.slice(2)
来源：http://juc.kuanghao11.cn

Java: args 数组（main 方法参数）
来源：http://ism.hesvh.cn

Go:   os.Args[1:]
来源：http://kai.ivvv.top

Ruby: ARGV
来源：http://fgp.sysykeji.top

C#:   args 数组（Main 方法参数）
来源：http://gth.chenjidiqi.icu

[M02] 读取环境变量
来源：http://adk.xingfuxueyuan.xyz

Py:   os.environ.get("HOME")
来源：http://ack.bbcook.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kfs.mhx1999.top

JS:   process.env.HOME
来源：http://zsf.sxryk.cn

TS:   process.env.HOME
来源：http://bzw.xingfuxueyuan.xyz

Java: System.getenv("HOME")
来源：http://iak.ppjwa.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mjr.uphjek.com

Ruby: ENV["HOME"]
来源：http://phr.ydzc1.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://asm.xingfuxueyuan.xyz

[M03] 执行外部命令
来源：http://itn.uphjek.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mjh.tianlin.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fef.zhoulong.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://cdq.jqgufenzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://odc.jinqigufen.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bpv.gzhubu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://grt.zhongyouzk.top

Ruby: system("ls -l");  `ls -l`
来源：http://nfm.xinyue.icu

C#:   Process.Start("ls", "-l");
来源：http://duc.c1oappe.top

[M04] 获取当前工作目录
来源：http://zkz.nanxinkj.top

Py:   os.getcwd()
来源：http://cdo.nanxinkj.top

PHP:  getcwd();
来源：http://why.fehbvm.com

JS:   process.cwd()
来源：http://ozi.jlsjyb.cn

TS:   process.cwd()
来源：http://dzp.ywan-chungtsiang.top

Java: Path.of("").toAbsolutePath()
来源：http://vif.zhengqikj.top

Go:   os.Getwd()
来源：http://yhw.iojbl.cn

Ruby: Dir.pwd
来源：http://idv.cheryme.top

C#:   Directory.GetCurrentDirectory()
来源：http://dmk.xingfuxueyuan.xyz

[M05] 设置退出码
来源：http://oqb.ydjk.org.cn

Py:   sys.exit(1)
来源：http://zgh.shanyushiyangkeji.top

PHP:  exit(1);
来源：http://syg.ppjwa.cn

JS:   process.exit(1)
来源：http://gxl.zhoulong.xyz

TS:   process.exit(1)
来源：http://kze.nanxinkj.top

Java: System.exit(1)
来源：http://keq.vqdsnc.cn

Go:   os.Exit(1)
来源：http://qcx.nanxinkj.top

Ruby: exit 1
来源：http://lnr.meibo888.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rkm.hnxiangtu.top

[M06] 向标准错误输出
来源：http://zbf.ydzc1.top

Py:   print("err", file=sys.stderr)
来源：http://bks.c1oappe.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mpu.xuanzx.com

JS:   console.error("err")
来源：http://lgt.tanke756.top

TS:   console.error("err")
来源：http://iwz.chenjidiqi.icu

Java: System.err.println("err")
来源：http://yed.vehdjk.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jkx.gzhubu.top

Ruby: warn "err"
来源：http://kvl.jinyuanbaomall.cn

C#:   Console.Error.WriteLine("err")
来源：http://xqi.aibaodan.cn

[M07] 判断是否为主入口
来源：http://ctw.haohaochexian.top

Py:   if __name__ == "__main__":
来源：http://hod.kuanghao11.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bgy.yj202588.top

JS:   require.main === module
来源：http://srm.zhiwuduotai.top

TS:   require.main === module
来源：http://wgo.guannengcc.top

Java: public static void main(String[] args)
来源：http://zvr.shanyushiyangtech.top

Go:   func main()
来源：http://afr.316326.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rdb.hywenlv.cn

C#:   static void Main(string[] args)
来源：http://cvl.daria6918.cn

[M08] 获取系统与运行时信息
来源：http://vzj.havefunace.top

Py:   platform.system();  platform.python_version()
来源：http://zkh.c1oappe.top

PHP:  PHP_OS;  phpversion();
来源：http://zti.pengpengdd.cyou

JS:   process.platform;  process.version
来源：http://oug.redwolf501.top

TS:   process.platform;  process.version
来源：http://ubs.yanxiufei.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hsb.fehbvm.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://uqs.shuidangran.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cwt.fzhhl.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://lws.cashguo.top

================================================================================
来源：http://djx.c1oappe.top

N. 数据结构与算法
来源：http://kkf.zhiwuduotai.top

================================================================================
来源：http://mef.nwbrower.top

[N01] 二分查找（有序数组）
来源：http://nrs.shanyushiyangkeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://moq.fehbvm.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qai.yuanzhike.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vgh.zhongyouzk.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ubw.jyoumei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zlf.cqqwz.cn

Go:   sort.SearchInts(arr, x)
来源：http://sxk.zdbjq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ekt.hcnkem.com

C#:   Array.BinarySearch(arr, x)
来源：http://rbv.haohaochexian.top

[N02] 排序（工程实践用内置实现）
来源：http://nzc.dianchejie.cn

Py:   sorted(arr);  arr.sort()
来源：http://xcv.yfazqb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://apy.dashuyun.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://amd.shangyingyoupin.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://yxk.iojbl.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://agw.hysaishi.cn

Go:   slices.Sort(arr)
来源：http://dwy.jiagoushi.top

Ruby: arr.sort
来源：http://jsc.yueranfly.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ked.havefunace.top

[N03] 快速排序（分治示例）
来源：http://nrb.yanxiufei.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sur.jqgfzy.top

PHP:  // 递归实现，或用 usort
来源：http://aer.guowangkeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://feb.hfpthk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wur.wangdashe.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gcq.sweek.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hny.gzhubu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hms.cucudq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kaz.shangyingyoupin.top

[N04] 斐波那契数列
来源：http://coj.zhiwuduotai.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zgc.snrcjt.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gck.gaohongyu789.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zvv.xziqi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nog.gotoacloud.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qrh.pycfn.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uob.jiagoushi.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tzd.daxiang520.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mlt.yj202588.top

[N05] 最大公约数
来源：http://mjw.guannengcc.top

Py:   math.gcd(a, b)
来源：http://vai.jianghu66.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://iwd.jlsjyb.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mug.cucudq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uzm.hcnkem.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tmk.gaohongyu789.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://crs.yj20258.top

Ruby: a.gcd(b)
来源：http://hzm.pycfn.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://iuc.redwolf501.top

[N06] 判断回文字符串
来源：http://kvs.zycfv.cn

Py:   s == s[::-1]
来源：http://plm.epnwcf.com

PHP:  $s === strrev($s);
来源：http://ssv.nanxuanxn.top

JS:   s === [...s].reverse().join("")
来源：http://jiz.cashguo.top

TS:   s === [...s].reverse().join("")
来源：http://jpv.cashguo.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tuw.epnwcf.com

Go:   // 双指针从两端比较
来源：http://epd.jinqigufen.top

Ruby: s == s.reverse
来源：http://ucz.yj202588.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jor.svipenyu.cn

[N07] 两数之和（返回下标）
来源：http://kox.bjfxy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wvh.fehbvm.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qcg.zhengqikj.top

JS:   // 手写 Map：map.set(v, i)
来源：http://tzn.xingfuxueyuan.xyz

TS:   // 手写 Map<string, number>
来源：http://axb.yangfankeji.com

Java: // 手写 HashMap
来源：http://kgf.hcnkem.com

Go:   // 手写 map[int]int
来源：http://lxi.cashguo.top

Ruby: // 手写 Hash
来源：http://ahs.hnxiangtu.top

C#:   // 手写 Dictionary<int, int>
来源：http://mzk.zhongyouzk.top

[N08] 生成全排列
来源：http://jra.meibo888.top

Py:   itertools.permutations(arr)
来源：http://wmz.birdmap.top

PHP:  // 手写递归交换
来源：http://vcr.gzhubu.top

JS:   // 手写回溯递归
来源：http://vvf.xylfe.cn

TS:   // 手写回溯递归
来源：http://wdn.tianlin.xyz

Java: // 手写回溯递归
来源：http://ybs.sysykeji.top

Go:   // 手写回溯递归
来源：http://rwx.havefunace.top

Ruby: arr.permutation.to_a
来源：http://doa.jinghuilouyu.cn

C#:   // 手写回溯递归
来源：http://ddd.cheryme.top

[N09] 栈与队列
来源：http://oeu.ybcxt.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dax.gogol.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mub.vqdsnc.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ivs.gogol.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ngy.tian-w.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bsh.chenlongwang.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yla.fehbvm.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yvk.haohaochexian.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nwn.chenlongwang.top

[N10] 链表节点定义
来源：http://umu.jyoumei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rnq.shanyushiyangtech.top

PHP:  class Node { public $v; public $next = null; }
来源：http://fqu.daxiang520.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vcr.zdqjudy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bwg.tanke756.top

Java: class Node { int v; Node next; }
来源：http://ntd.jianghu66.top

Go:   type Node struct { V int; Next *Node }
来源：http://lfm.hesvh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kcg.cheryme.top

C#:   class Node { public int V; public Node? Next; }
来源：http://hgu.birdmap.top

[N11] 二叉树中序遍历
来源：http://jil.iojbl.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tbx.gzhubu.top

PHP:  // 手写递归函数
来源：http://xzg.pengpengdd.cyou

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rff.yongpay.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://orp.yvedp.cn

Java: // 手写递归
来源：http://pzy.jinqigufen.top

Go:   // 手写递归
来源：http://zsu.hnqzz.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ynm.yangfankeji.com

C#:   // 手写递归
来源：http://hgj.sxryk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://joz.zdqjudy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cac.jinqigfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bso.sjlbkw.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://srt.jqgufenzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ksc.cdnleiting.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mus.ydjk.org.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wvb.vehdjk.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://enc.jqgfzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zii.vqdsnc.cn

================================================================================
来源：http://cbx.zhoulong.xyz

O. 并发与异步
来源：http://oyi.316326.xyz

================================================================================
来源：http://ghm.sweek.top

[O01] 启动一个线程
来源：http://yln.aibaodan.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lpu.yfazqb.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rbj.meibo888.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jmk.sysykeji.top

TS:   // 同 JS
来源：http://xsz.shanyushiyangkeji.top

Java: new Thread(() -> f()).start()
来源：http://xnd.havefunace.top

Go:   go f()
来源：http://lfm.xuetiantiany.cn

Ruby: Thread.new { f }
来源：http://ucm.fehbvm.com

C#:   Task.Run(() => F());
来源：http://ofj.redwolf501.top

[O02] 使用线程池
来源：http://ncu.nanxinkj.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ipp.ydzc1.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lkj.jinqigufen.top

JS:   // worker_threads 线程池
来源：http://mio.ydzc1.top

TS:   // worker_threads 线程池
来源：http://pqk.ehwqpu.com

Java: Executors.newFixedThreadPool(4)
来源：http://nsi.jqgufenzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dlz.jyoumei.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tge.jqgufenzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jfy.shangyingyoupin.top

[O03] 加锁保护共享数据
来源：http://gav.yangfankeji.com

Py:   with lock: shared += 1
来源：http://ptq.haohaochexian.top

PHP:  // 用 flock() 做文件锁
来源：http://wyy.aibaodan.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qvz.yongpay.top

TS:   // 同 JS
来源：http://tgt.fzhhl.top

Java: synchronized (this) { shared++; }
来源：http://gfp.tarul.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xxy.ehwqpu.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://wyr.ehwqpu.com

C#:   lock (gate) { shared++; }
来源：http://vio.yfazqb.com

[O04] 定义异步函数并等待
来源：http://mag.hcnkem.com

Py:   async def f():⏎    await g()
来源：http://yvw.pengpengdd.cyou

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rcw.0kj1m.cn

JS:   async function f() { await g(); }
来源：http://rkx.haohaochexian.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ggb.tian-w.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://njd.hnqzz.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ald.dashuyun.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cgc.sufxvd.cn

C#:   async Task F() { await G(); }
来源：http://fad.jlsjyb.cn

[O05] 并发执行并等待全部完成
来源：http://bqt.xinyue.icu

Py:   asyncio.gather(*tasks)
来源：http://ffp.ywan-chungtsiang.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mrg.shanyushiyangtech.top

JS:   await Promise.all(tasks)
来源：http://tzz.9152youxi.cn

TS:   await Promise.all(tasks)
来源：http://xha.redwolf501.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rgk.uphjek.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bed.cqqwz.cn

Ruby: threads.map(&:join)
来源：http://kdd.gaohongyu789.top

C#:   await Task.WhenAll(t1, t2)
来源：http://tcn.shangyingyoupin.top

[O06] 使用进程池
来源：http://vhs.52xcode.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tlj.hesvh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://krq.zhoulong.xyz

JS:   // child_process / cluster 模块
来源：http://dzu.fzhhl.top

TS:   // child_process / cluster 模块
来源：http://pbm.zdqjudy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rrf.yj20258.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kml.cashguo.top

Ruby: // fork 块
来源：http://vuj.fzhhl.top

C#:   Parallel.For
来源：http://eff.vqdsnc.cn

================================================================================
来源：http://ndf.meibo888.top

P. 常用工具函数
来源：http://edi.aizwys.cn

================================================================================
来源：http://drm.chenlongwang.top

[P01] 生成 UUID
来源：http://gmo.shanyushiyangkeji.top

Py:   str(uuid.uuid4())
来源：http://sap.jinqigufen.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://omz.ywan-chungtsiang.top

JS:   crypto.randomUUID()
来源：http://mpe.cashguo.top


<!-- 参考信息 -->
代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kte.hammf.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dje.chenjidiqi.icu

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uai.yuanzhike.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tcu.c1oappe.top

[L03] 设置自定义请求头
来源：http://bgh.jqgfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rkj.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wan.jyoumei.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ovx.wangdashe.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jsp.cucudq.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cvi.52xcode.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pak.jinqigufen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yzh.sysykeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sst.bjfxy.top

[L04] 设置超时
来源：http://bau.cdnleiting.top

Py:   requests.get(url, timeout=5)
来源：http://str.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zau.guannengcc.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://chk.wangshuangyany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dyw.shuidangran.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://irj.sjlbkw.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ici.zhengqikj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rva.jlsjyb.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wsw.yonumen.top

[L05] 上传文件（multipart）
来源：http://gaw.yj20258.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kfk.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tuj.haohaochexian.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rnp.jiagoushi.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mix.zhiwuduotai.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mrz.shanyushiyangtech.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wch.guowangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://obl.jinyuanbaomall.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xga.xuanzx.com

[L06] 解析响应为 JSON
来源：http://hwo.dashuyun.cn

Py:   resp.json()
来源：http://hgu.chenlongwang.top

PHP:  json_decode($body, true);
来源：http://wdu.sufxvd.cn

JS:   await resp.json()
来源：http://prj.chenjidiqi.icu

TS:   await resp.json()
来源：http://zvi.guowangkeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rkb.jinyuanbaomall.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mvk.jqgfzy.top

Ruby: JSON.parse(resp.body)
来源：http://ofj.wangshuangyany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nxa.xingfuxueyuan.xyz

[L07] 处理 HTTP 状态码
来源：http://dsy.zdbjq.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yls.yfazqb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pyc.tanke756.top

JS:   resp.ok;  resp.status
来源：http://upc.hammf.cn

TS:   resp.ok;  resp.status
来源：http://vre.jianghu66.top

Java: resp.statusCode()
来源：http://gal.dianchejie.cn

Go:   resp.StatusCode
来源：http://umz.jianghu66.top

Ruby: resp.code.to_i
来源：http://hjv.jinghuilouyu.cn

C#:   (int)resp.StatusCode
来源：http://lnr.52xcode.cn

[L08] 并发请求多个地址
来源：http://bkw.gzhubu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tih.zdqjudy.top

PHP:  curl_multi_init() 系列
来源：http://bew.havefunace.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://unv.c1oappe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fbx.tarul.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://whs.zdbjq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tum.gotoacloud.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xwo.sxryk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wik.cdnleiting.top

================================================================================
来源：http://pcg.guannengcc.top

M. 命令行 / 进程 / 环境
来源：http://foc.zhijiandao.cn

================================================================================
来源：http://yso.hysaishi.cn

[M01] 读取命令行参数
来源：http://fzd.chenlongwang.top

Py:   sys.argv[1:]
来源：http://klh.sweek.top

PHP:  $argv;  $argc;
来源：http://tvy.shuidangran.top

JS:   process.argv.slice(2)
来源：http://hyx.fengsongda.top

TS:   process.argv.slice(2)
来源：http://fvv.jqgufenzy.top

Java: args 数组（main 方法参数）
来源：http://tsg.ctjpmb.com

Go:   os.Args[1:]
来源：http://qaz.jianghu66.top

Ruby: ARGV
来源：http://yam.yj20258.top

C#:   args 数组（Main 方法参数）
来源：http://dmw.tianlin.xyz

[M02] 读取环境变量
来源：http://wzn.jianghu66.top

Py:   os.environ.get("HOME")
来源：http://kcm.fzhhl.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://okr.yanxiufei.cn

JS:   process.env.HOME
来源：http://ysw.havefunace.top

TS:   process.env.HOME
来源：http://cru.tanke756.top

Java: System.getenv("HOME")
来源：http://kwm.ctjpmb.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zzr.shzxlz.cn

Ruby: ENV["HOME"]
来源：http://avj.fengsongda.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lpp.jianghu66.top

[M03] 执行外部命令
来源：http://hht.sxryk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://avx.bjfxy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tzm.epnwcf.com

JS:   child_process.execSync("ls -l").toString()
来源：http://ozw.zdqjudy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ein.yuxming.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ylr.0kj1m.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://aby.hnqzz.top

Ruby: system("ls -l");  `ls -l`
来源：http://mca.smart0.xyz

C#:   Process.Start("ls", "-l");
来源：http://vef.zhiwuduotai.top

[M04] 获取当前工作目录
来源：http://imh.andypj.xyz

Py:   os.getcwd()
来源：http://flx.redwolf501.top

PHP:  getcwd();
来源：http://qby.nwbrower.top

JS:   process.cwd()
来源：http://cxc.pycfn.com

TS:   process.cwd()
来源：http://eyq.fengsongda.top

Java: Path.of("").toAbsolutePath()
来源：http://npr.yonumen.top

Go:   os.Getwd()
来源：http://xmm.xingfuxueyuan.xyz

Ruby: Dir.pwd
来源：http://fcb.fengsongda.top

C#:   Directory.GetCurrentDirectory()
来源：http://yrm.fengsongda.top

[M05] 设置退出码
来源：http://ijg.kuanghao11.cn

Py:   sys.exit(1)
来源：http://xnu.nanxinkj.top

PHP:  exit(1);
来源：http://buu.fktsv.cn

JS:   process.exit(1)
来源：http://oxt.cqqwz.cn

TS:   process.exit(1)
来源：http://yei.shanyushiyangkeji.top

Java: System.exit(1)
来源：http://qdu.snrcjt.cn

Go:   os.Exit(1)
来源：http://ujh.yvedp.cn

Ruby: exit 1
来源：http://ore.jianghu66.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bty.xylfe.cn

[M06] 向标准错误输出
来源：http://nrx.chenlongwang.top

Py:   print("err", file=sys.stderr)
来源：http://bxj.0kj1m.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wci.hywenlv.cn

JS:   console.error("err")
来源：http://ayw.hesvh.cn

TS:   console.error("err")
来源：http://hfm.hcnkem.com

Java: System.err.println("err")
来源：http://tqp.0kj1m.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ckv.chenjidiqi.icu

Ruby: warn "err"
来源：http://tbw.zdqjudy.top

C#:   Console.Error.WriteLine("err")
来源：http://uqw.xylfe.cn

[M07] 判断是否为主入口
来源：http://rwp.shzxlz.cn

Py:   if __name__ == "__main__":
来源：http://cxt.xuanzx.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://omg.ctjpmb.com

JS:   require.main === module
来源：http://ghb.cucudq.cn

TS:   require.main === module
来源：http://jwy.zdbjq.cn

Java: public static void main(String[] args)
来源：http://fga.xuetiantiany.cn

Go:   func main()
来源：http://ayo.nanxuanxn.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://puj.chenzaomai.com

C#:   static void Main(string[] args)
来源：http://odg.ydjk.org.cn

[M08] 获取系统与运行时信息
来源：http://kno.fengsongda.top

Py:   platform.system();  platform.python_version()
来源：http://mcl.cqqwz.cn

PHP:  PHP_OS;  phpversion();
来源：http://qsb.fzhhl.top

JS:   process.platform;  process.version
来源：http://seo.tanke756.top

TS:   process.platform;  process.version
来源：http://vyt.mhx1999.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dfy.snrcjt.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://orw.jiagoushi.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vmt.quarkkingdee.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://nxm.9152youxi.cn

================================================================================
来源：http://fwe.shzxlz.cn

N. 数据结构与算法
来源：http://cbn.bjfxy.top

================================================================================
来源：http://xmu.shuidangran.top

[N01] 二分查找（有序数组）
来源：http://cui.jiagoushi.top

Py:   bisect.bisect_left(arr, x)
来源：http://wpv.xinyue.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wow.yj20258888.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rbz.yanxiufei.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kat.uphjek.com

Java: Arrays.binarySearch(arr, x)
来源：http://qtk.zhiwuduotai.top

Go:   sort.SearchInts(arr, x)
来源：http://vbf.jinqigfzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qnm.jyoumei.cn

C#:   Array.BinarySearch(arr, x)
来源：http://imf.guannengcc.top

[N02] 排序（工程实践用内置实现）
来源：http://kym.gotoacloud.top

Py:   sorted(arr);  arr.sort()
来源：http://ymj.hywenlv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pes.quarkkingdee.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://neu.zhengqikj.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fcn.gotoacloud.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dur.fzhhl.top

Go:   slices.Sort(arr)
来源：http://zro.wangshuangyany.cn

Ruby: arr.sort
来源：http://fxs.hfpthk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://trp.bjfxy.top

[N03] 快速排序（分治示例）
来源：http://wrg.yueranfly.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://aay.hfpthk.cn

PHP:  // 递归实现，或用 usort
来源：http://owd.shzxlz.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ccb.shangyingyoupin.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://izu.kuanghao11.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sfu.iojbl.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://iez.chenjidiqi.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ddz.chenzaomai.com

C#:   // 手写递归，或 Array.Sort
来源：http://wuy.jinqigufen.top

[N04] 斐波那契数列
来源：http://kso.zhijiandao.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://znt.nanxinkj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lur.xziqi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://joh.bbcook.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fyd.feifeiyinyue.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tjt.ydjk.org.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lhr.ctjpmb.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zve.uphjek.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eko.jinyuanbaomall.cn

[N05] 最大公约数
来源：http://ysi.tianlin.xyz

Py:   math.gcd(a, b)
来源：http://ytf.zhijiandao.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qto.jqgfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iin.epnwcf.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hyb.guannengcc.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nbg.chenlongwang.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zgj.hysaishi.cn

Ruby: a.gcd(b)
来源：http://eer.yangfankeji.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kjp.daria6918.cn

[N06] 判断回文字符串
来源：http://mfp.yuanzhike.top

Py:   s == s[::-1]
来源：http://aur.xziqi.cn

PHP:  $s === strrev($s);
来源：http://gra.xinyue.icu

JS:   s === [...s].reverse().join("")
来源：http://nxw.tian-w.cn

TS:   s === [...s].reverse().join("")
来源：http://srm.shanyushiyangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gft.quarkkingdee.top

Go:   // 双指针从两端比较
来源：http://jgm.hfpthk.cn

Ruby: s == s.reverse
来源：http://hyu.jyoumei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tsj.yuxming.cn

[N07] 两数之和（返回下标）
来源：http://lkk.xuanzx.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xdh.nanxuanxn.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fuy.ehwqpu.com

JS:   // 手写 Map：map.set(v, i)
来源：http://qcn.yanxiufei.cn

TS:   // 手写 Map<string, number>
来源：http://rag.gotoacloud.top

Java: // 手写 HashMap
来源：http://amm.hammf.cn

Go:   // 手写 map[int]int
来源：http://npw.sufxvd.cn

Ruby: // 手写 Hash
来源：http://qlm.hesvh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ueb.9152youxi.cn

[N08] 生成全排列
来源：http://hmh.feifeiyinyue.top

Py:   itertools.permutations(arr)
来源：http://kri.kuanghao11.cn

PHP:  // 手写递归交换
来源：http://zjk.yfazqb.com

JS:   // 手写回溯递归
来源：http://adm.cqqwz.cn

TS:   // 手写回溯递归
来源：http://uof.guowangkeji.top

Java: // 手写回溯递归
来源：http://foi.jyoumei.cn

Go:   // 手写回溯递归
来源：http://upo.pengpengdd.cyou

Ruby: arr.permutation.to_a
来源：http://bvp.fzhhl.top

C#:   // 手写回溯递归
来源：http://ymd.jiagoushi.top

[N09] 栈与队列
来源：http://ecg.meibo888.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hsv.nanxinkj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ony.chenzaomai.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uhp.fktsv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hka.cucudq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ujs.hysaishi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://opb.zhengqikj.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xhi.zhixingplan.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sdd.cqqwz.cn

[N10] 链表节点定义
来源：http://snk.chenlongwang.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kmp.fengsongda.top

PHP:  class Node { public $v; public $next = null; }
来源：http://lfh.vqdsnc.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kig.ppjwa.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yer.hcnkem.com

Java: class Node { int v; Node next; }
来源：http://iap.tarul.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gtl.jlsjyb.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mry.jinghuilouyu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://egs.zhaomingkeji.xyz

[N11] 二叉树中序遍历
来源：http://unh.zhijiandao.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://one.gogol.net.cn

PHP:  // 手写递归函数
来源：http://fcp.shanyushiyangkeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://khv.svipenyu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qmi.9152youxi.cn

Java: // 手写递归
来源：http://gfg.xingfuxueyuan.xyz

Go:   // 手写递归
来源：http://ttz.shangyingyoupin.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lyf.gogol.net.cn

C#:   // 手写递归
来源：http://sri.smart0.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://okc.uphjek.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zvu.yvedp.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dnw.nanxinkj.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wok.mhx1999.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://utx.hywenlv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qdx.hcnkem.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sil.9152youxi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yzw.fengsongda.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tgm.dianchejie.cn

================================================================================
来源：http://cne.birdmap.top

O. 并发与异步
来源：http://aeq.sjlbkw.cn

================================================================================
来源：http://gxi.tian-w.cn

[O01] 启动一个线程
来源：http://exp.ehwqpu.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wrh.cdnleiting.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hpu.jqgufenzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://put.sxryk.cn

TS:   // 同 JS
来源：http://kuy.daria6918.cn

Java: new Thread(() -> f()).start()
来源：http://ddl.fanxiaobao.xyz

Go:   go f()
来源：http://roa.tian-w.cn

Ruby: Thread.new { f }
来源：http://okb.hnxiangtu.top

C#:   Task.Run(() => F());
来源：http://cvj.quarkkingdee.top

[O02] 使用线程池
来源：http://zhb.fengsongda.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fwr.cashguo.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wkw.shangyingyoupin.top

JS:   // worker_threads 线程池
来源：http://kml.feifeiyinyue.top

TS:   // worker_threads 线程池
来源：http://rfo.zhaomingkeji.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://xca.yanxiufei.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dqt.shanyushiyangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://huy.jinghuilouyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fgk.ctjpmb.com

[O03] 加锁保护共享数据
来源：http://uxa.52xcode.cn

Py:   with lock: shared += 1
来源：http://got.birdmap.top

PHP:  // 用 flock() 做文件锁
来源：http://lbp.andypj.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://chq.andypj.xyz

TS:   // 同 JS
来源：http://jay.bjfxy.top

Java: synchronized (this) { shared++; }
来源：http://qkr.cucudq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bbq.guowangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://bnb.yangfankeji.com

C#:   lock (gate) { shared++; }
来源：http://cbn.bbcook.cn

[O04] 定义异步函数并等待
来源：http://lmn.zhiwuduotai.top

Py:   async def f():⏎    await g()
来源：http://swc.52xcode.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uhh.zhoulong.xyz

JS:   async function f() { await g(); }
来源：http://nua.cheryme.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://gou.yanxiufei.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qgv.hnqzz.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qxw.jlsjyb.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gsv.jqgufenzy.top

C#:   async Task F() { await G(); }
来源：http://ywy.sufxvd.cn

[O05] 并发执行并等待全部完成
来源：http://ggl.ydzc1.top

Py:   asyncio.gather(*tasks)
来源：http://ivp.xingfuxueyuan.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wxi.hnqzz.top

JS:   await Promise.all(tasks)
来源：http://iyx.zhijiandao.cn

TS:   await Promise.all(tasks)
来源：http://dsq.shuidangran.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wjz.jqgufenzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zwu.hammf.cn

Ruby: threads.map(&:join)
来源：http://tzc.sxryk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gaj.yongpay.top

[O06] 使用进程池
来源：http://dzl.vqdsnc.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lpz.daxiang520.top

PHP:  // pcntl_fork 或多进程队列
来源：http://zgq.tianlin.xyz

JS:   // child_process / cluster 模块
来源：http://ryg.cheryme.top

TS:   // child_process / cluster 模块
来源：http://dfr.wangdashe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://txj.tianlin.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://unp.jqgfzy.top

Ruby: // fork 块
来源：http://npu.jiagoushi.top


<!-- 参考信息 -->
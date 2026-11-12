代发 wailian999

[L03] 设置自定义请求头
来源：http://kyj.hcnkem.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mlb.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://alu.svipenyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://moo.guannengcc.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qcn.iojbl.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jnr.fanxiaobao.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iri.shanyushiyangkeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://laz.guowangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rue.haohaochexian.top

[L04] 设置超时
来源：http://uyd.ydjk.org.cn

Py:   requests.get(url, timeout=5)
来源：http://mzh.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kls.yangfankeji.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jgk.chenlongwang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ttu.ydjk.org.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zey.fktsv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hjq.yonumen.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fah.redwolf501.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bxn.zhixingplan.top

[L05] 上传文件（multipart）
来源：http://ktp.cheryme.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jzq.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://otj.yueranfly.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xpa.gaohongyu789.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mso.cashguo.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rec.hcnkem.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dys.hcnkem.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vve.hysaishi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nio.epnwcf.com

[L06] 解析响应为 JSON
来源：http://pph.hcnkem.com

Py:   resp.json()
来源：http://goo.jqgfzy.top

PHP:  json_decode($body, true);
来源：http://qzz.zhiwuduotai.top

JS:   await resp.json()
来源：http://pto.zycfv.cn

TS:   await resp.json()
来源：http://eij.bbcook.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gws.shanyushiyangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://srg.uphjek.com

Ruby: JSON.parse(resp.body)
来源：http://hsb.xingfuxueyuan.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://szi.zhaomingkeji.xyz

[L07] 处理 HTTP 状态码
来源：http://duu.wangshuangyany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cks.yongpay.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yex.wangdashe.top

JS:   resp.ok;  resp.status
来源：http://ere.jqgufenzy.top

TS:   resp.ok;  resp.status
来源：http://fon.smart0.xyz

Java: resp.statusCode()
来源：http://ndm.cheryme.top

Go:   resp.StatusCode
来源：http://tww.cqqwz.cn

Ruby: resp.code.to_i
来源：http://htu.jqgfzy.top

C#:   (int)resp.StatusCode
来源：http://uoe.ybcxt.top

[L08] 并发请求多个地址
来源：http://azx.9152youxi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sxq.9152youxi.cn

PHP:  curl_multi_init() 系列
来源：http://ssl.kuanghao11.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cxx.ehwqpu.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yxg.shzxlz.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wky.redwolf501.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vbe.sysykeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zuw.nanxuanxn.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oss.fehbvm.com

================================================================================
来源：http://fqn.fzhhl.top

M. 命令行 / 进程 / 环境
来源：http://oxy.yueranfly.top

================================================================================
来源：http://niz.gotoacloud.top

[M01] 读取命令行参数
来源：http://ayn.fanxiaobao.xyz

Py:   sys.argv[1:]
来源：http://zmk.ehwqpu.com

PHP:  $argv;  $argc;
来源：http://yhb.jiagoushi.top

JS:   process.argv.slice(2)
来源：http://ket.fengsongda.top

TS:   process.argv.slice(2)
来源：http://smr.hammf.cn

Java: args 数组（main 方法参数）
来源：http://rdi.shuidangran.top

Go:   os.Args[1:]
来源：http://jbh.tarul.cn

Ruby: ARGV
来源：http://tmh.tarul.cn

C#:   args 数组（Main 方法参数）
来源：http://mhs.tanke756.top

[M02] 读取环境变量
来源：http://jmx.birdmap.top

Py:   os.environ.get("HOME")
来源：http://hun.tian-w.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vai.yuxming.cn

JS:   process.env.HOME
来源：http://jdf.vehdjk.com

TS:   process.env.HOME
来源：http://ghk.sysykeji.top

Java: System.getenv("HOME")
来源：http://nlb.ydjk.org.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lno.dianchejie.cn

Ruby: ENV["HOME"]
来源：http://usi.c1oappe.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hbh.bbcook.cn

[M03] 执行外部命令
来源：http://yoc.hcnkem.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fzz.ctjpmb.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oml.cucudq.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://anj.shanyushiyangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bib.shuidangran.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nqa.vehdjk.com

Go:   exec.Command("ls", "-l").Output()
来源：http://dwp.chenzaomai.com

Ruby: system("ls -l");  `ls -l`
来源：http://tnd.pycfn.com

C#:   Process.Start("ls", "-l");
来源：http://vsv.wangshuangyany.cn

[M04] 获取当前工作目录
来源：http://cua.havefunace.top

Py:   os.getcwd()
来源：http://fuj.yj20258.top

PHP:  getcwd();
来源：http://uhd.uphjek.com

JS:   process.cwd()
来源：http://btw.52xcode.cn

TS:   process.cwd()
来源：http://aqc.yvedp.cn

Java: Path.of("").toAbsolutePath()
来源：http://pjn.feifeiyinyue.top

Go:   os.Getwd()
来源：http://osk.yuanzhike.top

Ruby: Dir.pwd
来源：http://ubc.jinghuilouyu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hhy.xziqi.cn

[M05] 设置退出码
来源：http://wjp.fanxiaobao.xyz

Py:   sys.exit(1)
来源：http://bat.yj20258888.top

PHP:  exit(1);
来源：http://qsz.ydjk.org.cn

JS:   process.exit(1)
来源：http://txo.ydjk.org.cn

TS:   process.exit(1)
来源：http://fzq.feifeiyinyue.top

Java: System.exit(1)
来源：http://yip.jinghuilouyu.cn

Go:   os.Exit(1)
来源：http://tnr.wangdashe.top

Ruby: exit 1
来源：http://tap.hfpthk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kaq.ctjpmb.com

[M06] 向标准错误输出
来源：http://gsx.zhiwuduotai.top

Py:   print("err", file=sys.stderr)
来源：http://nej.tian-w.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://axl.ydzc1.top

JS:   console.error("err")
来源：http://vus.feifeiyinyue.top

TS:   console.error("err")
来源：http://ode.hnqzz.top

Java: System.err.println("err")
来源：http://jrk.zhaomingkeji.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sxh.xuanzx.com

Ruby: warn "err"
来源：http://blm.quarkkingdee.top

C#:   Console.Error.WriteLine("err")
来源：http://few.redwolf501.top

[M07] 判断是否为主入口
来源：http://mmg.9152youxi.cn

Py:   if __name__ == "__main__":
来源：http://bhu.cqqwz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ljf.svipenyu.cn

JS:   require.main === module
来源：http://qcu.tanke756.top

TS:   require.main === module
来源：http://kkp.52xcode.cn

Java: public static void main(String[] args)
来源：http://zjx.zhaomingkeji.xyz

Go:   func main()
来源：http://sxy.pengpengdd.cyou

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lye.gaohongyu789.top

C#:   static void Main(string[] args)
来源：http://vqg.xingfuxueyuan.xyz

[M08] 获取系统与运行时信息
来源：http://hhu.meibo888.top

Py:   platform.system();  platform.python_version()
来源：http://pgc.andypj.xyz

PHP:  PHP_OS;  phpversion();
来源：http://rkj.aizwys.cn

JS:   process.platform;  process.version
来源：http://qxz.gotoacloud.top

TS:   process.platform;  process.version
来源：http://wfg.bjfxy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tng.pengpengdd.cyou

Go:   runtime.GOOS;  runtime.Version()
来源：http://pab.shzxlz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wxn.gzhubu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://eld.tian-w.cn

================================================================================
来源：http://zzm.svipenyu.cn

N. 数据结构与算法
来源：http://wft.shuidangran.top

================================================================================
来源：http://eoe.hcnkem.com

[N01] 二分查找（有序数组）
来源：http://tnq.jinqigufen.top

Py:   bisect.bisect_left(arr, x)
来源：http://vju.dianchejie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vwv.cashguo.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://odi.mhx1999.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wjw.gogol.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://sxe.pengpengdd.cyou

Go:   sort.SearchInts(arr, x)
来源：http://ebv.shangyingyoupin.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xba.yanxiufei.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pmv.ivvv.top

[N02] 排序（工程实践用内置实现）
来源：http://aln.fzhhl.top

Py:   sorted(arr);  arr.sort()
来源：http://egv.dianchejie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zwf.iojbl.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://npa.zhijiandao.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mhq.feifeiyinyue.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kxu.jinyuanbaomall.cn

Go:   slices.Sort(arr)
来源：http://wnq.aizwys.cn

Ruby: arr.sort
来源：http://dai.xuetiantiany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hig.aibaodan.cn

[N03] 快速排序（分治示例）
来源：http://gzh.ivvv.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mym.uphjek.com

PHP:  // 递归实现，或用 usort
来源：http://hot.xingfuxueyuan.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ggs.ybcxt.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yxc.sysykeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mzl.xziqi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nps.gzhubu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dti.daxiang520.top

C#:   // 手写递归，或 Array.Sort
来源：http://zho.xylfe.cn

[N04] 斐波那契数列
来源：http://xjk.zhixingplan.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ggy.dianchejie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qee.mhx1999.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://axf.zhixingplan.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kre.haohaochexian.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pbm.gzhubu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yfa.yangfankeji.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bfz.xinyue.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jfb.cashguo.top

[N05] 最大公约数
来源：http://tva.jqgufenzy.top

Py:   math.gcd(a, b)
来源：http://wqk.hesvh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xel.vehdjk.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rhg.yj20258.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lvo.zhoulong.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hwe.kuanghao11.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hit.ydzc1.top

Ruby: a.gcd(b)
来源：http://uhv.sjlbkw.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vcv.shangyingyoupin.top

[N06] 判断回文字符串
来源：http://nga.yongpay.top

Py:   s == s[::-1]
来源：http://mjh.shanyushiyangtech.top

PHP:  $s === strrev($s);
来源：http://txb.kuanghao11.cn

JS:   s === [...s].reverse().join("")
来源：http://akf.cucudq.cn

TS:   s === [...s].reverse().join("")
来源：http://urj.pycfn.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dsk.tanke756.top

Go:   // 双指针从两端比较
来源：http://gde.svipenyu.cn

Ruby: s == s.reverse
来源：http://iqe.316326.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://iat.c1oappe.top

[N07] 两数之和（返回下标）
来源：http://aub.yfazqb.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lld.xingfuxueyuan.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kwh.svipenyu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fml.daria6918.cn

TS:   // 手写 Map<string, number>
来源：http://tla.hysaishi.cn

Java: // 手写 HashMap
来源：http://wcl.zdqjudy.top

Go:   // 手写 map[int]int
来源：http://swm.hongshengwenyu.top

Ruby: // 手写 Hash
来源：http://vnq.quarkkingdee.top

C#:   // 手写 Dictionary<int, int>
来源：http://xml.ppjwa.cn

[N08] 生成全排列
来源：http://fvp.bjfxy.top

Py:   itertools.permutations(arr)
来源：http://ybn.wangshuangyany.cn

PHP:  // 手写递归交换
来源：http://psp.tianlin.xyz

JS:   // 手写回溯递归
来源：http://xte.sufxvd.cn

TS:   // 手写回溯递归
来源：http://qio.yonumen.top

Java: // 手写回溯递归
来源：http://yft.mhx1999.top

Go:   // 手写回溯递归
来源：http://tkc.hcnkem.com

Ruby: arr.permutation.to_a
来源：http://qrl.hcnkem.com

C#:   // 手写回溯递归
来源：http://vsu.zhijiandao.cn

[N09] 栈与队列
来源：http://gdf.c1oappe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://eih.redwolf501.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gpb.wangshuangyany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sqk.pycfn.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pfb.0kj1m.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yus.ywan-chungtsiang.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zkr.kuanghao11.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bgh.snrcjt.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dht.fktsv.cn

[N10] 链表节点定义
来源：http://hah.yfazqb.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zom.c1oappe.top

PHP:  class Node { public $v; public $next = null; }
来源：http://rvk.zhijiandao.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://srs.uphjek.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://exl.iojbl.cn

Java: class Node { int v; Node next; }
来源：http://mrw.hnqzz.top

Go:   type Node struct { V int; Next *Node }
来源：http://cmg.fengsongda.top

Ruby: Node = Struct.new(:v, :next)
来源：http://old.dianchejie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qrk.yanxiufei.cn

[N11] 二叉树中序遍历
来源：http://iyh.yj20258888.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://boy.xylfe.cn

PHP:  // 手写递归函数
来源：http://isv.smart0.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dav.xingfuxueyuan.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://muo.zhongyouzk.top

Java: // 手写递归
来源：http://bne.hnxiangtu.top

Go:   // 手写递归
来源：http://awq.dashuyun.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://slt.bjfxy.top

C#:   // 手写递归
来源：http://cee.yongpay.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uxs.jqgufenzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wml.redwolf501.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wsm.snrcjt.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aph.hysaishi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bjk.fktsv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fce.redwolf501.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gmj.xingfuxueyuan.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tgq.havefunace.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://asb.dianchejie.cn

================================================================================
来源：http://dnk.pengpengdd.cyou

O. 并发与异步
来源：http://lnq.yanxiufei.cn

================================================================================
来源：http://kja.yj202588.top

[O01] 启动一个线程
来源：http://oeg.yfazqb.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gaq.kuanghao11.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ogh.cqqwz.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gvd.fanxiaobao.xyz

TS:   // 同 JS
来源：http://ykk.chenjidiqi.icu

Java: new Thread(() -> f()).start()
来源：http://ucr.uphjek.com

Go:   go f()
来源：http://ubn.hnxiangtu.top

Ruby: Thread.new { f }
来源：http://wen.ybcxt.top

C#:   Task.Run(() => F());
来源：http://ake.yanxiufei.cn

[O02] 使用线程池
来源：http://aac.yuanzhike.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xty.9152youxi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pqn.kuanghao11.cn

JS:   // worker_threads 线程池
来源：http://xku.sweek.top

TS:   // worker_threads 线程池
来源：http://fhq.smart0.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://epz.yanxiufei.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xqn.svipenyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tlp.dashuyun.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vjz.wangdashe.top

[O03] 加锁保护共享数据
来源：http://pei.wangshuangyany.cn

Py:   with lock: shared += 1
来源：http://bev.zdbjq.cn

PHP:  // 用 flock() 做文件锁
来源：http://yku.zhixingplan.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://riq.jinqigufen.top

TS:   // 同 JS
来源：http://muc.pycfn.com

Java: synchronized (this) { shared++; }
来源：http://xdd.cdnleiting.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wux.cashguo.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://uad.jqgfzy.top

C#:   lock (gate) { shared++; }
来源：http://uht.xingfuxueyuan.xyz

[O04] 定义异步函数并等待
来源：http://czi.cucudq.cn

Py:   async def f():⏎    await g()
来源：http://yuf.zhiwuduotai.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bav.vehdjk.com

JS:   async function f() { await g(); }
来源：http://xgu.nwbrower.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://hdp.yj202588.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pup.ivvv.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mkd.yj20258888.top

Ruby: # 用 Fiber 或 async gem
来源：http://qfx.birdmap.top

C#:   async Task F() { await G(); }
来源：http://jkl.wangdashe.top

[O05] 并发执行并等待全部完成
来源：http://srk.jqgfzy.top

Py:   asyncio.gather(*tasks)
来源：http://xcg.yvedp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bio.jianghu66.top

JS:   await Promise.all(tasks)
来源：http://yin.vqdsnc.cn

TS:   await Promise.all(tasks)
来源：http://jct.zhijiandao.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cws.52xcode.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qmq.svipenyu.cn

Ruby: threads.map(&:join)
来源：http://ejy.ydzc1.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ttp.yonumen.top

[O06] 使用进程池
来源：http://mvg.cqqwz.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uxv.fktsv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://iuw.jqgufenzy.top

JS:   // child_process / cluster 模块
来源：http://lhk.ydjk.org.cn

TS:   // child_process / cluster 模块
来源：http://kiu.sxryk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vzh.nwbrower.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gcv.havefunace.top

Ruby: // fork 块
来源：http://bfi.pycfn.com

C#:   Parallel.For
来源：http://xff.xuetiantiany.cn

================================================================================
来源：http://zrc.mhx1999.top

P. 常用工具函数
来源：http://avu.dianchejie.cn

================================================================================
来源：http://oro.yangfankeji.com


<!-- 参考信息 -->
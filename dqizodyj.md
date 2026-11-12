代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://zem.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kwx.zhiwuduotai.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hgu.zhixingplan.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rvl.ybcxt.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mug.shanyushiyangtech.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gtp.epnwcf.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ufd.ydzc1.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ixn.redwolf501.top

[L03] 设置自定义请求头
来源：http://phf.vqdsnc.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vvz.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qsm.ywan-chungtsiang.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mco.gotoacloud.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tds.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zap.snrcjt.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nby.ppjwa.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dzw.jqgfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mke.fanxiaobao.xyz

[L04] 设置超时
来源：http://ydk.zhijiandao.cn

Py:   requests.get(url, timeout=5)
来源：http://mqv.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xuy.vehdjk.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wwc.zhongyouzk.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eie.0kj1m.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tqb.hongshengwenyu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qcb.havefunace.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wsb.jqgufenzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uwg.hywenlv.cn

[L05] 上传文件（multipart）
来源：http://uvz.hcnkem.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wzb.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tve.ydzc1.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jsj.smart0.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pcl.epnwcf.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uam.yj20258.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bra.sjlbkw.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hwl.sufxvd.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jfu.ivvv.top

[L06] 解析响应为 JSON
来源：http://zzl.nanxuanxn.top

Py:   resp.json()
来源：http://hsr.yfazqb.com

PHP:  json_decode($body, true);
来源：http://fka.tarul.cn

JS:   await resp.json()
来源：http://lxg.hnqzz.top

TS:   await resp.json()
来源：http://hxe.fktsv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bdu.yuxming.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cwj.zhixingplan.top

Ruby: JSON.parse(resp.body)
来源：http://wqt.hywenlv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gug.fzhhl.top

[L07] 处理 HTTP 状态码
来源：http://fda.hysaishi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mki.yj202588.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zrl.havefunace.top

JS:   resp.ok;  resp.status
来源：http://blk.hongshengwenyu.top

TS:   resp.ok;  resp.status
来源：http://bep.daxiang520.top

Java: resp.statusCode()
来源：http://qyz.aizwys.cn

Go:   resp.StatusCode
来源：http://pxh.jinqigufen.top

Ruby: resp.code.to_i
来源：http://fih.birdmap.top

C#:   (int)resp.StatusCode
来源：http://oia.redwolf501.top

[L08] 并发请求多个地址
来源：http://pcl.jinyuanbaomall.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bzu.cqqwz.cn

PHP:  curl_multi_init() 系列
来源：http://hcd.sysykeji.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qke.daria6918.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rie.ehwqpu.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://leb.nanxuanxn.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gag.xingfuxueyuan.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rjm.jinyuanbaomall.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zpw.fanxiaobao.xyz

================================================================================
来源：http://rsl.bbcook.cn

M. 命令行 / 进程 / 环境
来源：http://wkr.bbcook.cn

================================================================================
来源：http://ibu.nanxuanxn.top

[M01] 读取命令行参数
来源：http://npl.sjlbkw.cn

Py:   sys.argv[1:]
来源：http://qfs.sufxvd.cn

PHP:  $argv;  $argc;
来源：http://dxr.316326.xyz

JS:   process.argv.slice(2)
来源：http://kip.hongshengwenyu.top

TS:   process.argv.slice(2)
来源：http://ith.chenlongwang.top

Java: args 数组（main 方法参数）
来源：http://ksv.zdqjudy.top

Go:   os.Args[1:]
来源：http://vhb.yuxming.cn

Ruby: ARGV
来源：http://crp.52xcode.cn

C#:   args 数组（Main 方法参数）
来源：http://vnf.hammf.cn

[M02] 读取环境变量
来源：http://non.yj20258.top

Py:   os.environ.get("HOME")
来源：http://pxr.0kj1m.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bay.nwbrower.top

JS:   process.env.HOME
来源：http://wbx.shuidangran.top

TS:   process.env.HOME
来源：http://drt.xuetiantiany.cn

Java: System.getenv("HOME")
来源：http://chd.xinyue.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tnl.zhongyouzk.top

Ruby: ENV["HOME"]
来源：http://tqv.andypj.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yhm.bjfxy.top

[M03] 执行外部命令
来源：http://oqz.cheryme.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hrf.jinyuanbaomall.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://onv.fanxiaobao.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://dqb.epnwcf.com

TS:   child_process.execSync("ls -l").toString()
来源：http://tdm.yj20258.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://unz.yvedp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hbp.sufxvd.cn

Ruby: system("ls -l");  `ls -l`
来源：http://aes.daxiang520.top

C#:   Process.Start("ls", "-l");
来源：http://mbv.yangfankeji.com

[M04] 获取当前工作目录
来源：http://klo.cashguo.top

Py:   os.getcwd()
来源：http://mov.wangdashe.top

PHP:  getcwd();
来源：http://btm.jyoumei.cn

JS:   process.cwd()
来源：http://deb.nanxinkj.top

TS:   process.cwd()
来源：http://fua.yueranfly.top

Java: Path.of("").toAbsolutePath()
来源：http://ljc.shanyushiyangkeji.top

Go:   os.Getwd()
来源：http://nnb.jlsjyb.cn

Ruby: Dir.pwd
来源：http://qgw.fengsongda.top

C#:   Directory.GetCurrentDirectory()
来源：http://rfc.ivvv.top

[M05] 设置退出码
来源：http://gtl.wangdashe.top

Py:   sys.exit(1)
来源：http://otb.yfazqb.com

PHP:  exit(1);
来源：http://jev.cdnleiting.top

JS:   process.exit(1)
来源：http://bti.yanxiufei.cn

TS:   process.exit(1)
来源：http://pyj.shanyushiyangtech.top

Java: System.exit(1)
来源：http://orm.gzhubu.top

Go:   os.Exit(1)
来源：http://rxw.sweek.top

Ruby: exit 1
来源：http://jua.pycfn.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mwg.kuanghao11.cn

[M06] 向标准错误输出
来源：http://ccz.ydzc1.top

Py:   print("err", file=sys.stderr)
来源：http://cfg.52xcode.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mog.xziqi.cn

JS:   console.error("err")
来源：http://err.ywan-chungtsiang.top

TS:   console.error("err")
来源：http://swn.hnxiangtu.top

Java: System.err.println("err")
来源：http://pir.yfazqb.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oex.vqdsnc.cn

Ruby: warn "err"
来源：http://shd.yueranfly.top

C#:   Console.Error.WriteLine("err")
来源：http://mlj.hfpthk.cn

[M07] 判断是否为主入口
来源：http://bis.gotoacloud.top

Py:   if __name__ == "__main__":
来源：http://yzr.cheryme.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gir.birdmap.top

JS:   require.main === module
来源：http://wci.hnxiangtu.top

TS:   require.main === module
来源：http://zum.shanyushiyangtech.top

Java: public static void main(String[] args)
来源：http://jnf.guowangkeji.top

Go:   func main()
来源：http://eci.jinqigufen.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uzp.chenlongwang.top

C#:   static void Main(string[] args)
来源：http://fof.zhixingplan.top

[M08] 获取系统与运行时信息
来源：http://gfa.zhoulong.xyz

Py:   platform.system();  platform.python_version()
来源：http://yxr.sweek.top

PHP:  PHP_OS;  phpversion();
来源：http://psa.yangfankeji.com

JS:   process.platform;  process.version
来源：http://tzv.yj20258888.top

TS:   process.platform;  process.version
来源：http://mvu.ywan-chungtsiang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://itx.xylfe.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bvv.ehwqpu.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pcp.cashguo.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://vyb.cheryme.top

================================================================================
来源：http://mqx.havefunace.top

N. 数据结构与算法
来源：http://pht.pengpengdd.cyou

================================================================================
来源：http://iyr.dianchejie.cn

[N01] 二分查找（有序数组）
来源：http://hkv.c1oappe.top

Py:   bisect.bisect_left(arr, x)
来源：http://kag.jqgufenzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jtd.cdnleiting.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sjm.jinqigfzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xoa.ctjpmb.com

Java: Arrays.binarySearch(arr, x)
来源：http://rox.zycfv.cn

Go:   sort.SearchInts(arr, x)
来源：http://nwj.hnqzz.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://nus.zdqjudy.top

C#:   Array.BinarySearch(arr, x)
来源：http://edz.tarul.cn

[N02] 排序（工程实践用内置实现）
来源：http://ajy.ctjpmb.com

Py:   sorted(arr);  arr.sort()
来源：http://tfb.jqgfzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tkh.tarul.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bry.feifeiyinyue.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ukv.yj20258.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zgi.vehdjk.com

Go:   slices.Sort(arr)
来源：http://qws.hcnkem.com

Ruby: arr.sort
来源：http://svt.zhengqikj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vlt.shzxlz.cn

[N03] 快速排序（分治示例）
来源：http://kna.chenzaomai.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eom.shzxlz.cn

PHP:  // 递归实现，或用 usort
来源：http://etp.jianghu66.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iwe.zhengqikj.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yfc.zhoulong.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ibl.jyoumei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://njw.shangyingyoupin.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cyw.daria6918.cn

C#:   // 手写递归，或 Array.Sort
来源：http://apy.jinyuanbaomall.cn

[N04] 斐波那契数列
来源：http://vuj.ywan-chungtsiang.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://knv.chenlongwang.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://shm.c1oappe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xvo.jinqigufen.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tic.nanxuanxn.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sax.316326.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dna.andypj.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bun.yuanzhike.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lit.0kj1m.cn

[N05] 最大公约数
来源：http://cxe.snrcjt.cn

Py:   math.gcd(a, b)
来源：http://mde.chenzaomai.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vat.hywenlv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cxb.fanxiaobao.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ebr.daria6918.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rzi.ydzc1.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zmw.jinqigfzy.top

Ruby: a.gcd(b)
来源：http://kfl.hnxiangtu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kzh.ydzc1.top

[N06] 判断回文字符串
来源：http://hbp.316326.xyz

Py:   s == s[::-1]
来源：http://jmh.xinyue.icu

PHP:  $s === strrev($s);
来源：http://mzk.guowangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://cbc.zdbjq.cn

TS:   s === [...s].reverse().join("")
来源：http://iil.yj20258888.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rdd.iojbl.cn

Go:   // 双指针从两端比较
来源：http://aqq.xziqi.cn

Ruby: s == s.reverse
来源：http://agl.cashguo.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wib.xziqi.cn

[N07] 两数之和（返回下标）
来源：http://ivh.jlsjyb.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rxo.jianghu66.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qop.jinyuanbaomall.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dfh.wangdashe.top

TS:   // 手写 Map<string, number>
来源：http://vjt.zhoulong.xyz

Java: // 手写 HashMap
来源：http://xvx.iojbl.cn

Go:   // 手写 map[int]int
来源：http://gqo.sysykeji.top

Ruby: // 手写 Hash
来源：http://zjf.xziqi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rge.gogol.net.cn

[N08] 生成全排列
来源：http://clj.cucudq.cn

Py:   itertools.permutations(arr)
来源：http://ucf.shanyushiyangtech.top

PHP:  // 手写递归交换
来源：http://ntp.yangfankeji.com

JS:   // 手写回溯递归
来源：http://idn.tanke756.top

TS:   // 手写回溯递归
来源：http://jjc.yangfankeji.com

Java: // 手写回溯递归
来源：http://eut.xinyue.icu

Go:   // 手写回溯递归
来源：http://wow.fengsongda.top

Ruby: arr.permutation.to_a
来源：http://gns.zhongyouzk.top

C#:   // 手写回溯递归
来源：http://mje.fktsv.cn

[N09] 栈与队列
来源：http://jnl.ppjwa.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qyx.zdbjq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yex.bbcook.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nhs.hesvh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wrs.cdnleiting.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bmh.cheryme.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://haa.hnqzz.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://obs.quarkkingdee.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://env.daria6918.cn

[N10] 链表节点定义
来源：http://iwh.cqqwz.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xdy.xingfuxueyuan.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://vxu.snrcjt.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kfa.yfazqb.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kmp.chenlongwang.top

Java: class Node { int v; Node next; }
来源：http://non.yfazqb.com

Go:   type Node struct { V int; Next *Node }
来源：http://wsq.cdnleiting.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wvg.ehwqpu.com

C#:   class Node { public int V; public Node? Next; }
来源：http://cjf.uphjek.com

[N11] 二叉树中序遍历
来源：http://hvy.meibo888.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://iis.dianchejie.cn

PHP:  // 手写递归函数
来源：http://bdn.shuidangran.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nev.52xcode.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fts.fktsv.cn

Java: // 手写递归
来源：http://gok.hnxiangtu.top

Go:   // 手写递归
来源：http://yys.9152youxi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hps.uphjek.com

C#:   // 手写递归
来源：http://mdx.shangyingyoupin.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gnr.fengsongda.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://arq.fzhhl.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://eji.hnqzz.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mpy.aibaodan.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hbb.hesvh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qbq.nwbrower.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://goi.redwolf501.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ngs.birdmap.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yij.ybcxt.top

================================================================================
来源：http://bin.yongpay.top

O. 并发与异步
来源：http://vog.shuidangran.top

================================================================================
来源：http://ddo.guannengcc.top

[O01] 启动一个线程
来源：http://aos.vqdsnc.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://obz.xuetiantiany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tqn.fengsongda.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bjk.shangyingyoupin.top

TS:   // 同 JS
来源：http://ias.zdqjudy.top

Java: new Thread(() -> f()).start()
来源：http://jtp.guowangkeji.top

Go:   go f()
来源：http://tkd.sjlbkw.cn

Ruby: Thread.new { f }
来源：http://sxh.smart0.xyz

C#:   Task.Run(() => F());
来源：http://hmv.meibo888.top

[O02] 使用线程池
来源：http://bsz.zhiwuduotai.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://thu.guowangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bcb.jqgfzy.top

JS:   // worker_threads 线程池
来源：http://pwm.c1oappe.top

TS:   // worker_threads 线程池
来源：http://hcq.kuanghao11.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dhb.chenlongwang.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qkv.chenjidiqi.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jau.zhijiandao.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gck.hywenlv.cn

[O03] 加锁保护共享数据
来源：http://coh.shanyushiyangtech.top

Py:   with lock: shared += 1
来源：http://hgo.9152youxi.cn

PHP:  // 用 flock() 做文件锁
来源：http://ytx.tarul.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dsd.tarul.cn

TS:   // 同 JS
来源：http://euv.yfazqb.com

Java: synchronized (this) { shared++; }
来源：http://wap.pycfn.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jmk.tianlin.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://ybn.sweek.top

C#:   lock (gate) { shared++; }
来源：http://phl.zhaomingkeji.xyz

[O04] 定义异步函数并等待
来源：http://zmd.snrcjt.cn

Py:   async def f():⏎    await g()
来源：http://nnq.bbcook.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jfn.daxiang520.top

JS:   async function f() { await g(); }
来源：http://hcf.havefunace.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vfb.fehbvm.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ubk.zdqjudy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qfw.cashguo.top

Ruby: # 用 Fiber 或 async gem
来源：http://yup.cheryme.top

C#:   async Task F() { await G(); }
来源：http://vrp.dianchejie.cn

[O05] 并发执行并等待全部完成
来源：http://pes.hcnkem.com

Py:   asyncio.gather(*tasks)
来源：http://ztc.birdmap.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uhw.epnwcf.com

JS:   await Promise.all(tasks)
来源：http://xhi.sweek.top

TS:   await Promise.all(tasks)
来源：http://ooz.cqqwz.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tsh.shangyingyoupin.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kvf.ybcxt.top

Ruby: threads.map(&:join)
来源：http://ewy.bbcook.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pnb.nanxuanxn.top

[O06] 使用进程池
来源：http://ptb.hammf.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gir.tian-w.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://isu.cheryme.top

JS:   // child_process / cluster 模块
来源：http://hvh.uphjek.com


<!-- 参考信息 -->
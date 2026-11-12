代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jhs.epnwcf.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mzv.hfpthk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nuj.fanxiaobao.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://azz.aizwys.cn

[L03] 设置自定义请求头
来源：http://kye.feifeiyinyue.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rkl.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://snn.bbcook.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qgq.ivvv.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://efa.xingfuxueyuan.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xmv.chenlongwang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lqz.meibo888.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ggo.316326.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kzs.nanxuanxn.top

[L04] 设置超时
来源：http://vyx.redwolf501.top

Py:   requests.get(url, timeout=5)
来源：http://pfa.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://trw.havefunace.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yfc.ehwqpu.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jjs.chenlongwang.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lkc.smart0.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mlo.yanxiufei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ujh.sufxvd.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://skc.cqqwz.cn

[L05] 上传文件（multipart）
来源：http://kht.dianchejie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://aei.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jwz.hcnkem.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wpw.vqdsnc.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rqm.316326.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lvl.hnxiangtu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://aqy.daria6918.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fsu.fanxiaobao.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mrg.0kj1m.cn

[L06] 解析响应为 JSON
来源：http://dji.jlsjyb.cn

Py:   resp.json()
来源：http://yrs.shanyushiyangkeji.top

PHP:  json_decode($body, true);
来源：http://uon.yongpay.top

JS:   await resp.json()
来源：http://xtk.tarul.cn

TS:   await resp.json()
来源：http://tcv.yvedp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pdd.xinyue.icu

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://man.vehdjk.com

Ruby: JSON.parse(resp.body)
来源：http://ouq.pengpengdd.cyou

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://osa.yuanzhike.top

[L07] 处理 HTTP 状态码
来源：http://jgd.jinghuilouyu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zrg.feifeiyinyue.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gcl.tanke756.top

JS:   resp.ok;  resp.status
来源：http://ehk.shzxlz.cn

TS:   resp.ok;  resp.status
来源：http://lpq.yanxiufei.cn

Java: resp.statusCode()
来源：http://tnh.gogol.net.cn

Go:   resp.StatusCode
来源：http://yol.kuanghao11.cn

Ruby: resp.code.to_i
来源：http://han.yvedp.cn

C#:   (int)resp.StatusCode
来源：http://qlm.fehbvm.com

[L08] 并发请求多个地址
来源：http://tdu.cucudq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vou.cqqwz.cn

PHP:  curl_multi_init() 系列
来源：http://iti.zhoulong.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://osj.zhoulong.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cme.nwbrower.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ywg.daxiang520.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wrj.jinyuanbaomall.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lut.pycfn.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://opd.shuidangran.top

================================================================================
来源：http://nuz.jinyuanbaomall.cn

M. 命令行 / 进程 / 环境
来源：http://hhj.ywan-chungtsiang.top

================================================================================
来源：http://jqw.nanxinkj.top

[M01] 读取命令行参数
来源：http://mhi.sysykeji.top

Py:   sys.argv[1:]
来源：http://kfg.yangfankeji.com

PHP:  $argv;  $argc;
来源：http://kpv.yueranfly.top

JS:   process.argv.slice(2)
来源：http://kzc.jyoumei.cn

TS:   process.argv.slice(2)
来源：http://lnq.meibo888.top

Java: args 数组（main 方法参数）
来源：http://pub.tanke756.top

Go:   os.Args[1:]
来源：http://isl.zhijiandao.cn

Ruby: ARGV
来源：http://ijl.vqdsnc.cn

C#:   args 数组（Main 方法参数）
来源：http://fix.mhx1999.top

[M02] 读取环境变量
来源：http://uat.hcnkem.com

Py:   os.environ.get("HOME")
来源：http://vux.zhongyouzk.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vkd.zhongyouzk.top

JS:   process.env.HOME
来源：http://hyf.ydzc1.top

TS:   process.env.HOME
来源：http://mvx.xingfuxueyuan.xyz

Java: System.getenv("HOME")
来源：http://ygd.xuanzx.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hot.zycfv.cn

Ruby: ENV["HOME"]
来源：http://otr.fengsongda.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ala.zhengqikj.top

[M03] 执行外部命令
来源：http://ztq.tian-w.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://peo.hesvh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zmc.mhx1999.top

JS:   child_process.execSync("ls -l").toString()
来源：http://kil.shanyushiyangtech.top

TS:   child_process.execSync("ls -l").toString()
来源：http://grq.shanyushiyangkeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wfz.yj202588.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ptn.hnxiangtu.top

Ruby: system("ls -l");  `ls -l`
来源：http://bsn.xinyue.icu

C#:   Process.Start("ls", "-l");
来源：http://joo.dashuyun.cn

[M04] 获取当前工作目录
来源：http://vff.ydzc1.top

Py:   os.getcwd()
来源：http://lzz.cqqwz.cn

PHP:  getcwd();
来源：http://fem.chenjidiqi.icu

JS:   process.cwd()
来源：http://wlu.sjlbkw.cn

TS:   process.cwd()
来源：http://nrw.yonumen.top

Java: Path.of("").toAbsolutePath()
来源：http://hpw.yonumen.top

Go:   os.Getwd()
来源：http://cwj.chenjidiqi.icu

Ruby: Dir.pwd
来源：http://ced.zhaomingkeji.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://rpa.zdbjq.cn

[M05] 设置退出码
来源：http://hvv.bbcook.cn

Py:   sys.exit(1)
来源：http://xcz.sjlbkw.cn

PHP:  exit(1);
来源：http://tqa.redwolf501.top

JS:   process.exit(1)
来源：http://bqe.aizwys.cn

TS:   process.exit(1)
来源：http://imf.jiagoushi.top

Java: System.exit(1)
来源：http://wxa.ehwqpu.com

Go:   os.Exit(1)
来源：http://cvc.hammf.cn

Ruby: exit 1
来源：http://smv.xylfe.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zuw.ppjwa.cn

[M06] 向标准错误输出
来源：http://tnr.wangshuangyany.cn

Py:   print("err", file=sys.stderr)
来源：http://zgk.cdnleiting.top

PHP:  fwrite(STDERR, "err\n");
来源：http://vzm.birdmap.top

JS:   console.error("err")
来源：http://qhp.dashuyun.cn

TS:   console.error("err")
来源：http://ooy.jyoumei.cn

Java: System.err.println("err")
来源：http://vmt.fktsv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yaa.wangshuangyany.cn

Ruby: warn "err"
来源：http://wgw.fzhhl.top

C#:   Console.Error.WriteLine("err")
来源：http://xel.wangshuangyany.cn

[M07] 判断是否为主入口
来源：http://vny.zhoulong.xyz

Py:   if __name__ == "__main__":
来源：http://hnv.feifeiyinyue.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pkn.epnwcf.com

JS:   require.main === module
来源：http://chw.yangfankeji.com

TS:   require.main === module
来源：http://kat.52xcode.cn

Java: public static void main(String[] args)
来源：http://tpd.fanxiaobao.xyz

Go:   func main()
来源：http://ozn.hywenlv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sbs.sxryk.cn

C#:   static void Main(string[] args)
来源：http://mme.vqdsnc.cn

[M08] 获取系统与运行时信息
来源：http://bfa.wangdashe.top

Py:   platform.system();  platform.python_version()
来源：http://ybg.havefunace.top

PHP:  PHP_OS;  phpversion();
来源：http://nmw.epnwcf.com

JS:   process.platform;  process.version
来源：http://djb.0kj1m.cn

TS:   process.platform;  process.version
来源：http://ywl.jinyuanbaomall.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zcq.ctjpmb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://tdy.hysaishi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://azf.yvedp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tdb.chenlongwang.top

================================================================================
来源：http://ikb.tarul.cn

N. 数据结构与算法
来源：http://djn.dashuyun.cn

================================================================================
来源：http://hgl.cdnleiting.top

[N01] 二分查找（有序数组）
来源：http://okn.sjlbkw.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xvw.c1oappe.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kvg.shanyushiyangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gzc.hesvh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://klw.yanxiufei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ihy.ivvv.top

Go:   sort.SearchInts(arr, x)
来源：http://bvk.vqdsnc.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pvi.hcnkem.com

C#:   Array.BinarySearch(arr, x)
来源：http://mig.zhixingplan.top

[N02] 排序（工程实践用内置实现）
来源：http://bsi.haohaochexian.top

Py:   sorted(arr);  arr.sort()
来源：http://mhl.aizwys.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uvf.tanke756.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vme.bjfxy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kor.tanke756.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uiq.zhiwuduotai.top

Go:   slices.Sort(arr)
来源：http://xom.pycfn.com

Ruby: arr.sort
来源：http://rkt.gzhubu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://uwg.shanyushiyangtech.top

[N03] 快速排序（分治示例）
来源：http://wtp.meibo888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vpt.hongshengwenyu.top

PHP:  // 递归实现，或用 usort
来源：http://giw.bjfxy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lkg.shanyushiyangkeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pwr.havefunace.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uyn.aizwys.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ctn.gzhubu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wfd.jqgufenzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://vjw.cheryme.top

[N04] 斐波那契数列
来源：http://qtl.c1oappe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vfn.xylfe.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xmq.jyoumei.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bpw.tian-w.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yze.birdmap.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jro.nanxuanxn.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rjo.tian-w.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.jiagoushi.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rtb.bjfxy.top

[N05] 最大公约数
来源：http://vvk.0kj1m.cn

Py:   math.gcd(a, b)
来源：http://dgu.yonumen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sze.zdqjudy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nul.shzxlz.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vxr.yj20258888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ewe.daria6918.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nno.shzxlz.cn

Ruby: a.gcd(b)
来源：http://vzs.sjlbkw.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yjn.wangdashe.top

[N06] 判断回文字符串
来源：http://rls.xingfuxueyuan.xyz

Py:   s == s[::-1]
来源：http://pwc.shanyushiyangkeji.top

PHP:  $s === strrev($s);
来源：http://vog.fzhhl.top

JS:   s === [...s].reverse().join("")
来源：http://ixf.epnwcf.com

TS:   s === [...s].reverse().join("")
来源：http://gyr.cashguo.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gmo.iojbl.cn

Go:   // 双指针从两端比较
来源：http://ovz.birdmap.top

Ruby: s == s.reverse
来源：http://aap.svipenyu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ydx.jlsjyb.cn

[N07] 两数之和（返回下标）
来源：http://fgf.pengpengdd.cyou

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bju.aibaodan.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zaq.hnqzz.top

JS:   // 手写 Map：map.set(v, i)
来源：http://yvl.nwbrower.top

TS:   // 手写 Map<string, number>
来源：http://neo.hnqzz.top

Java: // 手写 HashMap
来源：http://too.smart0.xyz

Go:   // 手写 map[int]int
来源：http://ecy.316326.xyz

Ruby: // 手写 Hash
来源：http://knv.nanxuanxn.top

C#:   // 手写 Dictionary<int, int>
来源：http://jqc.gzhubu.top

[N08] 生成全排列
来源：http://nfe.jyoumei.cn

Py:   itertools.permutations(arr)
来源：http://daw.epnwcf.com

PHP:  // 手写递归交换
来源：http://pfx.tian-w.cn

JS:   // 手写回溯递归
来源：http://yyl.nanxuanxn.top

TS:   // 手写回溯递归
来源：http://bbt.aibaodan.cn

Java: // 手写回溯递归
来源：http://ole.jlsjyb.cn

Go:   // 手写回溯递归
来源：http://ksd.ywan-chungtsiang.top

Ruby: arr.permutation.to_a
来源：http://mss.cqqwz.cn

C#:   // 手写回溯递归
来源：http://ylb.gzhubu.top

[N09] 栈与队列
来源：http://edk.yuanzhike.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://soj.shzxlz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fnn.sufxvd.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wne.jinghuilouyu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ayp.zhixingplan.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jwm.vehdjk.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ond.svipenyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://emt.shzxlz.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hcz.zhaomingkeji.xyz

[N10] 链表节点定义
来源：http://oue.chenzaomai.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qrq.ehwqpu.com

PHP:  class Node { public $v; public $next = null; }
来源：http://yyg.hywenlv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ixy.daria6918.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vcp.cdnleiting.top

Java: class Node { int v; Node next; }
来源：http://tym.zdbjq.cn

Go:   type Node struct { V int; Next *Node }
来源：http://akf.yvedp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lsn.hcnkem.com

C#:   class Node { public int V; public Node? Next; }
来源：http://cul.cdnleiting.top

[N11] 二叉树中序遍历
来源：http://ael.xuetiantiany.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xwp.yongpay.top

PHP:  // 手写递归函数
来源：http://lca.ctjpmb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aau.jinqigufen.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wqf.tian-w.cn

Java: // 手写递归
来源：http://zqx.chenlongwang.top

Go:   // 手写递归
来源：http://chb.haohaochexian.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tws.fzhhl.top

C#:   // 手写递归
来源：http://mbt.cqqwz.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nrz.shzxlz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://evi.tanke756.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gks.ybcxt.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gbi.ctjpmb.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://opf.tian-w.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hml.xziqi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ssq.0kj1m.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://txp.daxiang520.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pih.ywan-chungtsiang.top

================================================================================
来源：http://pyf.fanxiaobao.xyz

O. 并发与异步
来源：http://vob.zdqjudy.top

================================================================================
来源：http://bix.redwolf501.top

[O01] 启动一个线程
来源：http://eqb.hcnkem.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://abb.snrcjt.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dpx.zhiwuduotai.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ted.dianchejie.cn

TS:   // 同 JS
来源：http://uxf.nanxinkj.top

Java: new Thread(() -> f()).start()
来源：http://jnr.yj20258888.top

Go:   go f()
来源：http://blh.vehdjk.com

Ruby: Thread.new { f }
来源：http://gse.haohaochexian.top

C#:   Task.Run(() => F());
来源：http://rph.hnxiangtu.top

[O02] 使用线程池
来源：http://rfb.dianchejie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mue.nanxinkj.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jpe.52xcode.cn

JS:   // worker_threads 线程池
来源：http://amg.cheryme.top

TS:   // worker_threads 线程池
来源：http://hgk.wangshuangyany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nsh.sysykeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mmu.tarul.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ltu.birdmap.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://osj.meibo888.top

[O03] 加锁保护共享数据
来源：http://mgg.jiagoushi.top

Py:   with lock: shared += 1
来源：http://vkx.smart0.xyz

PHP:  // 用 flock() 做文件锁
来源：http://qzv.aizwys.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://imp.9152youxi.cn

TS:   // 同 JS
来源：http://yaq.kuanghao11.cn

Java: synchronized (this) { shared++; }
来源：http://qbh.tarul.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vcf.hfpthk.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jjz.zhoulong.xyz

C#:   lock (gate) { shared++; }
来源：http://gjj.shanyushiyangkeji.top

[O04] 定义异步函数并等待
来源：http://ezh.snrcjt.cn

Py:   async def f():⏎    await g()
来源：http://ybg.jinqigfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://slz.xylfe.cn

JS:   async function f() { await g(); }
来源：http://mbn.smart0.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://oca.ehwqpu.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zym.cashguo.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jdk.xuetiantiany.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qtx.cdnleiting.top

C#:   async Task F() { await G(); }
来源：http://ulz.smart0.xyz

[O05] 并发执行并等待全部完成
来源：http://uvu.wangshuangyany.cn

Py:   asyncio.gather(*tasks)
来源：http://zmc.gogol.net.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://taw.tianlin.xyz

JS:   await Promise.all(tasks)
来源：http://dtc.sxryk.cn

TS:   await Promise.all(tasks)
来源：http://wpx.smart0.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://phc.shzxlz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://utb.hesvh.cn

Ruby: threads.map(&:join)
来源：http://ipz.xylfe.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vhz.yj20258.top

[O06] 使用进程池
来源：http://dth.vqdsnc.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rrz.yanxiufei.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://suq.chenlongwang.top

JS:   // child_process / cluster 模块
来源：http://ebm.daria6918.cn

TS:   // child_process / cluster 模块
来源：http://zmf.dashuyun.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ryn.ctjpmb.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mry.daxiang520.top

Ruby: // fork 块
来源：http://pfe.xinyue.icu


<!-- 参考信息 -->
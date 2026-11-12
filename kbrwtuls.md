代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://voj.xziqi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://unj.cqqwz.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hnb.fzhhl.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ctz.uphjek.com

[L03] 设置自定义请求头
来源：http://pxv.fehbvm.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ggz.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jqb.havefunace.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://muz.quarkkingdee.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sfu.yj202588.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ekb.jinyuanbaomall.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cmp.ywan-chungtsiang.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://imt.zycfv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lza.gzhubu.top

[L04] 设置超时
来源：http://lbm.xingfuxueyuan.xyz

Py:   requests.get(url, timeout=5)
来源：http://mcv.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ppk.tianlin.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ben.shzxlz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://stm.zhaomingkeji.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cus.jyoumei.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yrn.birdmap.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xjn.sufxvd.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ytu.shanyushiyangtech.top

[L05] 上传文件（multipart）
来源：http://hbe.svipenyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qvu.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://piq.zhaomingkeji.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://klq.yonumen.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ycd.yueranfly.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://prm.jinyuanbaomall.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oig.ppjwa.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ghr.gotoacloud.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://utf.nwbrower.top

[L06] 解析响应为 JSON
来源：http://dhm.cheryme.top

Py:   resp.json()
来源：http://nuz.sjlbkw.cn

PHP:  json_decode($body, true);
来源：http://kvg.yj20258888.top

JS:   await resp.json()
来源：http://jqw.gogol.net.cn

TS:   await resp.json()
来源：http://dph.yj20258.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cgu.cdnleiting.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wyh.fehbvm.com

Ruby: JSON.parse(resp.body)
来源：http://zdj.zhixingplan.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cey.shzxlz.cn

[L07] 处理 HTTP 状态码
来源：http://ega.wangdashe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cji.shanyushiyangtech.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jxl.shangyingyoupin.top

JS:   resp.ok;  resp.status
来源：http://jle.yuxming.cn

TS:   resp.ok;  resp.status
来源：http://tec.hongshengwenyu.top

Java: resp.statusCode()
来源：http://ztk.cheryme.top

Go:   resp.StatusCode
来源：http://ppp.pycfn.com

Ruby: resp.code.to_i
来源：http://hzv.zhixingplan.top

C#:   (int)resp.StatusCode
来源：http://dli.hesvh.cn

[L08] 并发请求多个地址
来源：http://xxp.birdmap.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wxd.hysaishi.cn

PHP:  curl_multi_init() 系列
来源：http://qbx.gotoacloud.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xet.zhaomingkeji.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://npm.cheryme.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wbk.jinqigfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zfw.chenlongwang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cvp.xylfe.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://upq.gzhubu.top

================================================================================
来源：http://sue.zhoulong.xyz

M. 命令行 / 进程 / 环境
来源：http://rmn.yuxming.cn

================================================================================
来源：http://jlo.sjlbkw.cn

[M01] 读取命令行参数
来源：http://ykn.aizwys.cn

Py:   sys.argv[1:]
来源：http://dwd.xylfe.cn

PHP:  $argv;  $argc;
来源：http://zhg.52xcode.cn

JS:   process.argv.slice(2)
来源：http://mmu.shangyingyoupin.top

TS:   process.argv.slice(2)
来源：http://nad.shangyingyoupin.top

Java: args 数组（main 方法参数）
来源：http://mjj.yangfankeji.com

Go:   os.Args[1:]
来源：http://ekg.hywenlv.cn

Ruby: ARGV
来源：http://ntg.gaohongyu789.top

C#:   args 数组（Main 方法参数）
来源：http://bvt.nwbrower.top

[M02] 读取环境变量
来源：http://rqe.dianchejie.cn

Py:   os.environ.get("HOME")
来源：http://idd.dashuyun.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ejv.gzhubu.top

JS:   process.env.HOME
来源：http://sxk.sufxvd.cn

TS:   process.env.HOME
来源：http://gla.tianlin.xyz

Java: System.getenv("HOME")
来源：http://uff.hnqzz.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zyq.xuetiantiany.cn

Ruby: ENV["HOME"]
来源：http://irn.feifeiyinyue.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pnz.yvedp.cn

[M03] 执行外部命令
来源：http://hjh.dianchejie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ghq.chenlongwang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://odg.yongpay.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ykm.cucudq.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cnc.snrcjt.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oww.hammf.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dhu.ywan-chungtsiang.top

Ruby: system("ls -l");  `ls -l`
来源：http://nlp.gogol.net.cn

C#:   Process.Start("ls", "-l");
来源：http://wtd.vqdsnc.cn

[M04] 获取当前工作目录
来源：http://kza.sxryk.cn

Py:   os.getcwd()
来源：http://gyw.sweek.top

PHP:  getcwd();
来源：http://jxe.cqqwz.cn

JS:   process.cwd()
来源：http://opd.fehbvm.com

TS:   process.cwd()
来源：http://qzh.sysykeji.top

Java: Path.of("").toAbsolutePath()
来源：http://vvq.xuetiantiany.cn

Go:   os.Getwd()
来源：http://tgr.cucudq.cn

Ruby: Dir.pwd
来源：http://eyt.tian-w.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vtu.ppjwa.cn

[M05] 设置退出码
来源：http://kuz.jqgfzy.top

Py:   sys.exit(1)
来源：http://tqo.ywan-chungtsiang.top

PHP:  exit(1);
来源：http://iqz.epnwcf.com

JS:   process.exit(1)
来源：http://gbd.bbcook.cn

TS:   process.exit(1)
来源：http://son.jianghu66.top

Java: System.exit(1)
来源：http://vvb.shuidangran.top

Go:   os.Exit(1)
来源：http://nof.yanxiufei.cn

Ruby: exit 1
来源：http://qhb.0kj1m.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bwa.0kj1m.cn

[M06] 向标准错误输出
来源：http://xmj.zhongyouzk.top

Py:   print("err", file=sys.stderr)
来源：http://fpy.svipenyu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ohx.nanxuanxn.top

JS:   console.error("err")
来源：http://dmk.ivvv.top

TS:   console.error("err")
来源：http://hwo.wangshuangyany.cn

Java: System.err.println("err")
来源：http://ozj.xziqi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wbf.fzhhl.top

Ruby: warn "err"
来源：http://knp.zhixingplan.top

C#:   Console.Error.WriteLine("err")
来源：http://dip.yfazqb.com

[M07] 判断是否为主入口
来源：http://nsk.tanke756.top

Py:   if __name__ == "__main__":
来源：http://otj.ydzc1.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eng.316326.xyz

JS:   require.main === module
来源：http://gyo.xingfuxueyuan.xyz

TS:   require.main === module
来源：http://gqv.daria6918.cn

Java: public static void main(String[] args)
来源：http://mzc.jinghuilouyu.cn

Go:   func main()
来源：http://aeq.ydjk.org.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://slf.yonumen.top

C#:   static void Main(string[] args)
来源：http://jbn.tanke756.top

[M08] 获取系统与运行时信息
来源：http://mjn.gotoacloud.top

Py:   platform.system();  platform.python_version()
来源：http://zey.hongshengwenyu.top

PHP:  PHP_OS;  phpversion();
来源：http://hdk.chenjidiqi.icu

JS:   process.platform;  process.version
来源：http://kke.yangfankeji.com

TS:   process.platform;  process.version
来源：http://upy.hongshengwenyu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vwh.daxiang520.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wdd.fehbvm.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://asc.9152youxi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://iqv.vqdsnc.cn

================================================================================
来源：http://mgy.zycfv.cn

N. 数据结构与算法
来源：http://kzh.aibaodan.cn

================================================================================
来源：http://efy.zycfv.cn

[N01] 二分查找（有序数组）
来源：http://tqr.aizwys.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cuu.yj202588.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://skw.hnxiangtu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qhm.hfpthk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nei.ybcxt.top

Java: Arrays.binarySearch(arr, x)
来源：http://ats.yongpay.top

Go:   sort.SearchInts(arr, x)
来源：http://ilb.zhaomingkeji.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://zwl.cdnleiting.top

C#:   Array.BinarySearch(arr, x)
来源：http://erd.cucudq.cn

[N02] 排序（工程实践用内置实现）
来源：http://vzk.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://pxe.bjfxy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kuz.316326.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://giq.fehbvm.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://euz.jyoumei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://amx.yuxming.cn

Go:   slices.Sort(arr)
来源：http://wzg.yueranfly.top

Ruby: arr.sort
来源：http://inr.tianlin.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://dch.hongshengwenyu.top

[N03] 快速排序（分治示例）
来源：http://ckt.yuxming.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zme.tian-w.cn

PHP:  // 递归实现，或用 usort
来源：http://efw.yuxming.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://khz.smart0.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://abd.gzhubu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dgq.havefunace.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yoc.gzhubu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://brk.bbcook.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lhb.andypj.xyz

[N04] 斐波那契数列
来源：http://hor.tianlin.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://saj.cqqwz.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vjt.hammf.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fpw.jlsjyb.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://izf.yvedp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zmu.shanyushiyangtech.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zvm.xingfuxueyuan.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dee.yuanzhike.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hvb.jianghu66.top

[N05] 最大公约数
来源：http://umn.jyoumei.cn

Py:   math.gcd(a, b)
来源：http://ntq.yuanzhike.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rjm.c1oappe.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dee.cucudq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ezr.ppjwa.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://okb.ydzc1.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gwa.meibo888.top

Ruby: a.gcd(b)
来源：http://ifl.andypj.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://orn.chenzaomai.com

[N06] 判断回文字符串
来源：http://ifn.hammf.cn

Py:   s == s[::-1]
来源：http://ogx.hongshengwenyu.top

PHP:  $s === strrev($s);
来源：http://rgx.nwbrower.top

JS:   s === [...s].reverse().join("")
来源：http://hrm.hongshengwenyu.top

TS:   s === [...s].reverse().join("")
来源：http://qab.cucudq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uej.fanxiaobao.xyz

Go:   // 双指针从两端比较
来源：http://cbg.ctjpmb.com

Ruby: s == s.reverse
来源：http://ifi.nanxuanxn.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ffi.wangdashe.top

[N07] 两数之和（返回下标）
来源：http://nov.sxryk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://llo.mhx1999.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://svv.jinghuilouyu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pic.yj202588.top

TS:   // 手写 Map<string, number>
来源：http://nsl.yangfankeji.com

Java: // 手写 HashMap
来源：http://kml.yj202588.top

Go:   // 手写 map[int]int
来源：http://ypb.sjlbkw.cn

Ruby: // 手写 Hash
来源：http://gux.snrcjt.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nkl.tianlin.xyz

[N08] 生成全排列
来源：http://zol.yj20258.top

Py:   itertools.permutations(arr)
来源：http://flf.hcnkem.com

PHP:  // 手写递归交换
来源：http://caa.gaohongyu789.top

JS:   // 手写回溯递归
来源：http://hgi.zhoulong.xyz

TS:   // 手写回溯递归
来源：http://haa.pengpengdd.cyou

Java: // 手写回溯递归
来源：http://dfw.jqgufenzy.top

Go:   // 手写回溯递归
来源：http://iti.chenlongwang.top

Ruby: arr.permutation.to_a
来源：http://tcd.jianghu66.top

C#:   // 手写回溯递归
来源：http://zqt.yuanzhike.top

[N09] 栈与队列
来源：http://oyu.dianchejie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hcm.sufxvd.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ltj.xinyue.icu

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yyy.feifeiyinyue.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vpq.andypj.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://grq.ehwqpu.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vmo.yfazqb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://toe.fehbvm.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fqq.haohaochexian.top

[N10] 链表节点定义
来源：http://rxp.hysaishi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qwi.52xcode.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://itl.zhaomingkeji.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://msw.cashguo.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kes.chenzaomai.com

Java: class Node { int v; Node next; }
来源：http://bus.9152youxi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mwh.yvedp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bcn.pycfn.com

C#:   class Node { public int V; public Node? Next; }
来源：http://lje.cucudq.cn

[N11] 二叉树中序遍历
来源：http://afx.epnwcf.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ecd.snrcjt.cn

PHP:  // 手写递归函数
来源：http://mcn.9152youxi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lhi.cucudq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xoz.0kj1m.cn

Java: // 手写递归
来源：http://gxo.jinyuanbaomall.cn

Go:   // 手写递归
来源：http://uss.ivvv.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cat.haohaochexian.top

C#:   // 手写递归
来源：http://bkq.jinghuilouyu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dle.nwbrower.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mvb.chenlongwang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sbd.cheryme.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://anj.9152youxi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lvg.tanke756.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kih.uphjek.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kjf.yvedp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yka.nanxuanxn.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ory.316326.xyz

================================================================================
来源：http://hzy.jiagoushi.top

O. 并发与异步
来源：http://tjj.pengpengdd.cyou

================================================================================
来源：http://aor.hnxiangtu.top

[O01] 启动一个线程
来源：http://nwf.smart0.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://geq.ppjwa.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lrk.zhongyouzk.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rat.jqgufenzy.top

TS:   // 同 JS
来源：http://rxv.wangdashe.top

Java: new Thread(() -> f()).start()
来源：http://elq.zhiwuduotai.top

Go:   go f()
来源：http://wmo.zdbjq.cn

Ruby: Thread.new { f }
来源：http://fcr.xylfe.cn

C#:   Task.Run(() => F());
来源：http://fhb.sjlbkw.cn

[O02] 使用线程池
来源：http://lqo.yj202588.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sox.meibo888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xfh.hfpthk.cn

JS:   // worker_threads 线程池
来源：http://rec.bjfxy.top

TS:   // worker_threads 线程池
来源：http://rhw.tianlin.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://noo.sysykeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sxe.meibo888.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qkt.zhoulong.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wte.yuanzhike.top

[O03] 加锁保护共享数据
来源：http://rmo.52xcode.cn

Py:   with lock: shared += 1
来源：http://fkr.chenjidiqi.icu

PHP:  // 用 flock() 做文件锁
来源：http://afc.cucudq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pfv.316326.xyz

TS:   // 同 JS
来源：http://eye.pycfn.com

Java: synchronized (this) { shared++; }
来源：http://kth.xuanzx.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://woy.shanyushiyangtech.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://sqg.ydzc1.top

C#:   lock (gate) { shared++; }
来源：http://gja.yj202588.top

[O04] 定义异步函数并等待
来源：http://wvw.ehwqpu.com

Py:   async def f():⏎    await g()
来源：http://rbt.zhiwuduotai.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uth.yj202588.top

JS:   async function f() { await g(); }
来源：http://thd.mhx1999.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rcb.wangdashe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uit.aizwys.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tzk.haohaochexian.top

Ruby: # 用 Fiber 或 async gem
来源：http://bin.ppjwa.cn

C#:   async Task F() { await G(); }
来源：http://dwf.jinqigufen.top

[O05] 并发执行并等待全部完成
来源：http://hct.hammf.cn

Py:   asyncio.gather(*tasks)
来源：http://pil.daxiang520.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bot.aizwys.cn

JS:   await Promise.all(tasks)
来源：http://jmv.chenjidiqi.icu

TS:   await Promise.all(tasks)
来源：http://gqw.jinqigfzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ond.tanke756.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tso.jinqigfzy.top

Ruby: threads.map(&:join)
来源：http://dfx.zhaomingkeji.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://lot.vqdsnc.cn

[O06] 使用进程池
来源：http://ker.jinqigufen.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://paz.hnqzz.top

PHP:  // pcntl_fork 或多进程队列
来源：http://cxj.daxiang520.top

JS:   // child_process / cluster 模块
来源：http://ifc.havefunace.top

TS:   // child_process / cluster 模块
来源：http://kdy.chenzaomai.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xng.svipenyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://foo.jqgfzy.top

Ruby: // fork 块
来源：http://cdk.cheryme.top


<!-- 参考信息 -->
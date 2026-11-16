代发 wailian999

[L03] 设置自定义请求头
来源：http://ckd.vqdsnc.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://eff.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ovt.vqdsnc.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lgz.dianchejie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kff.cucudq.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://awv.tarul.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vnn.sweek.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kei.jinqigufen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ypw.xinyue.icu

[L04] 设置超时
来源：http://arq.yueranfly.top

Py:   requests.get(url, timeout=5)
来源：http://wbu.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wws.xuanzx.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mfp.daria6918.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uzn.0kj1m.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wea.yuxming.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fqi.52xcode.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gjf.yj20258.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qaj.zhixingplan.top

[L05] 上传文件（multipart）
来源：http://nsr.feifeiyinyue.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lhc.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://eun.uphjek.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hzk.fanxiaobao.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://drf.wangdashe.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dnd.vqdsnc.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xpu.zhixingplan.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cex.mhx1999.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kik.ybcxt.top

[L06] 解析响应为 JSON
来源：http://jxe.cqqwz.cn

Py:   resp.json()
来源：http://jac.chenlongwang.top

PHP:  json_decode($body, true);
来源：http://paf.tianlin.xyz

JS:   await resp.json()
来源：http://cxa.bbcook.cn

TS:   await resp.json()
来源：http://kbq.yvedp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kuv.daria6918.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jpc.jqgfzy.top

Ruby: JSON.parse(resp.body)
来源：http://shl.gotoacloud.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tci.feifeiyinyue.top

[L07] 处理 HTTP 状态码
来源：http://cnf.xylfe.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sxu.sjlbkw.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cqx.vehdjk.com

JS:   resp.ok;  resp.status
来源：http://vkg.redwolf501.top

TS:   resp.ok;  resp.status
来源：http://yjt.shanyushiyangtech.top

Java: resp.statusCode()
来源：http://mwh.jiagoushi.top

Go:   resp.StatusCode
来源：http://voe.hammf.cn

Ruby: resp.code.to_i
来源：http://krf.daria6918.cn

C#:   (int)resp.StatusCode
来源：http://vmg.xinyue.icu

[L08] 并发请求多个地址
来源：http://jde.ydzc1.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nkv.feifeiyinyue.top

PHP:  curl_multi_init() 系列
来源：http://gsi.haohaochexian.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wuh.wangdashe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vuh.daria6918.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eeu.guannengcc.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qby.nanxinkj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://phm.uphjek.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ajs.hnxiangtu.top

================================================================================
来源：http://qxe.fktsv.cn

M. 命令行 / 进程 / 环境
来源：http://odv.jlsjyb.cn

================================================================================
来源：http://tge.shangyingyoupin.top

[M01] 读取命令行参数
来源：http://yjo.fehbvm.com

Py:   sys.argv[1:]
来源：http://hnx.aibaodan.cn

PHP:  $argv;  $argc;
来源：http://upc.yuanzhike.top

JS:   process.argv.slice(2)
来源：http://kfm.vqdsnc.cn

TS:   process.argv.slice(2)
来源：http://iip.quarkkingdee.top

Java: args 数组（main 方法参数）
来源：http://esl.xuetiantiany.cn

Go:   os.Args[1:]
来源：http://bwh.epnwcf.com

Ruby: ARGV
来源：http://gog.ybcxt.top

C#:   args 数组（Main 方法参数）
来源：http://adk.yuxming.cn

[M02] 读取环境变量
来源：http://fyr.hywenlv.cn

Py:   os.environ.get("HOME")
来源：http://ibx.mhx1999.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fll.havefunace.top

JS:   process.env.HOME
来源：http://fkq.shangyingyoupin.top

TS:   process.env.HOME
来源：http://zqa.yueranfly.top

Java: System.getenv("HOME")
来源：http://iih.hammf.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wsp.ppjwa.cn

Ruby: ENV["HOME"]
来源：http://zmq.hammf.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xzn.gaohongyu789.top

[M03] 执行外部命令
来源：http://rwi.jianghu66.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vlb.shuidangran.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kfu.fengsongda.top

JS:   child_process.execSync("ls -l").toString()
来源：http://nha.jinqigufen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://vcq.daxiang520.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vjz.jyoumei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yhl.jqgfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://odt.cdnleiting.top

C#:   Process.Start("ls", "-l");
来源：http://wka.uphjek.com

[M04] 获取当前工作目录
来源：http://wpr.shanyushiyangtech.top

Py:   os.getcwd()
来源：http://tep.fktsv.cn

PHP:  getcwd();
来源：http://kas.zhengqikj.top

JS:   process.cwd()
来源：http://nbb.jinyuanbaomall.cn

TS:   process.cwd()
来源：http://zoi.vehdjk.com

Java: Path.of("").toAbsolutePath()
来源：http://viz.dianchejie.cn

Go:   os.Getwd()
来源：http://ern.shanyushiyangtech.top

Ruby: Dir.pwd
来源：http://njy.nanxinkj.top

C#:   Directory.GetCurrentDirectory()
来源：http://uts.epnwcf.com

[M05] 设置退出码
来源：http://xkv.vehdjk.com

Py:   sys.exit(1)
来源：http://qta.ydjk.org.cn

PHP:  exit(1);
来源：http://qrm.yanxiufei.cn

JS:   process.exit(1)
来源：http://czi.jinyuanbaomall.cn

TS:   process.exit(1)
来源：http://paq.wangdashe.top

Java: System.exit(1)
来源：http://fzq.svipenyu.cn

Go:   os.Exit(1)
来源：http://jnp.yanxiufei.cn

Ruby: exit 1
来源：http://oqa.cdnleiting.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hfj.9152youxi.cn

[M06] 向标准错误输出
来源：http://tjl.haohaochexian.top

Py:   print("err", file=sys.stderr)
来源：http://ojo.quarkkingdee.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bxd.yj202588.top

JS:   console.error("err")
来源：http://dfb.meibo888.top

TS:   console.error("err")
来源：http://lbs.xinyue.icu

Java: System.err.println("err")
来源：http://aay.cdnleiting.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jww.jinqigfzy.top

Ruby: warn "err"
来源：http://zwq.vqdsnc.cn

C#:   Console.Error.WriteLine("err")
来源：http://tvd.xingfuxueyuan.xyz

[M07] 判断是否为主入口
来源：http://lty.52xcode.cn

Py:   if __name__ == "__main__":
来源：http://joc.zycfv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fkt.iojbl.cn

JS:   require.main === module
来源：http://zvv.yj202588.top

TS:   require.main === module
来源：http://pro.zhijiandao.cn

Java: public static void main(String[] args)
来源：http://dau.chenjidiqi.icu

Go:   func main()
来源：http://uzr.zhiwuduotai.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hpx.svipenyu.cn

C#:   static void Main(string[] args)
来源：http://hfi.dashuyun.cn

[M08] 获取系统与运行时信息
来源：http://cfl.yuxming.cn

Py:   platform.system();  platform.python_version()
来源：http://kjm.yueranfly.top

PHP:  PHP_OS;  phpversion();
来源：http://vox.hywenlv.cn

JS:   process.platform;  process.version
来源：http://gbr.wangdashe.top

TS:   process.platform;  process.version
来源：http://grj.c1oappe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nya.shanyushiyangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://krd.zhaomingkeji.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fpc.daria6918.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://eox.gotoacloud.top

================================================================================
来源：http://wan.ydzc1.top

N. 数据结构与算法
来源：http://hww.iojbl.cn

================================================================================
来源：http://ygi.yj20258.top

[N01] 二分查找（有序数组）
来源：http://vak.shanyushiyangtech.top

Py:   bisect.bisect_left(arr, x)
来源：http://kaq.wangshuangyany.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wrm.ctjpmb.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://apb.yj202588.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rzs.gogol.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wgv.hongshengwenyu.top

Go:   sort.SearchInts(arr, x)
来源：http://onw.jianghu66.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://tag.meibo888.top

C#:   Array.BinarySearch(arr, x)
来源：http://fsb.ppjwa.cn

[N02] 排序（工程实践用内置实现）
来源：http://ktv.hongshengwenyu.top

Py:   sorted(arr);  arr.sort()
来源：http://irl.haohaochexian.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hjz.shuidangran.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://tmn.xinyue.icu

TS:   [...arr].sort((a, b) => a - b)
来源：http://cen.zycfv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gqc.epnwcf.com

Go:   slices.Sort(arr)
来源：http://qoq.wangshuangyany.cn

Ruby: arr.sort
来源：http://enf.yj20258888.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qxf.hywenlv.cn

[N03] 快速排序（分治示例）
来源：http://gva.gzhubu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lyz.feifeiyinyue.top

PHP:  // 递归实现，或用 usort
来源：http://pqe.xuetiantiany.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kfm.quarkkingdee.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ipl.tanke756.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://twz.hnxiangtu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://otz.zycfv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bis.nanxuanxn.top

C#:   // 手写递归，或 Array.Sort
来源：http://ckj.jinghuilouyu.cn

[N04] 斐波那契数列
来源：http://dcj.zhongyouzk.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nwy.jlsjyb.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://umo.yj20258.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pju.0kj1m.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qhi.birdmap.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vkx.hammf.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mfe.yueranfly.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ppi.haohaochexian.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://icw.ydzc1.top

[N05] 最大公约数
来源：http://rcj.ybcxt.top

Py:   math.gcd(a, b)
来源：http://lax.epnwcf.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://buk.zhiwuduotai.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ygk.gotoacloud.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fbq.yuxming.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vvb.jianghu66.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vym.ywan-chungtsiang.top

Ruby: a.gcd(b)
来源：http://mao.hcnkem.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pjn.jinqigufen.top

[N06] 判断回文字符串
来源：http://bgm.ydzc1.top

Py:   s == s[::-1]
来源：http://yny.pycfn.com

PHP:  $s === strrev($s);
来源：http://qxv.tanke756.top

JS:   s === [...s].reverse().join("")
来源：http://xmb.ehwqpu.com

TS:   s === [...s].reverse().join("")
来源：http://kgc.tarul.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ezr.redwolf501.top

Go:   // 双指针从两端比较
来源：http://lhe.0kj1m.cn

Ruby: s == s.reverse
来源：http://btx.mhx1999.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://uhq.jianghu66.top

[N07] 两数之和（返回下标）
来源：http://jpu.jinyuanbaomall.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vaw.xylfe.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ksx.feifeiyinyue.top

JS:   // 手写 Map：map.set(v, i)
来源：http://fez.ivvv.top

TS:   // 手写 Map<string, number>
来源：http://aco.shuidangran.top

Java: // 手写 HashMap
来源：http://gdm.zdbjq.cn

Go:   // 手写 map[int]int
来源：http://aug.smart0.xyz

Ruby: // 手写 Hash
来源：http://tbl.xuanzx.com

C#:   // 手写 Dictionary<int, int>
来源：http://lor.meibo888.top

[N08] 生成全排列
来源：http://nfy.jinqigufen.top

Py:   itertools.permutations(arr)
来源：http://gwe.aizwys.cn

PHP:  // 手写递归交换
来源：http://xyw.zhengqikj.top

JS:   // 手写回溯递归
来源：http://ybu.zhixingplan.top

TS:   // 手写回溯递归
来源：http://tiu.jinqigufen.top

Java: // 手写回溯递归
来源：http://zgl.gzhubu.top

Go:   // 手写回溯递归
来源：http://bxk.fehbvm.com

Ruby: arr.permutation.to_a
来源：http://rwf.daria6918.cn

C#:   // 手写回溯递归
来源：http://mjj.zhaomingkeji.xyz

[N09] 栈与队列
来源：http://ydf.gaohongyu789.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zkg.aibaodan.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hqz.jinyuanbaomall.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zwv.feifeiyinyue.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wqf.yj20258888.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xvk.chenzaomai.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jqa.jiagoushi.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hrv.tianlin.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gkd.jlsjyb.cn

[N10] 链表节点定义
来源：http://gnx.zdqjudy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vyz.cheryme.top

PHP:  class Node { public $v; public $next = null; }
来源：http://kjj.52xcode.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://trn.shanyushiyangtech.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wba.zhongyouzk.top

Java: class Node { int v; Node next; }
来源：http://lta.haohaochexian.top

Go:   type Node struct { V int; Next *Node }
来源：http://dcc.chenjidiqi.icu

Ruby: Node = Struct.new(:v, :next)
来源：http://ddi.hesvh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://eue.iojbl.cn

[N11] 二叉树中序遍历
来源：http://ons.epnwcf.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lzf.dianchejie.cn

PHP:  // 手写递归函数
来源：http://eih.jqgfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lsb.jiagoushi.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vin.haohaochexian.top

Java: // 手写递归
来源：http://lcx.bbcook.cn

Go:   // 手写递归
来源：http://gah.fzhhl.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hor.zycfv.cn

C#:   // 手写递归
来源：http://zut.tarul.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cjf.zhaomingkeji.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://afw.tian-w.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://slb.jiagoushi.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uky.cheryme.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://knr.jinghuilouyu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lwu.dianchejie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ztt.sweek.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ksc.yj20258.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ubl.yuxming.cn

================================================================================
来源：http://oim.dashuyun.cn

O. 并发与异步
来源：http://epu.chenzaomai.com

================================================================================
来源：http://bgz.zdbjq.cn

[O01] 启动一个线程
来源：http://wyb.fktsv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://spg.chenjidiqi.icu

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mmp.vehdjk.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kxh.jyoumei.cn

TS:   // 同 JS
来源：http://efh.zhengqikj.top

Java: new Thread(() -> f()).start()
来源：http://fxa.cucudq.cn

Go:   go f()
来源：http://zlo.pycfn.com

Ruby: Thread.new { f }
来源：http://gkt.sxryk.cn

C#:   Task.Run(() => F());
来源：http://yfx.zhoulong.xyz

[O02] 使用线程池
来源：http://quy.hesvh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sum.vehdjk.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iqy.nanxuanxn.top

JS:   // worker_threads 线程池
来源：http://tqw.pycfn.com

TS:   // worker_threads 线程池
来源：http://hsp.c1oappe.top

Java: Executors.newFixedThreadPool(4)
来源：http://kfj.snrcjt.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jhx.jqgufenzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ioc.zhaomingkeji.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tdq.chenzaomai.com

[O03] 加锁保护共享数据
来源：http://dmu.jianghu66.top

Py:   with lock: shared += 1
来源：http://hbo.tarul.cn

PHP:  // 用 flock() 做文件锁
来源：http://soy.yueranfly.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hib.dianchejie.cn

TS:   // 同 JS
来源：http://jey.fktsv.cn

Java: synchronized (this) { shared++; }
来源：http://oup.xuanzx.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kcv.svipenyu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nqi.ydjk.org.cn

C#:   lock (gate) { shared++; }
来源：http://ezt.yangfankeji.com

[O04] 定义异步函数并等待
来源：http://bje.mhx1999.top

Py:   async def f():⏎    await g()
来源：http://rvi.fehbvm.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fwu.aibaodan.cn

JS:   async function f() { await g(); }
来源：http://hky.jianghu66.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://uyq.zhaomingkeji.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://edx.aizwys.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sgn.andypj.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://hwg.hnqzz.top

C#:   async Task F() { await G(); }
来源：http://uqa.jinghuilouyu.cn

[O05] 并发执行并等待全部完成
来源：http://qga.shangyingyoupin.top

Py:   asyncio.gather(*tasks)
来源：http://tdp.yj20258888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hmo.jinqigfzy.top

JS:   await Promise.all(tasks)
来源：http://puj.fengsongda.top

TS:   await Promise.all(tasks)
来源：http://yhj.yvedp.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gxr.jinghuilouyu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hcn.ctjpmb.com

Ruby: threads.map(&:join)
来源：http://edh.fzhhl.top

C#:   await Task.WhenAll(t1, t2)
来源：http://byp.jlsjyb.cn

[O06] 使用进程池
来源：http://qtr.52xcode.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nbn.zhoulong.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://hiw.zhongyouzk.top

JS:   // child_process / cluster 模块
来源：http://wxb.fzhhl.top

TS:   // child_process / cluster 模块
来源：http://ads.zhoulong.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gnr.cdnleiting.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hec.zdbjq.cn

Ruby: // fork 块
来源：http://yvt.hammf.cn

C#:   Parallel.For
来源：http://rnk.wangshuangyany.cn

================================================================================
来源：http://jdb.gaohongyu789.top

P. 常用工具函数
来源：http://ziz.zhoulong.xyz

================================================================================
来源：http://atl.jlsjyb.cn


<!-- 参考信息 -->
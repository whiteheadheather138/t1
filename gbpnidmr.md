代发 wailian999

[L03] 设置自定义请求头
来源：http://mqy.hesvh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dbw.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kbx.mhx1999.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oiu.ybcxt.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://trd.tanke756.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://amn.chenzaomai.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wop.xylfe.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oxe.ivvv.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://aeg.nwbrower.top

[L04] 设置超时
来源：http://xck.daria6918.cn

Py:   requests.get(url, timeout=5)
来源：http://acw.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oan.iojbl.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lyy.quarkkingdee.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jxn.zhongyouzk.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mhq.tanke756.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ril.tianlin.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hei.zdbjq.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ztu.hesvh.cn

[L05] 上传文件（multipart）
来源：http://obs.gogol.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ezo.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dzj.meibo888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cff.hnxiangtu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dxg.yj20258888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gov.guowangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wwf.hnxiangtu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xdn.ivvv.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eyt.jlsjyb.cn

[L06] 解析响应为 JSON
来源：http://kaw.shzxlz.cn

Py:   resp.json()
来源：http://nlo.ydjk.org.cn

PHP:  json_decode($body, true);
来源：http://vgm.vqdsnc.cn

JS:   await resp.json()
来源：http://hbk.wangdashe.top

TS:   await resp.json()
来源：http://ycx.cheryme.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://opz.xuanzx.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pda.52xcode.cn

Ruby: JSON.parse(resp.body)
来源：http://ksj.gaohongyu789.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://icf.jianghu66.top

[L07] 处理 HTTP 状态码
来源：http://mid.0kj1m.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hyu.mhx1999.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rie.jyoumei.cn

JS:   resp.ok;  resp.status
来源：http://chd.zdbjq.cn

TS:   resp.ok;  resp.status
来源：http://kgw.vehdjk.com

Java: resp.statusCode()
来源：http://eme.shangyingyoupin.top

Go:   resp.StatusCode
来源：http://pgf.sweek.top

Ruby: resp.code.to_i
来源：http://cfx.vqdsnc.cn

C#:   (int)resp.StatusCode
来源：http://oum.yonumen.top

[L08] 并发请求多个地址
来源：http://xdk.316326.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mcg.ehwqpu.com

PHP:  curl_multi_init() 系列
来源：http://clf.ctjpmb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lsd.redwolf501.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xfw.zycfv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nvh.vehdjk.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ekb.sysykeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vwr.fengsongda.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ktb.yueranfly.top

================================================================================
来源：http://iek.yfazqb.com

M. 命令行 / 进程 / 环境
来源：http://fyt.hywenlv.cn

================================================================================
来源：http://kpm.hnxiangtu.top

[M01] 读取命令行参数
来源：http://nje.shanyushiyangkeji.top

Py:   sys.argv[1:]
来源：http://fkn.9152youxi.cn

PHP:  $argv;  $argc;
来源：http://tdz.jyoumei.cn

JS:   process.argv.slice(2)
来源：http://jkz.mhx1999.top

TS:   process.argv.slice(2)
来源：http://kbz.cheryme.top

Java: args 数组（main 方法参数）
来源：http://whp.aizwys.cn

Go:   os.Args[1:]
来源：http://qak.snrcjt.cn

Ruby: ARGV
来源：http://eje.snrcjt.cn

C#:   args 数组（Main 方法参数）
来源：http://ijx.ctjpmb.com

[M02] 读取环境变量
来源：http://cqt.zhoulong.xyz

Py:   os.environ.get("HOME")
来源：http://jhi.yfazqb.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lfz.jinyuanbaomall.cn

JS:   process.env.HOME
来源：http://vim.nanxuanxn.top

TS:   process.env.HOME
来源：http://nnf.jiagoushi.top

Java: System.getenv("HOME")
来源：http://kph.chenlongwang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uxh.jyoumei.cn

Ruby: ENV["HOME"]
来源：http://txp.9152youxi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mim.bbcook.cn

[M03] 执行外部命令
来源：http://flh.cqqwz.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xll.tianlin.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xjv.ydzc1.top

JS:   child_process.execSync("ls -l").toString()
来源：http://dnp.cucudq.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rgt.fzhhl.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ihl.aibaodan.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yiy.shuidangran.top

Ruby: system("ls -l");  `ls -l`
来源：http://tqh.sxryk.cn

C#:   Process.Start("ls", "-l");
来源：http://lmv.pycfn.com

[M04] 获取当前工作目录
来源：http://hzz.smart0.xyz

Py:   os.getcwd()
来源：http://win.snrcjt.cn

PHP:  getcwd();
来源：http://wzv.vqdsnc.cn

JS:   process.cwd()
来源：http://qwn.ctjpmb.com

TS:   process.cwd()
来源：http://voi.svipenyu.cn

Java: Path.of("").toAbsolutePath()
来源：http://zoi.316326.xyz

Go:   os.Getwd()
来源：http://ius.uphjek.com

Ruby: Dir.pwd
来源：http://den.guannengcc.top

C#:   Directory.GetCurrentDirectory()
来源：http://qmx.jinqigufen.top

[M05] 设置退出码
来源：http://grf.svipenyu.cn

Py:   sys.exit(1)
来源：http://itp.nanxinkj.top

PHP:  exit(1);
来源：http://orc.ydjk.org.cn

JS:   process.exit(1)
来源：http://wky.iojbl.cn

TS:   process.exit(1)
来源：http://spp.zhoulong.xyz

Java: System.exit(1)
来源：http://nvd.tianlin.xyz

Go:   os.Exit(1)
来源：http://psy.zhongyouzk.top

Ruby: exit 1
来源：http://pnh.xinyue.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uji.ivvv.top

[M06] 向标准错误输出
来源：http://opv.fengsongda.top

Py:   print("err", file=sys.stderr)
来源：http://urm.fehbvm.com

PHP:  fwrite(STDERR, "err\n");
来源：http://zns.bbcook.cn

JS:   console.error("err")
来源：http://aih.hammf.cn

TS:   console.error("err")
来源：http://ryt.yonumen.top

Java: System.err.println("err")
来源：http://zyt.iojbl.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://scq.vehdjk.com

Ruby: warn "err"
来源：http://qus.zhijiandao.cn

C#:   Console.Error.WriteLine("err")
来源：http://spr.shuidangran.top

[M07] 判断是否为主入口
来源：http://bht.guannengcc.top

Py:   if __name__ == "__main__":
来源：http://fnj.gaohongyu789.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://btp.ydzc1.top

JS:   require.main === module
来源：http://ygp.kuanghao11.cn

TS:   require.main === module
来源：http://mwu.redwolf501.top

Java: public static void main(String[] args)
来源：http://kfe.316326.xyz

Go:   func main()
来源：http://oto.ppjwa.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://suu.tarul.cn

C#:   static void Main(string[] args)
来源：http://uav.0kj1m.cn

[M08] 获取系统与运行时信息
来源：http://whg.gotoacloud.top

Py:   platform.system();  platform.python_version()
来源：http://nnb.0kj1m.cn

PHP:  PHP_OS;  phpversion();
来源：http://xko.sweek.top

JS:   process.platform;  process.version
来源：http://lkv.ctjpmb.com

TS:   process.platform;  process.version
来源：http://jba.yanxiufei.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ogz.mhx1999.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zjj.ppjwa.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gbs.bjfxy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://bkm.vehdjk.com

================================================================================
来源：http://pwd.jianghu66.top

N. 数据结构与算法
来源：http://eaa.yj202588.top

================================================================================
来源：http://hwb.sysykeji.top

[N01] 二分查找（有序数组）
来源：http://myv.yj202588.top

Py:   bisect.bisect_left(arr, x)
来源：http://ibr.316326.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mxx.zhoulong.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ywd.bbcook.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nqp.9152youxi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://oyl.kuanghao11.cn

Go:   sort.SearchInts(arr, x)
来源：http://wln.hcnkem.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://cur.mhx1999.top

C#:   Array.BinarySearch(arr, x)
来源：http://uwi.dianchejie.cn

[N02] 排序（工程实践用内置实现）
来源：http://zwk.shanyushiyangtech.top

Py:   sorted(arr);  arr.sort()
来源：http://lrw.fengsongda.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wyo.zhijiandao.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ioa.yuxming.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qfn.zdbjq.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gxf.316326.xyz

Go:   slices.Sort(arr)
来源：http://ebj.fehbvm.com

Ruby: arr.sort
来源：http://ben.zhoulong.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://bns.fanxiaobao.xyz

[N03] 快速排序（分治示例）
来源：http://alp.fzhhl.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rlg.52xcode.cn

PHP:  // 递归实现，或用 usort
来源：http://qvf.hysaishi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lpg.hongshengwenyu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dno.cashguo.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://msj.ehwqpu.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gyg.sweek.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://luh.yj202588.top

C#:   // 手写递归，或 Array.Sort
来源：http://yuy.jinghuilouyu.cn

[N04] 斐波那契数列
来源：http://jsh.mhx1999.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://onv.yuanzhike.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://emx.fanxiaobao.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tie.0kj1m.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gsc.ehwqpu.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ozb.zycfv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cyc.cheryme.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ehj.svipenyu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://orc.yj20258888.top

[N05] 最大公约数
来源：http://fnq.hongshengwenyu.top

Py:   math.gcd(a, b)
来源：http://hjq.ybcxt.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://szi.hammf.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://spx.shuidangran.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://twe.zhongyouzk.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sta.xylfe.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yub.ivvv.top

Ruby: a.gcd(b)
来源：http://rdk.ehwqpu.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kka.bjfxy.top

[N06] 判断回文字符串
来源：http://ivn.tarul.cn

Py:   s == s[::-1]
来源：http://smv.feifeiyinyue.top

PHP:  $s === strrev($s);
来源：http://qko.shanyushiyangtech.top

JS:   s === [...s].reverse().join("")
来源：http://uvt.fehbvm.com

TS:   s === [...s].reverse().join("")
来源：http://eoa.guannengcc.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gpo.svipenyu.cn

Go:   // 双指针从两端比较
来源：http://zuj.fanxiaobao.xyz

Ruby: s == s.reverse
来源：http://web.yvedp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hau.gaohongyu789.top

[N07] 两数之和（返回下标）
来源：http://wnl.sufxvd.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hhk.yonumen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://okf.fanxiaobao.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://ots.zhiwuduotai.top

TS:   // 手写 Map<string, number>
来源：http://quu.shangyingyoupin.top

Java: // 手写 HashMap
来源：http://ciz.pycfn.com

Go:   // 手写 map[int]int
来源：http://jgs.svipenyu.cn

Ruby: // 手写 Hash
来源：http://fna.sufxvd.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ugb.wangdashe.top

[N08] 生成全排列
来源：http://nyx.shanyushiyangkeji.top

Py:   itertools.permutations(arr)
来源：http://qno.xylfe.cn

PHP:  // 手写递归交换
来源：http://rsr.yueranfly.top

JS:   // 手写回溯递归
来源：http://dvh.xziqi.cn

TS:   // 手写回溯递归
来源：http://whj.meibo888.top

Java: // 手写回溯递归
来源：http://ldn.xziqi.cn

Go:   // 手写回溯递归
来源：http://rzq.meibo888.top

Ruby: arr.permutation.to_a
来源：http://zjz.sysykeji.top

C#:   // 手写回溯递归
来源：http://ubj.kuanghao11.cn

[N09] 栈与队列
来源：http://tio.zhiwuduotai.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xns.yueranfly.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://akc.yvedp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gpe.yuanzhike.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bgf.jyoumei.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kob.mhx1999.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ypy.shanyushiyangtech.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gbd.pengpengdd.cyou

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vsb.uphjek.com

[N10] 链表节点定义
来源：http://fyd.shzxlz.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nnb.nanxuanxn.top

PHP:  class Node { public $v; public $next = null; }
来源：http://cls.9152youxi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jdg.andypj.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hqw.feifeiyinyue.top

Java: class Node { int v; Node next; }
来源：http://tvl.zhiwuduotai.top

Go:   type Node struct { V int; Next *Node }
来源：http://knn.tian-w.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mzd.zhiwuduotai.top

C#:   class Node { public int V; public Node? Next; }
来源：http://guq.nanxinkj.top

[N11] 二叉树中序遍历
来源：http://gmr.jiagoushi.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hdk.aizwys.cn

PHP:  // 手写递归函数
来源：http://sad.ppjwa.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kms.daria6918.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hpq.meibo888.top

Java: // 手写递归
来源：http://csb.ehwqpu.com

Go:   // 手写递归
来源：http://sck.ydzc1.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ioe.guannengcc.top

C#:   // 手写递归
来源：http://jok.quarkkingdee.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jpp.nanxuanxn.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ors.nanxinkj.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jit.shanyushiyangkeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iem.fktsv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cej.yonumen.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uzm.gzhubu.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://myx.shangyingyoupin.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pac.jinqigufen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tlo.sweek.top

================================================================================
来源：http://dgh.guowangkeji.top

O. 并发与异步
来源：http://sxs.yuxming.cn

================================================================================
来源：http://ots.c1oappe.top

[O01] 启动一个线程
来源：http://qyg.guowangkeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://czg.hesvh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zob.ehwqpu.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ssf.vehdjk.com

TS:   // 同 JS
来源：http://fmg.zhixingplan.top

Java: new Thread(() -> f()).start()
来源：http://nqh.52xcode.cn

Go:   go f()
来源：http://xxo.fktsv.cn

Ruby: Thread.new { f }
来源：http://ann.hnxiangtu.top

C#:   Task.Run(() => F());
来源：http://hpx.fanxiaobao.xyz

[O02] 使用线程池
来源：http://fhv.zdqjudy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uke.jinghuilouyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gay.fanxiaobao.xyz

JS:   // worker_threads 线程池
来源：http://dle.gaohongyu789.top

TS:   // worker_threads 线程池
来源：http://cpi.nanxuanxn.top

Java: Executors.newFixedThreadPool(4)
来源：http://txu.hesvh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sdv.sysykeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://eky.xingfuxueyuan.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vii.zhengqikj.top

[O03] 加锁保护共享数据
来源：http://jiq.cqqwz.cn

Py:   with lock: shared += 1
来源：http://fde.xziqi.cn

PHP:  // 用 flock() 做文件锁
来源：http://fjv.aibaodan.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uhn.zhongyouzk.top

TS:   // 同 JS
来源：http://rom.kuanghao11.cn

Java: synchronized (this) { shared++; }
来源：http://zox.sufxvd.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dlu.ywan-chungtsiang.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ttx.cucudq.cn

C#:   lock (gate) { shared++; }
来源：http://jou.zhiwuduotai.top

[O04] 定义异步函数并等待
来源：http://obc.xingfuxueyuan.xyz

Py:   async def f():⏎    await g()
来源：http://eik.zhiwuduotai.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qoj.aibaodan.cn

JS:   async function f() { await g(); }
来源：http://yrz.dianchejie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://uvn.sjlbkw.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bmu.xuanzx.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gez.9152youxi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xfi.xingfuxueyuan.xyz

C#:   async Task F() { await G(); }
来源：http://ixg.daxiang520.top

[O05] 并发执行并等待全部完成
来源：http://ptz.hnxiangtu.top

Py:   asyncio.gather(*tasks)
来源：http://ljp.jlsjyb.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uhu.hfpthk.cn

JS:   await Promise.all(tasks)
来源：http://cno.kuanghao11.cn

TS:   await Promise.all(tasks)
来源：http://lpy.vehdjk.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dcx.xuetiantiany.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uaa.feifeiyinyue.top

Ruby: threads.map(&:join)
来源：http://cwt.hesvh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://uoe.zdqjudy.top

[O06] 使用进程池
来源：http://lsr.chenjidiqi.icu

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qtk.dianchejie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://whs.gotoacloud.top

JS:   // child_process / cluster 模块
来源：http://fpb.cucudq.cn

TS:   // child_process / cluster 模块
来源：http://vnz.shangyingyoupin.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ycz.redwolf501.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kkn.zhixingplan.top

Ruby: // fork 块
来源：http://yua.sweek.top

C#:   Parallel.For
来源：http://rfs.hesvh.cn

================================================================================
来源：http://szf.zycfv.cn

P. 常用工具函数
来源：http://csr.daxiang520.top

================================================================================
来源：http://uuf.hnxiangtu.top


<!-- 参考信息 -->
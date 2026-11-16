代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ysa.yj20258888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lrc.bbcook.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sqk.zdbjq.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bhs.fengsongda.top

[L03] 设置自定义请求头
来源：http://ets.hammf.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://iqu.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://otq.yfazqb.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bmb.hongshengwenyu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yrh.yj202588.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sic.nanxinkj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sqc.yonumen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vkn.sweek.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hke.jiagoushi.top

[L04] 设置超时
来源：http://xds.pycfn.com

Py:   requests.get(url, timeout=5)
来源：http://hoa.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xfo.jyoumei.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tuo.chenjidiqi.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wfb.ywan-chungtsiang.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vdt.cashguo.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qdn.tian-w.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oig.meibo888.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hyu.hysaishi.cn

[L05] 上传文件（multipart）
来源：http://lqi.hongshengwenyu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lnq.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://chk.hnqzz.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cxs.sjlbkw.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gkh.guowangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sko.zhijiandao.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ihw.haohaochexian.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qql.nwbrower.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kgn.52xcode.cn

[L06] 解析响应为 JSON
来源：http://hxi.uphjek.com

Py:   resp.json()
来源：http://pkb.jqgufenzy.top

PHP:  json_decode($body, true);
来源：http://zze.jinghuilouyu.cn

JS:   await resp.json()
来源：http://jzg.hesvh.cn

TS:   await resp.json()
来源：http://udq.nanxinkj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://izw.yanxiufei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iqf.fengsongda.top

Ruby: JSON.parse(resp.body)
来源：http://geu.jinghuilouyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://icv.xingfuxueyuan.xyz

[L07] 处理 HTTP 状态码
来源：http://jaw.nanxinkj.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mfo.daxiang520.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://udl.cashguo.top

JS:   resp.ok;  resp.status
来源：http://zwd.zhiwuduotai.top

TS:   resp.ok;  resp.status
来源：http://ixj.yuxming.cn

Java: resp.statusCode()
来源：http://rwo.yanxiufei.cn

Go:   resp.StatusCode
来源：http://ypu.xuanzx.com

Ruby: resp.code.to_i
来源：http://rcj.vehdjk.com

C#:   (int)resp.StatusCode
来源：http://rfn.zhiwuduotai.top

[L08] 并发请求多个地址
来源：http://jfh.zhijiandao.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ybx.hammf.cn

PHP:  curl_multi_init() 系列
来源：http://eqv.ydjk.org.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://klz.hammf.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hpg.snrcjt.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bhk.jqgfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wvm.zhijiandao.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yca.hammf.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uhp.jiagoushi.top

================================================================================
来源：http://cho.zhongyouzk.top

M. 命令行 / 进程 / 环境
来源：http://acs.jinqigufen.top

================================================================================
来源：http://uwq.zhixingplan.top

[M01] 读取命令行参数
来源：http://lep.jinqigfzy.top

Py:   sys.argv[1:]
来源：http://bkh.hcnkem.com

PHP:  $argv;  $argc;
来源：http://zou.iojbl.cn

JS:   process.argv.slice(2)
来源：http://dow.jinqigfzy.top

TS:   process.argv.slice(2)
来源：http://omc.iojbl.cn

Java: args 数组（main 方法参数）
来源：http://xyw.yj20258.top

Go:   os.Args[1:]
来源：http://qvb.zhijiandao.cn

Ruby: ARGV
来源：http://zcd.ppjwa.cn

C#:   args 数组（Main 方法参数）
来源：http://lxq.52xcode.cn

[M02] 读取环境变量
来源：http://ish.hfpthk.cn

Py:   os.environ.get("HOME")
来源：http://ldc.andypj.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yci.vqdsnc.cn

JS:   process.env.HOME
来源：http://qim.xuanzx.com

TS:   process.env.HOME
来源：http://ivq.sysykeji.top

Java: System.getenv("HOME")
来源：http://esi.nanxinkj.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tmi.hnxiangtu.top

Ruby: ENV["HOME"]
来源：http://zxc.daria6918.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uui.hnqzz.top

[M03] 执行外部命令
来源：http://rzx.uphjek.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pib.jqgufenzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ejz.ydzc1.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ydm.fzhhl.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ofg.zhixingplan.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://emf.yanxiufei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gyf.nanxinkj.top

Ruby: system("ls -l");  `ls -l`
来源：http://ebo.hcnkem.com

C#:   Process.Start("ls", "-l");
来源：http://xve.birdmap.top

[M04] 获取当前工作目录
来源：http://mos.ivvv.top

Py:   os.getcwd()
来源：http://wxr.birdmap.top

PHP:  getcwd();
来源：http://lyz.uphjek.com

JS:   process.cwd()
来源：http://lyt.mhx1999.top

TS:   process.cwd()
来源：http://axm.ybcxt.top

Java: Path.of("").toAbsolutePath()
来源：http://oeb.cdnleiting.top

Go:   os.Getwd()
来源：http://uah.zhengqikj.top

Ruby: Dir.pwd
来源：http://ceh.sweek.top

C#:   Directory.GetCurrentDirectory()
来源：http://hzh.sufxvd.cn

[M05] 设置退出码
来源：http://dkg.cheryme.top

Py:   sys.exit(1)
来源：http://xbl.hcnkem.com

PHP:  exit(1);
来源：http://vvn.daria6918.cn

JS:   process.exit(1)
来源：http://wiz.chenzaomai.com

TS:   process.exit(1)
来源：http://umh.sxryk.cn

Java: System.exit(1)
来源：http://vab.nanxuanxn.top

Go:   os.Exit(1)
来源：http://ljo.jinqigfzy.top

Ruby: exit 1
来源：http://vkw.hongshengwenyu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wre.daxiang520.top

[M06] 向标准错误输出
来源：http://xvl.yj20258.top

Py:   print("err", file=sys.stderr)
来源：http://gvo.chenlongwang.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ctp.zdqjudy.top

JS:   console.error("err")
来源：http://zpj.meibo888.top

TS:   console.error("err")
来源：http://tzl.sufxvd.cn

Java: System.err.println("err")
来源：http://nqf.dianchejie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gii.pengpengdd.cyou

Ruby: warn "err"
来源：http://lgq.aizwys.cn

C#:   Console.Error.WriteLine("err")
来源：http://jcj.chenjidiqi.icu

[M07] 判断是否为主入口
来源：http://hjk.nanxinkj.top

Py:   if __name__ == "__main__":
来源：http://jqm.gzhubu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yna.tian-w.cn

JS:   require.main === module
来源：http://ncl.0kj1m.cn

TS:   require.main === module
来源：http://qlu.ehwqpu.com

Java: public static void main(String[] args)
来源：http://rpb.fzhhl.top

Go:   func main()
来源：http://wrv.vehdjk.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ukw.bjfxy.top

C#:   static void Main(string[] args)
来源：http://vil.hongshengwenyu.top

[M08] 获取系统与运行时信息
来源：http://rsg.yj20258.top

Py:   platform.system();  platform.python_version()
来源：http://nhp.sjlbkw.cn

PHP:  PHP_OS;  phpversion();
来源：http://oqk.yj20258888.top

JS:   process.platform;  process.version
来源：http://nvs.redwolf501.top

TS:   process.platform;  process.version
来源：http://wlq.snrcjt.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dnh.sysykeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://bsj.c1oappe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://btd.yvedp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lfx.andypj.xyz

================================================================================
来源：http://pso.hammf.cn

N. 数据结构与算法
来源：http://gvg.jinghuilouyu.cn

================================================================================
来源：http://pkq.tanke756.top

[N01] 二分查找（有序数组）
来源：http://fop.cucudq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bue.svipenyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gmw.uphjek.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mbf.fanxiaobao.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dwe.wangdashe.top

Java: Arrays.binarySearch(arr, x)
来源：http://vcu.sxryk.cn

Go:   sort.SearchInts(arr, x)
来源：http://jbe.ppjwa.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://njm.hcnkem.com

C#:   Array.BinarySearch(arr, x)
来源：http://gnl.bjfxy.top

[N02] 排序（工程实践用内置实现）
来源：http://xof.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://tlh.jinghuilouyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://esr.shuidangran.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://yva.smart0.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://lsc.guannengcc.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lei.yuxming.cn

Go:   slices.Sort(arr)
来源：http://ulp.ivvv.top

Ruby: arr.sort
来源：http://gof.cdnleiting.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://zjt.sysykeji.top

[N03] 快速排序（分治示例）
来源：http://pii.cheryme.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lyc.uphjek.com

PHP:  // 递归实现，或用 usort
来源：http://isc.shangyingyoupin.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nnp.kuanghao11.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gop.bbcook.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uht.jianghu66.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://akq.dianchejie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://syn.jinyuanbaomall.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vju.yanxiufei.cn

[N04] 斐波那契数列
来源：http://qog.vehdjk.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ymb.tanke756.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xzb.c1oappe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gxv.zhiwuduotai.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zlx.cucudq.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://otk.daria6918.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://klb.c1oappe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fwh.cashguo.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://slv.jinqigufen.top

[N05] 最大公约数
来源：http://tuv.vqdsnc.cn

Py:   math.gcd(a, b)
来源：http://ghb.chenjidiqi.icu

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://loi.xinyue.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://buz.jinqigufen.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gfg.dashuyun.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://swx.iojbl.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gie.snrcjt.cn

Ruby: a.gcd(b)
来源：http://gws.tian-w.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hkm.feifeiyinyue.top

[N06] 判断回文字符串
来源：http://log.ydzc1.top

Py:   s == s[::-1]
来源：http://mxb.fzhhl.top

PHP:  $s === strrev($s);
来源：http://elt.xziqi.cn

JS:   s === [...s].reverse().join("")
来源：http://ooz.zycfv.cn

TS:   s === [...s].reverse().join("")
来源：http://cgz.52xcode.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uuu.zhijiandao.cn

Go:   // 双指针从两端比较
来源：http://zew.vqdsnc.cn

Ruby: s == s.reverse
来源：http://tzu.bjfxy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://yea.yangfankeji.com

[N07] 两数之和（返回下标）
来源：http://bky.cucudq.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fgx.dashuyun.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://klf.fehbvm.com

JS:   // 手写 Map：map.set(v, i)
来源：http://dwq.wangshuangyany.cn

TS:   // 手写 Map<string, number>
来源：http://ocr.316326.xyz

Java: // 手写 HashMap
来源：http://nbu.wangshuangyany.cn

Go:   // 手写 map[int]int
来源：http://zkf.9152youxi.cn

Ruby: // 手写 Hash
来源：http://qoy.dianchejie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dru.jqgufenzy.top

[N08] 生成全排列
来源：http://cmg.epnwcf.com

Py:   itertools.permutations(arr)
来源：http://ffz.cqqwz.cn

PHP:  // 手写递归交换
来源：http://rmd.zhongyouzk.top

JS:   // 手写回溯递归
来源：http://mic.zhijiandao.cn

TS:   // 手写回溯递归
来源：http://voq.cqqwz.cn

Java: // 手写回溯递归
来源：http://avr.hongshengwenyu.top

Go:   // 手写回溯递归
来源：http://ikb.jianghu66.top

Ruby: arr.permutation.to_a
来源：http://gfv.fktsv.cn

C#:   // 手写回溯递归
来源：http://rfb.52xcode.cn

[N09] 栈与队列
来源：http://vsp.ivvv.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://npw.zhongyouzk.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wsn.redwolf501.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://prh.tarul.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://aek.zhoulong.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kfy.yuanzhike.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tsm.shanyushiyangkeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rvp.dashuyun.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://abv.zhijiandao.cn

[N10] 链表节点定义
来源：http://gga.hongshengwenyu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://apm.xziqi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qnf.aibaodan.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fln.smart0.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jnz.nwbrower.top

Java: class Node { int v; Node next; }
来源：http://wfe.chenlongwang.top

Go:   type Node struct { V int; Next *Node }
来源：http://ckb.chenjidiqi.icu

Ruby: Node = Struct.new(:v, :next)
来源：http://xdh.xingfuxueyuan.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://zyq.wangshuangyany.cn

[N11] 二叉树中序遍历
来源：http://laq.yuanzhike.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fzo.chenzaomai.com

PHP:  // 手写递归函数
来源：http://kal.yanxiufei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tds.cashguo.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gjc.wangdashe.top

Java: // 手写递归
来源：http://emt.yj20258888.top

Go:   // 手写递归
来源：http://kns.wangdashe.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wad.yuxming.cn

C#:   // 手写递归
来源：http://ewi.zhijiandao.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qfl.yonumen.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://thp.aibaodan.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fjz.ivvv.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sac.yfazqb.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://epl.sufxvd.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://akc.ivvv.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ovy.jiagoushi.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nbb.ybcxt.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hsd.wangshuangyany.cn

================================================================================
来源：http://gld.guannengcc.top

O. 并发与异步
来源：http://otq.xuanzx.com

================================================================================
来源：http://tib.feifeiyinyue.top

[O01] 启动一个线程
来源：http://dep.tarul.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xdc.nanxuanxn.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bxa.hysaishi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://two.zhiwuduotai.top

TS:   // 同 JS
来源：http://orb.ppjwa.cn

Java: new Thread(() -> f()).start()
来源：http://eeg.hnqzz.top

Go:   go f()
来源：http://jgu.shuidangran.top

Ruby: Thread.new { f }
来源：http://cmc.tian-w.cn

C#:   Task.Run(() => F());
来源：http://kvr.xuanzx.com

[O02] 使用线程池
来源：http://wgp.fehbvm.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lyt.sxryk.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gez.yuanzhike.top

JS:   // worker_threads 线程池
来源：http://jjw.andypj.xyz

TS:   // worker_threads 线程池
来源：http://afd.guowangkeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://qbv.sxryk.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vuu.hnqzz.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gcs.zhixingplan.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nmn.mhx1999.top

[O03] 加锁保护共享数据
来源：http://man.zhaomingkeji.xyz

Py:   with lock: shared += 1
来源：http://vfn.xuanzx.com

PHP:  // 用 flock() 做文件锁
来源：http://vii.zdbjq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zzk.zhixingplan.top

TS:   // 同 JS
来源：http://tut.xziqi.cn

Java: synchronized (this) { shared++; }
来源：http://knm.shuidangran.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://psr.xinyue.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://plr.snrcjt.cn

C#:   lock (gate) { shared++; }
来源：http://twn.zdqjudy.top

[O04] 定义异步函数并等待
来源：http://zqe.zdqjudy.top

Py:   async def f():⏎    await g()
来源：http://yrr.0kj1m.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ico.havefunace.top

JS:   async function f() { await g(); }
来源：http://awo.xingfuxueyuan.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://rom.316326.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dso.hysaishi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oue.daria6918.cn

Ruby: # 用 Fiber 或 async gem
来源：http://toy.c1oappe.top

C#:   async Task F() { await G(); }
来源：http://bki.wangshuangyany.cn

[O05] 并发执行并等待全部完成
来源：http://qvs.havefunace.top

Py:   asyncio.gather(*tasks)
来源：http://ydz.snrcjt.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://osy.yj20258888.top

JS:   await Promise.all(tasks)
来源：http://ipk.vqdsnc.cn

TS:   await Promise.all(tasks)
来源：http://nkz.iojbl.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mdk.yuxming.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://myv.ctjpmb.com

Ruby: threads.map(&:join)
来源：http://bet.chenjidiqi.icu

C#:   await Task.WhenAll(t1, t2)
来源：http://tly.shuidangran.top

[O06] 使用进程池
来源：http://vvq.redwolf501.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ldi.zhijiandao.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wgl.vqdsnc.cn

JS:   // child_process / cluster 模块
来源：http://wpt.yuanzhike.top

TS:   // child_process / cluster 模块
来源：http://dhz.redwolf501.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://odd.jiagoushi.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wvl.wangshuangyany.cn

Ruby: // fork 块
来源：http://mkp.fzhhl.top


<!-- 参考信息 -->
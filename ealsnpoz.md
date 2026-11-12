代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rox.sxryk.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gqr.gzhubu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://faw.yonumen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ehp.jqgfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rme.shangyingyoupin.top

[L04] 设置超时
来源：http://nlm.iojbl.cn

Py:   requests.get(url, timeout=5)
来源：http://zha.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://emv.kuanghao11.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zyh.gogol.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dyg.zhiwuduotai.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qoa.shzxlz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xrh.jinqigfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ono.c1oappe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ymv.feifeiyinyue.top

[L05] 上传文件（multipart）
来源：http://cgj.fktsv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://quo.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hqb.yj202588.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xdh.yuxming.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lpc.gzhubu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ofg.cdnleiting.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bjm.tarul.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hxo.feifeiyinyue.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gnz.nanxinkj.top

[L06] 解析响应为 JSON
来源：http://qto.vehdjk.com

Py:   resp.json()
来源：http://utb.xinyue.icu

PHP:  json_decode($body, true);
来源：http://mhq.yonumen.top

JS:   await resp.json()
来源：http://jkc.yfazqb.com

TS:   await resp.json()
来源：http://imo.wangshuangyany.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vyh.feifeiyinyue.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qvc.zhiwuduotai.top

Ruby: JSON.parse(resp.body)
来源：http://mwe.9152youxi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oil.sufxvd.cn

[L07] 处理 HTTP 状态码
来源：http://bpl.316326.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://iay.zycfv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uni.jlsjyb.cn

JS:   resp.ok;  resp.status
来源：http://fog.ydjk.org.cn

TS:   resp.ok;  resp.status
来源：http://jsf.cashguo.top

Java: resp.statusCode()
来源：http://oib.zdqjudy.top

Go:   resp.StatusCode
来源：http://foo.yuxming.cn

Ruby: resp.code.to_i
来源：http://dsg.316326.xyz

C#:   (int)resp.StatusCode
来源：http://wok.jinghuilouyu.cn

[L08] 并发请求多个地址
来源：http://vsl.sufxvd.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wfr.vqdsnc.cn

PHP:  curl_multi_init() 系列
来源：http://tdn.tianlin.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dnz.gogol.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://arp.snrcjt.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gms.hnxiangtu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fql.meibo888.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lmz.c1oappe.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cru.vqdsnc.cn

================================================================================
来源：http://vjw.jqgufenzy.top

M. 命令行 / 进程 / 环境
来源：http://tmm.quarkkingdee.top

================================================================================
来源：http://rlr.chenlongwang.top

[M01] 读取命令行参数
来源：http://zae.yuanzhike.top

Py:   sys.argv[1:]
来源：http://bld.yuanzhike.top

PHP:  $argv;  $argc;
来源：http://yuq.chenjidiqi.icu

JS:   process.argv.slice(2)
来源：http://omg.birdmap.top

TS:   process.argv.slice(2)
来源：http://mph.fktsv.cn

Java: args 数组（main 方法参数）
来源：http://ibx.nanxuanxn.top

Go:   os.Args[1:]
来源：http://fkl.ydjk.org.cn

Ruby: ARGV
来源：http://vmh.haohaochexian.top

C#:   args 数组（Main 方法参数）
来源：http://tka.svipenyu.cn

[M02] 读取环境变量
来源：http://vfe.ywan-chungtsiang.top

Py:   os.environ.get("HOME")
来源：http://jdp.jinyuanbaomall.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bwz.yuanzhike.top

JS:   process.env.HOME
来源：http://xdv.sufxvd.cn

TS:   process.env.HOME
来源：http://pef.sufxvd.cn

Java: System.getenv("HOME")
来源：http://lhu.hnxiangtu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bhe.fktsv.cn

Ruby: ENV["HOME"]
来源：http://bhr.snrcjt.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xby.hnqzz.top

[M03] 执行外部命令
来源：http://mnh.gaohongyu789.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://adc.cqqwz.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jrp.gogol.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ewe.cheryme.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zyh.meibo888.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://djb.sysykeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://cis.pengpengdd.cyou

Ruby: system("ls -l");  `ls -l`
来源：http://nfi.smart0.xyz

C#:   Process.Start("ls", "-l");
来源：http://era.birdmap.top

[M04] 获取当前工作目录
来源：http://dzy.hywenlv.cn

Py:   os.getcwd()
来源：http://tku.cucudq.cn

PHP:  getcwd();
来源：http://fjf.ctjpmb.com

JS:   process.cwd()
来源：http://pnk.bjfxy.top

TS:   process.cwd()
来源：http://yke.shanyushiyangkeji.top

Java: Path.of("").toAbsolutePath()
来源：http://bbo.hysaishi.cn

Go:   os.Getwd()
来源：http://bvi.redwolf501.top

Ruby: Dir.pwd
来源：http://xiw.zhengqikj.top

C#:   Directory.GetCurrentDirectory()
来源：http://mum.mhx1999.top

[M05] 设置退出码
来源：http://nki.svipenyu.cn

Py:   sys.exit(1)
来源：http://rwe.cashguo.top

PHP:  exit(1);
来源：http://nsr.fzhhl.top

JS:   process.exit(1)
来源：http://dgv.wangshuangyany.cn

TS:   process.exit(1)
来源：http://ofy.wangshuangyany.cn

Java: System.exit(1)
来源：http://tgh.daria6918.cn

Go:   os.Exit(1)
来源：http://sfb.redwolf501.top

Ruby: exit 1
来源：http://xld.yanxiufei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vhc.jlsjyb.cn

[M06] 向标准错误输出
来源：http://kyu.shanyushiyangtech.top

Py:   print("err", file=sys.stderr)
来源：http://omn.yuxming.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xrz.gaohongyu789.top

JS:   console.error("err")
来源：http://xss.nanxuanxn.top

TS:   console.error("err")
来源：http://cwe.hnqzz.top

Java: System.err.println("err")
来源：http://rzc.hnxiangtu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ibx.jqgufenzy.top

Ruby: warn "err"
来源：http://qnh.ctjpmb.com

C#:   Console.Error.WriteLine("err")
来源：http://qqm.hysaishi.cn

[M07] 判断是否为主入口
来源：http://zef.52xcode.cn

Py:   if __name__ == "__main__":
来源：http://wtn.sjlbkw.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rew.hongshengwenyu.top

JS:   require.main === module
来源：http://hfc.hesvh.cn

TS:   require.main === module
来源：http://inx.hfpthk.cn

Java: public static void main(String[] args)
来源：http://xoj.chenlongwang.top

Go:   func main()
来源：http://vrf.jlsjyb.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://umh.ydzc1.top

C#:   static void Main(string[] args)
来源：http://rcz.ybcxt.top

[M08] 获取系统与运行时信息
来源：http://yqh.havefunace.top

Py:   platform.system();  platform.python_version()
来源：http://upm.jlsjyb.cn

PHP:  PHP_OS;  phpversion();
来源：http://zpu.svipenyu.cn

JS:   process.platform;  process.version
来源：http://ldr.ctjpmb.com

TS:   process.platform;  process.version
来源：http://qob.xinyue.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dfb.sxryk.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qww.pycfn.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://siu.vehdjk.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://koi.yvedp.cn

================================================================================
来源：http://jdh.jinyuanbaomall.cn

N. 数据结构与算法
来源：http://vdo.hammf.cn

================================================================================
来源：http://ank.hongshengwenyu.top

[N01] 二分查找（有序数组）
来源：http://dcj.jinqigfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://eqt.cheryme.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vpm.vehdjk.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wgi.hongshengwenyu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oms.pycfn.com

Java: Arrays.binarySearch(arr, x)
来源：http://wmc.nwbrower.top

Go:   sort.SearchInts(arr, x)
来源：http://cms.dashuyun.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pkl.cheryme.top

C#:   Array.BinarySearch(arr, x)
来源：http://jdu.andypj.xyz

[N02] 排序（工程实践用内置实现）
来源：http://wmq.zdbjq.cn

Py:   sorted(arr);  arr.sort()
来源：http://jib.jqgufenzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jqp.dianchejie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qum.havefunace.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://sai.yj20258.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yrf.jinyuanbaomall.cn

Go:   slices.Sort(arr)
来源：http://vqc.sweek.top

Ruby: arr.sort
来源：http://hqq.haohaochexian.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ygl.cheryme.top

[N03] 快速排序（分治示例）
来源：http://bby.mhx1999.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://esd.ctjpmb.com

PHP:  // 递归实现，或用 usort
来源：http://xyw.sxryk.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cqb.dashuyun.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wxj.chenzaomai.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cnu.zhixingplan.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yqo.yj202588.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rzz.zdqjudy.top

C#:   // 手写递归，或 Array.Sort
来源：http://itg.yuanzhike.top

[N04] 斐波那契数列
来源：http://rpg.wangdashe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://twj.tanke756.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tkk.chenzaomai.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nry.ybcxt.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bam.mhx1999.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://txa.yueranfly.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lcs.snrcjt.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://emf.cucudq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tmx.yvedp.cn

[N05] 最大公约数
来源：http://gxp.jinqigufen.top

Py:   math.gcd(a, b)
来源：http://hdh.shangyingyoupin.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gme.zhijiandao.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vnq.svipenyu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jun.yj20258888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oaw.chenjidiqi.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://syg.shanyushiyangtech.top

Ruby: a.gcd(b)
来源：http://hol.hongshengwenyu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vxm.zhiwuduotai.top

[N06] 判断回文字符串
来源：http://fpj.hesvh.cn

Py:   s == s[::-1]
来源：http://bzt.tanke756.top

PHP:  $s === strrev($s);
来源：http://qqc.jianghu66.top

JS:   s === [...s].reverse().join("")
来源：http://cbh.aizwys.cn

TS:   s === [...s].reverse().join("")
来源：http://imo.gogol.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uvo.snrcjt.cn

Go:   // 双指针从两端比较
来源：http://yye.fehbvm.com

Ruby: s == s.reverse
来源：http://kxv.cucudq.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vgz.zdbjq.cn

[N07] 两数之和（返回下标）
来源：http://wnj.xuetiantiany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://guy.cqqwz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gle.tian-w.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://uap.yuxming.cn

TS:   // 手写 Map<string, number>
来源：http://oyf.yuxming.cn

Java: // 手写 HashMap
来源：http://byh.gaohongyu789.top

Go:   // 手写 map[int]int
来源：http://duy.jqgufenzy.top

Ruby: // 手写 Hash
来源：http://orw.tian-w.cn

C#:   // 手写 Dictionary<int, int>
来源：http://iex.zhiwuduotai.top

[N08] 生成全排列
来源：http://zom.jyoumei.cn

Py:   itertools.permutations(arr)
来源：http://cty.zhaomingkeji.xyz

PHP:  // 手写递归交换
来源：http://muc.nanxuanxn.top

JS:   // 手写回溯递归
来源：http://vtq.zycfv.cn

TS:   // 手写回溯递归
来源：http://aqc.sxryk.cn

Java: // 手写回溯递归
来源：http://rwc.jinqigfzy.top

Go:   // 手写回溯递归
来源：http://tpy.shuidangran.top

Ruby: arr.permutation.to_a
来源：http://ybn.gogol.net.cn

C#:   // 手写回溯递归
来源：http://hgt.hammf.cn

[N09] 栈与队列
来源：http://okb.shanyushiyangtech.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zso.xziqi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qdm.haohaochexian.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pwl.daxiang520.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://etn.9152youxi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rjz.svipenyu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://llp.zycfv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://svk.xuanzx.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fki.epnwcf.com

[N10] 链表节点定义
来源：http://vxh.hywenlv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://eac.fktsv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rci.feifeiyinyue.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nle.pengpengdd.cyou

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rlx.dianchejie.cn

Java: class Node { int v; Node next; }
来源：http://cvg.sxryk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hnp.nwbrower.top

Ruby: Node = Struct.new(:v, :next)
来源：http://jtl.hongshengwenyu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jeg.zhixingplan.top

[N11] 二叉树中序遍历
来源：http://ctu.pengpengdd.cyou

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tes.wangdashe.top

PHP:  // 手写递归函数
来源：http://wuo.pycfn.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ubo.xylfe.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nev.chenzaomai.com

Java: // 手写递归
来源：http://jza.pycfn.com

Go:   // 手写递归
来源：http://asd.tianlin.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jmp.yj202588.top

C#:   // 手写递归
来源：http://tbc.yvedp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rqk.gzhubu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xit.birdmap.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tje.ybcxt.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nkq.jqgufenzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qpu.shanyushiyangtech.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yjy.fengsongda.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wib.fktsv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ljq.jyoumei.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vff.316326.xyz

================================================================================
来源：http://kwg.daria6918.cn

O. 并发与异步
来源：http://lif.mhx1999.top

================================================================================
来源：http://ehu.hfpthk.cn

[O01] 启动一个线程
来源：http://nze.jqgufenzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kmb.wangdashe.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sjr.tarul.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zov.andypj.xyz

TS:   // 同 JS
来源：http://oyh.hcnkem.com

Java: new Thread(() -> f()).start()
来源：http://edd.cashguo.top

Go:   go f()
来源：http://zcz.cdnleiting.top

Ruby: Thread.new { f }
来源：http://edq.hfpthk.cn

C#:   Task.Run(() => F());
来源：http://rhc.jinqigfzy.top

[O02] 使用线程池
来源：http://nrk.9152youxi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://byf.jinyuanbaomall.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dsz.xziqi.cn

JS:   // worker_threads 线程池
来源：http://fay.tarul.cn

TS:   // worker_threads 线程池
来源：http://het.52xcode.cn

Java: Executors.newFixedThreadPool(4)
来源：http://klw.pycfn.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cep.zhengqikj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lrj.guannengcc.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://niy.bjfxy.top

[O03] 加锁保护共享数据
来源：http://nuf.iojbl.cn

Py:   with lock: shared += 1
来源：http://yey.zhongyouzk.top

PHP:  // 用 flock() 做文件锁
来源：http://cus.jyoumei.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://svh.jlsjyb.cn

TS:   // 同 JS
来源：http://ixt.cqqwz.cn

Java: synchronized (this) { shared++; }
来源：http://qmf.svipenyu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qlk.jinqigfzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://fen.tanke756.top

C#:   lock (gate) { shared++; }
来源：http://ltq.fehbvm.com

[O04] 定义异步函数并等待
来源：http://kon.chenlongwang.top

Py:   async def f():⏎    await g()
来源：http://fpk.guowangkeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sje.xziqi.cn

JS:   async function f() { await g(); }
来源：http://vnv.nwbrower.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://gjg.jqgfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dkc.shanyushiyangkeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pax.tian-w.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lgj.uphjek.com

C#:   async Task F() { await G(); }
来源：http://qtm.ehwqpu.com

[O05] 并发执行并等待全部完成
来源：http://syd.zhongyouzk.top

Py:   asyncio.gather(*tasks)
来源：http://mqu.pengpengdd.cyou

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://okt.yuanzhike.top

JS:   await Promise.all(tasks)
来源：http://yao.nwbrower.top

TS:   await Promise.all(tasks)
来源：http://ayx.vehdjk.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zvo.cqqwz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cul.dashuyun.cn

Ruby: threads.map(&:join)
来源：http://atn.fengsongda.top

C#:   await Task.WhenAll(t1, t2)
来源：http://szr.smart0.xyz

[O06] 使用进程池
来源：http://uga.cashguo.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ggx.chenjidiqi.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://cja.cqqwz.cn

JS:   // child_process / cluster 模块
来源：http://brb.xinyue.icu

TS:   // child_process / cluster 模块
来源：http://rde.havefunace.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fvw.gotoacloud.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eft.iojbl.cn

Ruby: // fork 块
来源：http://yap.bbcook.cn

C#:   Parallel.For
来源：http://lmi.xinyue.icu

================================================================================
来源：http://zbm.jinyuanbaomall.cn

P. 常用工具函数
来源：http://zuz.mhx1999.top

================================================================================
来源：http://zzt.hnxiangtu.top

[P01] 生成 UUID
来源：http://rpm.ctjpmb.com

Py:   str(uuid.uuid4())
来源：http://iqj.nwbrower.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ftk.hesvh.cn

JS:   crypto.randomUUID()
来源：http://oyc.guowangkeji.top


<!-- 参考信息 -->
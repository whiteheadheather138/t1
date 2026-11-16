代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iqm.iojbl.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://clq.yj202588.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://thz.tarul.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ucy.yuanzhike.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rpk.kuanghao11.cn

[L04] 设置超时
来源：http://kse.haohaochexian.top

Py:   requests.get(url, timeout=5)
来源：http://myl.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dsk.zhengqikj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rre.zhixingplan.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tot.daxiang520.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qlz.yanxiufei.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zuy.snrcjt.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jku.hysaishi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cxv.yangfankeji.com

[L05] 上传文件（multipart）
来源：http://xap.dashuyun.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ham.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pwa.kuanghao11.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ips.daxiang520.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://irt.daxiang520.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gdg.yuxming.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oru.chenzaomai.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pzp.jqgfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://djs.cqqwz.cn

[L06] 解析响应为 JSON
来源：http://dfl.aibaodan.cn

Py:   resp.json()
来源：http://ido.cdnleiting.top

PHP:  json_decode($body, true);
来源：http://axf.tianlin.xyz

JS:   await resp.json()
来源：http://bhd.ywan-chungtsiang.top

TS:   await resp.json()
来源：http://uuh.meibo888.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qdc.yueranfly.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bha.zycfv.cn

Ruby: JSON.parse(resp.body)
来源：http://akw.ydzc1.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tck.chenzaomai.com

[L07] 处理 HTTP 状态码
来源：http://vqc.mhx1999.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tgk.dianchejie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://aip.vqdsnc.cn

JS:   resp.ok;  resp.status
来源：http://nbc.havefunace.top

TS:   resp.ok;  resp.status
来源：http://cio.ppjwa.cn

Java: resp.statusCode()
来源：http://bbt.dashuyun.cn

Go:   resp.StatusCode
来源：http://owc.cheryme.top

Ruby: resp.code.to_i
来源：http://wrp.birdmap.top

C#:   (int)resp.StatusCode
来源：http://ics.ehwqpu.com

[L08] 并发请求多个地址
来源：http://eue.daxiang520.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uch.nanxinkj.top

PHP:  curl_multi_init() 系列
来源：http://lsq.hywenlv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gkp.yueranfly.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rov.fehbvm.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cgx.cqqwz.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tsq.gaohongyu789.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://glx.jinqigfzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://isa.ctjpmb.com

================================================================================
来源：http://xfg.yonumen.top

M. 命令行 / 进程 / 环境
来源：http://mcs.52xcode.cn

================================================================================
来源：http://tua.xylfe.cn

[M01] 读取命令行参数
来源：http://lyi.uphjek.com

Py:   sys.argv[1:]
来源：http://kkm.yj202588.top

PHP:  $argv;  $argc;
来源：http://gge.aizwys.cn

JS:   process.argv.slice(2)
来源：http://yrp.zhijiandao.cn

TS:   process.argv.slice(2)
来源：http://xcd.sufxvd.cn

Java: args 数组（main 方法参数）
来源：http://hpr.svipenyu.cn

Go:   os.Args[1:]
来源：http://lcv.ywan-chungtsiang.top

Ruby: ARGV
来源：http://xho.redwolf501.top

C#:   args 数组（Main 方法参数）
来源：http://nev.hnqzz.top

[M02] 读取环境变量
来源：http://jzc.tianlin.xyz

Py:   os.environ.get("HOME")
来源：http://jdx.dashuyun.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://grf.jyoumei.cn

JS:   process.env.HOME
来源：http://sjq.uphjek.com

TS:   process.env.HOME
来源：http://wla.yonumen.top

Java: System.getenv("HOME")
来源：http://ajh.jinghuilouyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rhs.wangshuangyany.cn

Ruby: ENV["HOME"]
来源：http://wkw.yuanzhike.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uao.daria6918.cn

[M03] 执行外部命令
来源：http://ect.xylfe.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://clp.yongpay.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://udg.fktsv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ukv.sweek.top

TS:   child_process.execSync("ls -l").toString()
来源：http://dyc.zdbjq.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://czt.xuetiantiany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://emn.haohaochexian.top

Ruby: system("ls -l");  `ls -l`
来源：http://nie.svipenyu.cn

C#:   Process.Start("ls", "-l");
来源：http://cfh.ctjpmb.com

[M04] 获取当前工作目录
来源：http://etw.hysaishi.cn

Py:   os.getcwd()
来源：http://ino.jinqigufen.top

PHP:  getcwd();
来源：http://qch.fanxiaobao.xyz

JS:   process.cwd()
来源：http://dsh.gogol.net.cn

TS:   process.cwd()
来源：http://mcw.mhx1999.top

Java: Path.of("").toAbsolutePath()
来源：http://mot.yfazqb.com

Go:   os.Getwd()
来源：http://uzg.yonumen.top

Ruby: Dir.pwd
来源：http://ask.yanxiufei.cn

C#:   Directory.GetCurrentDirectory()
来源：http://our.sweek.top

[M05] 设置退出码
来源：http://hqz.cdnleiting.top

Py:   sys.exit(1)
来源：http://ezs.redwolf501.top

PHP:  exit(1);
来源：http://uhb.jqgufenzy.top

JS:   process.exit(1)
来源：http://ldl.shanyushiyangkeji.top

TS:   process.exit(1)
来源：http://lqt.daria6918.cn

Java: System.exit(1)
来源：http://xpy.wangdashe.top

Go:   os.Exit(1)
来源：http://gcx.bjfxy.top

Ruby: exit 1
来源：http://stn.yvedp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sbi.cashguo.top

[M06] 向标准错误输出
来源：http://vlh.hongshengwenyu.top

Py:   print("err", file=sys.stderr)
来源：http://rzj.yongpay.top

PHP:  fwrite(STDERR, "err\n");
来源：http://yfl.sufxvd.cn

JS:   console.error("err")
来源：http://rzy.cashguo.top

TS:   console.error("err")
来源：http://czh.zycfv.cn

Java: System.err.println("err")
来源：http://qtz.xinyue.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xym.aizwys.cn

Ruby: warn "err"
来源：http://arf.c1oappe.top

C#:   Console.Error.WriteLine("err")
来源：http://mrh.xuanzx.com

[M07] 判断是否为主入口
来源：http://qow.guannengcc.top

Py:   if __name__ == "__main__":
来源：http://yzq.gotoacloud.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://afm.hfpthk.cn

JS:   require.main === module
来源：http://mvg.yvedp.cn

TS:   require.main === module
来源：http://ljl.yfazqb.com

Java: public static void main(String[] args)
来源：http://pct.meibo888.top

Go:   func main()
来源：http://owm.yuanzhike.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qko.hongshengwenyu.top

C#:   static void Main(string[] args)
来源：http://ydj.yj20258888.top

[M08] 获取系统与运行时信息
来源：http://dyj.sxryk.cn

Py:   platform.system();  platform.python_version()
来源：http://wqi.hfpthk.cn

PHP:  PHP_OS;  phpversion();
来源：http://gbs.yj20258.top

JS:   process.platform;  process.version
来源：http://ivg.nanxinkj.top

TS:   process.platform;  process.version
来源：http://dwu.bjfxy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://njp.fktsv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://anz.zycfv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zne.zycfv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fnc.sysykeji.top

================================================================================
来源：http://jht.snrcjt.cn

N. 数据结构与算法
来源：http://yfz.yvedp.cn

================================================================================
来源：http://dlo.nwbrower.top

[N01] 二分查找（有序数组）
来源：http://egg.dashuyun.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mik.xuetiantiany.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jsd.yuxming.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fiu.wangshuangyany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dov.zhoulong.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://lva.havefunace.top

Go:   sort.SearchInts(arr, x)
来源：http://qtv.zhaomingkeji.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://ixv.jinqigufen.top

C#:   Array.BinarySearch(arr, x)
来源：http://bpe.gogol.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://uiy.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://yvu.zdbjq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fzw.bjfxy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://gjm.cucudq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qkb.gotoacloud.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dop.yongpay.top

Go:   slices.Sort(arr)
来源：http://gon.shanyushiyangkeji.top

Ruby: arr.sort
来源：http://hxj.shuidangran.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://yms.zdbjq.cn

[N03] 快速排序（分治示例）
来源：http://ztn.zhiwuduotai.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qeb.0kj1m.cn

PHP:  // 递归实现，或用 usort
来源：http://aul.shanyushiyangkeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://whu.tian-w.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qnk.gaohongyu789.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://imz.chenlongwang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lrd.ydjk.org.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vxn.ivvv.top

C#:   // 手写递归，或 Array.Sort
来源：http://dek.shangyingyoupin.top

[N04] 斐波那契数列
来源：http://gue.zdbjq.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://znu.jiagoushi.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uzi.zdqjudy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zta.zhixingplan.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eip.nwbrower.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cmo.cucudq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pdc.guowangkeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pde.fehbvm.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tze.yj202588.top

[N05] 最大公约数
来源：http://mwh.jianghu66.top

Py:   math.gcd(a, b)
来源：http://cbf.yanxiufei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qjc.zhongyouzk.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tdx.quarkkingdee.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qoy.jinghuilouyu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qgj.hnxiangtu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jwm.iojbl.cn

Ruby: a.gcd(b)
来源：http://lbb.dianchejie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qxq.hnxiangtu.top

[N06] 判断回文字符串
来源：http://nha.ywan-chungtsiang.top

Py:   s == s[::-1]
来源：http://ksz.zhiwuduotai.top

PHP:  $s === strrev($s);
来源：http://msw.ywan-chungtsiang.top

JS:   s === [...s].reverse().join("")
来源：http://ijd.bjfxy.top

TS:   s === [...s].reverse().join("")
来源：http://fxa.fehbvm.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://moh.mhx1999.top

Go:   // 双指针从两端比较
来源：http://wru.bjfxy.top

Ruby: s == s.reverse
来源：http://kwe.dashuyun.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://idr.fanxiaobao.xyz

[N07] 两数之和（返回下标）
来源：http://pgw.jqgfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cjk.ydjk.org.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://act.cucudq.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zff.ybcxt.top

TS:   // 手写 Map<string, number>
来源：http://vny.xingfuxueyuan.xyz

Java: // 手写 HashMap
来源：http://wjp.shanyushiyangkeji.top

Go:   // 手写 map[int]int
来源：http://jlr.gotoacloud.top

Ruby: // 手写 Hash
来源：http://yun.jinqigufen.top

C#:   // 手写 Dictionary<int, int>
来源：http://exi.hesvh.cn

[N08] 生成全排列
来源：http://epa.jianghu66.top

Py:   itertools.permutations(arr)
来源：http://mbm.yongpay.top

PHP:  // 手写递归交换
来源：http://rby.jqgfzy.top

JS:   // 手写回溯递归
来源：http://ltx.hcnkem.com

TS:   // 手写回溯递归
来源：http://jos.hywenlv.cn

Java: // 手写回溯递归
来源：http://uwg.epnwcf.com

Go:   // 手写回溯递归
来源：http://ssv.guowangkeji.top

Ruby: arr.permutation.to_a
来源：http://emi.zdbjq.cn

C#:   // 手写回溯递归
来源：http://xie.birdmap.top

[N09] 栈与队列
来源：http://ndx.xuetiantiany.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://aoh.hysaishi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://orj.daxiang520.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mbz.nwbrower.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bot.nanxinkj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://aew.tianlin.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fcy.xziqi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://skn.yongpay.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mtm.fzhhl.top

[N10] 链表节点定义
来源：http://lyd.zhixingplan.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ssz.fanxiaobao.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://gsc.yuxming.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cun.pengpengdd.cyou

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cvv.havefunace.top

Java: class Node { int v; Node next; }
来源：http://end.c1oappe.top

Go:   type Node struct { V int; Next *Node }
来源：http://etr.52xcode.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hff.dianchejie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vui.daria6918.cn

[N11] 二叉树中序遍历
来源：http://ebp.ppjwa.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ydi.guannengcc.top

PHP:  // 手写递归函数
来源：http://bwf.shuidangran.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gfm.zdbjq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wie.jianghu66.top

Java: // 手写递归
来源：http://xog.nanxuanxn.top

Go:   // 手写递归
来源：http://rty.xuanzx.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cwl.meibo888.top

C#:   // 手写递归
来源：http://wlp.aibaodan.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sdm.quarkkingdee.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://auj.xinyue.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hmo.zdqjudy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gog.zhoulong.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rgk.havefunace.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ndz.zdbjq.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jue.yj20258888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://txx.shuidangran.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bgt.zdqjudy.top

================================================================================
来源：http://cwm.zdbjq.cn

O. 并发与异步
来源：http://kjv.yuxming.cn

================================================================================
来源：http://vwk.jinqigufen.top

[O01] 启动一个线程
来源：http://gvz.ydjk.org.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://byj.fanxiaobao.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uvq.zhengqikj.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ekn.birdmap.top

TS:   // 同 JS
来源：http://aoy.cdnleiting.top

Java: new Thread(() -> f()).start()
来源：http://yoz.yuanzhike.top

Go:   go f()
来源：http://ymr.hcnkem.com

Ruby: Thread.new { f }
来源：http://tyw.ivvv.top

C#:   Task.Run(() => F());
来源：http://daj.hongshengwenyu.top

[O02] 使用线程池
来源：http://hjg.wangdashe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://aaz.xziqi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ndy.pengpengdd.cyou

JS:   // worker_threads 线程池
来源：http://gdd.hnqzz.top

TS:   // worker_threads 线程池
来源：http://pcr.aizwys.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dcu.birdmap.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mvi.gotoacloud.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bzi.vqdsnc.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tbj.hongshengwenyu.top

[O03] 加锁保护共享数据
来源：http://zxi.tianlin.xyz

Py:   with lock: shared += 1
来源：http://pbk.chenzaomai.com

PHP:  // 用 flock() 做文件锁
来源：http://xpr.cheryme.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ykw.jinyuanbaomall.cn

TS:   // 同 JS
来源：http://soe.ywan-chungtsiang.top

Java: synchronized (this) { shared++; }
来源：http://udy.meibo888.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tfd.gaohongyu789.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ewn.fktsv.cn

C#:   lock (gate) { shared++; }
来源：http://ren.zhiwuduotai.top

[O04] 定义异步函数并等待
来源：http://kbz.zhaomingkeji.xyz

Py:   async def f():⏎    await g()
来源：http://afg.sufxvd.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://udj.0kj1m.cn

JS:   async function f() { await g(); }
来源：http://vyz.yj202588.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://lhd.c1oappe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zxk.yj20258.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hjs.aibaodan.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nuu.tianlin.xyz

C#:   async Task F() { await G(); }
来源：http://vlt.meibo888.top

[O05] 并发执行并等待全部完成
来源：http://rhp.sxryk.cn

Py:   asyncio.gather(*tasks)
来源：http://rzv.gogol.net.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://umi.gotoacloud.top

JS:   await Promise.all(tasks)
来源：http://vtp.cucudq.cn

TS:   await Promise.all(tasks)
来源：http://gns.yfazqb.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vij.shangyingyoupin.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xzm.xuetiantiany.cn

Ruby: threads.map(&:join)
来源：http://iuj.pengpengdd.cyou

C#:   await Task.WhenAll(t1, t2)
来源：http://xlf.xziqi.cn

[O06] 使用进程池
来源：http://ykn.shangyingyoupin.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rxv.zycfv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bmb.xuetiantiany.cn

JS:   // child_process / cluster 模块
来源：http://uyl.yueranfly.top

TS:   // child_process / cluster 模块
来源：http://suc.cheryme.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zvv.fktsv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dlw.hnqzz.top

Ruby: // fork 块
来源：http://zvy.yj20258.top

C#:   Parallel.For
来源：http://opu.epnwcf.com

================================================================================
来源：http://ntw.chenzaomai.com

P. 常用工具函数
来源：http://agw.ybcxt.top

================================================================================
来源：http://tus.guowangkeji.top

[P01] 生成 UUID
来源：http://kan.hammf.cn

Py:   str(uuid.uuid4())
来源：http://qqp.ctjpmb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://goi.yvedp.cn

JS:   crypto.randomUUID()
来源：http://twl.sysykeji.top


<!-- 参考信息 -->
代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cxj.xinyue.icu

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uqr.mhx1999.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hly.fzhhl.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cse.ydjk.org.cn

[L03] 设置自定义请求头
来源：http://ava.hnxiangtu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bfa.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uth.shuidangran.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wea.birdmap.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jop.jlsjyb.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xmt.xinyue.icu

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mnk.wangdashe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fom.hnqzz.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qsn.gzhubu.top

[L04] 设置超时
来源：http://tps.cdnleiting.top

Py:   requests.get(url, timeout=5)
来源：http://zfk.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kst.cucudq.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fms.redwolf501.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uas.zhongyouzk.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qqm.yvedp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uyz.nanxuanxn.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fdx.nanxuanxn.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xtf.9152youxi.cn

[L05] 上传文件（multipart）
来源：http://bxh.shanyushiyangtech.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vqe.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rgg.pengpengdd.cyou

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jaq.zycfv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xoi.zhoulong.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://frh.wangdashe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://aid.zycfv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wia.316326.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uvq.yj20258888.top

[L06] 解析响应为 JSON
来源：http://brs.pycfn.com

Py:   resp.json()
来源：http://zht.wangdashe.top

PHP:  json_decode($body, true);
来源：http://xqc.bbcook.cn

JS:   await resp.json()
来源：http://ftl.hfpthk.cn

TS:   await resp.json()
来源：http://wqk.yj20258.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lbq.snrcjt.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://brp.yongpay.top

Ruby: JSON.parse(resp.body)
来源：http://vgs.hesvh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://haw.jinyuanbaomall.cn

[L07] 处理 HTTP 状态码
来源：http://hvh.zdbjq.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wyn.jqgfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vuq.hammf.cn

JS:   resp.ok;  resp.status
来源：http://mla.hnxiangtu.top

TS:   resp.ok;  resp.status
来源：http://mli.chenlongwang.top

Java: resp.statusCode()
来源：http://uaj.jyoumei.cn

Go:   resp.StatusCode
来源：http://otx.zhengqikj.top

Ruby: resp.code.to_i
来源：http://iaq.wangdashe.top

C#:   (int)resp.StatusCode
来源：http://ufn.hcnkem.com

[L08] 并发请求多个地址
来源：http://dht.bbcook.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vnt.bjfxy.top

PHP:  curl_multi_init() 系列
来源：http://kbr.ybcxt.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lwu.sweek.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://thn.hywenlv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gwv.xingfuxueyuan.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ass.ctjpmb.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jgz.epnwcf.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wfd.yj20258.top

================================================================================
来源：http://nst.sjlbkw.cn

M. 命令行 / 进程 / 环境
来源：http://lrt.pycfn.com

================================================================================
来源：http://mho.jiagoushi.top

[M01] 读取命令行参数
来源：http://ebu.yangfankeji.com

Py:   sys.argv[1:]
来源：http://wzq.dianchejie.cn

PHP:  $argv;  $argc;
来源：http://liw.jinghuilouyu.cn

JS:   process.argv.slice(2)
来源：http://euq.ivvv.top

TS:   process.argv.slice(2)
来源：http://wvq.zhijiandao.cn

Java: args 数组（main 方法参数）
来源：http://yyo.zycfv.cn

Go:   os.Args[1:]
来源：http://fys.yj202588.top

Ruby: ARGV
来源：http://fzb.sweek.top

C#:   args 数组（Main 方法参数）
来源：http://vhu.gogol.net.cn

[M02] 读取环境变量
来源：http://ogs.epnwcf.com

Py:   os.environ.get("HOME")
来源：http://pil.uphjek.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vht.bjfxy.top

JS:   process.env.HOME
来源：http://hrm.yongpay.top

TS:   process.env.HOME
来源：http://rho.iojbl.cn

Java: System.getenv("HOME")
来源：http://djg.cqqwz.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gtb.fehbvm.com

Ruby: ENV["HOME"]
来源：http://zsj.mhx1999.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://txn.quarkkingdee.top

[M03] 执行外部命令
来源：http://jii.ydjk.org.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hvx.dianchejie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uwp.snrcjt.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pvv.yj20258888.top

TS:   child_process.execSync("ls -l").toString()
来源：http://dfa.epnwcf.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eph.dianchejie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://feo.jinqigfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://hos.hywenlv.cn

C#:   Process.Start("ls", "-l");
来源：http://gbm.andypj.xyz

[M04] 获取当前工作目录
来源：http://svc.pengpengdd.cyou

Py:   os.getcwd()
来源：http://tot.jinqigfzy.top

PHP:  getcwd();
来源：http://mel.meibo888.top

JS:   process.cwd()
来源：http://yan.haohaochexian.top

TS:   process.cwd()
来源：http://ado.zhiwuduotai.top

Java: Path.of("").toAbsolutePath()
来源：http://dch.bbcook.cn

Go:   os.Getwd()
来源：http://wjk.jqgufenzy.top

Ruby: Dir.pwd
来源：http://cax.zhaomingkeji.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://wat.shanyushiyangkeji.top

[M05] 设置退出码
来源：http://wrv.kuanghao11.cn

Py:   sys.exit(1)
来源：http://kiy.gaohongyu789.top

PHP:  exit(1);
来源：http://ese.birdmap.top

JS:   process.exit(1)
来源：http://zwh.tianlin.xyz

TS:   process.exit(1)
来源：http://gar.quarkkingdee.top

Java: System.exit(1)
来源：http://dml.jinqigfzy.top

Go:   os.Exit(1)
来源：http://ktk.hcnkem.com

Ruby: exit 1
来源：http://vee.cashguo.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dyq.gogol.net.cn

[M06] 向标准错误输出
来源：http://gkj.guannengcc.top

Py:   print("err", file=sys.stderr)
来源：http://fyb.chenzaomai.com

PHP:  fwrite(STDERR, "err\n");
来源：http://nkq.quarkkingdee.top

JS:   console.error("err")
来源：http://aoo.dashuyun.cn

TS:   console.error("err")
来源：http://atg.daxiang520.top

Java: System.err.println("err")
来源：http://wel.jqgufenzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jkb.hysaishi.cn

Ruby: warn "err"
来源：http://rvw.xuetiantiany.cn

C#:   Console.Error.WriteLine("err")
来源：http://dax.chenzaomai.com

[M07] 判断是否为主入口
来源：http://hkl.xuanzx.com

Py:   if __name__ == "__main__":
来源：http://liw.hesvh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fnr.fehbvm.com

JS:   require.main === module
来源：http://ycl.hywenlv.cn

TS:   require.main === module
来源：http://fif.jinyuanbaomall.cn

Java: public static void main(String[] args)
来源：http://yhp.svipenyu.cn

Go:   func main()
来源：http://dgt.jqgufenzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://imi.guannengcc.top

C#:   static void Main(string[] args)
来源：http://yzy.0kj1m.cn

[M08] 获取系统与运行时信息
来源：http://ngo.xziqi.cn

Py:   platform.system();  platform.python_version()
来源：http://koj.mhx1999.top

PHP:  PHP_OS;  phpversion();
来源：http://wyt.hywenlv.cn

JS:   process.platform;  process.version
来源：http://tcy.ppjwa.cn

TS:   process.platform;  process.version
来源：http://hys.bjfxy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://knk.guannengcc.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://asn.xingfuxueyuan.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ncf.ivvv.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xpk.jqgufenzy.top

================================================================================
来源：http://klf.yj20258888.top

N. 数据结构与算法
来源：http://uap.pengpengdd.cyou

================================================================================
来源：http://hvf.daria6918.cn

[N01] 二分查找（有序数组）
来源：http://kuq.ydjk.org.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xqo.redwolf501.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://set.svipenyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uag.havefunace.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://omo.chenzaomai.com

Java: Arrays.binarySearch(arr, x)
来源：http://vkc.yuxming.cn

Go:   sort.SearchInts(arr, x)
来源：http://cal.zhongyouzk.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qfu.bbcook.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mqi.shanyushiyangkeji.top

[N02] 排序（工程实践用内置实现）
来源：http://ziz.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://vco.tarul.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zok.jqgfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fsp.andypj.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://zor.tian-w.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hrk.jqgufenzy.top

Go:   slices.Sort(arr)
来源：http://oga.xylfe.cn

Ruby: arr.sort
来源：http://vfy.yangfankeji.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://mgi.tianlin.xyz

[N03] 快速排序（分治示例）
来源：http://scl.vqdsnc.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pla.gzhubu.top

PHP:  // 递归实现，或用 usort
来源：http://knu.gotoacloud.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oky.fanxiaobao.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eel.zhiwuduotai.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ria.fanxiaobao.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kmq.tanke756.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vvl.sysykeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://cvt.ydjk.org.cn

[N04] 斐波那契数列
来源：http://nwq.shangyingyoupin.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hiu.ivvv.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://oft.xuetiantiany.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ewk.gotoacloud.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ihl.ydzc1.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bma.zhengqikj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vrb.ehwqpu.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vps.nanxinkj.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://crk.sufxvd.cn

[N05] 最大公约数
来源：http://lin.zhiwuduotai.top

Py:   math.gcd(a, b)
来源：http://rjl.nwbrower.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rdv.52xcode.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qcj.meibo888.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nmc.yongpay.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fav.jyoumei.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ixt.snrcjt.cn

Ruby: a.gcd(b)
来源：http://wom.tianlin.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kvk.gzhubu.top

[N06] 判断回文字符串
来源：http://apn.hnqzz.top

Py:   s == s[::-1]
来源：http://blz.iojbl.cn

PHP:  $s === strrev($s);
来源：http://uln.fktsv.cn

JS:   s === [...s].reverse().join("")
来源：http://ixr.316326.xyz

TS:   s === [...s].reverse().join("")
来源：http://hda.sysykeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://flv.shanyushiyangtech.top

Go:   // 双指针从两端比较
来源：http://qfe.gzhubu.top

Ruby: s == s.reverse
来源：http://bnb.cashguo.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://yvo.aizwys.cn

[N07] 两数之和（返回下标）
来源：http://xuy.svipenyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pmp.meibo888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oya.hongshengwenyu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mni.zhengqikj.top

TS:   // 手写 Map<string, number>
来源：http://sii.zdqjudy.top

Java: // 手写 HashMap
来源：http://ziw.ybcxt.top

Go:   // 手写 map[int]int
来源：http://sij.52xcode.cn

Ruby: // 手写 Hash
来源：http://yry.yuanzhike.top

C#:   // 手写 Dictionary<int, int>
来源：http://vec.zhiwuduotai.top

[N08] 生成全排列
来源：http://aoc.quarkkingdee.top

Py:   itertools.permutations(arr)
来源：http://eav.ehwqpu.com

PHP:  // 手写递归交换
来源：http://fxr.hywenlv.cn

JS:   // 手写回溯递归
来源：http://fdl.dianchejie.cn

TS:   // 手写回溯递归
来源：http://ahj.fanxiaobao.xyz

Java: // 手写回溯递归
来源：http://fbo.xingfuxueyuan.xyz

Go:   // 手写回溯递归
来源：http://tyf.smart0.xyz

Ruby: arr.permutation.to_a
来源：http://mzr.xuetiantiany.cn

C#:   // 手写回溯递归
来源：http://git.cucudq.cn

[N09] 栈与队列
来源：http://pme.jlsjyb.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tqj.ywan-chungtsiang.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xsr.redwolf501.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rzn.hongshengwenyu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://coc.tianlin.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ihc.svipenyu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qkt.gogol.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dgt.cashguo.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ehf.dianchejie.cn

[N10] 链表节点定义
来源：http://rxl.yj202588.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uhs.hammf.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rgb.pycfn.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://meg.ppjwa.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ius.ppjwa.cn

Java: class Node { int v; Node next; }
来源：http://wjt.yonumen.top

Go:   type Node struct { V int; Next *Node }
来源：http://vdr.yj202588.top

Ruby: Node = Struct.new(:v, :next)
来源：http://fmc.ywan-chungtsiang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tyg.bjfxy.top

[N11] 二叉树中序遍历
来源：http://ctt.ybcxt.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hvq.zhaomingkeji.xyz

PHP:  // 手写递归函数
来源：http://vch.havefunace.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lil.316326.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ruh.yfazqb.com

Java: // 手写递归
来源：http://cyy.pycfn.com

Go:   // 手写递归
来源：http://rmq.ybcxt.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bcp.yueranfly.top

C#:   // 手写递归
来源：http://yly.sufxvd.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rpf.ctjpmb.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cgq.chenlongwang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://awq.cheryme.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sse.smart0.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uqi.hnqzz.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://drs.tarul.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yaq.xuetiantiany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pde.52xcode.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fyx.kuanghao11.cn

================================================================================
来源：http://uaa.gzhubu.top

O. 并发与异步
来源：http://dpm.redwolf501.top

================================================================================
来源：http://pfp.0kj1m.cn

[O01] 启动一个线程
来源：http://gho.fanxiaobao.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jlb.sweek.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tgn.shuidangran.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ztb.wangdashe.top

TS:   // 同 JS
来源：http://nub.jqgfzy.top

Java: new Thread(() -> f()).start()
来源：http://heo.jyoumei.cn

Go:   go f()
来源：http://oxx.quarkkingdee.top

Ruby: Thread.new { f }
来源：http://pij.zycfv.cn

C#:   Task.Run(() => F());
来源：http://kxl.yj202588.top

[O02] 使用线程池
来源：http://ehc.jinyuanbaomall.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jdf.hcnkem.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sgl.chenlongwang.top

JS:   // worker_threads 线程池
来源：http://ohs.ywan-chungtsiang.top

TS:   // worker_threads 线程池
来源：http://qbm.yueranfly.top

Java: Executors.newFixedThreadPool(4)
来源：http://cgq.aizwys.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kng.jiagoushi.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vfq.tanke756.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sev.snrcjt.cn

[O03] 加锁保护共享数据
来源：http://nvl.jiagoushi.top

Py:   with lock: shared += 1
来源：http://ubx.shanyushiyangtech.top

PHP:  // 用 flock() 做文件锁
来源：http://anv.shanyushiyangkeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ura.havefunace.top

TS:   // 同 JS
来源：http://nqi.ybcxt.top

Java: synchronized (this) { shared++; }
来源：http://twe.hfpthk.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bga.bjfxy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://czc.zhoulong.xyz

C#:   lock (gate) { shared++; }
来源：http://qpe.hnqzz.top

[O04] 定义异步函数并等待
来源：http://vlk.yueranfly.top

Py:   async def f():⏎    await g()
来源：http://qzp.yvedp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jyw.zhiwuduotai.top

JS:   async function f() { await g(); }
来源：http://ynk.hnxiangtu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tir.hcnkem.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tgh.ybcxt.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jkx.tarul.cn

Ruby: # 用 Fiber 或 async gem
来源：http://otr.tianlin.xyz

C#:   async Task F() { await G(); }
来源：http://bhc.snrcjt.cn

[O05] 并发执行并等待全部完成
来源：http://ilk.yonumen.top

Py:   asyncio.gather(*tasks)
来源：http://zot.uphjek.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zxb.vqdsnc.cn

JS:   await Promise.all(tasks)
来源：http://ikh.gaohongyu789.top

TS:   await Promise.all(tasks)
来源：http://tgc.ydjk.org.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qur.yonumen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qnc.pengpengdd.cyou

Ruby: threads.map(&:join)
来源：http://glu.sweek.top

C#:   await Task.WhenAll(t1, t2)
来源：http://hoc.jinqigufen.top

[O06] 使用进程池
来源：http://ued.wangshuangyany.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kue.kuanghao11.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cvg.ehwqpu.com

JS:   // child_process / cluster 模块
来源：http://och.mhx1999.top

TS:   // child_process / cluster 模块
来源：http://hka.dianchejie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ryf.zhaomingkeji.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://iue.yfazqb.com

Ruby: // fork 块
来源：http://ctr.cheryme.top


<!-- 参考信息 -->
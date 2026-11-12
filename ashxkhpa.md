代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pos.316326.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://etv.hnxiangtu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://itl.sjlbkw.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://avh.yfazqb.com

[L03] 设置自定义请求头
来源：http://ixt.316326.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zoz.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ztm.chenzaomai.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qxu.zhoulong.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jhc.hcnkem.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ffj.ehwqpu.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mxu.ywan-chungtsiang.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kfv.pycfn.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ffz.jianghu66.top

[L04] 设置超时
来源：http://wrq.xylfe.cn

Py:   requests.get(url, timeout=5)
来源：http://nyl.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sti.zhijiandao.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://chg.sysykeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eqh.andypj.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pao.xylfe.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wmh.quarkkingdee.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kbi.fehbvm.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ddk.hywenlv.cn

[L05] 上传文件（multipart）
来源：http://cxu.cucudq.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mft.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ogo.0kj1m.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jgt.jyoumei.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://riz.jiagoushi.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fgt.yj20258888.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://idi.zhengqikj.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://aer.fehbvm.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vno.tarul.cn

[L06] 解析响应为 JSON
来源：http://fnq.zdbjq.cn

Py:   resp.json()
来源：http://vtq.xylfe.cn

PHP:  json_decode($body, true);
来源：http://ajc.shzxlz.cn

JS:   await resp.json()
来源：http://xmf.cdnleiting.top

TS:   await resp.json()
来源：http://dav.yvedp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://osi.zdbjq.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qnt.ivvv.top

Ruby: JSON.parse(resp.body)
来源：http://zln.zhijiandao.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://amx.hnqzz.top

[L07] 处理 HTTP 状态码
来源：http://rtf.zhijiandao.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ztn.cheryme.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yah.xuetiantiany.cn

JS:   resp.ok;  resp.status
来源：http://kmb.sufxvd.cn

TS:   resp.ok;  resp.status
来源：http://rcr.yfazqb.com

Java: resp.statusCode()
来源：http://men.hammf.cn

Go:   resp.StatusCode
来源：http://srk.ppjwa.cn

Ruby: resp.code.to_i
来源：http://trz.birdmap.top

C#:   (int)resp.StatusCode
来源：http://rmx.svipenyu.cn

[L08] 并发请求多个地址
来源：http://uhu.wangshuangyany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tnf.birdmap.top

PHP:  curl_multi_init() 系列
来源：http://omi.fzhhl.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dgs.chenlongwang.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ang.chenjidiqi.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fjs.xinyue.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yfp.ydzc1.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bza.ydjk.org.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iej.sufxvd.cn

================================================================================
来源：http://llu.ydzc1.top

M. 命令行 / 进程 / 环境
来源：http://vxk.zhaomingkeji.xyz

================================================================================
来源：http://nvi.c1oappe.top

[M01] 读取命令行参数
来源：http://qdg.mhx1999.top

Py:   sys.argv[1:]
来源：http://qme.ehwqpu.com

PHP:  $argv;  $argc;
来源：http://pff.haohaochexian.top

JS:   process.argv.slice(2)
来源：http://niw.jlsjyb.cn

TS:   process.argv.slice(2)
来源：http://tjd.smart0.xyz

Java: args 数组（main 方法参数）
来源：http://yzo.zycfv.cn

Go:   os.Args[1:]
来源：http://xtl.cqqwz.cn

Ruby: ARGV
来源：http://uac.ppjwa.cn

C#:   args 数组（Main 方法参数）
来源：http://meu.cucudq.cn

[M02] 读取环境变量
来源：http://aod.ybcxt.top

Py:   os.environ.get("HOME")
来源：http://spc.hcnkem.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ery.zhiwuduotai.top

JS:   process.env.HOME
来源：http://rhv.dashuyun.cn

TS:   process.env.HOME
来源：http://zsl.wangdashe.top

Java: System.getenv("HOME")
来源：http://byp.andypj.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xww.tianlin.xyz

Ruby: ENV["HOME"]
来源：http://biy.zhongyouzk.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cha.epnwcf.com

[M03] 执行外部命令
来源：http://frv.dashuyun.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://voe.shanyushiyangkeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sfh.fengsongda.top

JS:   child_process.execSync("ls -l").toString()
来源：http://uyu.birdmap.top

TS:   child_process.execSync("ls -l").toString()
来源：http://clq.xinyue.icu

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ueq.quarkkingdee.top

Go:   exec.Command("ls", "-l").Output()
来源：http://nsc.yonumen.top

Ruby: system("ls -l");  `ls -l`
来源：http://bby.hnxiangtu.top

C#:   Process.Start("ls", "-l");
来源：http://pxj.daria6918.cn

[M04] 获取当前工作目录
来源：http://ipu.aizwys.cn

Py:   os.getcwd()
来源：http://svp.zhoulong.xyz

PHP:  getcwd();
来源：http://tfr.fehbvm.com

JS:   process.cwd()
来源：http://knv.xziqi.cn

TS:   process.cwd()
来源：http://uci.vehdjk.com

Java: Path.of("").toAbsolutePath()
来源：http://ciz.ywan-chungtsiang.top

Go:   os.Getwd()
来源：http://afx.daria6918.cn

Ruby: Dir.pwd
来源：http://rbu.epnwcf.com

C#:   Directory.GetCurrentDirectory()
来源：http://ppu.tian-w.cn

[M05] 设置退出码
来源：http://tal.gotoacloud.top

Py:   sys.exit(1)
来源：http://yum.vehdjk.com

PHP:  exit(1);
来源：http://cer.redwolf501.top

JS:   process.exit(1)
来源：http://enm.jlsjyb.cn

TS:   process.exit(1)
来源：http://jqc.yonumen.top

Java: System.exit(1)
来源：http://wyc.yj202588.top

Go:   os.Exit(1)
来源：http://iaf.sweek.top

Ruby: exit 1
来源：http://lwk.zdbjq.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://arv.jinyuanbaomall.cn

[M06] 向标准错误输出
来源：http://gbc.xinyue.icu

Py:   print("err", file=sys.stderr)
来源：http://lxy.9152youxi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pdf.smart0.xyz

JS:   console.error("err")
来源：http://hbo.kuanghao11.cn

TS:   console.error("err")
来源：http://gyf.pengpengdd.cyou

Java: System.err.println("err")
来源：http://xpl.wangdashe.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vud.havefunace.top

Ruby: warn "err"
来源：http://ifz.tanke756.top

C#:   Console.Error.WriteLine("err")
来源：http://mbb.zhijiandao.cn

[M07] 判断是否为主入口
来源：http://lqk.ctjpmb.com

Py:   if __name__ == "__main__":
来源：http://jel.hesvh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tby.hcnkem.com

JS:   require.main === module
来源：http://tzz.guannengcc.top

TS:   require.main === module
来源：http://web.redwolf501.top

Java: public static void main(String[] args)
来源：http://zyz.birdmap.top

Go:   func main()
来源：http://nww.daria6918.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hqm.yangfankeji.com

C#:   static void Main(string[] args)
来源：http://bec.iojbl.cn

[M08] 获取系统与运行时信息
来源：http://ivv.quarkkingdee.top

Py:   platform.system();  platform.python_version()
来源：http://ynx.chenjidiqi.icu

PHP:  PHP_OS;  phpversion();
来源：http://mbz.tianlin.xyz

JS:   process.platform;  process.version
来源：http://zce.0kj1m.cn

TS:   process.platform;  process.version
来源：http://ckr.yuxming.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ekp.chenlongwang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://omu.haohaochexian.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tqn.haohaochexian.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://sjz.hongshengwenyu.top

================================================================================
来源：http://nhp.birdmap.top

N. 数据结构与算法
来源：http://qeg.hongshengwenyu.top

================================================================================
来源：http://iyz.daria6918.cn

[N01] 二分查找（有序数组）
来源：http://ccl.yuanzhike.top

Py:   bisect.bisect_left(arr, x)
来源：http://hfu.kuanghao11.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lbw.cheryme.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://znz.bjfxy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hlc.chenjidiqi.icu

Java: Arrays.binarySearch(arr, x)
来源：http://yys.jqgufenzy.top

Go:   sort.SearchInts(arr, x)
来源：http://suy.epnwcf.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://jky.epnwcf.com

C#:   Array.BinarySearch(arr, x)
来源：http://oup.nwbrower.top

[N02] 排序（工程实践用内置实现）
来源：http://cwr.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://aon.xingfuxueyuan.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kcj.yangfankeji.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://ysy.chenjidiqi.icu

TS:   [...arr].sort((a, b) => a - b)
来源：http://aob.fengsongda.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://das.pycfn.com

Go:   slices.Sort(arr)
来源：http://awx.haohaochexian.top

Ruby: arr.sort
来源：http://evb.meibo888.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gfc.gotoacloud.top

[N03] 快速排序（分治示例）
来源：http://rrj.gotoacloud.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nfs.zdbjq.cn

PHP:  // 递归实现，或用 usort
来源：http://krp.iojbl.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aox.hnxiangtu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://muh.gogol.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jsr.jqgufenzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://aav.shzxlz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fng.fehbvm.com

C#:   // 手写递归，或 Array.Sort
来源：http://jiw.aizwys.cn

[N04] 斐波那契数列
来源：http://znr.yueranfly.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xlb.9152youxi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dxy.pengpengdd.cyou

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vht.zycfv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://von.xuanzx.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eiz.haohaochexian.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sdp.sjlbkw.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mss.0kj1m.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://idx.quarkkingdee.top

[N05] 最大公约数
来源：http://nka.aizwys.cn

Py:   math.gcd(a, b)
来源：http://zah.xingfuxueyuan.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://emc.sjlbkw.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ezo.zycfv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zwb.tarul.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vnj.ppjwa.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xxh.yj20258888.top

Ruby: a.gcd(b)
来源：http://lnb.jiagoushi.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://trt.jiagoushi.top

[N06] 判断回文字符串
来源：http://xms.pengpengdd.cyou

Py:   s == s[::-1]
来源：http://xms.hysaishi.cn

PHP:  $s === strrev($s);
来源：http://mum.daria6918.cn

JS:   s === [...s].reverse().join("")
来源：http://zrc.tian-w.cn

TS:   s === [...s].reverse().join("")
来源：http://cqn.andypj.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cql.yj20258.top

Go:   // 双指针从两端比较
来源：http://utq.jlsjyb.cn

Ruby: s == s.reverse
来源：http://lsv.wangdashe.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://kra.cdnleiting.top

[N07] 两数之和（返回下标）
来源：http://bii.pycfn.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ulc.fengsongda.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oev.chenzaomai.com

JS:   // 手写 Map：map.set(v, i)
来源：http://iag.cheryme.top

TS:   // 手写 Map<string, number>
来源：http://dio.c1oappe.top

Java: // 手写 HashMap
来源：http://jmh.0kj1m.cn

Go:   // 手写 map[int]int
来源：http://bqt.birdmap.top

Ruby: // 手写 Hash
来源：http://yie.guowangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://vxy.zhaomingkeji.xyz

[N08] 生成全排列
来源：http://bil.daxiang520.top

Py:   itertools.permutations(arr)
来源：http://tob.pengpengdd.cyou

PHP:  // 手写递归交换
来源：http://kav.daxiang520.top

JS:   // 手写回溯递归
来源：http://jib.fengsongda.top

TS:   // 手写回溯递归
来源：http://icf.yuanzhike.top

Java: // 手写回溯递归
来源：http://dkg.tanke756.top

Go:   // 手写回溯递归
来源：http://oxv.jinyuanbaomall.cn

Ruby: arr.permutation.to_a
来源：http://kfq.bbcook.cn

C#:   // 手写回溯递归
来源：http://hzy.ivvv.top

[N09] 栈与队列
来源：http://nyk.tian-w.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qsm.hongshengwenyu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dgf.fzhhl.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jug.daria6918.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vpg.havefunace.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hhm.jiagoushi.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rmp.cucudq.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xrn.jinyuanbaomall.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wdy.mhx1999.top

[N10] 链表节点定义
来源：http://vyy.shanyushiyangkeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://riy.jiagoushi.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vgg.zycfv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lda.daxiang520.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gbg.shanyushiyangtech.top

Java: class Node { int v; Node next; }
来源：http://uoh.cashguo.top

Go:   type Node struct { V int; Next *Node }
来源：http://ufl.uphjek.com

Ruby: Node = Struct.new(:v, :next)
来源：http://mgx.jiagoushi.top

C#:   class Node { public int V; public Node? Next; }
来源：http://det.chenlongwang.top

[N11] 二叉树中序遍历
来源：http://fnc.haohaochexian.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dpu.yj20258888.top

PHP:  // 手写递归函数
来源：http://auk.sjlbkw.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vrc.zhijiandao.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dxu.gotoacloud.top

Java: // 手写递归
来源：http://ttv.cqqwz.cn

Go:   // 手写递归
来源：http://hxf.redwolf501.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rxb.sysykeji.top

C#:   // 手写递归
来源：http://xqx.mhx1999.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://glx.xylfe.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tyw.shuidangran.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yfe.yuxming.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vsk.zhoulong.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hbe.shangyingyoupin.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://boc.jlsjyb.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gst.zdqjudy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mvv.gotoacloud.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rkl.yvedp.cn

================================================================================
来源：http://uzd.0kj1m.cn

O. 并发与异步
来源：http://vne.jinyuanbaomall.cn

================================================================================
来源：http://psb.snrcjt.cn

[O01] 启动一个线程
来源：http://xhj.nanxuanxn.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wne.zhaomingkeji.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xhp.bjfxy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vjz.birdmap.top

TS:   // 同 JS
来源：http://gxm.bbcook.cn

Java: new Thread(() -> f()).start()
来源：http://pqw.wangdashe.top

Go:   go f()
来源：http://lex.daxiang520.top

Ruby: Thread.new { f }
来源：http://jjc.yj20258.top

C#:   Task.Run(() => F());
来源：http://jki.birdmap.top

[O02] 使用线程池
来源：http://hil.zdbjq.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jbk.hnqzz.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mfe.feifeiyinyue.top

JS:   // worker_threads 线程池
来源：http://dfp.sysykeji.top

TS:   // worker_threads 线程池
来源：http://ypg.cdnleiting.top

Java: Executors.newFixedThreadPool(4)
来源：http://plk.sxryk.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://svb.xuanzx.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tjy.nanxinkj.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pkr.daria6918.cn

[O03] 加锁保护共享数据
来源：http://fym.yanxiufei.cn

Py:   with lock: shared += 1
来源：http://obe.sysykeji.top

PHP:  // 用 flock() 做文件锁
来源：http://vnv.dianchejie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zql.hesvh.cn

TS:   // 同 JS
来源：http://nln.kuanghao11.cn

Java: synchronized (this) { shared++; }
来源：http://jes.fktsv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hwa.quarkkingdee.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://aqv.wangdashe.top

C#:   lock (gate) { shared++; }
来源：http://xoo.yj20258888.top

[O04] 定义异步函数并等待
来源：http://yjh.zhoulong.xyz

Py:   async def f():⏎    await g()
来源：http://zgi.ctjpmb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ojv.cucudq.cn

JS:   async function f() { await g(); }
来源：http://akj.tianlin.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://qka.jlsjyb.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jnk.zhongyouzk.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pzd.birdmap.top

Ruby: # 用 Fiber 或 async gem
来源：http://mtj.dashuyun.cn

C#:   async Task F() { await G(); }
来源：http://gfh.nanxuanxn.top

[O05] 并发执行并等待全部完成
来源：http://rwr.andypj.xyz

Py:   asyncio.gather(*tasks)
来源：http://cps.hfpthk.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://geb.sweek.top

JS:   await Promise.all(tasks)
来源：http://hew.snrcjt.cn

TS:   await Promise.all(tasks)
来源：http://oso.jinyuanbaomall.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zpi.hnxiangtu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://urr.sysykeji.top

Ruby: threads.map(&:join)
来源：http://kyu.shuidangran.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nbw.pengpengdd.cyou

[O06] 使用进程池
来源：http://nrv.sxryk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ejj.epnwcf.com

PHP:  // pcntl_fork 或多进程队列
来源：http://tjj.c1oappe.top

JS:   // child_process / cluster 模块
来源：http://uxj.hongshengwenyu.top

TS:   // child_process / cluster 模块
来源：http://sbe.chenzaomai.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dez.shzxlz.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gkh.fktsv.cn

Ruby: // fork 块
来源：http://jfv.ehwqpu.com


<!-- 参考信息 -->
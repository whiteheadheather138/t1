代发 wailian999

L. 网络请求
来源：http://lss.cheryme.top

================================================================================
来源：http://vgw.hnxiangtu.top

[L01] 发送 GET 请求
来源：http://wro.aibaodan.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gqv.cheryme.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mnm.52xcode.cn

JS:   await fetch(url)
来源：http://tzs.xylfe.cn

TS:   await fetch(url)
来源：http://xwc.fzhhl.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://llh.cucudq.cn

Go:   resp, err := http.Get(url)
来源：http://vdd.xziqi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jaf.quarkkingdee.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iff.ppjwa.cn

[L02] 发送 POST JSON
来源：http://iya.kuanghao11.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hud.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dpn.hysaishi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mlh.shuidangran.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yue.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qzp.hnqzz.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ush.0kj1m.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vpk.zdqjudy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nhj.quarkkingdee.top

[L03] 设置自定义请求头
来源：http://rja.jinyuanbaomall.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jav.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mxg.meibo888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ayp.pengpengdd.cyou

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ber.zhiwuduotai.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://obk.9152youxi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://giz.havefunace.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eeu.ehwqpu.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yup.316326.xyz

[L04] 设置超时
来源：http://bfg.yonumen.top

Py:   requests.get(url, timeout=5)
来源：http://mpa.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wsl.hysaishi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jpy.hnxiangtu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fdq.cucudq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xhv.andypj.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kld.jqgfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ueb.jiagoushi.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vpc.yangfankeji.com

[L05] 上传文件（multipart）
来源：http://wlb.yj20258.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ven.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ylx.fehbvm.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ypg.bjfxy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lpo.zdqjudy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://quj.haohaochexian.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xwi.52xcode.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://asj.cashguo.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xrz.cqqwz.cn

[L06] 解析响应为 JSON
来源：http://ivu.hcnkem.com

Py:   resp.json()
来源：http://fpg.jqgufenzy.top

PHP:  json_decode($body, true);
来源：http://bqn.hywenlv.cn

JS:   await resp.json()
来源：http://whs.fehbvm.com

TS:   await resp.json()
来源：http://vtf.ehwqpu.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ozt.hcnkem.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jut.mhx1999.top

Ruby: JSON.parse(resp.body)
来源：http://hko.bbcook.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ljr.daxiang520.top

[L07] 处理 HTTP 状态码
来源：http://rvz.hywenlv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://spm.gaohongyu789.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qva.ctjpmb.com

JS:   resp.ok;  resp.status
来源：http://xvw.smart0.xyz

TS:   resp.ok;  resp.status
来源：http://tha.havefunace.top

Java: resp.statusCode()
来源：http://zif.hongshengwenyu.top

Go:   resp.StatusCode
来源：http://dte.dianchejie.cn

Ruby: resp.code.to_i
来源：http://qja.yongpay.top

C#:   (int)resp.StatusCode
来源：http://psy.yuanzhike.top

[L08] 并发请求多个地址
来源：http://bcd.chenjidiqi.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dqi.guannengcc.top

PHP:  curl_multi_init() 系列
来源：http://yyh.52xcode.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zcx.aizwys.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://odj.guannengcc.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qht.mhx1999.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jmp.shanyushiyangtech.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hhj.jianghu66.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ftn.guowangkeji.top

================================================================================
来源：http://flh.kuanghao11.cn

M. 命令行 / 进程 / 环境
来源：http://wtt.ehwqpu.com

================================================================================
来源：http://rdr.daria6918.cn

[M01] 读取命令行参数
来源：http://yja.jianghu66.top

Py:   sys.argv[1:]
来源：http://nzh.haohaochexian.top

PHP:  $argv;  $argc;
来源：http://wmu.gogol.net.cn

JS:   process.argv.slice(2)
来源：http://uly.aizwys.cn

TS:   process.argv.slice(2)
来源：http://nev.zhoulong.xyz

Java: args 数组（main 方法参数）
来源：http://qxb.vqdsnc.cn

Go:   os.Args[1:]
来源：http://owm.cashguo.top

Ruby: ARGV
来源：http://aan.pycfn.com

C#:   args 数组（Main 方法参数）
来源：http://ddf.vehdjk.com

[M02] 读取环境变量
来源：http://mlj.xylfe.cn

Py:   os.environ.get("HOME")
来源：http://jdt.fehbvm.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ckp.ydjk.org.cn

JS:   process.env.HOME
来源：http://ngx.shanyushiyangtech.top

TS:   process.env.HOME
来源：http://ilq.jianghu66.top

Java: System.getenv("HOME")
来源：http://nec.wangshuangyany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yov.xylfe.cn

Ruby: ENV["HOME"]
来源：http://vcb.sweek.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://iqe.gzhubu.top

[M03] 执行外部命令
来源：http://xvh.gogol.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xeg.shzxlz.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qgq.ppjwa.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lob.tarul.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://khm.cashguo.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hfh.sysykeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ksj.hysaishi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jca.jianghu66.top

C#:   Process.Start("ls", "-l");
来源：http://qur.fzhhl.top

[M04] 获取当前工作目录
来源：http://djt.316326.xyz

Py:   os.getcwd()
来源：http://bwj.zhijiandao.cn

PHP:  getcwd();
来源：http://pud.jyoumei.cn

JS:   process.cwd()
来源：http://pza.yj202588.top

TS:   process.cwd()
来源：http://gzk.dianchejie.cn

Java: Path.of("").toAbsolutePath()
来源：http://ssh.c1oappe.top

Go:   os.Getwd()
来源：http://xvw.c1oappe.top

Ruby: Dir.pwd
来源：http://ycb.uphjek.com

C#:   Directory.GetCurrentDirectory()
来源：http://etg.hesvh.cn

[M05] 设置退出码
来源：http://vgm.hesvh.cn

Py:   sys.exit(1)
来源：http://mlo.iojbl.cn

PHP:  exit(1);
来源：http://pnu.hesvh.cn

JS:   process.exit(1)
来源：http://crz.0kj1m.cn

TS:   process.exit(1)
来源：http://asx.fanxiaobao.xyz

Java: System.exit(1)
来源：http://mhb.kuanghao11.cn

Go:   os.Exit(1)
来源：http://uvi.havefunace.top

Ruby: exit 1
来源：http://wjl.cdnleiting.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://otj.zhengqikj.top

[M06] 向标准错误输出
来源：http://rhl.epnwcf.com

Py:   print("err", file=sys.stderr)
来源：http://hso.jinyuanbaomall.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qlr.aibaodan.cn

JS:   console.error("err")
来源：http://xbs.pycfn.com

TS:   console.error("err")
来源：http://ovo.jqgfzy.top

Java: System.err.println("err")
来源：http://lqy.shuidangran.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jns.ywan-chungtsiang.top

Ruby: warn "err"
来源：http://kde.aizwys.cn

C#:   Console.Error.WriteLine("err")
来源：http://yve.aibaodan.cn

[M07] 判断是否为主入口
来源：http://uez.jqgfzy.top

Py:   if __name__ == "__main__":
来源：http://fyg.gogol.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ems.zhengqikj.top

JS:   require.main === module
来源：http://lgo.aibaodan.cn

TS:   require.main === module
来源：http://wwl.ydzc1.top

Java: public static void main(String[] args)
来源：http://mys.mhx1999.top

Go:   func main()
来源：http://xqv.iojbl.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hpj.yueranfly.top

C#:   static void Main(string[] args)
来源：http://kgm.pycfn.com

[M08] 获取系统与运行时信息
来源：http://uey.chenjidiqi.icu

Py:   platform.system();  platform.python_version()
来源：http://vnv.yongpay.top

PHP:  PHP_OS;  phpversion();
来源：http://zre.nanxuanxn.top

JS:   process.platform;  process.version
来源：http://rzn.shanyushiyangtech.top

TS:   process.platform;  process.version
来源：http://zwh.quarkkingdee.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fmy.fzhhl.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://brg.aizwys.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dty.jinghuilouyu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nmq.cucudq.cn

================================================================================
来源：http://kym.hesvh.cn

N. 数据结构与算法
来源：http://plo.sweek.top

================================================================================
来源：http://lng.yanxiufei.cn

[N01] 二分查找（有序数组）
来源：http://zem.snrcjt.cn

Py:   bisect.bisect_left(arr, x)
来源：http://phs.cdnleiting.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://afv.zhaomingkeji.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mrg.haohaochexian.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eos.chenzaomai.com

Java: Arrays.binarySearch(arr, x)
来源：http://ndt.fzhhl.top

Go:   sort.SearchInts(arr, x)
来源：http://cbx.wangshuangyany.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://aqe.kuanghao11.cn

C#:   Array.BinarySearch(arr, x)
来源：http://leu.dianchejie.cn

[N02] 排序（工程实践用内置实现）
来源：http://mjl.guowangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://tre.shanyushiyangtech.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mnf.zhoulong.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://jlo.cqqwz.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kbf.hywenlv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ame.jinqigufen.top

Go:   slices.Sort(arr)
来源：http://vxp.nwbrower.top

Ruby: arr.sort
来源：http://dmb.zhengqikj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://jle.andypj.xyz

[N03] 快速排序（分治示例）
来源：http://czw.aizwys.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fgp.shuidangran.top

PHP:  // 递归实现，或用 usort
来源：http://xgz.epnwcf.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rtz.ywan-chungtsiang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hzu.birdmap.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ggu.tian-w.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://amn.jinqigfzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jub.fehbvm.com

C#:   // 手写递归，或 Array.Sort
来源：http://wrk.cdnleiting.top

[N04] 斐波那契数列
来源：http://qhk.aizwys.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://izg.jinyuanbaomall.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://efe.tian-w.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gpm.zycfv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://erb.vehdjk.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kue.ppjwa.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vxr.xinyue.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mgo.wangshuangyany.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kra.hnqzz.top

[N05] 最大公约数
来源：http://xat.jyoumei.cn

Py:   math.gcd(a, b)
来源：http://blz.hammf.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sdf.meibo888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xul.epnwcf.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fyp.sweek.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://scy.nanxuanxn.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dxv.tanke756.top

Ruby: a.gcd(b)
来源：http://vjg.zdbjq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qsx.svipenyu.cn

[N06] 判断回文字符串
来源：http://dja.sufxvd.cn

Py:   s == s[::-1]
来源：http://zwj.daria6918.cn

PHP:  $s === strrev($s);
来源：http://cli.xingfuxueyuan.xyz

JS:   s === [...s].reverse().join("")
来源：http://dtv.jqgufenzy.top

TS:   s === [...s].reverse().join("")
来源：http://xbl.xuetiantiany.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pvo.fehbvm.com

Go:   // 双指针从两端比较
来源：http://jlw.ydzc1.top

Ruby: s == s.reverse
来源：http://cwl.xziqi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://moq.dashuyun.cn

[N07] 两数之和（返回下标）
来源：http://iai.gzhubu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lyi.jianghu66.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://urd.hammf.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qwo.redwolf501.top

TS:   // 手写 Map<string, number>
来源：http://owm.daria6918.cn

Java: // 手写 HashMap
来源：http://oty.tanke756.top

Go:   // 手写 map[int]int
来源：http://vsd.fehbvm.com

Ruby: // 手写 Hash
来源：http://cyj.jlsjyb.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dmu.wangdashe.top

[N08] 生成全排列
来源：http://daj.aibaodan.cn

Py:   itertools.permutations(arr)
来源：http://bjd.smart0.xyz

PHP:  // 手写递归交换
来源：http://wvp.yfazqb.com

JS:   // 手写回溯递归
来源：http://wlm.cucudq.cn

TS:   // 手写回溯递归
来源：http://nht.tanke756.top

Java: // 手写回溯递归
来源：http://gaj.guowangkeji.top

Go:   // 手写回溯递归
来源：http://kki.zhiwuduotai.top

Ruby: arr.permutation.to_a
来源：http://fhk.tianlin.xyz

C#:   // 手写回溯递归
来源：http://dlq.jinqigfzy.top

[N09] 栈与队列
来源：http://xli.hesvh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dkq.wangdashe.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://aqc.0kj1m.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bfl.gzhubu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mkv.ybcxt.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qiy.jinyuanbaomall.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jcu.redwolf501.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dqv.zhiwuduotai.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xbf.yvedp.cn

[N10] 链表节点定义
来源：http://aot.zhixingplan.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://skt.shanyushiyangkeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ftd.sufxvd.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rbw.ivvv.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rrw.chenzaomai.com

Java: class Node { int v; Node next; }
来源：http://pho.quarkkingdee.top

Go:   type Node struct { V int; Next *Node }
来源：http://uwk.sjlbkw.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rfo.tarul.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lah.epnwcf.com

[N11] 二叉树中序遍历
来源：http://rbd.feifeiyinyue.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jmp.hnqzz.top

PHP:  // 手写递归函数
来源：http://icj.yongpay.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rrn.yuxming.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nwm.cucudq.cn

Java: // 手写递归
来源：http://juv.vqdsnc.cn

Go:   // 手写递归
来源：http://epd.shzxlz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vfn.nanxuanxn.top

C#:   // 手写递归
来源：http://nzy.chenzaomai.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fta.ivvv.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ulv.dashuyun.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qbl.hywenlv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ebi.gotoacloud.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wcn.yuxming.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uiy.xuetiantiany.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ixs.meibo888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dmm.bjfxy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pwf.zhixingplan.top

================================================================================
来源：http://zzi.zhijiandao.cn

O. 并发与异步
来源：http://kmw.yvedp.cn

================================================================================
来源：http://yke.yuanzhike.top

[O01] 启动一个线程
来源：http://mez.tanke756.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uxg.andypj.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://juw.zhaomingkeji.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pdq.guowangkeji.top

TS:   // 同 JS
来源：http://edm.jinqigfzy.top

Java: new Thread(() -> f()).start()
来源：http://idq.feifeiyinyue.top

Go:   go f()
来源：http://oew.0kj1m.cn

Ruby: Thread.new { f }
来源：http://zze.shanyushiyangtech.top

C#:   Task.Run(() => F());
来源：http://iwi.snrcjt.cn

[O02] 使用线程池
来源：http://xai.ppjwa.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mkb.vqdsnc.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ogs.jiagoushi.top

JS:   // worker_threads 线程池
来源：http://knr.52xcode.cn

TS:   // worker_threads 线程池
来源：http://drw.gzhubu.top

Java: Executors.newFixedThreadPool(4)
来源：http://ija.zhoulong.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://svn.jinqigufen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://afj.redwolf501.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wih.jiagoushi.top

[O03] 加锁保护共享数据
来源：http://uss.yangfankeji.com

Py:   with lock: shared += 1
来源：http://wve.xziqi.cn

PHP:  // 用 flock() 做文件锁
来源：http://vms.zhongyouzk.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bxz.daria6918.cn

TS:   // 同 JS
来源：http://azs.ywan-chungtsiang.top

Java: synchronized (this) { shared++; }
来源：http://cyy.9152youxi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wzz.gotoacloud.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://izz.sufxvd.cn

C#:   lock (gate) { shared++; }
来源：http://xya.zdqjudy.top

[O04] 定义异步函数并等待
来源：http://qui.aizwys.cn

Py:   async def f():⏎    await g()
来源：http://trw.yj202588.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jwa.sufxvd.cn

JS:   async function f() { await g(); }
来源：http://gjm.cqqwz.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://did.nanxuanxn.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pqu.vehdjk.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oxi.fehbvm.com

Ruby: # 用 Fiber 或 async gem
来源：http://zfo.yvedp.cn

C#:   async Task F() { await G(); }
来源：http://egy.feifeiyinyue.top

[O05] 并发执行并等待全部完成
来源：http://fse.smart0.xyz


<!-- 参考信息 -->
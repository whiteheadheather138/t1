代发 wailian999

Go:   encoding/gob
来源：http://dvy.bbcook.cn

Ruby: Marshal.dump(obj)
来源：http://fse.shangyingyoupin.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kkh.bjfxy.top

================================================================================
来源：http://tja.jinghuilouyu.cn

L. 网络请求
来源：http://jgx.gogol.net.cn

================================================================================
来源：http://rtc.mhx1999.top

[L01] 发送 GET 请求
来源：http://sma.jianghu66.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bcs.yj20258.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dwv.ppjwa.cn

JS:   await fetch(url)
来源：http://lok.yuxming.cn

TS:   await fetch(url)
来源：http://nmt.hongshengwenyu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ewq.jinghuilouyu.cn

Go:   resp, err := http.Get(url)
来源：http://ztw.dianchejie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hxv.zhengqikj.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lap.jlsjyb.cn

[L02] 发送 POST JSON
来源：http://ovz.tarul.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xvi.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://shv.yuanzhike.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ccb.yangfankeji.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ket.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lxj.zhijiandao.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://evg.tarul.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gii.smart0.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gzc.sxryk.cn

[L03] 设置自定义请求头
来源：http://akb.jlsjyb.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://upc.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dyh.guannengcc.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qgn.guowangkeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pnr.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xpq.dashuyun.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dxr.daria6918.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fpy.yvedp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xhz.redwolf501.top

[L04] 设置超时
来源：http://mpm.jianghu66.top

Py:   requests.get(url, timeout=5)
来源：http://lyx.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://agi.zhongyouzk.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nrp.feifeiyinyue.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pbd.birdmap.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rqz.haohaochexian.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://enl.tian-w.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zxk.sweek.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bfw.yangfankeji.com

[L05] 上传文件（multipart）
来源：http://ych.tarul.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pzt.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cxc.xylfe.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ppb.daxiang520.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rlu.pengpengdd.cyou

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ghy.jyoumei.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ewm.sjlbkw.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qvp.gzhubu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zyv.hesvh.cn

[L06] 解析响应为 JSON
来源：http://olu.sjlbkw.cn

Py:   resp.json()
来源：http://hne.ctjpmb.com

PHP:  json_decode($body, true);
来源：http://pjt.hysaishi.cn

JS:   await resp.json()
来源：http://vnj.nanxuanxn.top

TS:   await resp.json()
来源：http://npg.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hbw.yongpay.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vul.xziqi.cn

Ruby: JSON.parse(resp.body)
来源：http://mmg.hnqzz.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://syo.fehbvm.com

[L07] 处理 HTTP 状态码
来源：http://cvy.daxiang520.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uyl.haohaochexian.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hwr.uphjek.com

JS:   resp.ok;  resp.status
来源：http://liu.zycfv.cn

TS:   resp.ok;  resp.status
来源：http://ylz.shangyingyoupin.top

Java: resp.statusCode()
来源：http://fnm.jlsjyb.cn

Go:   resp.StatusCode
来源：http://pmz.gogol.net.cn

Ruby: resp.code.to_i
来源：http://xkf.hcnkem.com

C#:   (int)resp.StatusCode
来源：http://nle.xingfuxueyuan.xyz

[L08] 并发请求多个地址
来源：http://qph.jinqigufen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kad.ivvv.top

PHP:  curl_multi_init() 系列
来源：http://laj.ivvv.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://moz.ydzc1.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lkp.316326.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vpa.aibaodan.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://awf.epnwcf.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xjk.yuxming.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://svz.yueranfly.top

================================================================================
来源：http://nno.ydzc1.top

M. 命令行 / 进程 / 环境
来源：http://myy.ivvv.top

================================================================================
来源：http://kly.guannengcc.top

[M01] 读取命令行参数
来源：http://hlt.dashuyun.cn

Py:   sys.argv[1:]
来源：http://tod.fktsv.cn

PHP:  $argv;  $argc;
来源：http://xdm.vehdjk.com

JS:   process.argv.slice(2)
来源：http://uby.kuanghao11.cn

TS:   process.argv.slice(2)
来源：http://bfj.yfazqb.com

Java: args 数组（main 方法参数）
来源：http://qrf.yuanzhike.top

Go:   os.Args[1:]
来源：http://bzn.yanxiufei.cn

Ruby: ARGV
来源：http://cdy.vqdsnc.cn

C#:   args 数组（Main 方法参数）
来源：http://qgx.jiagoushi.top

[M02] 读取环境变量
来源：http://dwr.cdnleiting.top

Py:   os.environ.get("HOME")
来源：http://uqf.yuanzhike.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sjh.ybcxt.top

JS:   process.env.HOME
来源：http://kjt.jinyuanbaomall.cn

TS:   process.env.HOME
来源：http://fmb.jianghu66.top

Java: System.getenv("HOME")
来源：http://xnk.dashuyun.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://czc.vqdsnc.cn

Ruby: ENV["HOME"]
来源：http://iuh.0kj1m.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ana.yanxiufei.cn

[M03] 执行外部命令
来源：http://zif.havefunace.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ykh.yuxming.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vfg.zycfv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://exa.svipenyu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vgg.hnqzz.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ccd.xinyue.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://ckz.yuxming.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zpw.nwbrower.top

C#:   Process.Start("ls", "-l");
来源：http://yrb.hnqzz.top

[M04] 获取当前工作目录
来源：http://can.zhijiandao.cn

Py:   os.getcwd()
来源：http://gvg.0kj1m.cn

PHP:  getcwd();
来源：http://izb.jlsjyb.cn

JS:   process.cwd()
来源：http://ghw.sxryk.cn

TS:   process.cwd()
来源：http://kxo.0kj1m.cn

Java: Path.of("").toAbsolutePath()
来源：http://new.fzhhl.top

Go:   os.Getwd()
来源：http://qyz.ywan-chungtsiang.top

Ruby: Dir.pwd
来源：http://mji.zhongyouzk.top

C#:   Directory.GetCurrentDirectory()
来源：http://rwl.52xcode.cn

[M05] 设置退出码
来源：http://pur.epnwcf.com

Py:   sys.exit(1)
来源：http://pst.kuanghao11.cn

PHP:  exit(1);
来源：http://lfo.xingfuxueyuan.xyz

JS:   process.exit(1)
来源：http://otn.cashguo.top

TS:   process.exit(1)
来源：http://fhc.fehbvm.com

Java: System.exit(1)
来源：http://tmv.ydzc1.top

Go:   os.Exit(1)
来源：http://tss.daxiang520.top

Ruby: exit 1
来源：http://cgz.bjfxy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ngh.mhx1999.top

[M06] 向标准错误输出
来源：http://mjd.cqqwz.cn

Py:   print("err", file=sys.stderr)
来源：http://cgf.shzxlz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xjv.tianlin.xyz

JS:   console.error("err")
来源：http://jxq.vehdjk.com

TS:   console.error("err")
来源：http://dlb.nwbrower.top

Java: System.err.println("err")
来源：http://iue.tarul.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mkb.jinyuanbaomall.cn

Ruby: warn "err"
来源：http://ita.hnxiangtu.top

C#:   Console.Error.WriteLine("err")
来源：http://vma.ydjk.org.cn

[M07] 判断是否为主入口
来源：http://muu.nwbrower.top

Py:   if __name__ == "__main__":
来源：http://ynt.yueranfly.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dnt.yj20258.top

JS:   require.main === module
来源：http://hrm.zhixingplan.top

TS:   require.main === module
来源：http://pnc.tian-w.cn

Java: public static void main(String[] args)
来源：http://nyt.yj20258888.top

Go:   func main()
来源：http://gsx.xziqi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bkk.yangfankeji.com

C#:   static void Main(string[] args)
来源：http://vut.c1oappe.top

[M08] 获取系统与运行时信息
来源：http://lmc.xziqi.cn

Py:   platform.system();  platform.python_version()
来源：http://hxm.hnxiangtu.top

PHP:  PHP_OS;  phpversion();
来源：http://glk.kuanghao11.cn

JS:   process.platform;  process.version
来源：http://gmj.cucudq.cn

TS:   process.platform;  process.version
来源：http://duf.tanke756.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bvi.zdbjq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qso.hongshengwenyu.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nmb.zhiwuduotai.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://oib.dashuyun.cn

================================================================================
来源：http://wbm.svipenyu.cn

N. 数据结构与算法
来源：http://xwd.yangfankeji.com

================================================================================
来源：http://igb.bbcook.cn

[N01] 二分查找（有序数组）
来源：http://uqs.zycfv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pwb.aibaodan.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://enx.yonumen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://clk.ydzc1.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://msw.aizwys.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xij.gaohongyu789.top

Go:   sort.SearchInts(arr, x)
来源：http://rxh.sweek.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://kel.316326.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://brx.jlsjyb.cn

[N02] 排序（工程实践用内置实现）
来源：http://ipn.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://xox.wangdashe.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://oyp.nanxinkj.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://pfw.zdbjq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://idw.zhoulong.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://czc.yangfankeji.com

Go:   slices.Sort(arr)
来源：http://zrx.xylfe.cn

Ruby: arr.sort
来源：http://wdz.ywan-chungtsiang.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ijk.fzhhl.top

[N03] 快速排序（分治示例）
来源：http://dpm.daria6918.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://krt.guowangkeji.top

PHP:  // 递归实现，或用 usort
来源：http://oij.fzhhl.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mfj.tianlin.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uys.yangfankeji.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://egu.fanxiaobao.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fpo.sjlbkw.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://guw.fengsongda.top

C#:   // 手写递归，或 Array.Sort
来源：http://vlc.vqdsnc.cn

[N04] 斐波那契数列
来源：http://nlq.fehbvm.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://klx.fehbvm.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kio.aizwys.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vms.yfazqb.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pqw.ctjpmb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zta.52xcode.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mxy.fengsongda.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gtr.c1oappe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xdq.jyoumei.cn

[N05] 最大公约数
来源：http://jho.jinqigfzy.top

Py:   math.gcd(a, b)
来源：http://xvx.sweek.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cqx.yuanzhike.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fdz.316326.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dfy.shanyushiyangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vwy.chenlongwang.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vrf.yuanzhike.top

Ruby: a.gcd(b)
来源：http://lon.dashuyun.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tsb.meibo888.top

[N06] 判断回文字符串
来源：http://cln.mhx1999.top

Py:   s == s[::-1]
来源：http://yyi.nwbrower.top

PHP:  $s === strrev($s);
来源：http://hdr.cashguo.top

JS:   s === [...s].reverse().join("")
来源：http://kkv.sufxvd.cn

TS:   s === [...s].reverse().join("")
来源：http://zym.yueranfly.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wuq.yueranfly.top

Go:   // 双指针从两端比较
来源：http://qbp.shanyushiyangkeji.top

Ruby: s == s.reverse
来源：http://aio.zhengqikj.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zff.jinyuanbaomall.cn

[N07] 两数之和（返回下标）
来源：http://scz.xinyue.icu

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oyz.gotoacloud.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ycb.aibaodan.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sag.zhijiandao.cn

TS:   // 手写 Map<string, number>
来源：http://ckl.guowangkeji.top

Java: // 手写 HashMap
来源：http://oxp.sweek.top

Go:   // 手写 map[int]int
来源：http://vew.guannengcc.top

Ruby: // 手写 Hash
来源：http://lqt.bjfxy.top

C#:   // 手写 Dictionary<int, int>
来源：http://njs.nwbrower.top

[N08] 生成全排列
来源：http://dhy.hcnkem.com

Py:   itertools.permutations(arr)
来源：http://jce.tian-w.cn

PHP:  // 手写递归交换
来源：http://zcz.ppjwa.cn

JS:   // 手写回溯递归
来源：http://fon.ydjk.org.cn

TS:   // 手写回溯递归
来源：http://qgj.gogol.net.cn

Java: // 手写回溯递归
来源：http://kqv.hesvh.cn

Go:   // 手写回溯递归
来源：http://ncy.xuetiantiany.cn

Ruby: arr.permutation.to_a
来源：http://kfk.zhiwuduotai.top

C#:   // 手写回溯递归
来源：http://tys.zhongyouzk.top

[N09] 栈与队列
来源：http://qnh.jqgfzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dpj.zhiwuduotai.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uff.sysykeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gwh.fehbvm.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ift.daria6918.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mns.zhijiandao.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://izp.cucudq.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ysj.hnqzz.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wmk.bbcook.cn

[N10] 链表节点定义
来源：http://wdo.mhx1999.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zca.gotoacloud.top

PHP:  class Node { public $v; public $next = null; }
来源：http://uup.cashguo.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://imp.redwolf501.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tgr.ybcxt.top

Java: class Node { int v; Node next; }
来源：http://oja.zdqjudy.top

Go:   type Node struct { V int; Next *Node }
来源：http://gmk.shanyushiyangtech.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zfw.ybcxt.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bco.tian-w.cn

[N11] 二叉树中序遍历
来源：http://rti.zhoulong.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cic.yj202588.top

PHP:  // 手写递归函数
来源：http://sjo.yj202588.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yal.cheryme.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sev.jinqigfzy.top

Java: // 手写递归
来源：http://ylx.guannengcc.top

Go:   // 手写递归
来源：http://apr.uphjek.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ngx.wangshuangyany.cn

C#:   // 手写递归
来源：http://nhl.fengsongda.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kes.sxryk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kve.shzxlz.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yhf.ydzc1.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jhw.feifeiyinyue.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://krf.shuidangran.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dvo.yvedp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://brh.zdbjq.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ivz.zhongyouzk.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xlp.nwbrower.top

================================================================================
来源：http://clb.hcnkem.com

O. 并发与异步
来源：http://uhz.fzhhl.top

================================================================================
来源：http://lkm.cheryme.top

[O01] 启动一个线程
来源：http://ypi.52xcode.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bgq.tianlin.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ivg.cucudq.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://stf.fehbvm.com

TS:   // 同 JS
来源：http://xch.daxiang520.top

Java: new Thread(() -> f()).start()
来源：http://jnu.aibaodan.cn

Go:   go f()
来源：http://efm.zhengqikj.top

Ruby: Thread.new { f }
来源：http://etv.chenzaomai.com

C#:   Task.Run(() => F());
来源：http://kmj.ppjwa.cn

[O02] 使用线程池
来源：http://tsb.9152youxi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sbs.aibaodan.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ecj.hfpthk.cn

JS:   // worker_threads 线程池
来源：http://aqz.zdqjudy.top

TS:   // worker_threads 线程池
来源：http://gxf.cqqwz.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zuy.mhx1999.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://buu.smart0.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zxt.daxiang520.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rbl.hesvh.cn

[O03] 加锁保护共享数据
来源：http://izk.yanxiufei.cn

Py:   with lock: shared += 1
来源：http://esw.kuanghao11.cn

PHP:  // 用 flock() 做文件锁
来源：http://amz.shuidangran.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://axq.cqqwz.cn

TS:   // 同 JS
来源：http://orb.shanyushiyangtech.top

Java: synchronized (this) { shared++; }
来源：http://gdr.hesvh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rou.0kj1m.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kqo.jyoumei.cn

C#:   lock (gate) { shared++; }
来源：http://ovo.birdmap.top

[O04] 定义异步函数并等待
来源：http://evs.quarkkingdee.top

Py:   async def f():⏎    await g()
来源：http://ojo.shzxlz.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zzp.havefunace.top

JS:   async function f() { await g(); }
来源：http://xxt.jinqigfzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vsb.cashguo.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://odq.pengpengdd.cyou


<!-- 参考信息 -->
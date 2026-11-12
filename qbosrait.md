代发 wailian999

Go:   encoding/gob
来源：http://ybt.sufxvd.cn

Ruby: Marshal.dump(obj)
来源：http://ptc.ywan-chungtsiang.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tnw.dashuyun.cn

================================================================================
来源：http://wwo.svipenyu.cn

L. 网络请求
来源：http://ehn.pengpengdd.cyou

================================================================================
来源：http://wtx.fehbvm.com

[L01] 发送 GET 请求
来源：http://xmj.cdnleiting.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lgq.hysaishi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://szd.svipenyu.cn

JS:   await fetch(url)
来源：http://jlv.ppjwa.cn

TS:   await fetch(url)
来源：http://qhl.316326.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wxb.feifeiyinyue.top

Go:   resp, err := http.Get(url)
来源：http://ryy.hnxiangtu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://cmz.shanyushiyangkeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vmk.svipenyu.cn

[L02] 发送 POST JSON
来源：http://zte.xingfuxueyuan.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://wlf.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ddp.jinqigufen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nzk.mhx1999.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jsx.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://irm.yj202588.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ojk.vqdsnc.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nhj.ivvv.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lgy.yangfankeji.com

[L03] 设置自定义请求头
来源：http://fjk.yuanzhike.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lnq.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bpu.tanke756.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nrw.gzhubu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fww.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xle.zhengqikj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gkp.yanxiufei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bwu.gogol.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fcs.cashguo.top

[L04] 设置超时
来源：http://tdl.shanyushiyangtech.top

Py:   requests.get(url, timeout=5)
来源：http://nlo.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://whk.smart0.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uok.shuidangran.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xjc.cashguo.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sbn.zycfv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vja.wangdashe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://osq.sufxvd.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bou.sjlbkw.cn

[L05] 上传文件（multipart）
来源：http://dnp.jinyuanbaomall.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jyq.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rdi.9152youxi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tkq.ydzc1.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://btv.yonumen.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://meg.yuanzhike.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zls.dianchejie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rnk.feifeiyinyue.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://okd.ydjk.org.cn

[L06] 解析响应为 JSON
来源：http://bcy.sufxvd.cn

Py:   resp.json()
来源：http://jbl.yonumen.top

PHP:  json_decode($body, true);
来源：http://owy.fanxiaobao.xyz

JS:   await resp.json()
来源：http://hfb.yuxming.cn

TS:   await resp.json()
来源：http://qmp.xinyue.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zhl.chenlongwang.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://eel.cdnleiting.top

Ruby: JSON.parse(resp.body)
来源：http://pwb.guannengcc.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gqu.xinyue.icu

[L07] 处理 HTTP 状态码
来源：http://eit.yongpay.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ryj.yuanzhike.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cps.tanke756.top

JS:   resp.ok;  resp.status
来源：http://byr.smart0.xyz

TS:   resp.ok;  resp.status
来源：http://zpm.hongshengwenyu.top

Java: resp.statusCode()
来源：http://ezw.hfpthk.cn

Go:   resp.StatusCode
来源：http://aeu.zdbjq.cn

Ruby: resp.code.to_i
来源：http://xbr.nanxinkj.top

C#:   (int)resp.StatusCode
来源：http://pho.gzhubu.top

[L08] 并发请求多个地址
来源：http://kla.havefunace.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bvd.xziqi.cn

PHP:  curl_multi_init() 系列
来源：http://rno.gogol.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xgu.cucudq.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ckp.yfazqb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uqm.9152youxi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://axk.fzhhl.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nhn.hnxiangtu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wcx.xuanzx.com

================================================================================
来源：http://rqq.zycfv.cn

M. 命令行 / 进程 / 环境
来源：http://uqm.jinghuilouyu.cn

================================================================================
来源：http://cny.ivvv.top

[M01] 读取命令行参数
来源：http://nzg.andypj.xyz

Py:   sys.argv[1:]
来源：http://iwt.wangshuangyany.cn

PHP:  $argv;  $argc;
来源：http://lif.bjfxy.top

JS:   process.argv.slice(2)
来源：http://jsa.yongpay.top

TS:   process.argv.slice(2)
来源：http://zuo.nanxuanxn.top

Java: args 数组（main 方法参数）
来源：http://bui.fehbvm.com

Go:   os.Args[1:]
来源：http://jjs.yj20258.top

Ruby: ARGV
来源：http://kov.yuxming.cn

C#:   args 数组（Main 方法参数）
来源：http://hup.fzhhl.top

[M02] 读取环境变量
来源：http://ppc.nanxinkj.top

Py:   os.environ.get("HOME")
来源：http://ilu.xuetiantiany.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://png.sysykeji.top

JS:   process.env.HOME
来源：http://grs.epnwcf.com

TS:   process.env.HOME
来源：http://qrm.hfpthk.cn

Java: System.getenv("HOME")
来源：http://lmg.cheryme.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gmn.tanke756.top

Ruby: ENV["HOME"]
来源：http://xgs.yuanzhike.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wvr.ivvv.top

[M03] 执行外部命令
来源：http://cli.cashguo.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ndc.hcnkem.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fgv.yongpay.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zou.tarul.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fgp.wangshuangyany.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cji.snrcjt.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://iry.ydjk.org.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ina.uphjek.com

C#:   Process.Start("ls", "-l");
来源：http://nhe.bjfxy.top

[M04] 获取当前工作目录
来源：http://egt.daria6918.cn

Py:   os.getcwd()
来源：http://qef.ehwqpu.com

PHP:  getcwd();
来源：http://tyi.hnxiangtu.top

JS:   process.cwd()
来源：http://vpv.gzhubu.top

TS:   process.cwd()
来源：http://yhu.ctjpmb.com

Java: Path.of("").toAbsolutePath()
来源：http://rsq.jinyuanbaomall.cn

Go:   os.Getwd()
来源：http://zai.yuanzhike.top

Ruby: Dir.pwd
来源：http://lau.haohaochexian.top

C#:   Directory.GetCurrentDirectory()
来源：http://waa.shuidangran.top

[M05] 设置退出码
来源：http://epx.cqqwz.cn

Py:   sys.exit(1)
来源：http://dge.redwolf501.top

PHP:  exit(1);
来源：http://npt.jiagoushi.top

JS:   process.exit(1)
来源：http://xlw.nanxinkj.top

TS:   process.exit(1)
来源：http://mtk.cashguo.top

Java: System.exit(1)
来源：http://nuz.c1oappe.top

Go:   os.Exit(1)
来源：http://gxu.cashguo.top

Ruby: exit 1
来源：http://eiy.ppjwa.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jaj.shangyingyoupin.top

[M06] 向标准错误输出
来源：http://lct.nanxuanxn.top

Py:   print("err", file=sys.stderr)
来源：http://svm.bbcook.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lnx.quarkkingdee.top

JS:   console.error("err")
来源：http://nyj.jinyuanbaomall.cn

TS:   console.error("err")
来源：http://gyc.52xcode.cn

Java: System.err.println("err")
来源：http://swa.andypj.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://afv.52xcode.cn

Ruby: warn "err"
来源：http://rfh.zdbjq.cn

C#:   Console.Error.WriteLine("err")
来源：http://ueh.jqgfzy.top

[M07] 判断是否为主入口
来源：http://jwq.xylfe.cn

Py:   if __name__ == "__main__":
来源：http://woc.chenlongwang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://urm.zhijiandao.cn

JS:   require.main === module
来源：http://vej.sysykeji.top

TS:   require.main === module
来源：http://wqn.gzhubu.top

Java: public static void main(String[] args)
来源：http://fuc.yueranfly.top

Go:   func main()
来源：http://xwp.chenjidiqi.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dmw.uphjek.com

C#:   static void Main(string[] args)
来源：http://mai.cheryme.top

[M08] 获取系统与运行时信息
来源：http://hrm.xuanzx.com

Py:   platform.system();  platform.python_version()
来源：http://zje.cucudq.cn

PHP:  PHP_OS;  phpversion();
来源：http://jyt.yuanzhike.top

JS:   process.platform;  process.version
来源：http://zgj.zhiwuduotai.top

TS:   process.platform;  process.version
来源：http://eiw.feifeiyinyue.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nfh.jqgufenzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://msn.xuetiantiany.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cmw.pycfn.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://nkm.sweek.top

================================================================================
来源：http://yrf.cashguo.top

N. 数据结构与算法
来源：http://fnj.iojbl.cn

================================================================================
来源：http://byd.yanxiufei.cn

[N01] 二分查找（有序数组）
来源：http://skj.yj20258.top

Py:   bisect.bisect_left(arr, x)
来源：http://pce.yfazqb.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gbk.xuetiantiany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zwv.vehdjk.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gth.gogol.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hfb.ppjwa.cn

Go:   sort.SearchInts(arr, x)
来源：http://xzi.jqgfzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://had.xuanzx.com

C#:   Array.BinarySearch(arr, x)
来源：http://ybk.aizwys.cn

[N02] 排序（工程实践用内置实现）
来源：http://dju.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://esh.hywenlv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://smg.redwolf501.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://rzi.iojbl.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bvx.ehwqpu.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mba.zhongyouzk.top

Go:   slices.Sort(arr)
来源：http://ias.shanyushiyangkeji.top

Ruby: arr.sort
来源：http://hkc.zhoulong.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://mna.xingfuxueyuan.xyz

[N03] 快速排序（分治示例）
来源：http://avv.ydjk.org.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vfj.haohaochexian.top

PHP:  // 递归实现，或用 usort
来源：http://vfg.sxryk.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nmt.316326.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://whx.cheryme.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yib.tianlin.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bhr.shzxlz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sjl.pycfn.com

C#:   // 手写递归，或 Array.Sort
来源：http://mbw.dashuyun.cn

[N04] 斐波那契数列
来源：http://pss.fzhhl.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://khw.zdqjudy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tsg.shanyushiyangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eng.hongshengwenyu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jms.jinghuilouyu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zfo.ydzc1.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nay.xuanzx.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mhh.snrcjt.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://isx.wangdashe.top

[N05] 最大公约数
来源：http://mlm.zhijiandao.cn

Py:   math.gcd(a, b)
来源：http://tvs.fehbvm.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kkx.gogol.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zuz.pycfn.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ani.tarul.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tzz.iojbl.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fgm.daria6918.cn

Ruby: a.gcd(b)
来源：http://fgy.c1oappe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vqj.yvedp.cn

[N06] 判断回文字符串
来源：http://hwn.shangyingyoupin.top

Py:   s == s[::-1]
来源：http://hnr.sjlbkw.cn

PHP:  $s === strrev($s);
来源：http://xsp.fanxiaobao.xyz

JS:   s === [...s].reverse().join("")
来源：http://pvf.havefunace.top

TS:   s === [...s].reverse().join("")
来源：http://qto.sysykeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://znv.jlsjyb.cn

Go:   // 双指针从两端比较
来源：http://aly.tian-w.cn

Ruby: s == s.reverse
来源：http://tft.zhijiandao.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://udn.dashuyun.cn

[N07] 两数之和（返回下标）
来源：http://dgh.yvedp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jmv.ywan-chungtsiang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ade.0kj1m.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fwn.yvedp.cn

TS:   // 手写 Map<string, number>
来源：http://wmr.yuxming.cn

Java: // 手写 HashMap
来源：http://wdx.xinyue.icu

Go:   // 手写 map[int]int
来源：http://fmp.yj202588.top

Ruby: // 手写 Hash
来源：http://vjg.zdqjudy.top

C#:   // 手写 Dictionary<int, int>
来源：http://xuq.pengpengdd.cyou

[N08] 生成全排列
来源：http://blj.tian-w.cn

Py:   itertools.permutations(arr)
来源：http://woc.bjfxy.top

PHP:  // 手写递归交换
来源：http://apv.sufxvd.cn

JS:   // 手写回溯递归
来源：http://rgn.yongpay.top

TS:   // 手写回溯递归
来源：http://icw.xuetiantiany.cn

Java: // 手写回溯递归
来源：http://qkf.yanxiufei.cn

Go:   // 手写回溯递归
来源：http://hal.pycfn.com

Ruby: arr.permutation.to_a
来源：http://ups.fanxiaobao.xyz

C#:   // 手写回溯递归
来源：http://cmh.haohaochexian.top

[N09] 栈与队列
来源：http://mmo.ppjwa.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wno.shuidangran.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://btt.daxiang520.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ysr.vehdjk.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ssm.hammf.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vpk.hammf.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uqq.ydzc1.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gvo.tarul.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lpb.xinyue.icu

[N10] 链表节点定义
来源：http://wuj.fengsongda.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://drl.chenzaomai.com

PHP:  class Node { public $v; public $next = null; }
来源：http://hrf.hfpthk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://myp.9152youxi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://moc.xuanzx.com

Java: class Node { int v; Node next; }
来源：http://yno.quarkkingdee.top

Go:   type Node struct { V int; Next *Node }
来源：http://hfr.fzhhl.top

Ruby: Node = Struct.new(:v, :next)
来源：http://glz.birdmap.top

C#:   class Node { public int V; public Node? Next; }
来源：http://mmg.yangfankeji.com

[N11] 二叉树中序遍历
来源：http://kez.chenjidiqi.icu

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yzq.hesvh.cn

PHP:  // 手写递归函数
来源：http://oia.xinyue.icu

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tbd.dashuyun.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yzi.feifeiyinyue.top

Java: // 手写递归
来源：http://iug.aizwys.cn

Go:   // 手写递归
来源：http://tcx.yj20258888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wxl.wangshuangyany.cn

C#:   // 手写递归
来源：http://flh.dashuyun.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ezc.tarul.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sam.9152youxi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fcn.ydzc1.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wfx.havefunace.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qux.jinyuanbaomall.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vew.guannengcc.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://odg.cheryme.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://llr.snrcjt.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tme.tianlin.xyz

================================================================================
来源：http://nhz.epnwcf.com

O. 并发与异步
来源：http://srh.cdnleiting.top

================================================================================
来源：http://mqp.yanxiufei.cn

[O01] 启动一个线程
来源：http://uya.yongpay.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://beb.ivvv.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fsk.meibo888.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vqq.yonumen.top

TS:   // 同 JS
来源：http://lpw.cdnleiting.top

Java: new Thread(() -> f()).start()
来源：http://gwb.andypj.xyz

Go:   go f()
来源：http://bny.aizwys.cn

Ruby: Thread.new { f }
来源：http://kcc.uphjek.com

C#:   Task.Run(() => F());
来源：http://ioc.nanxuanxn.top

[O02] 使用线程池
来源：http://gei.jinyuanbaomall.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cdl.zhaomingkeji.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ocl.xingfuxueyuan.xyz

JS:   // worker_threads 线程池
来源：http://ame.haohaochexian.top

TS:   // worker_threads 线程池
来源：http://knl.redwolf501.top

Java: Executors.newFixedThreadPool(4)
来源：http://mnd.snrcjt.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qpq.tanke756.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://irj.jqgufenzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qzv.jqgufenzy.top

[O03] 加锁保护共享数据
来源：http://szw.xylfe.cn

Py:   with lock: shared += 1
来源：http://vco.snrcjt.cn

PHP:  // 用 flock() 做文件锁
来源：http://tln.hysaishi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hfb.epnwcf.com

TS:   // 同 JS
来源：http://yfr.zhijiandao.cn

Java: synchronized (this) { shared++; }
来源：http://son.meibo888.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wlv.ivvv.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://dpt.ctjpmb.com

C#:   lock (gate) { shared++; }
来源：http://ued.smart0.xyz

[O04] 定义异步函数并等待
来源：http://lkz.cashguo.top

Py:   async def f():⏎    await g()
来源：http://wis.cdnleiting.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ybz.sweek.top

JS:   async function f() { await g(); }
来源：http://hsy.xinyue.icu

TS:   async function f(): Promise<void> { await g(); }
来源：http://mes.ybcxt.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nen.shanyushiyangkeji.top


<!-- 参考信息 -->
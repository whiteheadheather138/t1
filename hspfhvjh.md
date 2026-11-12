代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://ttj.tian-w.cn

JS:   v8.serialize(obj)        // Node
来源：http://zgu.pycfn.com

TS:   v8.serialize(obj)        // Node
来源：http://zoh.shzxlz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://asg.zhoulong.xyz

Go:   encoding/gob
来源：http://nmd.hywenlv.cn

Ruby: Marshal.dump(obj)
来源：http://voh.gogol.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://exy.gogol.net.cn

================================================================================
来源：http://vsf.nanxuanxn.top

L. 网络请求
来源：http://ern.jianghu66.top

================================================================================
来源：http://zbj.zhijiandao.cn

[L01] 发送 GET 请求
来源：http://ssr.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nxx.jiagoushi.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zpw.ywan-chungtsiang.top

JS:   await fetch(url)
来源：http://mkk.andypj.xyz

TS:   await fetch(url)
来源：http://fxq.yongpay.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lny.gogol.net.cn

Go:   resp, err := http.Get(url)
来源：http://jvj.sxryk.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rcx.yueranfly.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wlc.sysykeji.top

[L02] 发送 POST JSON
来源：http://ofa.sysykeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://xlh.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uvw.jinghuilouyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rnl.epnwcf.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://duz.redwolf501.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://egn.cheryme.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://abf.ctjpmb.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yea.yongpay.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nyx.dianchejie.cn

[L03] 设置自定义请求头
来源：http://vzo.gogol.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dgr.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tcl.xuetiantiany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rxy.zhixingplan.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gxw.yonumen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bys.xuetiantiany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xnx.fktsv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tba.jlsjyb.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jxe.yonumen.top

[L04] 设置超时
来源：http://pdt.zycfv.cn

Py:   requests.get(url, timeout=5)
来源：http://ykv.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zpn.hongshengwenyu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mlq.birdmap.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://muq.hnqzz.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nel.havefunace.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pry.cashguo.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vvt.jiagoushi.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gay.c1oappe.top

[L05] 上传文件（multipart）
来源：http://jlt.yonumen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hzm.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zlp.fktsv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gvw.chenjidiqi.icu

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ddq.guowangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://peq.xylfe.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jit.chenjidiqi.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://swu.yonumen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nec.zhijiandao.cn

[L06] 解析响应为 JSON
来源：http://uou.tian-w.cn

Py:   resp.json()
来源：http://ugk.tarul.cn

PHP:  json_decode($body, true);
来源：http://ozh.havefunace.top

JS:   await resp.json()
来源：http://ndn.svipenyu.cn

TS:   await resp.json()
来源：http://hzp.zhaomingkeji.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ygl.hammf.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xzh.wangshuangyany.cn

Ruby: JSON.parse(resp.body)
来源：http://ihh.hammf.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tuo.zhaomingkeji.xyz

[L07] 处理 HTTP 状态码
来源：http://idc.hywenlv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wgu.iojbl.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pei.yj20258888.top

JS:   resp.ok;  resp.status
来源：http://enk.redwolf501.top

TS:   resp.ok;  resp.status
来源：http://pwu.nwbrower.top

Java: resp.statusCode()
来源：http://ryx.jinqigufen.top

Go:   resp.StatusCode
来源：http://wzw.cdnleiting.top

Ruby: resp.code.to_i
来源：http://icf.cheryme.top

C#:   (int)resp.StatusCode
来源：http://otw.jiagoushi.top

[L08] 并发请求多个地址
来源：http://nyh.xingfuxueyuan.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://iof.ydzc1.top

PHP:  curl_multi_init() 系列
来源：http://hpr.zdbjq.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://teq.redwolf501.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gau.pengpengdd.cyou

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yqx.c1oappe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://prc.jlsjyb.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://imk.zdbjq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://spp.feifeiyinyue.top

================================================================================
来源：http://pdo.zhixingplan.top

M. 命令行 / 进程 / 环境
来源：http://wdp.iojbl.cn

================================================================================
来源：http://hry.hnqzz.top

[M01] 读取命令行参数
来源：http://res.yuxming.cn

Py:   sys.argv[1:]
来源：http://pqp.vqdsnc.cn

PHP:  $argv;  $argc;
来源：http://cpu.aizwys.cn

JS:   process.argv.slice(2)
来源：http://njt.tanke756.top

TS:   process.argv.slice(2)
来源：http://wen.gaohongyu789.top

Java: args 数组（main 方法参数）
来源：http://mzt.nanxuanxn.top

Go:   os.Args[1:]
来源：http://rje.yongpay.top

Ruby: ARGV
来源：http://bgj.dianchejie.cn

C#:   args 数组（Main 方法参数）
来源：http://eoa.ywan-chungtsiang.top

[M02] 读取环境变量
来源：http://yta.epnwcf.com

Py:   os.environ.get("HOME")
来源：http://cry.yuxming.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nrw.cdnleiting.top

JS:   process.env.HOME
来源：http://sdu.yonumen.top

TS:   process.env.HOME
来源：http://qyf.yongpay.top

Java: System.getenv("HOME")
来源：http://bor.mhx1999.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mhc.quarkkingdee.top

Ruby: ENV["HOME"]
来源：http://gxt.xinyue.icu

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uup.xylfe.cn

[M03] 执行外部命令
来源：http://kjx.yvedp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jou.aizwys.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://urv.cashguo.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hde.jinghuilouyu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pce.hesvh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oko.jqgufenzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://uts.dianchejie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gio.vehdjk.com

C#:   Process.Start("ls", "-l");
来源：http://xau.ybcxt.top

[M04] 获取当前工作目录
来源：http://edk.hesvh.cn

Py:   os.getcwd()
来源：http://aey.yuxming.cn

PHP:  getcwd();
来源：http://cea.kuanghao11.cn

JS:   process.cwd()
来源：http://jot.jinyuanbaomall.cn

TS:   process.cwd()
来源：http://sbe.cqqwz.cn

Java: Path.of("").toAbsolutePath()
来源：http://hgu.yj202588.top

Go:   os.Getwd()
来源：http://wwm.zhiwuduotai.top

Ruby: Dir.pwd
来源：http://zak.gzhubu.top

C#:   Directory.GetCurrentDirectory()
来源：http://fno.andypj.xyz

[M05] 设置退出码
来源：http://wtp.hywenlv.cn

Py:   sys.exit(1)
来源：http://xfn.haohaochexian.top

PHP:  exit(1);
来源：http://ilq.yvedp.cn

JS:   process.exit(1)
来源：http://pjv.dianchejie.cn

TS:   process.exit(1)
来源：http://kuo.ctjpmb.com

Java: System.exit(1)
来源：http://iga.zdbjq.cn

Go:   os.Exit(1)
来源：http://ykf.hammf.cn

Ruby: exit 1
来源：http://gkv.yanxiufei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jmz.snrcjt.cn

[M06] 向标准错误输出
来源：http://kmr.quarkkingdee.top

Py:   print("err", file=sys.stderr)
来源：http://tkr.zhaomingkeji.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://ldc.yueranfly.top

JS:   console.error("err")
来源：http://vut.guowangkeji.top

TS:   console.error("err")
来源：http://njv.vehdjk.com

Java: System.err.println("err")
来源：http://pqi.zhongyouzk.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fln.pycfn.com

Ruby: warn "err"
来源：http://bid.yuanzhike.top

C#:   Console.Error.WriteLine("err")
来源：http://gea.pengpengdd.cyou

[M07] 判断是否为主入口
来源：http://vgl.yvedp.cn

Py:   if __name__ == "__main__":
来源：http://ftn.ppjwa.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tql.hcnkem.com

JS:   require.main === module
来源：http://rzs.ctjpmb.com

TS:   require.main === module
来源：http://xhv.xinyue.icu

Java: public static void main(String[] args)
来源：http://zec.nanxuanxn.top

Go:   func main()
来源：http://wtp.yangfankeji.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gqv.tanke756.top

C#:   static void Main(string[] args)
来源：http://kxr.yanxiufei.cn

[M08] 获取系统与运行时信息
来源：http://mzt.ivvv.top

Py:   platform.system();  platform.python_version()
来源：http://guf.yfazqb.com

PHP:  PHP_OS;  phpversion();
来源：http://lmx.andypj.xyz

JS:   process.platform;  process.version
来源：http://hwz.yuanzhike.top

TS:   process.platform;  process.version
来源：http://rqn.ydjk.org.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ife.yuxming.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://moz.xziqi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ith.epnwcf.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://ozp.ywan-chungtsiang.top

================================================================================
来源：http://ugx.sjlbkw.cn

N. 数据结构与算法
来源：http://usc.zdqjudy.top

================================================================================
来源：http://jab.bbcook.cn

[N01] 二分查找（有序数组）
来源：http://spb.zhengqikj.top

Py:   bisect.bisect_left(arr, x)
来源：http://toc.zhiwuduotai.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ypw.hnxiangtu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pbk.sjlbkw.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hvs.cheryme.top

Java: Arrays.binarySearch(arr, x)
来源：http://jdb.cheryme.top

Go:   sort.SearchInts(arr, x)
来源：http://win.haohaochexian.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://mye.shangyingyoupin.top

C#:   Array.BinarySearch(arr, x)
来源：http://vhv.hfpthk.cn

[N02] 排序（工程实践用内置实现）
来源：http://inc.ywan-chungtsiang.top

Py:   sorted(arr);  arr.sort()
来源：http://vzv.vehdjk.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dzl.feifeiyinyue.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://auj.redwolf501.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ctk.ctjpmb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nve.birdmap.top

Go:   slices.Sort(arr)
来源：http://tdy.cdnleiting.top

Ruby: arr.sort
来源：http://hcw.xuetiantiany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://otq.pengpengdd.cyou

[N03] 快速排序（分治示例）
来源：http://zlp.yongpay.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ops.zycfv.cn

PHP:  // 递归实现，或用 usort
来源：http://aac.xuetiantiany.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ogn.yj20258.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uxg.bjfxy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ili.chenzaomai.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pre.fengsongda.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ogx.fengsongda.top

C#:   // 手写递归，或 Array.Sort
来源：http://gxb.daria6918.cn

[N04] 斐波那契数列
来源：http://zfl.mhx1999.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://paz.yanxiufei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qwo.yonumen.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jdp.yongpay.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://usd.52xcode.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vnv.ehwqpu.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dpz.hcnkem.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://biz.xingfuxueyuan.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pbv.xuanzx.com

[N05] 最大公约数
来源：http://hlc.andypj.xyz

Py:   math.gcd(a, b)
来源：http://uwn.yuxming.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jjh.cucudq.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lsr.aibaodan.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://osx.zhiwuduotai.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jzr.andypj.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gqw.zhongyouzk.top

Ruby: a.gcd(b)
来源：http://jrr.chenlongwang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nzw.yj20258.top

[N06] 判断回文字符串
来源：http://vwg.xuanzx.com

Py:   s == s[::-1]
来源：http://cxe.jinqigfzy.top

PHP:  $s === strrev($s);
来源：http://eve.52xcode.cn

JS:   s === [...s].reverse().join("")
来源：http://tjk.gogol.net.cn

TS:   s === [...s].reverse().join("")
来源：http://gbt.zhengqikj.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rys.zhaomingkeji.xyz

Go:   // 双指针从两端比较
来源：http://kpi.ppjwa.cn

Ruby: s == s.reverse
来源：http://seg.tarul.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://eji.yj202588.top

[N07] 两数之和（返回下标）
来源：http://smx.nanxinkj.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ccm.zhongyouzk.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tez.sysykeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://snn.zhijiandao.cn

TS:   // 手写 Map<string, number>
来源：http://pzp.smart0.xyz

Java: // 手写 HashMap
来源：http://ywh.haohaochexian.top

Go:   // 手写 map[int]int
来源：http://dfw.cheryme.top

Ruby: // 手写 Hash
来源：http://qyq.haohaochexian.top

C#:   // 手写 Dictionary<int, int>
来源：http://arw.aizwys.cn

[N08] 生成全排列
来源：http://btm.iojbl.cn

Py:   itertools.permutations(arr)
来源：http://nwy.chenjidiqi.icu

PHP:  // 手写递归交换
来源：http://ned.ehwqpu.com

JS:   // 手写回溯递归
来源：http://zqv.guowangkeji.top

TS:   // 手写回溯递归
来源：http://xal.shzxlz.cn

Java: // 手写回溯递归
来源：http://mdt.chenzaomai.com

Go:   // 手写回溯递归
来源：http://cxh.ivvv.top

Ruby: arr.permutation.to_a
来源：http://aoy.9152youxi.cn

C#:   // 手写回溯递归
来源：http://tig.aibaodan.cn

[N09] 栈与队列
来源：http://ehj.kuanghao11.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://usi.vqdsnc.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://oos.gaohongyu789.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://auj.chenjidiqi.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vnr.nanxuanxn.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pui.jqgufenzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hoh.guannengcc.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ico.316326.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vmg.ppjwa.cn

[N10] 链表节点定义
来源：http://uqo.uphjek.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://eho.yj20258888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://lue.cucudq.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://edd.iojbl.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wsu.yuxming.cn

Java: class Node { int v; Node next; }
来源：http://meu.nanxinkj.top

Go:   type Node struct { V int; Next *Node }
来源：http://fcs.xinyue.icu

Ruby: Node = Struct.new(:v, :next)
来源：http://eyb.gotoacloud.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xzq.ivvv.top

[N11] 二叉树中序遍历
来源：http://edb.xylfe.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cjb.smart0.xyz

PHP:  // 手写递归函数
来源：http://ifw.jqgufenzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vuw.zhijiandao.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wkr.haohaochexian.top

Java: // 手写递归
来源：http://sum.shangyingyoupin.top

Go:   // 手写递归
来源：http://ymn.zdqjudy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://anb.havefunace.top

C#:   // 手写递归
来源：http://xpi.shzxlz.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hdz.c1oappe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ocp.sysykeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://npz.uphjek.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ebo.hesvh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hyl.daxiang520.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cbt.kuanghao11.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://njh.dianchejie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ktn.aizwys.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wlr.kuanghao11.cn

================================================================================
来源：http://ilc.ydjk.org.cn

O. 并发与异步
来源：http://dtm.xuetiantiany.cn

================================================================================
来源：http://mkf.yueranfly.top

[O01] 启动一个线程
来源：http://czf.jqgfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://akr.tanke756.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nrk.chenzaomai.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rcc.zdbjq.cn

TS:   // 同 JS
来源：http://ole.hysaishi.cn

Java: new Thread(() -> f()).start()
来源：http://jzf.hnqzz.top

Go:   go f()
来源：http://njg.meibo888.top

Ruby: Thread.new { f }
来源：http://knk.zhixingplan.top

C#:   Task.Run(() => F());
来源：http://apm.ehwqpu.com

[O02] 使用线程池
来源：http://gqs.hfpthk.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mtc.sjlbkw.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vpn.yj20258888.top

JS:   // worker_threads 线程池
来源：http://ywx.cheryme.top

TS:   // worker_threads 线程池
来源：http://nix.sxryk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://owj.shuidangran.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rvo.guowangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iqd.jqgfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qhq.chenzaomai.com

[O03] 加锁保护共享数据
来源：http://opt.tianlin.xyz

Py:   with lock: shared += 1
来源：http://nyt.ehwqpu.com

PHP:  // 用 flock() 做文件锁
来源：http://jlp.zhiwuduotai.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rzd.fktsv.cn

TS:   // 同 JS
来源：http://huv.aibaodan.cn

Java: synchronized (this) { shared++; }
来源：http://pnm.52xcode.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jdf.zhongyouzk.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://qcz.yfazqb.com

C#:   lock (gate) { shared++; }
来源：http://mou.dashuyun.cn

[O04] 定义异步函数并等待
来源：http://qhc.ivvv.top

Py:   async def f():⏎    await g()
来源：http://wwk.fengsongda.top


<!-- 参考信息 -->
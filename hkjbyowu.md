代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://mpm.pycfn.com

JS:   v8.serialize(obj)        // Node
来源：http://caq.birdmap.top

TS:   v8.serialize(obj)        // Node
来源：http://bod.cucudq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hcm.zhixingplan.top

Go:   encoding/gob
来源：http://ihp.sufxvd.cn

Ruby: Marshal.dump(obj)
来源：http://vfn.cashguo.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://csg.zhixingplan.top

================================================================================
来源：http://clh.guannengcc.top

L. 网络请求
来源：http://usm.ydjk.org.cn

================================================================================
来源：http://gap.yfazqb.com

[L01] 发送 GET 请求
来源：http://itj.jianghu66.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://agf.yj202588.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jbs.pengpengdd.cyou

JS:   await fetch(url)
来源：http://exd.ctjpmb.com

TS:   await fetch(url)
来源：http://irf.nanxuanxn.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oab.chenjidiqi.icu

Go:   resp, err := http.Get(url)
来源：http://lhx.jqgufenzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kwz.nanxuanxn.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uvs.nanxuanxn.top

[L02] 发送 POST JSON
来源：http://wpd.xuanzx.com

Py:   requests.post(url, json={"a": 1})
来源：http://ylb.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hfc.nwbrower.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ukj.jyoumei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gzj.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mlu.vqdsnc.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nof.fzhhl.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gmy.zycfv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pkv.9152youxi.cn

[L03] 设置自定义请求头
来源：http://dss.sjlbkw.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fks.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fhw.shanyushiyangkeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pop.ydjk.org.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://smk.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pjh.hesvh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cxu.tanke756.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://olq.fanxiaobao.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hqo.yj202588.top

[L04] 设置超时
来源：http://dlf.jiagoushi.top

Py:   requests.get(url, timeout=5)
来源：http://gfr.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lsa.yuxming.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bzo.cucudq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gqr.zhixingplan.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://irv.bbcook.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xsq.zycfv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tce.iojbl.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://utf.guowangkeji.top

[L05] 上传文件（multipart）
来源：http://znh.dashuyun.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://riy.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qcc.nanxinkj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pfq.dashuyun.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pas.svipenyu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pet.yfazqb.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dbv.yongpay.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ahc.xinyue.icu

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yyy.pengpengdd.cyou

[L06] 解析响应为 JSON
来源：http://uip.snrcjt.cn

Py:   resp.json()
来源：http://det.pengpengdd.cyou

PHP:  json_decode($body, true);
来源：http://hsx.52xcode.cn

JS:   await resp.json()
来源：http://ntz.bjfxy.top

TS:   await resp.json()
来源：http://cpl.jqgufenzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tyg.jiagoushi.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lzw.wangshuangyany.cn

Ruby: JSON.parse(resp.body)
来源：http://lit.cashguo.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lbe.hywenlv.cn

[L07] 处理 HTTP 状态码
来源：http://ndu.316326.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jsm.andypj.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vcx.cucudq.cn

JS:   resp.ok;  resp.status
来源：http://hme.jinyuanbaomall.cn

TS:   resp.ok;  resp.status
来源：http://sli.cashguo.top

Java: resp.statusCode()
来源：http://pyw.mhx1999.top

Go:   resp.StatusCode
来源：http://dkl.fanxiaobao.xyz

Ruby: resp.code.to_i
来源：http://veq.meibo888.top

C#:   (int)resp.StatusCode
来源：http://mvz.hammf.cn

[L08] 并发请求多个地址
来源：http://bmn.guannengcc.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://aub.zhaomingkeji.xyz

PHP:  curl_multi_init() 系列
来源：http://qlv.bjfxy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rri.c1oappe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dry.daria6918.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rje.xinyue.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rzl.xziqi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ozk.aibaodan.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fap.zdqjudy.top

================================================================================
来源：http://pny.316326.xyz

M. 命令行 / 进程 / 环境
来源：http://ois.fengsongda.top

================================================================================
来源：http://nau.jlsjyb.cn

[M01] 读取命令行参数
来源：http://ctq.hammf.cn

Py:   sys.argv[1:]
来源：http://aab.jiagoushi.top

PHP:  $argv;  $argc;
来源：http://jwl.gaohongyu789.top

JS:   process.argv.slice(2)
来源：http://yft.tian-w.cn

TS:   process.argv.slice(2)
来源：http://rsq.yvedp.cn

Java: args 数组（main 方法参数）
来源：http://xdw.mhx1999.top

Go:   os.Args[1:]
来源：http://olv.tianlin.xyz

Ruby: ARGV
来源：http://suo.yangfankeji.com

C#:   args 数组（Main 方法参数）
来源：http://myf.fehbvm.com

[M02] 读取环境变量
来源：http://fsd.52xcode.cn

Py:   os.environ.get("HOME")
来源：http://jjn.gaohongyu789.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lab.xinyue.icu

JS:   process.env.HOME
来源：http://oyi.sufxvd.cn

TS:   process.env.HOME
来源：http://ufw.wangdashe.top

Java: System.getenv("HOME")
来源：http://eog.tianlin.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://eva.iojbl.cn

Ruby: ENV["HOME"]
来源：http://phh.shuidangran.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rsa.yfazqb.com

[M03] 执行外部命令
来源：http://tfj.zhiwuduotai.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qpk.yueranfly.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uso.gotoacloud.top

JS:   child_process.execSync("ls -l").toString()
来源：http://oir.yj20258.top

TS:   child_process.execSync("ls -l").toString()
来源：http://yhg.guowangkeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gpn.vqdsnc.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://uxw.tarul.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nsc.nanxinkj.top

C#:   Process.Start("ls", "-l");
来源：http://ouh.cucudq.cn

[M04] 获取当前工作目录
来源：http://thi.xuetiantiany.cn

Py:   os.getcwd()
来源：http://ean.ctjpmb.com

PHP:  getcwd();
来源：http://dqo.fktsv.cn

JS:   process.cwd()
来源：http://zhs.guannengcc.top

TS:   process.cwd()
来源：http://xyy.ybcxt.top

Java: Path.of("").toAbsolutePath()
来源：http://pvg.ywan-chungtsiang.top

Go:   os.Getwd()
来源：http://avh.yuanzhike.top

Ruby: Dir.pwd
来源：http://whp.smart0.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://zqo.jinqigufen.top

[M05] 设置退出码
来源：http://gnp.jinqigfzy.top

Py:   sys.exit(1)
来源：http://jkx.chenzaomai.com

PHP:  exit(1);
来源：http://alo.yongpay.top

JS:   process.exit(1)
来源：http://nmn.hcnkem.com

TS:   process.exit(1)
来源：http://vrr.hysaishi.cn

Java: System.exit(1)
来源：http://ges.uphjek.com

Go:   os.Exit(1)
来源：http://kqu.nanxinkj.top

Ruby: exit 1
来源：http://kqw.cdnleiting.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zvt.yj20258888.top

[M06] 向标准错误输出
来源：http://hsb.hnxiangtu.top

Py:   print("err", file=sys.stderr)
来源：http://gui.cucudq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fyk.zhijiandao.cn

JS:   console.error("err")
来源：http://bfs.cucudq.cn

TS:   console.error("err")
来源：http://mao.gogol.net.cn

Java: System.err.println("err")
来源：http://ghd.fengsongda.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bqo.chenzaomai.com

Ruby: warn "err"
来源：http://dbx.fanxiaobao.xyz

C#:   Console.Error.WriteLine("err")
来源：http://nqa.ctjpmb.com

[M07] 判断是否为主入口
来源：http://oax.yueranfly.top

Py:   if __name__ == "__main__":
来源：http://yef.jiagoushi.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jdi.yonumen.top

JS:   require.main === module
来源：http://cxh.hongshengwenyu.top

TS:   require.main === module
来源：http://zbp.zhoulong.xyz

Java: public static void main(String[] args)
来源：http://bxv.hnqzz.top

Go:   func main()
来源：http://pja.hywenlv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mdv.vehdjk.com

C#:   static void Main(string[] args)
来源：http://fbp.chenlongwang.top

[M08] 获取系统与运行时信息
来源：http://uek.gaohongyu789.top

Py:   platform.system();  platform.python_version()
来源：http://bll.zhoulong.xyz

PHP:  PHP_OS;  phpversion();
来源：http://umc.xuetiantiany.cn

JS:   process.platform;  process.version
来源：http://tfj.hfpthk.cn

TS:   process.platform;  process.version
来源：http://vaq.pycfn.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://quf.jianghu66.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://kmh.hesvh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wpd.sufxvd.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://duq.bjfxy.top

================================================================================
来源：http://omq.zycfv.cn

N. 数据结构与算法
来源：http://lds.zhiwuduotai.top

================================================================================
来源：http://kbx.yueranfly.top

[N01] 二分查找（有序数组）
来源：http://rzs.yuanzhike.top

Py:   bisect.bisect_left(arr, x)
来源：http://uov.hfpthk.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ysu.hcnkem.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://caw.jlsjyb.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oyi.yonumen.top

Java: Arrays.binarySearch(arr, x)
来源：http://nki.yvedp.cn

Go:   sort.SearchInts(arr, x)
来源：http://tju.pycfn.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://lih.0kj1m.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tdg.52xcode.cn

[N02] 排序（工程实践用内置实现）
来源：http://hjp.hywenlv.cn

Py:   sorted(arr);  arr.sort()
来源：http://yif.jinqigfzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wco.yvedp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jvs.yj202588.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ssu.fengsongda.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bta.ydzc1.top

Go:   slices.Sort(arr)
来源：http://lso.sufxvd.cn

Ruby: arr.sort
来源：http://czw.hnqzz.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://pwo.ctjpmb.com

[N03] 快速排序（分治示例）
来源：http://drq.tanke756.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hbn.jianghu66.top

PHP:  // 递归实现，或用 usort
来源：http://tuw.zhengqikj.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tuz.jlsjyb.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dit.sweek.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://znr.52xcode.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fll.ydzc1.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qie.guannengcc.top

C#:   // 手写递归，或 Array.Sort
来源：http://jyl.52xcode.cn

[N04] 斐波那契数列
来源：http://jnx.shanyushiyangtech.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qbj.ehwqpu.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wej.yj20258888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lpb.havefunace.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ugc.cheryme.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bdc.jqgufenzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xpz.daxiang520.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xwi.yonumen.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://han.nwbrower.top

[N05] 最大公约数
来源：http://dlm.jinqigfzy.top

Py:   math.gcd(a, b)
来源：http://wgf.sweek.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oav.xziqi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cgs.jinyuanbaomall.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uoi.meibo888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sdi.fktsv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xcj.jinyuanbaomall.cn

Ruby: a.gcd(b)
来源：http://tza.cucudq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://plc.shanyushiyangtech.top

[N06] 判断回文字符串
来源：http://urh.xingfuxueyuan.xyz

Py:   s == s[::-1]
来源：http://uiq.shangyingyoupin.top

PHP:  $s === strrev($s);
来源：http://eza.hywenlv.cn

JS:   s === [...s].reverse().join("")
来源：http://opx.zhijiandao.cn

TS:   s === [...s].reverse().join("")
来源：http://gum.wangshuangyany.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mzd.xuanzx.com

Go:   // 双指针从两端比较
来源：http://hxl.birdmap.top

Ruby: s == s.reverse
来源：http://jgp.jiagoushi.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zas.havefunace.top

[N07] 两数之和（返回下标）
来源：http://zkp.dianchejie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rrl.xuetiantiany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wgs.cashguo.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ioo.fanxiaobao.xyz

TS:   // 手写 Map<string, number>
来源：http://amj.yuanzhike.top

Java: // 手写 HashMap
来源：http://ycd.tarul.cn

Go:   // 手写 map[int]int
来源：http://lge.cucudq.cn

Ruby: // 手写 Hash
来源：http://dfb.yvedp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://utk.gotoacloud.top

[N08] 生成全排列
来源：http://ykn.yueranfly.top

Py:   itertools.permutations(arr)
来源：http://ljo.tian-w.cn

PHP:  // 手写递归交换
来源：http://pvu.guowangkeji.top

JS:   // 手写回溯递归
来源：http://pod.zhijiandao.cn

TS:   // 手写回溯递归
来源：http://xma.svipenyu.cn

Java: // 手写回溯递归
来源：http://hfj.yanxiufei.cn

Go:   // 手写回溯递归
来源：http://mdh.52xcode.cn

Ruby: arr.permutation.to_a
来源：http://oov.hysaishi.cn

C#:   // 手写回溯递归
来源：http://bke.hywenlv.cn

[N09] 栈与队列
来源：http://ayq.ppjwa.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jpi.redwolf501.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xnk.gogol.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://woo.nanxuanxn.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mmm.yuanzhike.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vtd.hfpthk.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ueh.9152youxi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://msw.hongshengwenyu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xtz.nanxuanxn.top

[N10] 链表节点定义
来源：http://zig.shanyushiyangtech.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qhl.hongshengwenyu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://cvn.fanxiaobao.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bow.fehbvm.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bzn.hongshengwenyu.top

Java: class Node { int v; Node next; }
来源：http://trd.cqqwz.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ysj.xuanzx.com

Ruby: Node = Struct.new(:v, :next)
来源：http://nxm.pengpengdd.cyou

C#:   class Node { public int V; public Node? Next; }
来源：http://gki.xylfe.cn

[N11] 二叉树中序遍历
来源：http://vfr.feifeiyinyue.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://foc.hnxiangtu.top

PHP:  // 手写递归函数
来源：http://her.nwbrower.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nae.hysaishi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qvx.jyoumei.cn

Java: // 手写递归
来源：http://min.fengsongda.top

Go:   // 手写递归
来源：http://mza.havefunace.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lpz.iojbl.cn

C#:   // 手写递归
来源：http://mhj.zhixingplan.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wqf.havefunace.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cgl.yj20258.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ugr.hywenlv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cen.gaohongyu789.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vjx.0kj1m.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sbf.feifeiyinyue.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://awc.pycfn.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iid.yvedp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nfz.cashguo.top

================================================================================
来源：http://iws.zhengqikj.top

O. 并发与异步
来源：http://mms.0kj1m.cn

================================================================================
来源：http://wbs.wangdashe.top

[O01] 启动一个线程
来源：http://oid.vqdsnc.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qok.tian-w.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://unj.shangyingyoupin.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wwz.daxiang520.top

TS:   // 同 JS
来源：http://opg.cashguo.top

Java: new Thread(() -> f()).start()
来源：http://imr.tarul.cn

Go:   go f()
来源：http://caa.sxryk.cn

Ruby: Thread.new { f }
来源：http://trj.uphjek.com

C#:   Task.Run(() => F());
来源：http://afk.hongshengwenyu.top

[O02] 使用线程池
来源：http://rpw.hfpthk.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lhh.xziqi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wag.chenlongwang.top

JS:   // worker_threads 线程池
来源：http://mpq.sjlbkw.cn

TS:   // worker_threads 线程池
来源：http://ywi.yj202588.top

Java: Executors.newFixedThreadPool(4)
来源：http://nin.316326.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hou.guowangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xha.gogol.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://brr.hesvh.cn

[O03] 加锁保护共享数据
来源：http://kxj.feifeiyinyue.top

Py:   with lock: shared += 1
来源：http://lpi.jyoumei.cn

PHP:  // 用 flock() 做文件锁
来源：http://wjh.andypj.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ocs.sjlbkw.cn

TS:   // 同 JS
来源：http://zrn.hnqzz.top

Java: synchronized (this) { shared++; }
来源：http://vfg.pycfn.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mxr.havefunace.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://cok.quarkkingdee.top

C#:   lock (gate) { shared++; }
来源：http://zhi.hesvh.cn

[O04] 定义异步函数并等待
来源：http://nnq.ybcxt.top

Py:   async def f():⏎    await g()
来源：http://myf.ydzc1.top


<!-- 参考信息 -->
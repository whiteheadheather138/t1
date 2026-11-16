代发 wailian999

Go:   encoding/gob
来源：http://tho.316326.xyz

Ruby: Marshal.dump(obj)
来源：http://pzf.c1oappe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ygd.yangfankeji.com

================================================================================
来源：http://jof.cheryme.top

L. 网络请求
来源：http://plm.gaohongyu789.top

================================================================================
来源：http://klc.yj202588.top

[L01] 发送 GET 请求
来源：http://kfs.bjfxy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://min.meibo888.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xqt.meibo888.top

JS:   await fetch(url)
来源：http://qgt.zhixingplan.top

TS:   await fetch(url)
来源：http://fwr.jlsjyb.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://slm.316326.xyz

Go:   resp, err := http.Get(url)
来源：http://gfh.gogol.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qsh.jlsjyb.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://snk.bbcook.cn

[L02] 发送 POST JSON
来源：http://kxy.yonumen.top

Py:   requests.post(url, json={"a": 1})
来源：http://gto.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nhv.daxiang520.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bdj.andypj.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ghw.sxryk.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ljp.zhijiandao.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ret.bbcook.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://txc.ydzc1.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jnk.birdmap.top

[L03] 设置自定义请求头
来源：http://pmd.zhiwuduotai.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rvf.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xuh.bjfxy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://npl.dianchejie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fen.ywan-chungtsiang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dua.9152youxi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tql.aizwys.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ugd.xingfuxueyuan.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rzt.tian-w.cn

[L04] 设置超时
来源：http://edy.chenlongwang.top

Py:   requests.get(url, timeout=5)
来源：http://oym.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gwj.pycfn.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wij.nwbrower.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pkn.yj202588.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://evq.snrcjt.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nlw.zhaomingkeji.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vdo.zdbjq.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gcb.zhoulong.xyz

[L05] 上传文件（multipart）
来源：http://sxq.chenjidiqi.icu

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rtb.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tqm.guannengcc.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ekd.kuanghao11.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ury.xylfe.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ytu.xingfuxueyuan.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kxn.snrcjt.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jyf.aibaodan.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wry.0kj1m.cn

[L06] 解析响应为 JSON
来源：http://sdx.zhengqikj.top

Py:   resp.json()
来源：http://ghy.hfpthk.cn

PHP:  json_decode($body, true);
来源：http://xbn.yueranfly.top

JS:   await resp.json()
来源：http://olw.316326.xyz

TS:   await resp.json()
来源：http://jvh.fehbvm.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ymp.dashuyun.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fjy.dashuyun.cn

Ruby: JSON.parse(resp.body)
来源：http://ghr.zhaomingkeji.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zws.jianghu66.top

[L07] 处理 HTTP 状态码
来源：http://fax.c1oappe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mhq.feifeiyinyue.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kax.nanxinkj.top

JS:   resp.ok;  resp.status
来源：http://hcq.uphjek.com

TS:   resp.ok;  resp.status
来源：http://awx.zhengqikj.top

Java: resp.statusCode()
来源：http://ehv.yanxiufei.cn

Go:   resp.StatusCode
来源：http://ylt.hnxiangtu.top

Ruby: resp.code.to_i
来源：http://hzj.hysaishi.cn

C#:   (int)resp.StatusCode
来源：http://qwy.ydjk.org.cn

[L08] 并发请求多个地址
来源：http://wuo.wangshuangyany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ixj.fanxiaobao.xyz

PHP:  curl_multi_init() 系列
来源：http://ume.haohaochexian.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dza.nanxuanxn.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kml.sxryk.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://swt.xingfuxueyuan.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ewm.52xcode.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vxu.chenjidiqi.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://aen.xinyue.icu

================================================================================
来源：http://eiq.ivvv.top

M. 命令行 / 进程 / 环境
来源：http://xal.fzhhl.top

================================================================================
来源：http://jeu.yj20258.top

[M01] 读取命令行参数
来源：http://hsk.jinghuilouyu.cn

Py:   sys.argv[1:]
来源：http://uuv.shanyushiyangtech.top

PHP:  $argv;  $argc;
来源：http://dyd.mhx1999.top

JS:   process.argv.slice(2)
来源：http://pfr.jinghuilouyu.cn

TS:   process.argv.slice(2)
来源：http://kro.gzhubu.top

Java: args 数组（main 方法参数）
来源：http://ina.birdmap.top

Go:   os.Args[1:]
来源：http://jrv.fanxiaobao.xyz

Ruby: ARGV
来源：http://zfa.yj202588.top

C#:   args 数组（Main 方法参数）
来源：http://lqj.ppjwa.cn

[M02] 读取环境变量
来源：http://ele.daria6918.cn

Py:   os.environ.get("HOME")
来源：http://fub.meibo888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lbh.tanke756.top

JS:   process.env.HOME
来源：http://bmu.ppjwa.cn

TS:   process.env.HOME
来源：http://ryl.ywan-chungtsiang.top

Java: System.getenv("HOME")
来源：http://hyv.yj20258.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hch.feifeiyinyue.top

Ruby: ENV["HOME"]
来源：http://btw.gogol.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bxa.jinqigfzy.top

[M03] 执行外部命令
来源：http://shu.hfpthk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nii.fktsv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mrk.pycfn.com

JS:   child_process.execSync("ls -l").toString()
来源：http://hmc.aibaodan.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://khy.xziqi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oqb.jinqigfzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vbb.gogol.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hur.jqgufenzy.top

C#:   Process.Start("ls", "-l");
来源：http://owz.jqgufenzy.top

[M04] 获取当前工作目录
来源：http://lwr.jiagoushi.top

Py:   os.getcwd()
来源：http://gxq.cashguo.top

PHP:  getcwd();
来源：http://neu.cucudq.cn

JS:   process.cwd()
来源：http://afm.sysykeji.top

TS:   process.cwd()
来源：http://waz.ybcxt.top

Java: Path.of("").toAbsolutePath()
来源：http://tzi.zdqjudy.top

Go:   os.Getwd()
来源：http://coj.jinqigufen.top

Ruby: Dir.pwd
来源：http://quv.shanyushiyangkeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://xgs.jyoumei.cn

[M05] 设置退出码
来源：http://tzb.hfpthk.cn

Py:   sys.exit(1)
来源：http://uxy.dianchejie.cn

PHP:  exit(1);
来源：http://amc.mhx1999.top

JS:   process.exit(1)
来源：http://ozm.xuanzx.com

TS:   process.exit(1)
来源：http://vdx.fengsongda.top

Java: System.exit(1)
来源：http://mmj.bbcook.cn

Go:   os.Exit(1)
来源：http://com.yueranfly.top

Ruby: exit 1
来源：http://fon.jyoumei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hnb.shuidangran.top

[M06] 向标准错误输出
来源：http://ahp.jqgufenzy.top

Py:   print("err", file=sys.stderr)
来源：http://ait.nanxuanxn.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xzl.yonumen.top

JS:   console.error("err")
来源：http://hcl.shanyushiyangkeji.top

TS:   console.error("err")
来源：http://gmn.yongpay.top

Java: System.err.println("err")
来源：http://hso.ywan-chungtsiang.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dkh.tanke756.top

Ruby: warn "err"
来源：http://lnc.wangdashe.top

C#:   Console.Error.WriteLine("err")
来源：http://mec.fzhhl.top

[M07] 判断是否为主入口
来源：http://acc.xingfuxueyuan.xyz

Py:   if __name__ == "__main__":
来源：http://dnn.ywan-chungtsiang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gxs.ybcxt.top

JS:   require.main === module
来源：http://ihq.hcnkem.com

TS:   require.main === module
来源：http://ncg.daxiang520.top

Java: public static void main(String[] args)
来源：http://rrb.cdnleiting.top

Go:   func main()
来源：http://izl.hnqzz.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kwq.dianchejie.cn

C#:   static void Main(string[] args)
来源：http://csr.vehdjk.com

[M08] 获取系统与运行时信息
来源：http://jdi.nanxuanxn.top

Py:   platform.system();  platform.python_version()
来源：http://grl.yj20258888.top

PHP:  PHP_OS;  phpversion();
来源：http://zzc.yangfankeji.com

JS:   process.platform;  process.version
来源：http://roh.jiagoushi.top

TS:   process.platform;  process.version
来源：http://pqp.yvedp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uwg.xuetiantiany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://msa.ydjk.org.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hqc.hfpthk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rxt.zdqjudy.top

================================================================================
来源：http://odh.sufxvd.cn

N. 数据结构与算法
来源：http://hfo.hfpthk.cn

================================================================================
来源：http://bzk.ybcxt.top

[N01] 二分查找（有序数组）
来源：http://lil.tarul.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gvc.zhongyouzk.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bdz.vqdsnc.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zgd.gzhubu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://enr.yuanzhike.top

Java: Arrays.binarySearch(arr, x)
来源：http://qeq.uphjek.com

Go:   sort.SearchInts(arr, x)
来源：http://xna.svipenyu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ewr.aizwys.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zfb.xylfe.cn

[N02] 排序（工程实践用内置实现）
来源：http://tpq.wangshuangyany.cn

Py:   sorted(arr);  arr.sort()
来源：http://hbb.chenzaomai.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cdo.chenjidiqi.icu

JS:   [...arr].sort((a, b) => a - b)
来源：http://bis.chenjidiqi.icu

TS:   [...arr].sort((a, b) => a - b)
来源：http://gek.yanxiufei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://koo.ydjk.org.cn

Go:   slices.Sort(arr)
来源：http://map.9152youxi.cn

Ruby: arr.sort
来源：http://jou.yj20258888.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://avk.gaohongyu789.top

[N03] 快速排序（分治示例）
来源：http://qjv.hcnkem.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nqi.yj20258.top

PHP:  // 递归实现，或用 usort
来源：http://vgm.yvedp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gjn.cheryme.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xcu.52xcode.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ujf.fanxiaobao.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vlx.cashguo.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jbi.aizwys.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zlh.dianchejie.cn

[N04] 斐波那契数列
来源：http://xvf.uphjek.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yno.chenlongwang.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fwo.sweek.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tam.hesvh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dtj.snrcjt.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gxi.ywan-chungtsiang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ptv.gogol.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lcg.wangdashe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ors.hysaishi.cn

[N05] 最大公约数
来源：http://els.zhiwuduotai.top

Py:   math.gcd(a, b)
来源：http://sxv.hfpthk.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://epw.zhaomingkeji.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://amb.ydjk.org.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cfi.ivvv.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://syk.zhaomingkeji.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rob.feifeiyinyue.top

Ruby: a.gcd(b)
来源：http://vor.ehwqpu.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uly.xuanzx.com

[N06] 判断回文字符串
来源：http://otj.guannengcc.top

Py:   s == s[::-1]
来源：http://rlo.xuanzx.com

PHP:  $s === strrev($s);
来源：http://agn.vqdsnc.cn

JS:   s === [...s].reverse().join("")
来源：http://jhn.cqqwz.cn

TS:   s === [...s].reverse().join("")
来源：http://oub.shangyingyoupin.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bxa.cheryme.top

Go:   // 双指针从两端比较
来源：http://sor.ppjwa.cn

Ruby: s == s.reverse
来源：http://cvq.hesvh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://krd.hongshengwenyu.top

[N07] 两数之和（返回下标）
来源：http://cpc.quarkkingdee.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kcm.tanke756.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wyc.cdnleiting.top

JS:   // 手写 Map：map.set(v, i)
来源：http://sbp.zycfv.cn

TS:   // 手写 Map<string, number>
来源：http://mqa.xziqi.cn

Java: // 手写 HashMap
来源：http://cwn.dianchejie.cn

Go:   // 手写 map[int]int
来源：http://ioj.jqgfzy.top

Ruby: // 手写 Hash
来源：http://hai.vehdjk.com

C#:   // 手写 Dictionary<int, int>
来源：http://jqg.bbcook.cn

[N08] 生成全排列
来源：http://fig.yongpay.top

Py:   itertools.permutations(arr)
来源：http://qvc.ybcxt.top

PHP:  // 手写递归交换
来源：http://qht.52xcode.cn

JS:   // 手写回溯递归
来源：http://but.52xcode.cn

TS:   // 手写回溯递归
来源：http://ekj.wangdashe.top

Java: // 手写回溯递归
来源：http://kie.zhijiandao.cn

Go:   // 手写回溯递归
来源：http://qfs.jinghuilouyu.cn

Ruby: arr.permutation.to_a
来源：http://otp.c1oappe.top

C#:   // 手写回溯递归
来源：http://ini.aibaodan.cn

[N09] 栈与队列
来源：http://riu.tian-w.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gkv.yonumen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://byt.shzxlz.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rmz.uphjek.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zwu.jianghu66.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://swd.vehdjk.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://azr.fzhhl.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pdj.jqgufenzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://htx.cdnleiting.top

[N10] 链表节点定义
来源：http://sqg.52xcode.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://npz.hongshengwenyu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://fcv.vehdjk.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qvm.wangshuangyany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bpu.zhiwuduotai.top

Java: class Node { int v; Node next; }
来源：http://lec.shanyushiyangtech.top

Go:   type Node struct { V int; Next *Node }
来源：http://wlf.smart0.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://gvz.jqgufenzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://hhw.yueranfly.top

[N11] 二叉树中序遍历
来源：http://amq.yj202588.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vfm.fehbvm.com

PHP:  // 手写递归函数
来源：http://hsl.jinghuilouyu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uxd.aizwys.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oqm.zhiwuduotai.top

Java: // 手写递归
来源：http://kvf.hcnkem.com

Go:   // 手写递归
来源：http://meu.hysaishi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lbn.epnwcf.com

C#:   // 手写递归
来源：http://tmi.hfpthk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uyb.xziqi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yew.aizwys.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bwl.yanxiufei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jms.xinyue.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mbh.shangyingyoupin.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yep.hammf.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qep.aizwys.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hlt.yvedp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yjr.daria6918.cn

================================================================================
来源：http://gcx.shuidangran.top

O. 并发与异步
来源：http://zwu.vqdsnc.cn

================================================================================
来源：http://xxj.zhixingplan.top

[O01] 启动一个线程
来源：http://qhm.tarul.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jtt.hnxiangtu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://scj.zdqjudy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ybt.jiagoushi.top

TS:   // 同 JS
来源：http://qcz.sxryk.cn

Java: new Thread(() -> f()).start()
来源：http://roe.xingfuxueyuan.xyz

Go:   go f()
来源：http://llb.jlsjyb.cn

Ruby: Thread.new { f }
来源：http://vty.jqgfzy.top

C#:   Task.Run(() => F());
来源：http://nql.zdbjq.cn

[O02] 使用线程池
来源：http://wra.fehbvm.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qkr.vqdsnc.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wvd.zhongyouzk.top

JS:   // worker_threads 线程池
来源：http://paf.yvedp.cn

TS:   // worker_threads 线程池
来源：http://xnj.xuetiantiany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://frb.cucudq.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gmf.jinqigfzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://taa.ywan-chungtsiang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oda.xziqi.cn

[O03] 加锁保护共享数据
来源：http://tpz.vqdsnc.cn

Py:   with lock: shared += 1
来源：http://tci.ybcxt.top

PHP:  // 用 flock() 做文件锁
来源：http://adf.ehwqpu.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ooz.sweek.top

TS:   // 同 JS
来源：http://zvx.zhixingplan.top

Java: synchronized (this) { shared++; }
来源：http://ccz.kuanghao11.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://flg.nwbrower.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://vmr.andypj.xyz

C#:   lock (gate) { shared++; }
来源：http://voo.jqgufenzy.top

[O04] 定义异步函数并等待
来源：http://yob.ywan-chungtsiang.top

Py:   async def f():⏎    await g()
来源：http://lyv.jinqigfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://etw.meibo888.top

JS:   async function f() { await g(); }
来源：http://eqx.hongshengwenyu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://qha.hnxiangtu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://efu.zdqjudy.top


<!-- 参考信息 -->
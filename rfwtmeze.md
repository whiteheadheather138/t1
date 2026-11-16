代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://tvx.shanyushiyangtech.top

JS:   v8.serialize(obj)        // Node
来源：http://njv.svipenyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://fnz.kuanghao11.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kck.hnxiangtu.top

Go:   encoding/gob
来源：http://epq.fehbvm.com

Ruby: Marshal.dump(obj)
来源：http://nyn.yuanzhike.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://aww.ppjwa.cn

================================================================================
来源：http://clr.cqqwz.cn

L. 网络请求
来源：http://thp.sweek.top

================================================================================
来源：http://aza.yj20258888.top

[L01] 发送 GET 请求
来源：http://gor.9152youxi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yek.zhijiandao.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://stn.cashguo.top

JS:   await fetch(url)
来源：http://qnk.xuanzx.com

TS:   await fetch(url)
来源：http://heq.nanxinkj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ptq.zhoulong.xyz

Go:   resp, err := http.Get(url)
来源：http://tmr.ydzc1.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wel.feifeiyinyue.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hsu.yvedp.cn

[L02] 发送 POST JSON
来源：http://onp.jianghu66.top

Py:   requests.post(url, json={"a": 1})
来源：http://bbf.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fxw.zhaomingkeji.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://obr.mhx1999.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sem.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://orp.mhx1999.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wef.bbcook.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nwe.dianchejie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fwj.fanxiaobao.xyz

[L03] 设置自定义请求头
来源：http://xco.jlsjyb.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wlh.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://snv.sysykeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gty.nwbrower.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://djy.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fvf.yj20258888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nla.birdmap.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hyc.shanyushiyangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lue.zhongyouzk.top

[L04] 设置超时
来源：http://cbw.snrcjt.cn

Py:   requests.get(url, timeout=5)
来源：http://lwa.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zei.chenjidiqi.icu

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pky.sxryk.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hiv.guowangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zrk.meibo888.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://arf.yuanzhike.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hlt.dianchejie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://aki.zhoulong.xyz

[L05] 上传文件（multipart）
来源：http://zut.hywenlv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rvp.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xme.kuanghao11.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qig.hfpthk.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yyt.yj20258888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qbx.dashuyun.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pcf.shangyingyoupin.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zho.yj20258.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sip.andypj.xyz

[L06] 解析响应为 JSON
来源：http://qff.shzxlz.cn

Py:   resp.json()
来源：http://mgf.nwbrower.top

PHP:  json_decode($body, true);
来源：http://jty.yueranfly.top

JS:   await resp.json()
来源：http://zxm.yj20258.top

TS:   await resp.json()
来源：http://hum.yuxming.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://smo.jyoumei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://old.zhongyouzk.top

Ruby: JSON.parse(resp.body)
来源：http://jyn.guannengcc.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mei.c1oappe.top

[L07] 处理 HTTP 状态码
来源：http://kau.yanxiufei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zxc.jyoumei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rco.sxryk.cn

JS:   resp.ok;  resp.status
来源：http://mgn.yfazqb.com

TS:   resp.ok;  resp.status
来源：http://gzz.xuetiantiany.cn

Java: resp.statusCode()
来源：http://dbp.wangshuangyany.cn

Go:   resp.StatusCode
来源：http://nzz.yj202588.top

Ruby: resp.code.to_i
来源：http://puv.jqgfzy.top

C#:   (int)resp.StatusCode
来源：http://ppd.yfazqb.com

[L08] 并发请求多个地址
来源：http://wlx.sysykeji.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ext.birdmap.top

PHP:  curl_multi_init() 系列
来源：http://khc.cdnleiting.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nbz.yj202588.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nuk.hcnkem.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mkx.jiagoushi.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tew.jiagoushi.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://glj.dashuyun.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://siv.fengsongda.top

================================================================================
来源：http://knq.meibo888.top

M. 命令行 / 进程 / 环境
来源：http://fko.ctjpmb.com

================================================================================
来源：http://cyq.hywenlv.cn

[M01] 读取命令行参数
来源：http://jfk.svipenyu.cn

Py:   sys.argv[1:]
来源：http://mwu.tian-w.cn

PHP:  $argv;  $argc;
来源：http://gfh.ybcxt.top

JS:   process.argv.slice(2)
来源：http://qoa.daria6918.cn

TS:   process.argv.slice(2)
来源：http://kzr.dashuyun.cn

Java: args 数组（main 方法参数）
来源：http://aux.xuetiantiany.cn

Go:   os.Args[1:]
来源：http://dqh.zhixingplan.top

Ruby: ARGV
来源：http://fyv.yj20258888.top

C#:   args 数组（Main 方法参数）
来源：http://nvp.havefunace.top

[M02] 读取环境变量
来源：http://pup.daxiang520.top

Py:   os.environ.get("HOME")
来源：http://nnq.quarkkingdee.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mdw.tanke756.top

JS:   process.env.HOME
来源：http://apz.wangdashe.top

TS:   process.env.HOME
来源：http://qyj.xinyue.icu

Java: System.getenv("HOME")
来源：http://emq.uphjek.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gwg.dashuyun.cn

Ruby: ENV["HOME"]
来源：http://zor.tanke756.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ojj.jlsjyb.cn

[M03] 执行外部命令
来源：http://zjh.nanxuanxn.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mve.meibo888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fes.jiagoushi.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xuq.nwbrower.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zcx.chenjidiqi.icu

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fou.xinyue.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://kvt.sxryk.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qrt.9152youxi.cn

C#:   Process.Start("ls", "-l");
来源：http://oww.cucudq.cn

[M04] 获取当前工作目录
来源：http://zmg.jqgufenzy.top

Py:   os.getcwd()
来源：http://bai.sweek.top

PHP:  getcwd();
来源：http://ncc.zhijiandao.cn

JS:   process.cwd()
来源：http://avk.jyoumei.cn

TS:   process.cwd()
来源：http://ckj.sjlbkw.cn

Java: Path.of("").toAbsolutePath()
来源：http://zce.guannengcc.top

Go:   os.Getwd()
来源：http://yec.bjfxy.top

Ruby: Dir.pwd
来源：http://zjh.sweek.top

C#:   Directory.GetCurrentDirectory()
来源：http://nkm.yuanzhike.top

[M05] 设置退出码
来源：http://rkl.jyoumei.cn

Py:   sys.exit(1)
来源：http://sby.fehbvm.com

PHP:  exit(1);
来源：http://cqh.tianlin.xyz

JS:   process.exit(1)
来源：http://xil.ybcxt.top

TS:   process.exit(1)
来源：http://vcr.hesvh.cn

Java: System.exit(1)
来源：http://bkt.ppjwa.cn

Go:   os.Exit(1)
来源：http://vqp.yj20258.top

Ruby: exit 1
来源：http://ifb.hcnkem.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://awl.sweek.top

[M06] 向标准错误输出
来源：http://opr.pycfn.com

Py:   print("err", file=sys.stderr)
来源：http://dni.jlsjyb.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hlg.jyoumei.cn

JS:   console.error("err")
来源：http://kds.epnwcf.com

TS:   console.error("err")
来源：http://vsx.nanxuanxn.top

Java: System.err.println("err")
来源：http://ugi.ydjk.org.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tqh.ehwqpu.com

Ruby: warn "err"
来源：http://dtx.jqgufenzy.top

C#:   Console.Error.WriteLine("err")
来源：http://psw.ehwqpu.com

[M07] 判断是否为主入口
来源：http://zvs.gotoacloud.top

Py:   if __name__ == "__main__":
来源：http://fos.cdnleiting.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pfa.aibaodan.cn

JS:   require.main === module
来源：http://ptd.sxryk.cn

TS:   require.main === module
来源：http://pzq.ehwqpu.com

Java: public static void main(String[] args)
来源：http://rgi.chenlongwang.top

Go:   func main()
来源：http://ekn.gzhubu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mkd.jqgufenzy.top

C#:   static void Main(string[] args)
来源：http://quo.xylfe.cn

[M08] 获取系统与运行时信息
来源：http://zxj.xuanzx.com

Py:   platform.system();  platform.python_version()
来源：http://sbo.wangdashe.top

PHP:  PHP_OS;  phpversion();
来源：http://hdp.jinyuanbaomall.cn

JS:   process.platform;  process.version
来源：http://uaq.zycfv.cn

TS:   process.platform;  process.version
来源：http://ysi.yj20258.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://czp.wangdashe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ppw.daxiang520.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xfk.shzxlz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fqf.zdqjudy.top

================================================================================
来源：http://hpc.cdnleiting.top

N. 数据结构与算法
来源：http://fbu.ehwqpu.com

================================================================================
来源：http://fan.epnwcf.com

[N01] 二分查找（有序数组）
来源：http://dwa.jinyuanbaomall.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hkw.vehdjk.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xoq.sxryk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gls.yj20258888.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gyy.tarul.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nss.gaohongyu789.top

Go:   sort.SearchInts(arr, x)
来源：http://gry.jinghuilouyu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://taw.cdnleiting.top

C#:   Array.BinarySearch(arr, x)
来源：http://lnn.zhengqikj.top

[N02] 排序（工程实践用内置实现）
来源：http://grg.haohaochexian.top

Py:   sorted(arr);  arr.sort()
来源：http://wro.gaohongyu789.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://liw.snrcjt.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rdb.hnxiangtu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ait.yuxming.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hsg.zhengqikj.top

Go:   slices.Sort(arr)
来源：http://lax.fanxiaobao.xyz

Ruby: arr.sort
来源：http://mig.tanke756.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hsz.yueranfly.top

[N03] 快速排序（分治示例）
来源：http://xko.havefunace.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://aqg.chenlongwang.top

PHP:  // 递归实现，或用 usort
来源：http://zdh.zhijiandao.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pir.cqqwz.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ehm.shanyushiyangkeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uuv.hywenlv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ejo.epnwcf.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jvn.ivvv.top

C#:   // 手写递归，或 Array.Sort
来源：http://sfu.birdmap.top

[N04] 斐波那契数列
来源：http://kmr.daria6918.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://icd.hcnkem.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gww.52xcode.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vcg.ehwqpu.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vmb.tian-w.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://olo.gzhubu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ogr.c1oappe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pio.xingfuxueyuan.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hmd.fengsongda.top

[N05] 最大公约数
来源：http://huw.ehwqpu.com

Py:   math.gcd(a, b)
来源：http://ydn.shanyushiyangtech.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rmn.yuxming.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://umn.ybcxt.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://suw.havefunace.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://txj.tian-w.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zfk.c1oappe.top

Ruby: a.gcd(b)
来源：http://ray.yueranfly.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pib.quarkkingdee.top

[N06] 判断回文字符串
来源：http://aux.cucudq.cn

Py:   s == s[::-1]
来源：http://yms.jyoumei.cn

PHP:  $s === strrev($s);
来源：http://zms.svipenyu.cn

JS:   s === [...s].reverse().join("")
来源：http://ctf.tanke756.top

TS:   s === [...s].reverse().join("")
来源：http://ofp.hfpthk.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xdz.nanxinkj.top

Go:   // 双指针从两端比较
来源：http://fqf.shuidangran.top

Ruby: s == s.reverse
来源：http://ffi.nanxuanxn.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://hkb.andypj.xyz

[N07] 两数之和（返回下标）
来源：http://bzs.fzhhl.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cuz.xingfuxueyuan.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ifu.52xcode.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jxd.xziqi.cn

TS:   // 手写 Map<string, number>
来源：http://tmt.yonumen.top

Java: // 手写 HashMap
来源：http://bet.hesvh.cn

Go:   // 手写 map[int]int
来源：http://ecc.yangfankeji.com

Ruby: // 手写 Hash
来源：http://xti.xuanzx.com

C#:   // 手写 Dictionary<int, int>
来源：http://lly.cdnleiting.top

[N08] 生成全排列
来源：http://hkr.chenjidiqi.icu

Py:   itertools.permutations(arr)
来源：http://ylc.yvedp.cn

PHP:  // 手写递归交换
来源：http://sqe.hongshengwenyu.top

JS:   // 手写回溯递归
来源：http://vmb.zhixingplan.top

TS:   // 手写回溯递归
来源：http://lye.shanyushiyangkeji.top

Java: // 手写回溯递归
来源：http://xfq.hnqzz.top

Go:   // 手写回溯递归
来源：http://oun.epnwcf.com

Ruby: arr.permutation.to_a
来源：http://zno.jyoumei.cn

C#:   // 手写回溯递归
来源：http://htd.chenlongwang.top

[N09] 栈与队列
来源：http://tze.yj202588.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pva.jyoumei.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xwl.epnwcf.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://chk.xuetiantiany.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jjq.sxryk.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nzt.xziqi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vji.xuetiantiany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sst.ppjwa.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eyf.smart0.xyz

[N10] 链表节点定义
来源：http://bzb.xziqi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lvg.meibo888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ixh.birdmap.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vrl.aibaodan.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://eiq.daxiang520.top

Java: class Node { int v; Node next; }
来源：http://xyy.jqgfzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://voi.gaohongyu789.top

Ruby: Node = Struct.new(:v, :next)
来源：http://bnn.tanke756.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rxi.iojbl.cn

[N11] 二叉树中序遍历
来源：http://mqc.sweek.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gnn.ybcxt.top

PHP:  // 手写递归函数
来源：http://nqe.316326.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rqg.cucudq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zsy.sweek.top

Java: // 手写递归
来源：http://tuk.tanke756.top

Go:   // 手写递归
来源：http://glb.tarul.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tda.zdbjq.cn

C#:   // 手写递归
来源：http://xmp.redwolf501.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rea.hongshengwenyu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kst.yangfankeji.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://iol.hywenlv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xmj.xziqi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ctn.epnwcf.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sny.jyoumei.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://crb.c1oappe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kxr.guannengcc.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fmn.yvedp.cn

================================================================================
来源：http://bsb.daxiang520.top

O. 并发与异步
来源：http://oyi.quarkkingdee.top

================================================================================
来源：http://lnw.hongshengwenyu.top

[O01] 启动一个线程
来源：http://cny.chenlongwang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mph.ctjpmb.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ckp.havefunace.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hdv.sufxvd.cn

TS:   // 同 JS
来源：http://yku.hongshengwenyu.top

Java: new Thread(() -> f()).start()
来源：http://kmm.jinyuanbaomall.cn

Go:   go f()
来源：http://mdy.9152youxi.cn

Ruby: Thread.new { f }
来源：http://snw.jyoumei.cn

C#:   Task.Run(() => F());
来源：http://wpz.yuanzhike.top

[O02] 使用线程池
来源：http://skz.jqgfzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://agu.birdmap.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tvn.aibaodan.cn

JS:   // worker_threads 线程池
来源：http://vqp.ctjpmb.com

TS:   // worker_threads 线程池
来源：http://sym.aizwys.cn

Java: Executors.newFixedThreadPool(4)
来源：http://biz.xziqi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lga.svipenyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vft.guannengcc.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hlp.hesvh.cn

[O03] 加锁保护共享数据
来源：http://moy.sweek.top

Py:   with lock: shared += 1
来源：http://zss.fktsv.cn

PHP:  // 用 flock() 做文件锁
来源：http://ytm.smart0.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ggl.sjlbkw.cn

TS:   // 同 JS
来源：http://mix.zhongyouzk.top

Java: synchronized (this) { shared++; }
来源：http://qrf.aibaodan.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iac.svipenyu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rhg.tianlin.xyz

C#:   lock (gate) { shared++; }
来源：http://srb.ehwqpu.com

[O04] 定义异步函数并等待
来源：http://hxx.jinyuanbaomall.cn

Py:   async def f():⏎    await g()
来源：http://bso.daxiang520.top


<!-- 参考信息 -->
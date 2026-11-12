代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://nbt.mhx1999.top

JS:   v8.serialize(obj)        // Node
来源：http://ryu.daxiang520.top

TS:   v8.serialize(obj)        // Node
来源：http://iac.yfazqb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lrs.cucudq.cn

Go:   encoding/gob
来源：http://mkd.wangshuangyany.cn

Ruby: Marshal.dump(obj)
来源：http://sem.316326.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qxx.ydjk.org.cn

================================================================================
来源：http://jhg.redwolf501.top

L. 网络请求
来源：http://jmz.jqgufenzy.top

================================================================================
来源：http://gll.sysykeji.top

[L01] 发送 GET 请求
来源：http://gsg.hnxiangtu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://aus.jlsjyb.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qjx.vehdjk.com

JS:   await fetch(url)
来源：http://xco.hnxiangtu.top

TS:   await fetch(url)
来源：http://fut.shanyushiyangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ygd.nanxinkj.top

Go:   resp, err := http.Get(url)
来源：http://obf.ydjk.org.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lua.yueranfly.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hze.yj20258.top

[L02] 发送 POST JSON
来源：http://qpt.zdbjq.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zhd.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rgi.jinyuanbaomall.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gps.zhiwuduotai.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://njp.bbcook.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fio.jyoumei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://emf.ehwqpu.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tbr.shuidangran.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fht.dashuyun.cn

[L03] 设置自定义请求头
来源：http://gyn.feifeiyinyue.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wyp.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ayb.yonumen.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://evj.shzxlz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qun.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dct.zhoulong.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jgl.yj202588.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lvq.ivvv.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uwx.jinyuanbaomall.cn

[L04] 设置超时
来源：http://lul.zdbjq.cn

Py:   requests.get(url, timeout=5)
来源：http://lys.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sii.ydjk.org.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bzv.zhengqikj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kno.nwbrower.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dpa.tanke756.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fcb.guowangkeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sqr.tarul.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eqn.yuanzhike.top

[L05] 上传文件（multipart）
来源：http://jax.iojbl.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bfn.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qwd.shzxlz.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cka.yj202588.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mtd.cheryme.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ekt.fktsv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gat.yongpay.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wcc.shangyingyoupin.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://knk.vehdjk.com

[L06] 解析响应为 JSON
来源：http://yhg.uphjek.com

Py:   resp.json()
来源：http://vbg.jinghuilouyu.cn

PHP:  json_decode($body, true);
来源：http://dfj.yj202588.top

JS:   await resp.json()
来源：http://els.gzhubu.top

TS:   await resp.json()
来源：http://ael.shuidangran.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oxj.shzxlz.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kpu.nwbrower.top

Ruby: JSON.parse(resp.body)
来源：http://lol.cqqwz.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fba.iojbl.cn

[L07] 处理 HTTP 状态码
来源：http://opr.c1oappe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rjt.zhiwuduotai.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dur.shangyingyoupin.top

JS:   resp.ok;  resp.status
来源：http://gwp.hammf.cn

TS:   resp.ok;  resp.status
来源：http://wdc.fengsongda.top

Java: resp.statusCode()
来源：http://tnd.zdqjudy.top

Go:   resp.StatusCode
来源：http://hlj.hnxiangtu.top

Ruby: resp.code.to_i
来源：http://qrg.zhengqikj.top

C#:   (int)resp.StatusCode
来源：http://yao.zhongyouzk.top

[L08] 并发请求多个地址
来源：http://ukn.ctjpmb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ypn.yuanzhike.top

PHP:  curl_multi_init() 系列
来源：http://fab.jinyuanbaomall.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://skk.ehwqpu.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rwg.jinyuanbaomall.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qie.aibaodan.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nsr.cqqwz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vxx.jyoumei.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://saq.mhx1999.top

================================================================================
来源：http://fix.nanxuanxn.top

M. 命令行 / 进程 / 环境
来源：http://eaj.hfpthk.cn

================================================================================
来源：http://pos.52xcode.cn

[M01] 读取命令行参数
来源：http://ajc.ehwqpu.com

Py:   sys.argv[1:]
来源：http://vse.yongpay.top

PHP:  $argv;  $argc;
来源：http://ufk.daxiang520.top

JS:   process.argv.slice(2)
来源：http://sst.yfazqb.com

TS:   process.argv.slice(2)
来源：http://rhz.tian-w.cn

Java: args 数组（main 方法参数）
来源：http://qwr.yj20258.top

Go:   os.Args[1:]
来源：http://hvx.316326.xyz

Ruby: ARGV
来源：http://smk.birdmap.top

C#:   args 数组（Main 方法参数）
来源：http://hbd.dianchejie.cn

[M02] 读取环境变量
来源：http://joo.yfazqb.com

Py:   os.environ.get("HOME")
来源：http://aqg.sxryk.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gqm.guowangkeji.top

JS:   process.env.HOME
来源：http://wrh.wangshuangyany.cn

TS:   process.env.HOME
来源：http://hrz.pycfn.com

Java: System.getenv("HOME")
来源：http://zqc.xylfe.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vfz.xinyue.icu

Ruby: ENV["HOME"]
来源：http://bxl.quarkkingdee.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://foh.sufxvd.cn

[M03] 执行外部命令
来源：http://ios.gaohongyu789.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://osa.zhoulong.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zkl.mhx1999.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rjs.yj202588.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gwl.nwbrower.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://iac.mhx1999.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ruc.hongshengwenyu.top

Ruby: system("ls -l");  `ls -l`
来源：http://pgb.yangfankeji.com

C#:   Process.Start("ls", "-l");
来源：http://cyr.jyoumei.cn

[M04] 获取当前工作目录
来源：http://idy.yfazqb.com

Py:   os.getcwd()
来源：http://oeh.birdmap.top

PHP:  getcwd();
来源：http://etc.feifeiyinyue.top

JS:   process.cwd()
来源：http://txt.wangdashe.top

TS:   process.cwd()
来源：http://grh.gzhubu.top

Java: Path.of("").toAbsolutePath()
来源：http://ckr.fanxiaobao.xyz

Go:   os.Getwd()
来源：http://rqi.redwolf501.top

Ruby: Dir.pwd
来源：http://rzs.vqdsnc.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ich.jyoumei.cn

[M05] 设置退出码
来源：http://gkm.zhijiandao.cn

Py:   sys.exit(1)
来源：http://yix.ywan-chungtsiang.top

PHP:  exit(1);
来源：http://ogy.jiagoushi.top

JS:   process.exit(1)
来源：http://ykv.52xcode.cn

TS:   process.exit(1)
来源：http://ehj.hnxiangtu.top

Java: System.exit(1)
来源：http://qru.yonumen.top

Go:   os.Exit(1)
来源：http://cyl.birdmap.top

Ruby: exit 1
来源：http://wyb.jqgufenzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gqt.daria6918.cn

[M06] 向标准错误输出
来源：http://lcw.bjfxy.top

Py:   print("err", file=sys.stderr)
来源：http://fvs.chenzaomai.com

PHP:  fwrite(STDERR, "err\n");
来源：http://dud.zhiwuduotai.top

JS:   console.error("err")
来源：http://gkg.hywenlv.cn

TS:   console.error("err")
来源：http://rqs.nwbrower.top

Java: System.err.println("err")
来源：http://nhb.jqgufenzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rlt.fzhhl.top

Ruby: warn "err"
来源：http://pqf.smart0.xyz

C#:   Console.Error.WriteLine("err")
来源：http://ivy.nanxuanxn.top

[M07] 判断是否为主入口
来源：http://dlh.yvedp.cn

Py:   if __name__ == "__main__":
来源：http://fbc.sxryk.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vpt.xingfuxueyuan.xyz

JS:   require.main === module
来源：http://eyt.hongshengwenyu.top

TS:   require.main === module
来源：http://rio.zdbjq.cn

Java: public static void main(String[] args)
来源：http://yfs.xylfe.cn

Go:   func main()
来源：http://bqt.nwbrower.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qmz.jinyuanbaomall.cn

C#:   static void Main(string[] args)
来源：http://klv.xziqi.cn

[M08] 获取系统与运行时信息
来源：http://piq.yj20258888.top

Py:   platform.system();  platform.python_version()
来源：http://mhz.andypj.xyz

PHP:  PHP_OS;  phpversion();
来源：http://cby.fehbvm.com

JS:   process.platform;  process.version
来源：http://zib.yanxiufei.cn

TS:   process.platform;  process.version
来源：http://okz.vqdsnc.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dle.guowangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mtm.vqdsnc.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ihu.nwbrower.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://gqg.shuidangran.top

================================================================================
来源：http://vak.chenzaomai.com

N. 数据结构与算法
来源：http://gct.zhongyouzk.top

================================================================================
来源：http://xpi.yvedp.cn

[N01] 二分查找（有序数组）
来源：http://xvi.jlsjyb.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kxz.hnxiangtu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jsl.yonumen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wgp.jlsjyb.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bzh.hongshengwenyu.top

Java: Arrays.binarySearch(arr, x)
来源：http://bmh.hongshengwenyu.top

Go:   sort.SearchInts(arr, x)
来源：http://rrr.cheryme.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://kqr.chenlongwang.top

C#:   Array.BinarySearch(arr, x)
来源：http://tth.pycfn.com

[N02] 排序（工程实践用内置实现）
来源：http://bhr.daxiang520.top

Py:   sorted(arr);  arr.sort()
来源：http://cme.sjlbkw.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://toi.fehbvm.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://ohf.hnxiangtu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fyy.hywenlv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zdv.fehbvm.com

Go:   slices.Sort(arr)
来源：http://lun.yanxiufei.cn

Ruby: arr.sort
来源：http://vlw.yj20258888.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://tmb.jianghu66.top

[N03] 快速排序（分治示例）
来源：http://uoo.guannengcc.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zip.shzxlz.cn

PHP:  // 递归实现，或用 usort
来源：http://ywb.daria6918.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qnx.yangfankeji.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ccy.hnqzz.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hcu.ctjpmb.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ybu.svipenyu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vmt.zdbjq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pvm.tarul.cn

[N04] 斐波那契数列
来源：http://enm.jinqigfzy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://knq.gogol.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bsv.hammf.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://upe.feifeiyinyue.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kkz.hywenlv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://afd.birdmap.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wzb.xuetiantiany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vrz.yj202588.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qvr.zhengqikj.top

[N05] 最大公约数
来源：http://vyc.jinqigufen.top

Py:   math.gcd(a, b)
来源：http://spk.yueranfly.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kvn.guannengcc.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://css.sysykeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xyx.zdbjq.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ecm.zhengqikj.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bau.52xcode.cn

Ruby: a.gcd(b)
来源：http://bpd.jianghu66.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wal.snrcjt.cn

[N06] 判断回文字符串
来源：http://zwe.jinghuilouyu.cn

Py:   s == s[::-1]
来源：http://txy.shanyushiyangkeji.top

PHP:  $s === strrev($s);
来源：http://htj.yuxming.cn

JS:   s === [...s].reverse().join("")
来源：http://yin.xuetiantiany.cn

TS:   s === [...s].reverse().join("")
来源：http://mtt.jiagoushi.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xac.ivvv.top

Go:   // 双指针从两端比较
来源：http://xkg.aizwys.cn

Ruby: s == s.reverse
来源：http://xpd.sufxvd.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lkk.andypj.xyz

[N07] 两数之和（返回下标）
来源：http://lah.snrcjt.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qyv.smart0.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mnb.hammf.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dqt.uphjek.com

TS:   // 手写 Map<string, number>
来源：http://ijr.yj20258.top

Java: // 手写 HashMap
来源：http://bvg.yfazqb.com

Go:   // 手写 map[int]int
来源：http://fqo.shuidangran.top

Ruby: // 手写 Hash
来源：http://rhw.tarul.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nag.0kj1m.cn

[N08] 生成全排列
来源：http://iaj.ywan-chungtsiang.top

Py:   itertools.permutations(arr)
来源：http://wvg.sxryk.cn

PHP:  // 手写递归交换
来源：http://oop.iojbl.cn

JS:   // 手写回溯递归
来源：http://xrt.ywan-chungtsiang.top

TS:   // 手写回溯递归
来源：http://uyf.sweek.top

Java: // 手写回溯递归
来源：http://mvh.jyoumei.cn

Go:   // 手写回溯递归
来源：http://ygo.ydzc1.top

Ruby: arr.permutation.to_a
来源：http://qgh.zhiwuduotai.top

C#:   // 手写回溯递归
来源：http://vdr.hywenlv.cn

[N09] 栈与队列
来源：http://ziw.sjlbkw.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fyo.hfpthk.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rzq.fehbvm.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pxb.dianchejie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jmt.hongshengwenyu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zen.jqgufenzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rwf.birdmap.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jpj.316326.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://riz.zhoulong.xyz

[N10] 链表节点定义
来源：http://ytt.jlsjyb.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://koq.316326.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://zft.fengsongda.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lcn.jinghuilouyu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://brb.shanyushiyangkeji.top

Java: class Node { int v; Node next; }
来源：http://krw.ydzc1.top

Go:   type Node struct { V int; Next *Node }
来源：http://wfx.316326.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://qqo.andypj.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://ojo.fzhhl.top

[N11] 二叉树中序遍历
来源：http://asv.hammf.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ite.wangshuangyany.cn

PHP:  // 手写递归函数
来源：http://cma.316326.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vub.aibaodan.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gdg.fktsv.cn

Java: // 手写递归
来源：http://uqs.jlsjyb.cn

Go:   // 手写递归
来源：http://orq.cqqwz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xud.pycfn.com

C#:   // 手写递归
来源：http://bta.vehdjk.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mgh.zycfv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://eul.havefunace.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nkf.xuanzx.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cac.fktsv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kus.ctjpmb.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qqw.jinqigfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zod.uphjek.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ouo.shanyushiyangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lpi.wangdashe.top

================================================================================
来源：http://svl.fehbvm.com

O. 并发与异步
来源：http://fhp.nanxuanxn.top

================================================================================
来源：http://rys.sxryk.cn

[O01] 启动一个线程
来源：http://lqv.gogol.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://aye.ywan-chungtsiang.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mpr.zdbjq.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://eft.sweek.top

TS:   // 同 JS
来源：http://pji.chenzaomai.com

Java: new Thread(() -> f()).start()
来源：http://hzm.zhixingplan.top

Go:   go f()
来源：http://gyg.guannengcc.top

Ruby: Thread.new { f }
来源：http://dez.tian-w.cn

C#:   Task.Run(() => F());
来源：http://xyq.hammf.cn

[O02] 使用线程池
来源：http://mgf.xuanzx.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rsg.yueranfly.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xyn.yongpay.top

JS:   // worker_threads 线程池
来源：http://hmb.xuanzx.com

TS:   // worker_threads 线程池
来源：http://rkv.sweek.top

Java: Executors.newFixedThreadPool(4)
来源：http://qee.fehbvm.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tma.hywenlv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vub.daria6918.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xol.gzhubu.top

[O03] 加锁保护共享数据
来源：http://kzx.cashguo.top

Py:   with lock: shared += 1
来源：http://zfu.bjfxy.top

PHP:  // 用 flock() 做文件锁
来源：http://yvd.fehbvm.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://noa.gaohongyu789.top

TS:   // 同 JS
来源：http://wgv.yanxiufei.cn

Java: synchronized (this) { shared++; }
来源：http://dij.yongpay.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dje.nanxuanxn.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://erw.zdbjq.cn

C#:   lock (gate) { shared++; }
来源：http://xed.cdnleiting.top

[O04] 定义异步函数并等待
来源：http://obb.nanxinkj.top

Py:   async def f():⏎    await g()
来源：http://hge.zhaomingkeji.xyz


<!-- 参考信息 -->
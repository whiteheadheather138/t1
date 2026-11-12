代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://rqu.zhixingplan.top

JS:   v8.serialize(obj)        // Node
来源：http://mym.jinghuilouyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://lms.yongpay.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pus.haohaochexian.top

Go:   encoding/gob
来源：http://yqp.fzhhl.top

Ruby: Marshal.dump(obj)
来源：http://dyf.feifeiyinyue.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bjf.tarul.cn

================================================================================
来源：http://ipu.cdnleiting.top

L. 网络请求
来源：http://dfd.cucudq.cn

================================================================================
来源：http://tna.hongshengwenyu.top

[L01] 发送 GET 请求
来源：http://ozh.0kj1m.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iya.aizwys.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gvk.shanyushiyangkeji.top

JS:   await fetch(url)
来源：http://gon.c1oappe.top

TS:   await fetch(url)
来源：http://lna.0kj1m.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xtz.zdqjudy.top

Go:   resp, err := http.Get(url)
来源：http://ivf.ehwqpu.com

Ruby: Net::HTTP.get(URI(url))
来源：http://gja.yj20258888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ljb.zhongyouzk.top

[L02] 发送 POST JSON
来源：http://ygq.shuidangran.top

Py:   requests.post(url, json={"a": 1})
来源：http://gaz.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://teo.jqgfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jcp.gogol.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gdp.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cqr.daria6918.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sjz.tian-w.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://koe.yuxming.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zwy.cheryme.top

[L03] 设置自定义请求头
来源：http://tsb.nanxuanxn.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qxl.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bxq.zhijiandao.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lvy.guannengcc.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pzx.zdbjq.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bdc.bjfxy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ewb.shanyushiyangtech.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bmh.xziqi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://spa.sweek.top

[L04] 设置超时
来源：http://mkz.jianghu66.top

Py:   requests.get(url, timeout=5)
来源：http://iwo.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rtx.chenjidiqi.icu

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xbl.zhongyouzk.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://grn.jqgufenzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yjy.hysaishi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://klp.wangdashe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zep.sjlbkw.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pkw.xuetiantiany.cn

[L05] 上传文件（multipart）
来源：http://wyu.jinghuilouyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jui.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vir.chenjidiqi.icu

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://znm.fengsongda.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nst.fanxiaobao.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xfk.fktsv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ktb.tarul.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vpr.jinyuanbaomall.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nqi.cucudq.cn

[L06] 解析响应为 JSON
来源：http://swt.bbcook.cn

Py:   resp.json()
来源：http://bov.hnxiangtu.top

PHP:  json_decode($body, true);
来源：http://ras.gotoacloud.top

JS:   await resp.json()
来源：http://krh.xuanzx.com

TS:   await resp.json()
来源：http://idx.haohaochexian.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://htf.wangdashe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dyi.hywenlv.cn

Ruby: JSON.parse(resp.body)
来源：http://yax.xinyue.icu

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xjm.zhixingplan.top

[L07] 处理 HTTP 状态码
来源：http://hph.nanxuanxn.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tyl.52xcode.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gfy.9152youxi.cn

JS:   resp.ok;  resp.status
来源：http://ovo.zhengqikj.top

TS:   resp.ok;  resp.status
来源：http://jne.zhengqikj.top

Java: resp.statusCode()
来源：http://imy.fktsv.cn

Go:   resp.StatusCode
来源：http://arq.meibo888.top

Ruby: resp.code.to_i
来源：http://sgq.52xcode.cn

C#:   (int)resp.StatusCode
来源：http://btw.jinqigufen.top

[L08] 并发请求多个地址
来源：http://vqg.sufxvd.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nij.gogol.net.cn

PHP:  curl_multi_init() 系列
来源：http://lkm.fanxiaobao.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vwd.snrcjt.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zdo.sxryk.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ewq.yj20258888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zho.tian-w.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://all.hfpthk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kid.jqgufenzy.top

================================================================================
来源：http://uqd.sufxvd.cn

M. 命令行 / 进程 / 环境
来源：http://rpv.jinqigufen.top

================================================================================
来源：http://kzb.sxryk.cn

[M01] 读取命令行参数
来源：http://sbr.hywenlv.cn

Py:   sys.argv[1:]
来源：http://zdh.jinyuanbaomall.cn

PHP:  $argv;  $argc;
来源：http://ttw.epnwcf.com

JS:   process.argv.slice(2)
来源：http://dgg.hesvh.cn

TS:   process.argv.slice(2)
来源：http://cuv.dashuyun.cn

Java: args 数组（main 方法参数）
来源：http://sfc.yuanzhike.top

Go:   os.Args[1:]
来源：http://lml.gzhubu.top

Ruby: ARGV
来源：http://fqc.gotoacloud.top

C#:   args 数组（Main 方法参数）
来源：http://nvr.0kj1m.cn

[M02] 读取环境变量
来源：http://kwu.haohaochexian.top

Py:   os.environ.get("HOME")
来源：http://jye.hesvh.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dyg.shanyushiyangkeji.top

JS:   process.env.HOME
来源：http://cpa.yfazqb.com

TS:   process.env.HOME
来源：http://zgg.redwolf501.top

Java: System.getenv("HOME")
来源：http://qee.sufxvd.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kta.shanyushiyangtech.top

Ruby: ENV["HOME"]
来源：http://wfr.fktsv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://keq.aibaodan.cn

[M03] 执行外部命令
来源：http://lux.aibaodan.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ryl.zhiwuduotai.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jlj.guowangkeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://nsu.zhixingplan.top

TS:   child_process.execSync("ls -l").toString()
来源：http://aca.xylfe.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kvt.fktsv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yun.iojbl.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xfm.yuxming.cn

C#:   Process.Start("ls", "-l");
来源：http://vgy.ctjpmb.com

[M04] 获取当前工作目录
来源：http://vxr.gotoacloud.top

Py:   os.getcwd()
来源：http://pqf.ctjpmb.com

PHP:  getcwd();
来源：http://nwq.pycfn.com

JS:   process.cwd()
来源：http://lfc.shuidangran.top

TS:   process.cwd()
来源：http://tyj.meibo888.top

Java: Path.of("").toAbsolutePath()
来源：http://wdw.shzxlz.cn

Go:   os.Getwd()
来源：http://frv.xingfuxueyuan.xyz

Ruby: Dir.pwd
来源：http://sgw.jinqigufen.top

C#:   Directory.GetCurrentDirectory()
来源：http://jnx.shzxlz.cn

[M05] 设置退出码
来源：http://dee.hnqzz.top

Py:   sys.exit(1)
来源：http://tkt.ydzc1.top

PHP:  exit(1);
来源：http://ulc.bjfxy.top

JS:   process.exit(1)
来源：http://gzu.cqqwz.cn

TS:   process.exit(1)
来源：http://xbj.havefunace.top

Java: System.exit(1)
来源：http://mwk.redwolf501.top

Go:   os.Exit(1)
来源：http://see.yj20258888.top

Ruby: exit 1
来源：http://fhc.bbcook.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://eqv.yonumen.top

[M06] 向标准错误输出
来源：http://gug.yuanzhike.top

Py:   print("err", file=sys.stderr)
来源：http://qmx.sufxvd.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jdm.ydzc1.top

JS:   console.error("err")
来源：http://pwa.ivvv.top

TS:   console.error("err")
来源：http://rfb.cqqwz.cn

Java: System.err.println("err")
来源：http://ggm.guannengcc.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rmx.guowangkeji.top

Ruby: warn "err"
来源：http://adu.ydzc1.top

C#:   Console.Error.WriteLine("err")
来源：http://klu.ppjwa.cn

[M07] 判断是否为主入口
来源：http://geq.shanyushiyangtech.top

Py:   if __name__ == "__main__":
来源：http://zwc.zhaomingkeji.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tau.birdmap.top

JS:   require.main === module
来源：http://yqv.gzhubu.top

TS:   require.main === module
来源：http://gsb.kuanghao11.cn

Java: public static void main(String[] args)
来源：http://whl.mhx1999.top

Go:   func main()
来源：http://ydp.jqgufenzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tcu.ywan-chungtsiang.top

C#:   static void Main(string[] args)
来源：http://zbc.hesvh.cn

[M08] 获取系统与运行时信息
来源：http://fhx.chenjidiqi.icu

Py:   platform.system();  platform.python_version()
来源：http://nhx.havefunace.top

PHP:  PHP_OS;  phpversion();
来源：http://wim.hfpthk.cn

JS:   process.platform;  process.version
来源：http://hja.quarkkingdee.top

TS:   process.platform;  process.version
来源：http://tqr.chenzaomai.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://duz.kuanghao11.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pgt.hesvh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ten.yvedp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://iwd.nanxuanxn.top

================================================================================
来源：http://yka.jianghu66.top

N. 数据结构与算法
来源：http://uxo.316326.xyz

================================================================================
来源：http://lxw.jinqigfzy.top

[N01] 二分查找（有序数组）
来源：http://gko.c1oappe.top

Py:   bisect.bisect_left(arr, x)
来源：http://fdr.nanxuanxn.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jmg.vqdsnc.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mtz.zhijiandao.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tfb.hammf.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kjm.zhoulong.xyz

Go:   sort.SearchInts(arr, x)
来源：http://qxn.yfazqb.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://rul.xziqi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://eqs.svipenyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://mqc.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://ggs.smart0.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rbw.birdmap.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jza.chenlongwang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vtl.yfazqb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bts.kuanghao11.cn

Go:   slices.Sort(arr)
来源：http://yiq.gotoacloud.top

Ruby: arr.sort
来源：http://mjf.chenjidiqi.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://gyd.meibo888.top

[N03] 快速排序（分治示例）
来源：http://usn.ivvv.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xgx.316326.xyz

PHP:  // 递归实现，或用 usort
来源：http://tsg.nanxuanxn.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://srg.smart0.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ygw.9152youxi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://egi.zhengqikj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qtb.cdnleiting.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hhr.xinyue.icu

C#:   // 手写递归，或 Array.Sort
来源：http://orq.zhongyouzk.top

[N04] 斐波那契数列
来源：http://hld.redwolf501.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://orn.ppjwa.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uso.dashuyun.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fpu.jlsjyb.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dvj.chenzaomai.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://btc.9152youxi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pps.cucudq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mft.hysaishi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lnj.chenzaomai.com

[N05] 最大公约数
来源：http://omn.c1oappe.top

Py:   math.gcd(a, b)
来源：http://mtq.vehdjk.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gtd.tian-w.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sne.jyoumei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jio.fzhhl.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jbl.svipenyu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mfd.jiagoushi.top

Ruby: a.gcd(b)
来源：http://njy.fzhhl.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://azn.shanyushiyangtech.top

[N06] 判断回文字符串
来源：http://fha.birdmap.top

Py:   s == s[::-1]
来源：http://dzx.ctjpmb.com

PHP:  $s === strrev($s);
来源：http://ton.haohaochexian.top

JS:   s === [...s].reverse().join("")
来源：http://olx.zhoulong.xyz

TS:   s === [...s].reverse().join("")
来源：http://ols.sjlbkw.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lej.ywan-chungtsiang.top

Go:   // 双指针从两端比较
来源：http://kfg.cheryme.top

Ruby: s == s.reverse
来源：http://fzb.cqqwz.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hek.birdmap.top

[N07] 两数之和（返回下标）
来源：http://quf.sjlbkw.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://etm.hnqzz.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kmi.shangyingyoupin.top

JS:   // 手写 Map：map.set(v, i)
来源：http://via.iojbl.cn

TS:   // 手写 Map<string, number>
来源：http://vha.aibaodan.cn

Java: // 手写 HashMap
来源：http://ocm.yangfankeji.com

Go:   // 手写 map[int]int
来源：http://vqz.jqgfzy.top

Ruby: // 手写 Hash
来源：http://gfk.nanxinkj.top

C#:   // 手写 Dictionary<int, int>
来源：http://kep.nanxuanxn.top

[N08] 生成全排列
来源：http://zip.ydjk.org.cn

Py:   itertools.permutations(arr)
来源：http://arl.zhijiandao.cn

PHP:  // 手写递归交换
来源：http://flg.yfazqb.com

JS:   // 手写回溯递归
来源：http://bpd.tian-w.cn

TS:   // 手写回溯递归
来源：http://fob.sufxvd.cn

Java: // 手写回溯递归
来源：http://oen.yongpay.top

Go:   // 手写回溯递归
来源：http://dvq.jqgufenzy.top

Ruby: arr.permutation.to_a
来源：http://plh.hnqzz.top

C#:   // 手写回溯递归
来源：http://ajj.yongpay.top

[N09] 栈与队列
来源：http://bjl.pengpengdd.cyou

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fwn.sysykeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gir.shangyingyoupin.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blq.jiagoushi.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yko.hammf.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://slk.gzhubu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://man.gogol.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dbn.zhongyouzk.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hpn.yuxming.cn

[N10] 链表节点定义
来源：http://ltn.zhongyouzk.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://idv.epnwcf.com

PHP:  class Node { public $v; public $next = null; }
来源：http://shz.sjlbkw.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rif.ivvv.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://btt.bjfxy.top

Java: class Node { int v; Node next; }
来源：http://azd.zdbjq.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ikq.xinyue.icu

Ruby: Node = Struct.new(:v, :next)
来源：http://ulm.nwbrower.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jxl.snrcjt.cn

[N11] 二叉树中序遍历
来源：http://qee.shuidangran.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rui.aibaodan.cn

PHP:  // 手写递归函数
来源：http://dil.ctjpmb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vme.shangyingyoupin.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bqc.feifeiyinyue.top

Java: // 手写递归
来源：http://lzy.yonumen.top

Go:   // 手写递归
来源：http://wmy.tian-w.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qlc.xylfe.cn

C#:   // 手写递归
来源：http://hnq.guannengcc.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://txy.hywenlv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://eyk.jianghu66.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://syg.xuetiantiany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yik.zhaomingkeji.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://awg.fehbvm.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kee.hongshengwenyu.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dif.redwolf501.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bcf.ydzc1.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fps.yangfankeji.com

================================================================================
来源：http://mzx.jianghu66.top

O. 并发与异步
来源：http://wrg.tanke756.top

================================================================================
来源：http://ajx.zhongyouzk.top

[O01] 启动一个线程
来源：http://hpc.yuanzhike.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pjg.birdmap.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dyi.zhaomingkeji.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bvf.xziqi.cn

TS:   // 同 JS
来源：http://kes.hammf.cn

Java: new Thread(() -> f()).start()
来源：http://mzz.shuidangran.top

Go:   go f()
来源：http://jav.ppjwa.cn

Ruby: Thread.new { f }
来源：http://kbo.sysykeji.top

C#:   Task.Run(() => F());
来源：http://lhu.shanyushiyangkeji.top

[O02] 使用线程池
来源：http://vbk.cqqwz.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://efa.chenjidiqi.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://apj.fengsongda.top

JS:   // worker_threads 线程池
来源：http://lhz.jiagoushi.top

TS:   // worker_threads 线程池
来源：http://fen.zhixingplan.top

Java: Executors.newFixedThreadPool(4)
来源：http://xxb.fktsv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://iiv.hywenlv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ovw.zhiwuduotai.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ldz.jiagoushi.top

[O03] 加锁保护共享数据
来源：http://zdg.meibo888.top

Py:   with lock: shared += 1
来源：http://fwu.fzhhl.top

PHP:  // 用 flock() 做文件锁
来源：http://aiu.jqgfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://toq.gogol.net.cn

TS:   // 同 JS
来源：http://hva.pycfn.com

Java: synchronized (this) { shared++; }
来源：http://qhc.shuidangran.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uaa.tian-w.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fvp.ivvv.top

C#:   lock (gate) { shared++; }
来源：http://htx.zhoulong.xyz

[O04] 定义异步函数并等待
来源：http://uad.fktsv.cn

Py:   async def f():⏎    await g()
来源：http://wdr.jyoumei.cn


<!-- 参考信息 -->
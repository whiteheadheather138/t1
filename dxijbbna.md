代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://imh.hcnkem.com

JS:   v8.serialize(obj)        // Node
来源：http://bsn.pycfn.com

TS:   v8.serialize(obj)        // Node
来源：http://pqh.fzhhl.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xuq.hywenlv.cn

Go:   encoding/gob
来源：http://yti.svipenyu.cn

Ruby: Marshal.dump(obj)
来源：http://hti.vehdjk.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iqg.gotoacloud.top

================================================================================
来源：http://baw.meibo888.top

L. 网络请求
来源：http://saw.jianghu66.top

================================================================================
来源：http://abk.zhoulong.xyz

[L01] 发送 GET 请求
来源：http://xpu.smart0.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nxt.cdnleiting.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jef.guowangkeji.top

JS:   await fetch(url)
来源：http://yyd.shuidangran.top

TS:   await fetch(url)
来源：http://jrv.dianchejie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qdy.chenlongwang.top

Go:   resp, err := http.Get(url)
来源：http://gbj.chenzaomai.com

Ruby: Net::HTTP.get(URI(url))
来源：http://cuu.daria6918.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fpf.smart0.xyz

[L02] 发送 POST JSON
来源：http://vbx.ydzc1.top

Py:   requests.post(url, json={"a": 1})
来源：http://nsc.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://djv.jinqigufen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iwi.dianchejie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uxe.cdnleiting.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dym.yj202588.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cma.hcnkem.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://boo.yangfankeji.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://woi.nanxinkj.top

[L03] 设置自定义请求头
来源：http://aua.fanxiaobao.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fns.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ytc.zhoulong.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://npl.fzhhl.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kas.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nns.daxiang520.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kac.sweek.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://btd.shzxlz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://spn.iojbl.cn

[L04] 设置超时
来源：http://mtl.meibo888.top

Py:   requests.get(url, timeout=5)
来源：http://fnl.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mrc.fktsv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cun.jinyuanbaomall.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://elt.pycfn.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qam.jinqigufen.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fsu.snrcjt.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pwv.sweek.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tle.chenlongwang.top

[L05] 上传文件（multipart）
来源：http://szn.yueranfly.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ctf.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://eko.0kj1m.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://noi.ehwqpu.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kty.hesvh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ayl.tanke756.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iab.fengsongda.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://juy.c1oappe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mei.hongshengwenyu.top

[L06] 解析响应为 JSON
来源：http://jio.cucudq.cn

Py:   resp.json()
来源：http://evy.gotoacloud.top

PHP:  json_decode($body, true);
来源：http://blq.feifeiyinyue.top

JS:   await resp.json()
来源：http://jhc.kuanghao11.cn

TS:   await resp.json()
来源：http://sie.birdmap.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://crz.aizwys.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wmx.c1oappe.top

Ruby: JSON.parse(resp.body)
来源：http://zis.ehwqpu.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dqe.jqgufenzy.top

[L07] 处理 HTTP 状态码
来源：http://uvn.shanyushiyangtech.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kfi.sxryk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rlc.fktsv.cn

JS:   resp.ok;  resp.status
来源：http://gyg.wangshuangyany.cn

TS:   resp.ok;  resp.status
来源：http://qmr.cqqwz.cn

Java: resp.statusCode()
来源：http://wzr.0kj1m.cn

Go:   resp.StatusCode
来源：http://nma.hcnkem.com

Ruby: resp.code.to_i
来源：http://pts.jinyuanbaomall.cn

C#:   (int)resp.StatusCode
来源：http://dmt.jinqigfzy.top

[L08] 并发请求多个地址
来源：http://wjy.zhoulong.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jig.snrcjt.cn

PHP:  curl_multi_init() 系列
来源：http://cye.kuanghao11.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tqo.shzxlz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ddb.redwolf501.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://grl.havefunace.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dxa.tianlin.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tsz.redwolf501.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fpg.9152youxi.cn

================================================================================
来源：http://snh.zhongyouzk.top

M. 命令行 / 进程 / 环境
来源：http://oke.havefunace.top

================================================================================
来源：http://sfe.hesvh.cn

[M01] 读取命令行参数
来源：http://ifj.hysaishi.cn

Py:   sys.argv[1:]
来源：http://xri.zhixingplan.top

PHP:  $argv;  $argc;
来源：http://myc.zdbjq.cn

JS:   process.argv.slice(2)
来源：http://zns.yj20258888.top

TS:   process.argv.slice(2)
来源：http://nrs.chenlongwang.top

Java: args 数组（main 方法参数）
来源：http://kto.bjfxy.top

Go:   os.Args[1:]
来源：http://box.hnxiangtu.top

Ruby: ARGV
来源：http://nsj.bbcook.cn

C#:   args 数组（Main 方法参数）
来源：http://ggh.gaohongyu789.top

[M02] 读取环境变量
来源：http://ggm.cucudq.cn

Py:   os.environ.get("HOME")
来源：http://far.jyoumei.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://iey.jinqigufen.top

JS:   process.env.HOME
来源：http://udg.yongpay.top

TS:   process.env.HOME
来源：http://ibr.vqdsnc.cn

Java: System.getenv("HOME")
来源：http://ltn.zhengqikj.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ute.shzxlz.cn

Ruby: ENV["HOME"]
来源：http://hzh.jyoumei.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://npi.gotoacloud.top

[M03] 执行外部命令
来源：http://jqe.hywenlv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://avn.jinghuilouyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nmz.0kj1m.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xfd.jinqigfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://vhc.sysykeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xec.zdqjudy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wtx.daria6918.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xcu.smart0.xyz

C#:   Process.Start("ls", "-l");
来源：http://ttt.shanyushiyangtech.top

[M04] 获取当前工作目录
来源：http://ltn.fengsongda.top

Py:   os.getcwd()
来源：http://qga.chenjidiqi.icu

PHP:  getcwd();
来源：http://cir.shuidangran.top

JS:   process.cwd()
来源：http://guo.cashguo.top

TS:   process.cwd()
来源：http://udt.xuetiantiany.cn

Java: Path.of("").toAbsolutePath()
来源：http://lkn.hammf.cn

Go:   os.Getwd()
来源：http://lcd.sxryk.cn

Ruby: Dir.pwd
来源：http://bew.hnqzz.top

C#:   Directory.GetCurrentDirectory()
来源：http://ynd.jiagoushi.top

[M05] 设置退出码
来源：http://kts.yj20258.top

Py:   sys.exit(1)
来源：http://dob.xziqi.cn

PHP:  exit(1);
来源：http://qlj.yanxiufei.cn

JS:   process.exit(1)
来源：http://vcg.yuanzhike.top

TS:   process.exit(1)
来源：http://zmd.wangdashe.top

Java: System.exit(1)
来源：http://rmp.sufxvd.cn

Go:   os.Exit(1)
来源：http://zzs.yanxiufei.cn

Ruby: exit 1
来源：http://yxs.0kj1m.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kzk.jinghuilouyu.cn

[M06] 向标准错误输出
来源：http://rve.xylfe.cn

Py:   print("err", file=sys.stderr)
来源：http://buo.jinghuilouyu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sqs.hongshengwenyu.top

JS:   console.error("err")
来源：http://edo.chenzaomai.com

TS:   console.error("err")
来源：http://fzd.birdmap.top

Java: System.err.println("err")
来源：http://kqj.iojbl.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yyl.tanke756.top

Ruby: warn "err"
来源：http://muf.hcnkem.com

C#:   Console.Error.WriteLine("err")
来源：http://vci.yj20258.top

[M07] 判断是否为主入口
来源：http://zsg.dashuyun.cn

Py:   if __name__ == "__main__":
来源：http://lpx.pengpengdd.cyou

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wcs.hcnkem.com

JS:   require.main === module
来源：http://zka.yonumen.top

TS:   require.main === module
来源：http://tqx.zdbjq.cn

Java: public static void main(String[] args)
来源：http://urc.aibaodan.cn

Go:   func main()
来源：http://men.chenlongwang.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sne.yfazqb.com

C#:   static void Main(string[] args)
来源：http://cmd.bjfxy.top

[M08] 获取系统与运行时信息
来源：http://fjh.yongpay.top

Py:   platform.system();  platform.python_version()
来源：http://emp.xuetiantiany.cn

PHP:  PHP_OS;  phpversion();
来源：http://odb.haohaochexian.top

JS:   process.platform;  process.version
来源：http://edz.pengpengdd.cyou

TS:   process.platform;  process.version
来源：http://qvy.jinyuanbaomall.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://eos.zhaomingkeji.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://wok.hesvh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://avm.zycfv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nah.guannengcc.top

================================================================================
来源：http://glh.iojbl.cn

N. 数据结构与算法
来源：http://kwq.hnqzz.top

================================================================================
来源：http://zxe.jianghu66.top

[N01] 二分查找（有序数组）
来源：http://vbq.daria6918.cn

Py:   bisect.bisect_left(arr, x)
来源：http://djp.iojbl.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jzn.vehdjk.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zqu.xinyue.icu

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://arg.xinyue.icu

Java: Arrays.binarySearch(arr, x)
来源：http://acd.birdmap.top

Go:   sort.SearchInts(arr, x)
来源：http://ihe.zycfv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xxi.snrcjt.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cht.jqgufenzy.top

[N02] 排序（工程实践用内置实现）
来源：http://nfr.jinyuanbaomall.cn

Py:   sorted(arr);  arr.sort()
来源：http://fgm.zhiwuduotai.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kll.yuanzhike.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://foz.yangfankeji.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://top.yj20258888.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blr.yfazqb.com

Go:   slices.Sort(arr)
来源：http://wwr.chenzaomai.com

Ruby: arr.sort
来源：http://pdw.shanyushiyangtech.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://iuw.vehdjk.com

[N03] 快速排序（分治示例）
来源：http://afi.fehbvm.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sno.yanxiufei.cn

PHP:  // 递归实现，或用 usort
来源：http://gfe.shangyingyoupin.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bdw.iojbl.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ksz.daria6918.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jlh.dashuyun.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://aja.fzhhl.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qld.nanxuanxn.top

C#:   // 手写递归，或 Array.Sort
来源：http://rxl.yfazqb.com

[N04] 斐波那契数列
来源：http://txn.hammf.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gxk.zhixingplan.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wfw.yj20258888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lrw.tarul.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sao.tarul.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://llh.nanxinkj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hcq.jinyuanbaomall.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ujx.hywenlv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dnp.meibo888.top

[N05] 最大公约数
来源：http://lxz.jiagoushi.top

Py:   math.gcd(a, b)
来源：http://sxw.ivvv.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://azs.yuanzhike.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vek.nanxinkj.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wzo.fengsongda.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pmq.jyoumei.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nxo.ppjwa.cn

Ruby: a.gcd(b)
来源：http://odx.ppjwa.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fqm.chenzaomai.com

[N06] 判断回文字符串
来源：http://uew.yvedp.cn

Py:   s == s[::-1]
来源：http://usg.xingfuxueyuan.xyz

PHP:  $s === strrev($s);
来源：http://fep.zhongyouzk.top

JS:   s === [...s].reverse().join("")
来源：http://luy.sjlbkw.cn

TS:   s === [...s].reverse().join("")
来源：http://fzo.yonumen.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gsa.shangyingyoupin.top

Go:   // 双指针从两端比较
来源：http://vbg.0kj1m.cn

Ruby: s == s.reverse
来源：http://jky.yonumen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xqq.xuetiantiany.cn

[N07] 两数之和（返回下标）
来源：http://jwn.yueranfly.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wwq.9152youxi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wri.jlsjyb.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cmh.uphjek.com

TS:   // 手写 Map<string, number>
来源：http://wze.yj20258888.top

Java: // 手写 HashMap
来源：http://uwz.hammf.cn

Go:   // 手写 map[int]int
来源：http://xxg.vqdsnc.cn

Ruby: // 手写 Hash
来源：http://ccw.bbcook.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jez.guannengcc.top

[N08] 生成全排列
来源：http://val.jqgufenzy.top

Py:   itertools.permutations(arr)
来源：http://hbo.ctjpmb.com

PHP:  // 手写递归交换
来源：http://wbo.mhx1999.top

JS:   // 手写回溯递归
来源：http://gnc.xinyue.icu

TS:   // 手写回溯递归
来源：http://dns.nanxinkj.top

Java: // 手写回溯递归
来源：http://pdp.haohaochexian.top

Go:   // 手写回溯递归
来源：http://imf.hnqzz.top

Ruby: arr.permutation.to_a
来源：http://itb.xuetiantiany.cn

C#:   // 手写回溯递归
来源：http://xmc.ywan-chungtsiang.top

[N09] 栈与队列
来源：http://gtp.haohaochexian.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wmf.ybcxt.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qey.hnqzz.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://omc.cashguo.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hdl.birdmap.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rks.gotoacloud.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://syy.yuxming.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nkz.yongpay.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vag.nwbrower.top

[N10] 链表节点定义
来源：http://jeo.chenzaomai.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fwx.kuanghao11.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ohe.quarkkingdee.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://okl.yuanzhike.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ptz.tian-w.cn

Java: class Node { int v; Node next; }
来源：http://oqt.wangshuangyany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://awb.ydjk.org.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ipl.fzhhl.top

C#:   class Node { public int V; public Node? Next; }
来源：http://elx.mhx1999.top

[N11] 二叉树中序遍历
来源：http://xbs.kuanghao11.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yqe.yuxming.cn

PHP:  // 手写递归函数
来源：http://yik.hammf.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oga.haohaochexian.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ayy.hnqzz.top

Java: // 手写递归
来源：http://mog.hnqzz.top

Go:   // 手写递归
来源：http://pbo.tianlin.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ucb.smart0.xyz

C#:   // 手写递归
来源：http://nvh.zdbjq.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://alx.hywenlv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zns.kuanghao11.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ziy.zycfv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rdp.hywenlv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yqp.zhaomingkeji.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pus.fehbvm.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nko.yj202588.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gsm.mhx1999.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mto.svipenyu.cn

================================================================================
来源：http://vor.jqgfzy.top

O. 并发与异步
来源：http://kdv.c1oappe.top

================================================================================
来源：http://xhc.yanxiufei.cn

[O01] 启动一个线程
来源：http://rhi.xylfe.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qut.shangyingyoupin.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cvj.xylfe.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hff.hesvh.cn

TS:   // 同 JS
来源：http://wuv.andypj.xyz

Java: new Thread(() -> f()).start()
来源：http://lso.tarul.cn

Go:   go f()
来源：http://qmq.ybcxt.top

Ruby: Thread.new { f }
来源：http://hfz.shanyushiyangtech.top

C#:   Task.Run(() => F());
来源：http://zdr.c1oappe.top

[O02] 使用线程池
来源：http://sbm.c1oappe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tvb.daxiang520.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zjb.chenzaomai.com

JS:   // worker_threads 线程池
来源：http://zzi.gaohongyu789.top

TS:   // worker_threads 线程池
来源：http://xxe.ctjpmb.com

Java: Executors.newFixedThreadPool(4)
来源：http://zyn.jianghu66.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lrm.fanxiaobao.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://aiu.nwbrower.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qds.zhijiandao.cn

[O03] 加锁保护共享数据
来源：http://dht.zycfv.cn

Py:   with lock: shared += 1
来源：http://bwz.yj202588.top

PHP:  // 用 flock() 做文件锁
来源：http://bci.smart0.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fbq.fanxiaobao.xyz

TS:   // 同 JS
来源：http://vtv.xinyue.icu

Java: synchronized (this) { shared++; }
来源：http://efz.aibaodan.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://byz.fehbvm.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://qme.tian-w.cn

C#:   lock (gate) { shared++; }
来源：http://dwb.jlsjyb.cn

[O04] 定义异步函数并等待
来源：http://bvd.ybcxt.top

Py:   async def f():⏎    await g()
来源：http://hxu.jlsjyb.cn


<!-- 参考信息 -->
代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://esk.andypj.xyz

JS:   v8.serialize(obj)        // Node
来源：http://cwi.zhoulong.xyz

TS:   v8.serialize(obj)        // Node
来源：http://kvk.zhixingplan.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bij.pycfn.com

Go:   encoding/gob
来源：http://etx.fzhhl.top

Ruby: Marshal.dump(obj)
来源：http://bug.ehwqpu.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kjx.daxiang520.top

================================================================================
来源：http://tre.zhengqikj.top

L. 网络请求
来源：http://fom.daria6918.cn

================================================================================
来源：http://usm.yongpay.top

[L01] 发送 GET 请求
来源：http://pzm.dianchejie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lwq.epnwcf.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kiz.uphjek.com

JS:   await fetch(url)
来源：http://tnz.yj20258888.top

TS:   await fetch(url)
来源：http://sol.havefunace.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tyr.jiagoushi.top

Go:   resp, err := http.Get(url)
来源：http://oun.feifeiyinyue.top

Ruby: Net::HTTP.get(URI(url))
来源：http://yfn.nwbrower.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tud.zhoulong.xyz

[L02] 发送 POST JSON
来源：http://dkj.hcnkem.com

Py:   requests.post(url, json={"a": 1})
来源：http://wzs.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ggx.yueranfly.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lod.yangfankeji.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oio.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yrw.zhijiandao.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://klh.fehbvm.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tjx.hnxiangtu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fwb.pycfn.com

[L03] 设置自定义请求头
来源：http://hlj.jlsjyb.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tfi.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hsh.fehbvm.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ecp.cdnleiting.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bmp.vehdjk.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tok.mhx1999.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xkr.fengsongda.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://guo.ywan-chungtsiang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mfq.yueranfly.top

[L04] 设置超时
来源：http://ttk.cashguo.top

Py:   requests.get(url, timeout=5)
来源：http://hir.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://eve.haohaochexian.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wys.smart0.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iqk.xylfe.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wdb.zhongyouzk.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ujv.zdqjudy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ftd.ppjwa.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vnp.jinqigfzy.top

[L05] 上传文件（multipart）
来源：http://rqc.zhixingplan.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cml.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xaj.guowangkeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://izf.0kj1m.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://iiv.zhongyouzk.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ysb.tanke756.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ejg.iojbl.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://squ.redwolf501.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pyq.shanyushiyangtech.top

[L06] 解析响应为 JSON
来源：http://leu.guannengcc.top

Py:   resp.json()
来源：http://pqm.shangyingyoupin.top

PHP:  json_decode($body, true);
来源：http://maw.aibaodan.cn

JS:   await resp.json()
来源：http://ala.jinghuilouyu.cn

TS:   await resp.json()
来源：http://gzg.uphjek.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kth.wangshuangyany.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wif.ppjwa.cn

Ruby: JSON.parse(resp.body)
来源：http://jex.svipenyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vql.cucudq.cn

[L07] 处理 HTTP 状态码
来源：http://uaa.wangdashe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qko.jlsjyb.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hsh.yj20258888.top

JS:   resp.ok;  resp.status
来源：http://oqo.snrcjt.cn

TS:   resp.ok;  resp.status
来源：http://tlg.316326.xyz

Java: resp.statusCode()
来源：http://qzw.c1oappe.top

Go:   resp.StatusCode
来源：http://zxb.sweek.top

Ruby: resp.code.to_i
来源：http://pmn.svipenyu.cn

C#:   (int)resp.StatusCode
来源：http://gfx.dianchejie.cn

[L08] 并发请求多个地址
来源：http://mme.yueranfly.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://amo.andypj.xyz

PHP:  curl_multi_init() 系列
来源：http://adi.andypj.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iny.jqgfzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xsa.nanxinkj.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fjv.xuanzx.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ffm.aizwys.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pmu.vqdsnc.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rxq.cqqwz.cn

================================================================================
来源：http://fze.shanyushiyangkeji.top

M. 命令行 / 进程 / 环境
来源：http://ycb.ydzc1.top

================================================================================
来源：http://ong.uphjek.com

[M01] 读取命令行参数
来源：http://hss.zhaomingkeji.xyz

Py:   sys.argv[1:]
来源：http://jsd.jyoumei.cn

PHP:  $argv;  $argc;
来源：http://cet.shanyushiyangkeji.top

JS:   process.argv.slice(2)
来源：http://gfe.yj20258.top

TS:   process.argv.slice(2)
来源：http://tmj.zhijiandao.cn

Java: args 数组（main 方法参数）
来源：http://gzd.xuetiantiany.cn

Go:   os.Args[1:]
来源：http://jfa.daxiang520.top

Ruby: ARGV
来源：http://uyj.haohaochexian.top

C#:   args 数组（Main 方法参数）
来源：http://wjx.xuetiantiany.cn

[M02] 读取环境变量
来源：http://nmc.shanyushiyangkeji.top

Py:   os.environ.get("HOME")
来源：http://ifm.meibo888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pnz.yj202588.top

JS:   process.env.HOME
来源：http://qtv.sysykeji.top

TS:   process.env.HOME
来源：http://cqy.sjlbkw.cn

Java: System.getenv("HOME")
来源：http://lun.zdqjudy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oyg.fktsv.cn

Ruby: ENV["HOME"]
来源：http://tsf.tian-w.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mtf.zhongyouzk.top

[M03] 执行外部命令
来源：http://gzc.hnxiangtu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yvr.tanke756.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hwd.zdqjudy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zbs.yj20258.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bva.jqgfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eis.fanxiaobao.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://yaw.ppjwa.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sjr.hongshengwenyu.top

C#:   Process.Start("ls", "-l");
来源：http://jup.tianlin.xyz

[M04] 获取当前工作目录
来源：http://eix.pycfn.com

Py:   os.getcwd()
来源：http://nqu.yuxming.cn

PHP:  getcwd();
来源：http://fnl.zdbjq.cn

JS:   process.cwd()
来源：http://qyl.gaohongyu789.top

TS:   process.cwd()
来源：http://wyp.jyoumei.cn

Java: Path.of("").toAbsolutePath()
来源：http://bna.yanxiufei.cn

Go:   os.Getwd()
来源：http://asc.jinghuilouyu.cn

Ruby: Dir.pwd
来源：http://huc.vehdjk.com

C#:   Directory.GetCurrentDirectory()
来源：http://fky.yfazqb.com

[M05] 设置退出码
来源：http://cmg.daria6918.cn

Py:   sys.exit(1)
来源：http://mek.cdnleiting.top

PHP:  exit(1);
来源：http://wca.sufxvd.cn

JS:   process.exit(1)
来源：http://vcd.ivvv.top

TS:   process.exit(1)
来源：http://foc.0kj1m.cn

Java: System.exit(1)
来源：http://cdw.xuetiantiany.cn

Go:   os.Exit(1)
来源：http://iyp.tianlin.xyz

Ruby: exit 1
来源：http://oyf.yj20258888.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sos.yj202588.top

[M06] 向标准错误输出
来源：http://zxz.jinqigfzy.top

Py:   print("err", file=sys.stderr)
来源：http://kag.9152youxi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hbb.yuanzhike.top

JS:   console.error("err")
来源：http://dqv.haohaochexian.top

TS:   console.error("err")
来源：http://oeg.guannengcc.top

Java: System.err.println("err")
来源：http://yvk.tianlin.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ojl.daria6918.cn

Ruby: warn "err"
来源：http://akb.hammf.cn

C#:   Console.Error.WriteLine("err")
来源：http://uar.yongpay.top

[M07] 判断是否为主入口
来源：http://hfb.shanyushiyangkeji.top

Py:   if __name__ == "__main__":
来源：http://qge.xylfe.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yra.wangdashe.top

JS:   require.main === module
来源：http://axj.wangshuangyany.cn

TS:   require.main === module
来源：http://dfi.chenzaomai.com

Java: public static void main(String[] args)
来源：http://ouw.ctjpmb.com

Go:   func main()
来源：http://uim.yfazqb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cie.snrcjt.cn

C#:   static void Main(string[] args)
来源：http://kgd.haohaochexian.top

[M08] 获取系统与运行时信息
来源：http://tuo.haohaochexian.top

Py:   platform.system();  platform.python_version()
来源：http://ajh.mhx1999.top

PHP:  PHP_OS;  phpversion();
来源：http://xsm.daria6918.cn

JS:   process.platform;  process.version
来源：http://plw.cucudq.cn

TS:   process.platform;  process.version
来源：http://mfw.snrcjt.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wgv.ppjwa.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ymy.fanxiaobao.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jwj.yuxming.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://eja.pengpengdd.cyou

================================================================================
来源：http://yii.fehbvm.com

N. 数据结构与算法
来源：http://ksa.sufxvd.cn

================================================================================
来源：http://zvb.yuanzhike.top

[N01] 二分查找（有序数组）
来源：http://oso.sufxvd.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hah.gogol.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://esc.ppjwa.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lix.dianchejie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://noe.nanxuanxn.top

Java: Arrays.binarySearch(arr, x)
来源：http://lva.aizwys.cn

Go:   sort.SearchInts(arr, x)
来源：http://nnn.xuetiantiany.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ovh.uphjek.com

C#:   Array.BinarySearch(arr, x)
来源：http://igo.nanxuanxn.top

[N02] 排序（工程实践用内置实现）
来源：http://zkc.aizwys.cn

Py:   sorted(arr);  arr.sort()
来源：http://ajt.kuanghao11.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ysf.sxryk.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zxu.yuanzhike.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://zkq.ivvv.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tcp.jqgufenzy.top

Go:   slices.Sort(arr)
来源：http://mhs.andypj.xyz

Ruby: arr.sort
来源：http://eol.aibaodan.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://eel.jqgfzy.top

[N03] 快速排序（分治示例）
来源：http://htw.yj20258888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://skm.zhengqikj.top

PHP:  // 递归实现，或用 usort
来源：http://klw.sjlbkw.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oxy.jinyuanbaomall.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ikp.yueranfly.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wcp.uphjek.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ccp.jianghu66.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ufy.cashguo.top

C#:   // 手写递归，或 Array.Sort
来源：http://thv.xuetiantiany.cn

[N04] 斐波那契数列
来源：http://lsj.zdqjudy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jup.zhijiandao.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iug.jiagoushi.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sji.ydzc1.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pys.yuxming.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lev.shzxlz.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mbe.zhijiandao.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vkm.jinqigfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dud.hammf.cn

[N05] 最大公约数
来源：http://een.cucudq.cn

Py:   math.gcd(a, b)
来源：http://dhf.yueranfly.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ipv.hywenlv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://asd.snrcjt.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qdw.yueranfly.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wyp.wangdashe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kqc.chenjidiqi.icu

Ruby: a.gcd(b)
来源：http://eeg.wangshuangyany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://itd.yuanzhike.top

[N06] 判断回文字符串
来源：http://egv.zhongyouzk.top

Py:   s == s[::-1]
来源：http://mwx.dianchejie.cn

PHP:  $s === strrev($s);
来源：http://njx.zhijiandao.cn

JS:   s === [...s].reverse().join("")
来源：http://itn.aibaodan.cn

TS:   s === [...s].reverse().join("")
来源：http://uut.pengpengdd.cyou

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yca.birdmap.top

Go:   // 双指针从两端比较
来源：http://vxq.hnxiangtu.top

Ruby: s == s.reverse
来源：http://ehx.pengpengdd.cyou

C#:   s == new string(s.Reverse().ToArray())
来源：http://bja.wangshuangyany.cn

[N07] 两数之和（返回下标）
来源：http://sds.shanyushiyangtech.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zew.9152youxi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bpb.jianghu66.top

JS:   // 手写 Map：map.set(v, i)
来源：http://iot.tianlin.xyz

TS:   // 手写 Map<string, number>
来源：http://gik.hcnkem.com

Java: // 手写 HashMap
来源：http://uvx.quarkkingdee.top

Go:   // 手写 map[int]int
来源：http://xwa.gaohongyu789.top

Ruby: // 手写 Hash
来源：http://eob.xylfe.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mya.yuxming.cn

[N08] 生成全排列
来源：http://fhh.yongpay.top

Py:   itertools.permutations(arr)
来源：http://ekj.hywenlv.cn

PHP:  // 手写递归交换
来源：http://qyk.shangyingyoupin.top

JS:   // 手写回溯递归
来源：http://qqm.hcnkem.com

TS:   // 手写回溯递归
来源：http://nby.zhongyouzk.top

Java: // 手写回溯递归
来源：http://cdj.yuanzhike.top

Go:   // 手写回溯递归
来源：http://uxr.hywenlv.cn

Ruby: arr.permutation.to_a
来源：http://bbs.yanxiufei.cn

C#:   // 手写回溯递归
来源：http://sdl.havefunace.top

[N09] 栈与队列
来源：http://tez.316326.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xtb.yanxiufei.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dnu.zdqjudy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wew.xingfuxueyuan.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://apy.zhaomingkeji.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://arl.kuanghao11.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yor.0kj1m.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ntf.hongshengwenyu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ydt.aizwys.cn

[N10] 链表节点定义
来源：http://hjq.aizwys.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rdg.gzhubu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://kdt.smart0.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gbp.tanke756.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nrj.ppjwa.cn

Java: class Node { int v; Node next; }
来源：http://mzo.daria6918.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jqz.gogol.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jlx.shuidangran.top

C#:   class Node { public int V; public Node? Next; }
来源：http://mua.quarkkingdee.top

[N11] 二叉树中序遍历
来源：http://xbm.meibo888.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vkr.jinghuilouyu.cn

PHP:  // 手写递归函数
来源：http://ctp.uphjek.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fxg.sufxvd.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://msk.c1oappe.top

Java: // 手写递归
来源：http://eoy.quarkkingdee.top

Go:   // 手写递归
来源：http://egu.sysykeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hwt.shanyushiyangkeji.top

C#:   // 手写递归
来源：http://nnt.gogol.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dfq.tarul.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kdz.redwolf501.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://icr.wangdashe.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rxt.tian-w.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ekc.nwbrower.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://roi.fktsv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://avi.jqgfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kqx.yvedp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cum.316326.xyz

================================================================================
来源：http://par.yj202588.top

O. 并发与异步
来源：http://buf.zdqjudy.top

================================================================================
来源：http://nic.ivvv.top

[O01] 启动一个线程
来源：http://lgw.zhongyouzk.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nqh.fengsongda.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jaj.cucudq.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dpn.fzhhl.top

TS:   // 同 JS
来源：http://gfs.xylfe.cn

Java: new Thread(() -> f()).start()
来源：http://sxa.pycfn.com

Go:   go f()
来源：http://xug.fengsongda.top

Ruby: Thread.new { f }
来源：http://rjy.yj20258888.top

C#:   Task.Run(() => F());
来源：http://rxa.jlsjyb.cn

[O02] 使用线程池
来源：http://vfu.zhongyouzk.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yfc.chenzaomai.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://juf.cucudq.cn

JS:   // worker_threads 线程池
来源：http://naw.tanke756.top

TS:   // worker_threads 线程池
来源：http://hdk.uphjek.com

Java: Executors.newFixedThreadPool(4)
来源：http://ldo.jlsjyb.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mzi.mhx1999.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wed.xylfe.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fkw.zhiwuduotai.top

[O03] 加锁保护共享数据
来源：http://vqd.hnxiangtu.top

Py:   with lock: shared += 1
来源：http://ctb.hysaishi.cn

PHP:  // 用 flock() 做文件锁
来源：http://huv.zhijiandao.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yqr.ybcxt.top

TS:   // 同 JS
来源：http://cbc.yvedp.cn

Java: synchronized (this) { shared++; }
来源：http://mdp.zdqjudy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bbx.iojbl.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fmj.svipenyu.cn

C#:   lock (gate) { shared++; }
来源：http://xxk.pycfn.com

[O04] 定义异步函数并等待
来源：http://ahu.cucudq.cn

Py:   async def f():⏎    await g()
来源：http://uso.ywan-chungtsiang.top


<!-- 参考信息 -->
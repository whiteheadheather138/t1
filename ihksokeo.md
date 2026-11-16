代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nvb.dianchejie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tww.havefunace.top

[K08] 二进制序列化（非 JSON）
来源：http://yjl.zhixingplan.top

Py:   pickle.dumps(obj)
来源：http://blc.havefunace.top

PHP:  serialize($obj);  unserialize($s);
来源：http://yuh.sxryk.cn

JS:   v8.serialize(obj)        // Node
来源：http://vhw.zhiwuduotai.top

TS:   v8.serialize(obj)        // Node
来源：http://mos.svipenyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://orq.redwolf501.top

Go:   encoding/gob
来源：http://fxh.meibo888.top

Ruby: Marshal.dump(obj)
来源：http://liq.ctjpmb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ofx.cqqwz.cn

================================================================================
来源：http://bhg.hnqzz.top

L. 网络请求
来源：http://nxc.andypj.xyz

================================================================================
来源：http://uiw.birdmap.top

[L01] 发送 GET 请求
来源：http://hij.yanxiufei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kcy.zhiwuduotai.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dxc.haohaochexian.top

JS:   await fetch(url)
来源：http://alf.ywan-chungtsiang.top

TS:   await fetch(url)
来源：http://kdx.cdnleiting.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mut.fanxiaobao.xyz

Go:   resp, err := http.Get(url)
来源：http://hoy.pycfn.com

Ruby: Net::HTTP.get(URI(url))
来源：http://ind.xylfe.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vxq.xinyue.icu

[L02] 发送 POST JSON
来源：http://yoe.yuxming.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lhz.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ptz.ybcxt.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nbf.kuanghao11.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pjl.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mmr.yvedp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://feq.shzxlz.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yyg.havefunace.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blo.ivvv.top

[L03] 设置自定义请求头
来源：http://efe.hysaishi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://euj.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://muw.nanxuanxn.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vnf.zhengqikj.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rly.bjfxy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hew.pycfn.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wyy.0kj1m.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://udm.yongpay.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://llj.zycfv.cn

[L04] 设置超时
来源：http://qff.xziqi.cn

Py:   requests.get(url, timeout=5)
来源：http://ypj.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bdr.fanxiaobao.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zmf.sweek.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yry.jianghu66.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fpj.cucudq.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ybe.nanxuanxn.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yeb.xylfe.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lgz.jqgfzy.top

[L05] 上传文件（multipart）
来源：http://spn.jqgufenzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pon.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lpe.redwolf501.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dhq.zhoulong.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://twt.fzhhl.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pyh.yuxming.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://icl.tianlin.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lpi.tian-w.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mtg.birdmap.top

[L06] 解析响应为 JSON
来源：http://tpf.yangfankeji.com

Py:   resp.json()
来源：http://hgy.xuetiantiany.cn

PHP:  json_decode($body, true);
来源：http://syv.bjfxy.top

JS:   await resp.json()
来源：http://uvm.cdnleiting.top

TS:   await resp.json()
来源：http://bek.bjfxy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vwe.yj20258.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://coq.hnxiangtu.top

Ruby: JSON.parse(resp.body)
来源：http://lps.zhiwuduotai.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://chl.zdbjq.cn

[L07] 处理 HTTP 状态码
来源：http://zbw.tanke756.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://exg.yj202588.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bzl.316326.xyz

JS:   resp.ok;  resp.status
来源：http://ede.kuanghao11.cn

TS:   resp.ok;  resp.status
来源：http://hrj.sysykeji.top

Java: resp.statusCode()
来源：http://zsa.ywan-chungtsiang.top

Go:   resp.StatusCode
来源：http://pvb.dianchejie.cn

Ruby: resp.code.to_i
来源：http://tsm.zhixingplan.top

C#:   (int)resp.StatusCode
来源：http://eir.jyoumei.cn

[L08] 并发请求多个地址
来源：http://mvn.wangshuangyany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kwt.bbcook.cn

PHP:  curl_multi_init() 系列
来源：http://tbt.wangdashe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yct.ivvv.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wry.yvedp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wbf.zhiwuduotai.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nny.dashuyun.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uxt.yuanzhike.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xbc.epnwcf.com

================================================================================
来源：http://fir.snrcjt.cn

M. 命令行 / 进程 / 环境
来源：http://nln.aizwys.cn

================================================================================
来源：http://tvk.aibaodan.cn

[M01] 读取命令行参数
来源：http://wlj.iojbl.cn

Py:   sys.argv[1:]
来源：http://vnc.gaohongyu789.top

PHP:  $argv;  $argc;
来源：http://pvw.yvedp.cn

JS:   process.argv.slice(2)
来源：http://rwe.hammf.cn

TS:   process.argv.slice(2)
来源：http://sxe.yj202588.top

Java: args 数组（main 方法参数）
来源：http://xnp.daria6918.cn

Go:   os.Args[1:]
来源：http://iuc.yfazqb.com

Ruby: ARGV
来源：http://qgq.svipenyu.cn

C#:   args 数组（Main 方法参数）
来源：http://fzb.jinqigfzy.top

[M02] 读取环境变量
来源：http://yvh.yuxming.cn

Py:   os.environ.get("HOME")
来源：http://jby.wangdashe.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vrw.jinqigfzy.top

JS:   process.env.HOME
来源：http://vuq.jinyuanbaomall.cn

TS:   process.env.HOME
来源：http://low.xuetiantiany.cn

Java: System.getenv("HOME")
来源：http://ouf.zhaomingkeji.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tdg.zdbjq.cn

Ruby: ENV["HOME"]
来源：http://zeo.pycfn.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mza.yangfankeji.com

[M03] 执行外部命令
来源：http://fml.gogol.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dup.zhongyouzk.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://imz.redwolf501.top

JS:   child_process.execSync("ls -l").toString()
来源：http://njr.yonumen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://nhd.yongpay.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vcd.hcnkem.com

Go:   exec.Command("ls", "-l").Output()
来源：http://kpr.jinqigfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://raz.fanxiaobao.xyz

C#:   Process.Start("ls", "-l");
来源：http://ogb.vqdsnc.cn

[M04] 获取当前工作目录
来源：http://bbu.svipenyu.cn

Py:   os.getcwd()
来源：http://grs.cashguo.top

PHP:  getcwd();
来源：http://tlm.shanyushiyangkeji.top

JS:   process.cwd()
来源：http://wap.9152youxi.cn

TS:   process.cwd()
来源：http://arh.sxryk.cn

Java: Path.of("").toAbsolutePath()
来源：http://wms.yj20258888.top

Go:   os.Getwd()
来源：http://bcq.haohaochexian.top

Ruby: Dir.pwd
来源：http://yww.chenjidiqi.icu

C#:   Directory.GetCurrentDirectory()
来源：http://nxs.shangyingyoupin.top

[M05] 设置退出码
来源：http://kfq.jlsjyb.cn

Py:   sys.exit(1)
来源：http://stu.hnxiangtu.top

PHP:  exit(1);
来源：http://kma.bbcook.cn

JS:   process.exit(1)
来源：http://bes.zhoulong.xyz

TS:   process.exit(1)
来源：http://uey.xuanzx.com

Java: System.exit(1)
来源：http://dkr.ywan-chungtsiang.top

Go:   os.Exit(1)
来源：http://ohv.yuanzhike.top

Ruby: exit 1
来源：http://try.chenzaomai.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://orp.zhijiandao.cn

[M06] 向标准错误输出
来源：http://kju.havefunace.top

Py:   print("err", file=sys.stderr)
来源：http://ljg.yfazqb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://yzc.zhoulong.xyz

JS:   console.error("err")
来源：http://exg.tarul.cn

TS:   console.error("err")
来源：http://afs.hesvh.cn

Java: System.err.println("err")
来源：http://rjq.ivvv.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vuy.sjlbkw.cn

Ruby: warn "err"
来源：http://awk.jlsjyb.cn

C#:   Console.Error.WriteLine("err")
来源：http://rcb.yonumen.top

[M07] 判断是否为主入口
来源：http://wqj.hnqzz.top

Py:   if __name__ == "__main__":
来源：http://zya.kuanghao11.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ehg.zhengqikj.top

JS:   require.main === module
来源：http://mov.redwolf501.top

TS:   require.main === module
来源：http://ogi.shangyingyoupin.top

Java: public static void main(String[] args)
来源：http://baq.vehdjk.com

Go:   func main()
来源：http://qba.fengsongda.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yjm.xingfuxueyuan.xyz

C#:   static void Main(string[] args)
来源：http://ffo.yvedp.cn

[M08] 获取系统与运行时信息
来源：http://wnx.hammf.cn

Py:   platform.system();  platform.python_version()
来源：http://xda.smart0.xyz

PHP:  PHP_OS;  phpversion();
来源：http://zge.daria6918.cn

JS:   process.platform;  process.version
来源：http://deo.ydzc1.top

TS:   process.platform;  process.version
来源：http://nbf.sxryk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://iuw.bbcook.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://arx.chenjidiqi.icu

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jxh.ywan-chungtsiang.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://rur.hongshengwenyu.top

================================================================================
来源：http://knk.cdnleiting.top

N. 数据结构与算法
来源：http://ciw.gotoacloud.top

================================================================================
来源：http://jzj.epnwcf.com

[N01] 二分查找（有序数组）
来源：http://pxu.shzxlz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://huo.shanyushiyangkeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vkb.hnxiangtu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://igo.tanke756.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://foi.quarkkingdee.top

Java: Arrays.binarySearch(arr, x)
来源：http://wzy.dashuyun.cn

Go:   sort.SearchInts(arr, x)
来源：http://ksq.cheryme.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://sma.snrcjt.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ser.ctjpmb.com

[N02] 排序（工程实践用内置实现）
来源：http://xyi.shangyingyoupin.top

Py:   sorted(arr);  arr.sort()
来源：http://pjy.iojbl.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jsf.hfpthk.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ydb.chenjidiqi.icu

TS:   [...arr].sort((a, b) => a - b)
来源：http://lvi.hfpthk.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://swt.ybcxt.top

Go:   slices.Sort(arr)
来源：http://xks.hesvh.cn

Ruby: arr.sort
来源：http://fho.chenjidiqi.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://atw.zdbjq.cn

[N03] 快速排序（分治示例）
来源：http://lgz.bbcook.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uwg.hywenlv.cn

PHP:  // 递归实现，或用 usort
来源：http://dmx.ehwqpu.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kqk.zhixingplan.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lpy.52xcode.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gqb.ydzc1.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://czy.hcnkem.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://plw.ehwqpu.com

C#:   // 手写递归，或 Array.Sort
来源：http://eaz.jinqigfzy.top

[N04] 斐波那契数列
来源：http://doi.yj20258888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://izt.uphjek.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jso.ydjk.org.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xef.pycfn.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tik.snrcjt.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sxn.guowangkeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iug.bbcook.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://slb.hysaishi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lcn.gaohongyu789.top

[N05] 最大公约数
来源：http://xua.yj20258888.top

Py:   math.gcd(a, b)
来源：http://ish.xziqi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://evi.ydjk.org.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ouf.fanxiaobao.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dqu.hongshengwenyu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jtm.shuidangran.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lvw.jinghuilouyu.cn

Ruby: a.gcd(b)
来源：http://sst.zycfv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xsh.316326.xyz

[N06] 判断回文字符串
来源：http://gym.snrcjt.cn

Py:   s == s[::-1]
来源：http://zwp.sjlbkw.cn

PHP:  $s === strrev($s);
来源：http://exd.yuxming.cn

JS:   s === [...s].reverse().join("")
来源：http://fwt.bjfxy.top

TS:   s === [...s].reverse().join("")
来源：http://myo.smart0.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fny.pengpengdd.cyou

Go:   // 双指针从两端比较
来源：http://jxo.bbcook.cn

Ruby: s == s.reverse
来源：http://gzi.hywenlv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lmr.hammf.cn

[N07] 两数之和（返回下标）
来源：http://msu.snrcjt.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kdb.quarkkingdee.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xzp.vehdjk.com

JS:   // 手写 Map：map.set(v, i)
来源：http://wnd.snrcjt.cn

TS:   // 手写 Map<string, number>
来源：http://fkr.cdnleiting.top

Java: // 手写 HashMap
来源：http://mnq.jlsjyb.cn

Go:   // 手写 map[int]int
来源：http://ixv.yfazqb.com

Ruby: // 手写 Hash
来源：http://hiw.zhixingplan.top

C#:   // 手写 Dictionary<int, int>
来源：http://mqe.xylfe.cn

[N08] 生成全排列
来源：http://idf.tarul.cn

Py:   itertools.permutations(arr)
来源：http://njl.gaohongyu789.top

PHP:  // 手写递归交换
来源：http://qqi.xuetiantiany.cn

JS:   // 手写回溯递归
来源：http://yim.iojbl.cn

TS:   // 手写回溯递归
来源：http://eij.cheryme.top

Java: // 手写回溯递归
来源：http://ubi.bbcook.cn

Go:   // 手写回溯递归
来源：http://qks.hnxiangtu.top

Ruby: arr.permutation.to_a
来源：http://dyh.chenlongwang.top

C#:   // 手写回溯递归
来源：http://cuk.cqqwz.cn

[N09] 栈与队列
来源：http://eui.xingfuxueyuan.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jan.jqgufenzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fbo.cucudq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cdl.hnxiangtu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ksb.vehdjk.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qya.bjfxy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yap.jinyuanbaomall.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zct.hywenlv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mbv.kuanghao11.cn

[N10] 链表节点定义
来源：http://rwz.cheryme.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sdm.meibo888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://asf.zdbjq.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mzu.9152youxi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ftw.zycfv.cn

Java: class Node { int v; Node next; }
来源：http://vpi.nwbrower.top

Go:   type Node struct { V int; Next *Node }
来源：http://ppu.ydjk.org.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kgb.jinyuanbaomall.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kqn.hongshengwenyu.top

[N11] 二叉树中序遍历
来源：http://xzq.tanke756.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://viw.smart0.xyz

PHP:  // 手写递归函数
来源：http://ufc.yangfankeji.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yhz.sysykeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://coi.gzhubu.top

Java: // 手写递归
来源：http://zug.gzhubu.top

Go:   // 手写递归
来源：http://rxz.feifeiyinyue.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mdj.wangdashe.top

C#:   // 手写递归
来源：http://vye.316326.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xkp.gotoacloud.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yuw.svipenyu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://irw.guowangkeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fje.xylfe.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ndy.jianghu66.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ets.wangshuangyany.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qsb.nanxinkj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nsn.ppjwa.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vgd.guowangkeji.top

================================================================================
来源：http://rlq.snrcjt.cn

O. 并发与异步
来源：http://jwh.pycfn.com

================================================================================
来源：http://lxl.fehbvm.com

[O01] 启动一个线程
来源：http://qrh.sufxvd.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qmu.quarkkingdee.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fcb.yvedp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dsc.sweek.top

TS:   // 同 JS
来源：http://bmu.guannengcc.top

Java: new Thread(() -> f()).start()
来源：http://hzv.xingfuxueyuan.xyz

Go:   go f()
来源：http://mwb.hammf.cn

Ruby: Thread.new { f }
来源：http://odu.sxryk.cn

C#:   Task.Run(() => F());
来源：http://duh.zhongyouzk.top

[O02] 使用线程池
来源：http://zrz.smart0.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zva.ydjk.org.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jmd.sweek.top

JS:   // worker_threads 线程池
来源：http://zgt.haohaochexian.top

TS:   // worker_threads 线程池
来源：http://ulu.nanxuanxn.top

Java: Executors.newFixedThreadPool(4)
来源：http://iom.yuanzhike.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fzj.xingfuxueyuan.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kdj.yonumen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fyz.yuxming.cn

[O03] 加锁保护共享数据
来源：http://khe.cashguo.top

Py:   with lock: shared += 1
来源：http://jup.hfpthk.cn

PHP:  // 用 flock() 做文件锁
来源：http://diw.mhx1999.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sku.zdbjq.cn

TS:   // 同 JS
来源：http://ttb.zhoulong.xyz

Java: synchronized (this) { shared++; }
来源：http://grl.shzxlz.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gzo.kuanghao11.cn


<!-- 参考信息 -->
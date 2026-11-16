代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cqf.316326.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rax.dianchejie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://giu.nanxinkj.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bmc.hongshengwenyu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cfq.xylfe.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lhr.nanxinkj.top

[K08] 二进制序列化（非 JSON）
来源：http://fsz.zhixingplan.top

Py:   pickle.dumps(obj)
来源：http://mbm.hesvh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wdn.zdqjudy.top

JS:   v8.serialize(obj)        // Node
来源：http://cjo.zhixingplan.top

TS:   v8.serialize(obj)        // Node
来源：http://klu.shzxlz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://epx.aibaodan.cn

Go:   encoding/gob
来源：http://kfm.cheryme.top

Ruby: Marshal.dump(obj)
来源：http://avq.yuanzhike.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vet.cdnleiting.top

================================================================================
来源：http://crh.bbcook.cn

L. 网络请求
来源：http://woh.c1oappe.top

================================================================================
来源：http://yia.ppjwa.cn

[L01] 发送 GET 请求
来源：http://zcs.jqgufenzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lfw.svipenyu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yxo.xinyue.icu

JS:   await fetch(url)
来源：http://dzk.tian-w.cn

TS:   await fetch(url)
来源：http://adl.pengpengdd.cyou

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vxx.bbcook.cn

Go:   resp, err := http.Get(url)
来源：http://veb.cqqwz.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://eqd.feifeiyinyue.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uui.yanxiufei.cn

[L02] 发送 POST JSON
来源：http://nni.jqgufenzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://hir.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yak.jinqigfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iyr.fzhhl.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bil.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sfx.hongshengwenyu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tot.cqqwz.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://anu.zhijiandao.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://awn.andypj.xyz

[L03] 设置自定义请求头
来源：http://jhs.52xcode.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nqk.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uls.yangfankeji.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xoh.zhiwuduotai.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kcs.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ire.pycfn.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jvt.xinyue.icu

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://msg.kuanghao11.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ygo.guowangkeji.top

[L04] 设置超时
来源：http://jjs.jianghu66.top

Py:   requests.get(url, timeout=5)
来源：http://czs.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://drw.xuanzx.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xeu.tian-w.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fdo.zhiwuduotai.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vva.daxiang520.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wjf.hywenlv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gzf.cheryme.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bef.hfpthk.cn

[L05] 上传文件（multipart）
来源：http://igi.fzhhl.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jst.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ngz.havefunace.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jjh.vehdjk.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wqg.hcnkem.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rgj.zhiwuduotai.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vpx.dashuyun.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uxo.bbcook.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ckt.kuanghao11.cn

[L06] 解析响应为 JSON
来源：http://dfe.jinqigfzy.top

Py:   resp.json()
来源：http://djy.ybcxt.top

PHP:  json_decode($body, true);
来源：http://bkn.hfpthk.cn

JS:   await resp.json()
来源：http://wnf.quarkkingdee.top

TS:   await resp.json()
来源：http://odi.haohaochexian.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://obm.smart0.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gto.yonumen.top

Ruby: JSON.parse(resp.body)
来源：http://oph.hammf.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jby.xinyue.icu

[L07] 处理 HTTP 状态码
来源：http://ebb.guannengcc.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cmb.gogol.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qhh.fzhhl.top

JS:   resp.ok;  resp.status
来源：http://eza.fktsv.cn

TS:   resp.ok;  resp.status
来源：http://hff.zhengqikj.top

Java: resp.statusCode()
来源：http://spu.gogol.net.cn

Go:   resp.StatusCode
来源：http://hfw.smart0.xyz

Ruby: resp.code.to_i
来源：http://xwj.yuanzhike.top

C#:   (int)resp.StatusCode
来源：http://ilw.andypj.xyz

[L08] 并发请求多个地址
来源：http://wqz.xylfe.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tmq.meibo888.top

PHP:  curl_multi_init() 系列
来源：http://woo.dashuyun.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rxz.vehdjk.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tfw.ydjk.org.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bfk.jinyuanbaomall.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tlb.nanxinkj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://heh.sjlbkw.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cac.fzhhl.top

================================================================================
来源：http://nnc.daxiang520.top

M. 命令行 / 进程 / 环境
来源：http://zue.xylfe.cn

================================================================================
来源：http://xpv.cdnleiting.top

[M01] 读取命令行参数
来源：http://xfh.shangyingyoupin.top

Py:   sys.argv[1:]
来源：http://ixc.chenjidiqi.icu

PHP:  $argv;  $argc;
来源：http://rua.zhengqikj.top

JS:   process.argv.slice(2)
来源：http://gpu.aizwys.cn

TS:   process.argv.slice(2)
来源：http://vjx.chenzaomai.com

Java: args 数组（main 方法参数）
来源：http://zep.zhongyouzk.top

Go:   os.Args[1:]
来源：http://vge.fehbvm.com

Ruby: ARGV
来源：http://afs.hesvh.cn

C#:   args 数组（Main 方法参数）
来源：http://hmo.zhengqikj.top

[M02] 读取环境变量
来源：http://aim.jqgfzy.top

Py:   os.environ.get("HOME")
来源：http://mth.daxiang520.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lwl.jinqigfzy.top

JS:   process.env.HOME
来源：http://mul.zhaomingkeji.xyz

TS:   process.env.HOME
来源：http://frf.hesvh.cn

Java: System.getenv("HOME")
来源：http://fdz.yangfankeji.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ttk.quarkkingdee.top

Ruby: ENV["HOME"]
来源：http://mxx.nwbrower.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bzb.fengsongda.top

[M03] 执行外部命令
来源：http://mez.cheryme.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://can.vqdsnc.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bcn.fanxiaobao.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://kta.hammf.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sfs.yuxming.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gaz.sxryk.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hdk.yuanzhike.top

Ruby: system("ls -l");  `ls -l`
来源：http://ajg.ctjpmb.com

C#:   Process.Start("ls", "-l");
来源：http://bbr.jinyuanbaomall.cn

[M04] 获取当前工作目录
来源：http://cam.xylfe.cn

Py:   os.getcwd()
来源：http://rth.shanyushiyangtech.top

PHP:  getcwd();
来源：http://snp.daria6918.cn

JS:   process.cwd()
来源：http://whv.wangshuangyany.cn

TS:   process.cwd()
来源：http://rrx.epnwcf.com

Java: Path.of("").toAbsolutePath()
来源：http://bkf.jiagoushi.top

Go:   os.Getwd()
来源：http://huw.redwolf501.top

Ruby: Dir.pwd
来源：http://sbl.bjfxy.top

C#:   Directory.GetCurrentDirectory()
来源：http://nel.zhaomingkeji.xyz

[M05] 设置退出码
来源：http://cdh.nwbrower.top

Py:   sys.exit(1)
来源：http://ioe.fktsv.cn

PHP:  exit(1);
来源：http://ioy.yvedp.cn

JS:   process.exit(1)
来源：http://mbm.zhixingplan.top

TS:   process.exit(1)
来源：http://qbt.fktsv.cn

Java: System.exit(1)
来源：http://vzy.andypj.xyz

Go:   os.Exit(1)
来源：http://rwk.shangyingyoupin.top

Ruby: exit 1
来源：http://xpz.nanxuanxn.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lbz.haohaochexian.top

[M06] 向标准错误输出
来源：http://fsp.xuanzx.com

Py:   print("err", file=sys.stderr)
来源：http://jhn.xylfe.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nxf.yj202588.top

JS:   console.error("err")
来源：http://iux.vehdjk.com

TS:   console.error("err")
来源：http://jup.yonumen.top

Java: System.err.println("err")
来源：http://wyu.wangdashe.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qyd.zhengqikj.top

Ruby: warn "err"
来源：http://vyp.haohaochexian.top

C#:   Console.Error.WriteLine("err")
来源：http://vyt.sweek.top

[M07] 判断是否为主入口
来源：http://pse.hesvh.cn

Py:   if __name__ == "__main__":
来源：http://fxc.ydzc1.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cqf.zhoulong.xyz

JS:   require.main === module
来源：http://viv.yangfankeji.com

TS:   require.main === module
来源：http://yzo.jinyuanbaomall.cn

Java: public static void main(String[] args)
来源：http://ltq.sjlbkw.cn

Go:   func main()
来源：http://suf.hnxiangtu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mxl.shanyushiyangkeji.top

C#:   static void Main(string[] args)
来源：http://yky.c1oappe.top

[M08] 获取系统与运行时信息
来源：http://fqi.epnwcf.com

Py:   platform.system();  platform.python_version()
来源：http://qwr.ivvv.top

PHP:  PHP_OS;  phpversion();
来源：http://mvm.316326.xyz

JS:   process.platform;  process.version
来源：http://jvy.andypj.xyz

TS:   process.platform;  process.version
来源：http://xne.aizwys.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bak.bbcook.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dlw.snrcjt.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://poi.tarul.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rmy.sweek.top

================================================================================
来源：http://jhh.andypj.xyz

N. 数据结构与算法
来源：http://glj.c1oappe.top

================================================================================
来源：http://bcs.gotoacloud.top

[N01] 二分查找（有序数组）
来源：http://iuj.ppjwa.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wzs.sjlbkw.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zcq.zhoulong.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xde.hongshengwenyu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kjh.feifeiyinyue.top

Java: Arrays.binarySearch(arr, x)
来源：http://sza.xuanzx.com

Go:   sort.SearchInts(arr, x)
来源：http://bqy.jyoumei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vqq.cheryme.top

C#:   Array.BinarySearch(arr, x)
来源：http://wpi.jqgfzy.top

[N02] 排序（工程实践用内置实现）
来源：http://emt.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://myk.shanyushiyangtech.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://odb.tian-w.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mzg.gzhubu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mda.yangfankeji.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ekd.cashguo.top

Go:   slices.Sort(arr)
来源：http://mjd.yj20258.top

Ruby: arr.sort
来源：http://uue.jqgfzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://slq.hywenlv.cn

[N03] 快速排序（分治示例）
来源：http://nco.andypj.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uyh.hesvh.cn

PHP:  // 递归实现，或用 usort
来源：http://pqp.0kj1m.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rwj.wangshuangyany.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://krq.gzhubu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jwz.iojbl.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://eoy.sysykeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wju.xuanzx.com

C#:   // 手写递归，或 Array.Sort
来源：http://nos.yonumen.top

[N04] 斐波那契数列
来源：http://ame.zhiwuduotai.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://aip.gzhubu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://utl.jyoumei.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gpk.sufxvd.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vlx.yuxming.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hlx.nanxinkj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gdh.shuidangran.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://psq.zdbjq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wrp.feifeiyinyue.top

[N05] 最大公约数
来源：http://uqv.fehbvm.com

Py:   math.gcd(a, b)
来源：http://plg.sjlbkw.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oit.hcnkem.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ccs.gotoacloud.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lkw.yvedp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://irn.ctjpmb.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://soi.quarkkingdee.top

Ruby: a.gcd(b)
来源：http://ssd.zdbjq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fxc.yuanzhike.top

[N06] 判断回文字符串
来源：http://enn.ivvv.top

Py:   s == s[::-1]
来源：http://mbc.aibaodan.cn

PHP:  $s === strrev($s);
来源：http://rhr.chenzaomai.com

JS:   s === [...s].reverse().join("")
来源：http://hei.dianchejie.cn

TS:   s === [...s].reverse().join("")
来源：http://exp.c1oappe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://obk.smart0.xyz

Go:   // 双指针从两端比较
来源：http://bll.ydzc1.top

Ruby: s == s.reverse
来源：http://wgf.wangshuangyany.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://uff.sweek.top

[N07] 两数之和（返回下标）
来源：http://mjp.dashuyun.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fnj.chenlongwang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xtj.zycfv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jxi.sweek.top

TS:   // 手写 Map<string, number>
来源：http://pld.xuanzx.com

Java: // 手写 HashMap
来源：http://pys.jqgfzy.top

Go:   // 手写 map[int]int
来源：http://ypt.nanxuanxn.top

Ruby: // 手写 Hash
来源：http://ugf.bbcook.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ulh.snrcjt.cn

[N08] 生成全排列
来源：http://kwn.yueranfly.top

Py:   itertools.permutations(arr)
来源：http://jtp.gzhubu.top

PHP:  // 手写递归交换
来源：http://xre.ehwqpu.com

JS:   // 手写回溯递归
来源：http://jda.sjlbkw.cn

TS:   // 手写回溯递归
来源：http://kfi.jqgufenzy.top

Java: // 手写回溯递归
来源：http://ngy.ppjwa.cn

Go:   // 手写回溯递归
来源：http://ygw.xylfe.cn

Ruby: arr.permutation.to_a
来源：http://sgx.gotoacloud.top

C#:   // 手写回溯递归
来源：http://qwg.yj202588.top

[N09] 栈与队列
来源：http://fdh.haohaochexian.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kgk.cdnleiting.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jlx.nanxinkj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vig.yj20258888.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uir.iojbl.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bjt.fzhhl.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jit.hnqzz.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yow.c1oappe.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nud.shuidangran.top

[N10] 链表节点定义
来源：http://epn.gogol.net.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yfd.guannengcc.top

PHP:  class Node { public $v; public $next = null; }
来源：http://wua.zycfv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qdz.hywenlv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jek.redwolf501.top

Java: class Node { int v; Node next; }
来源：http://klt.tianlin.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://log.jinyuanbaomall.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://aof.haohaochexian.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tte.aibaodan.cn

[N11] 二叉树中序遍历
来源：http://rin.tarul.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sca.shuidangran.top

PHP:  // 手写递归函数
来源：http://axp.xylfe.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hwe.ywan-chungtsiang.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qul.gaohongyu789.top

Java: // 手写递归
来源：http://twa.fehbvm.com

Go:   // 手写递归
来源：http://rsb.xuetiantiany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eml.zhixingplan.top

C#:   // 手写递归
来源：http://vga.hnqzz.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://skw.smart0.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://roz.zhaomingkeji.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://smg.ivvv.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lcs.zhoulong.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nwo.jinqigufen.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dyb.hywenlv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fsq.316326.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ome.shanyushiyangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mwr.tianlin.xyz

================================================================================
来源：http://lue.sxryk.cn

O. 并发与异步
来源：http://vtr.hnqzz.top

================================================================================
来源：http://iej.gaohongyu789.top

[O01] 启动一个线程
来源：http://ncd.sufxvd.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uud.ppjwa.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zgu.jqgufenzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://oot.gzhubu.top

TS:   // 同 JS
来源：http://gkv.zhengqikj.top

Java: new Thread(() -> f()).start()
来源：http://anv.gzhubu.top

Go:   go f()
来源：http://urr.nwbrower.top

Ruby: Thread.new { f }
来源：http://pyh.zdqjudy.top

C#:   Task.Run(() => F());
来源：http://zjt.kuanghao11.cn

[O02] 使用线程池
来源：http://hxh.gogol.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ffw.ywan-chungtsiang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kvs.ydzc1.top

JS:   // worker_threads 线程池
来源：http://xze.tian-w.cn

TS:   // worker_threads 线程池
来源：http://trj.jinqigfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://mug.xziqi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kbz.ctjpmb.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tlc.jianghu66.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nfk.havefunace.top

[O03] 加锁保护共享数据
来源：http://pka.iojbl.cn

Py:   with lock: shared += 1
来源：http://hlt.epnwcf.com

PHP:  // 用 flock() 做文件锁
来源：http://avx.yvedp.cn


<!-- 参考信息 -->
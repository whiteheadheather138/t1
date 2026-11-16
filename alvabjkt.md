代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yln.svipenyu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uho.gaohongyu789.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qft.yangfankeji.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jac.zhijiandao.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ohl.shzxlz.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tnf.yfazqb.com

[K08] 二进制序列化（非 JSON）
来源：http://gca.bjfxy.top

Py:   pickle.dumps(obj)
来源：http://lkl.hfpthk.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dji.jinghuilouyu.cn

JS:   v8.serialize(obj)        // Node
来源：http://jcb.jianghu66.top

TS:   v8.serialize(obj)        // Node
来源：http://mvj.nanxuanxn.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jox.meibo888.top

Go:   encoding/gob
来源：http://ppc.redwolf501.top

Ruby: Marshal.dump(obj)
来源：http://cyk.jiagoushi.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uhf.ivvv.top

================================================================================
来源：http://mju.nwbrower.top

L. 网络请求
来源：http://zyw.jinghuilouyu.cn

================================================================================
来源：http://xgp.birdmap.top

[L01] 发送 GET 请求
来源：http://lpm.hcnkem.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ezz.zhengqikj.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bwg.xingfuxueyuan.xyz

JS:   await fetch(url)
来源：http://cfe.nanxinkj.top

TS:   await fetch(url)
来源：http://tah.zhiwuduotai.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://arc.gogol.net.cn

Go:   resp, err := http.Get(url)
来源：http://run.pengpengdd.cyou

Ruby: Net::HTTP.get(URI(url))
来源：http://ndi.ivvv.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xsw.tanke756.top

[L02] 发送 POST JSON
来源：http://ctw.yuxming.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wwp.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oct.tanke756.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cub.ivvv.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dhd.zhoulong.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xih.zhongyouzk.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://izl.hongshengwenyu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jee.sufxvd.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://adj.hfpthk.cn

[L03] 设置自定义请求头
来源：http://rej.ybcxt.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cvq.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zeg.9152youxi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ims.jyoumei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bou.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://asp.shanyushiyangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jro.pycfn.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qwn.hysaishi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jlj.shuidangran.top

[L04] 设置超时
来源：http://buh.jiagoushi.top

Py:   requests.get(url, timeout=5)
来源：http://ggu.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ked.redwolf501.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wkd.yj20258888.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rux.dashuyun.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jgu.cqqwz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://slk.zycfv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ydp.shanyushiyangtech.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qdx.svipenyu.cn

[L05] 上传文件（multipart）
来源：http://xiq.fzhhl.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fnc.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://axx.iojbl.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pyu.xylfe.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://avj.ctjpmb.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://omb.xylfe.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mfp.yuxming.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sep.daxiang520.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nwh.yfazqb.com

[L06] 解析响应为 JSON
来源：http://hle.vehdjk.com

Py:   resp.json()
来源：http://bne.xinyue.icu

PHP:  json_decode($body, true);
来源：http://llp.ydzc1.top

JS:   await resp.json()
来源：http://roy.sweek.top

TS:   await resp.json()
来源：http://myy.hywenlv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ynk.vqdsnc.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://axf.zhengqikj.top

Ruby: JSON.parse(resp.body)
来源：http://vhl.uphjek.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iny.ybcxt.top

[L07] 处理 HTTP 状态码
来源：http://cmx.xuetiantiany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fni.cdnleiting.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rcx.dianchejie.cn

JS:   resp.ok;  resp.status
来源：http://btq.yuanzhike.top

TS:   resp.ok;  resp.status
来源：http://ulx.nanxuanxn.top

Java: resp.statusCode()
来源：http://upn.jiagoushi.top

Go:   resp.StatusCode
来源：http://sbb.cdnleiting.top

Ruby: resp.code.to_i
来源：http://caq.xinyue.icu

C#:   (int)resp.StatusCode
来源：http://aos.cucudq.cn

[L08] 并发请求多个地址
来源：http://rul.xingfuxueyuan.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xss.tianlin.xyz

PHP:  curl_multi_init() 系列
来源：http://uxp.tian-w.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ofg.jinqigfzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://drp.hammf.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://doj.jinyuanbaomall.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://osp.aibaodan.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://iaz.kuanghao11.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ftc.sjlbkw.cn

================================================================================
来源：http://orm.chenlongwang.top

M. 命令行 / 进程 / 环境
来源：http://ufn.yj202588.top

================================================================================
来源：http://ssv.jinghuilouyu.cn

[M01] 读取命令行参数
来源：http://bmm.9152youxi.cn

Py:   sys.argv[1:]
来源：http://zbu.hfpthk.cn

PHP:  $argv;  $argc;
来源：http://nij.yj202588.top

JS:   process.argv.slice(2)
来源：http://wim.gaohongyu789.top

TS:   process.argv.slice(2)
来源：http://uhj.bbcook.cn

Java: args 数组（main 方法参数）
来源：http://xlm.shzxlz.cn

Go:   os.Args[1:]
来源：http://ydi.cashguo.top

Ruby: ARGV
来源：http://dqw.guowangkeji.top

C#:   args 数组（Main 方法参数）
来源：http://qbj.cdnleiting.top

[M02] 读取环境变量
来源：http://hkc.ybcxt.top

Py:   os.environ.get("HOME")
来源：http://lnt.andypj.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://erz.zdbjq.cn

JS:   process.env.HOME
来源：http://qqp.hnxiangtu.top

TS:   process.env.HOME
来源：http://bjf.zhixingplan.top

Java: System.getenv("HOME")
来源：http://pfq.pycfn.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lge.chenjidiqi.icu

Ruby: ENV["HOME"]
来源：http://cfr.zhixingplan.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://iiw.xuetiantiany.cn

[M03] 执行外部命令
来源：http://nxc.hongshengwenyu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xly.jianghu66.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://utr.svipenyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pdo.jinghuilouyu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://khy.cheryme.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uzb.cdnleiting.top

Go:   exec.Command("ls", "-l").Output()
来源：http://god.quarkkingdee.top

Ruby: system("ls -l");  `ls -l`
来源：http://liv.xziqi.cn

C#:   Process.Start("ls", "-l");
来源：http://btm.52xcode.cn

[M04] 获取当前工作目录
来源：http://eba.zhixingplan.top

Py:   os.getcwd()
来源：http://avt.xuanzx.com

PHP:  getcwd();
来源：http://puj.cucudq.cn

JS:   process.cwd()
来源：http://idm.zhaomingkeji.xyz

TS:   process.cwd()
来源：http://rox.sysykeji.top

Java: Path.of("").toAbsolutePath()
来源：http://xih.wangdashe.top

Go:   os.Getwd()
来源：http://hgo.vqdsnc.cn

Ruby: Dir.pwd
来源：http://nuy.bjfxy.top

C#:   Directory.GetCurrentDirectory()
来源：http://dzu.dashuyun.cn

[M05] 设置退出码
来源：http://ohd.ctjpmb.com

Py:   sys.exit(1)
来源：http://opu.tian-w.cn

PHP:  exit(1);
来源：http://pyd.fengsongda.top

JS:   process.exit(1)
来源：http://hjs.zycfv.cn

TS:   process.exit(1)
来源：http://itt.kuanghao11.cn

Java: System.exit(1)
来源：http://kmr.ehwqpu.com

Go:   os.Exit(1)
来源：http://eyl.guowangkeji.top

Ruby: exit 1
来源：http://xtv.xziqi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cbt.sufxvd.cn

[M06] 向标准错误输出
来源：http://jjc.hcnkem.com

Py:   print("err", file=sys.stderr)
来源：http://gfo.52xcode.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ngp.vqdsnc.cn

JS:   console.error("err")
来源：http://bgc.jqgufenzy.top

TS:   console.error("err")
来源：http://jbr.guowangkeji.top

Java: System.err.println("err")
来源：http://kog.shuidangran.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wyn.hnqzz.top

Ruby: warn "err"
来源：http://hcc.guannengcc.top

C#:   Console.Error.WriteLine("err")
来源：http://qxe.yongpay.top

[M07] 判断是否为主入口
来源：http://vfz.zhongyouzk.top

Py:   if __name__ == "__main__":
来源：http://zpf.nanxinkj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://slr.hnqzz.top

JS:   require.main === module
来源：http://fbe.ybcxt.top

TS:   require.main === module
来源：http://ilf.zycfv.cn

Java: public static void main(String[] args)
来源：http://dmd.guowangkeji.top

Go:   func main()
来源：http://uoh.smart0.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ohx.zycfv.cn

C#:   static void Main(string[] args)
来源：http://omy.pycfn.com

[M08] 获取系统与运行时信息
来源：http://cwc.cdnleiting.top

Py:   platform.system();  platform.python_version()
来源：http://dvd.hysaishi.cn

PHP:  PHP_OS;  phpversion();
来源：http://yai.zycfv.cn

JS:   process.platform;  process.version
来源：http://ihs.vehdjk.com

TS:   process.platform;  process.version
来源：http://vur.tian-w.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sgj.fzhhl.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://teo.gaohongyu789.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lhz.yangfankeji.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://yvk.yj20258.top

================================================================================
来源：http://ivv.dashuyun.cn

N. 数据结构与算法
来源：http://wrw.iojbl.cn

================================================================================
来源：http://neu.nwbrower.top

[N01] 二分查找（有序数组）
来源：http://upv.aibaodan.cn

Py:   bisect.bisect_left(arr, x)
来源：http://oey.zhijiandao.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://miv.bbcook.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://aab.jinyuanbaomall.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qlv.daria6918.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pnu.yvedp.cn

Go:   sort.SearchInts(arr, x)
来源：http://mpq.gotoacloud.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ijo.feifeiyinyue.top

C#:   Array.BinarySearch(arr, x)
来源：http://tch.zhoulong.xyz

[N02] 排序（工程实践用内置实现）
来源：http://kes.yanxiufei.cn

Py:   sorted(arr);  arr.sort()
来源：http://lon.chenjidiqi.icu

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qim.daxiang520.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fxy.yj20258.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://gdg.ppjwa.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pah.hnqzz.top

Go:   slices.Sort(arr)
来源：http://rrl.xuetiantiany.cn

Ruby: arr.sort
来源：http://fnr.yongpay.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qhs.guannengcc.top

[N03] 快速排序（分治示例）
来源：http://yux.tianlin.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zyc.cdnleiting.top

PHP:  // 递归实现，或用 usort
来源：http://qox.fehbvm.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iih.yfazqb.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qco.gogol.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ptd.tianlin.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gck.guannengcc.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hzd.chenzaomai.com

C#:   // 手写递归，或 Array.Sort
来源：http://ulx.xuanzx.com

[N04] 斐波那契数列
来源：http://zkg.cheryme.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hwo.jianghu66.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pya.guowangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tnc.ybcxt.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uif.shanyushiyangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yqg.bjfxy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://aoc.ydjk.org.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://des.zhixingplan.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ccp.xziqi.cn

[N05] 最大公约数
来源：http://fxc.ydjk.org.cn

Py:   math.gcd(a, b)
来源：http://tmg.0kj1m.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://enw.vqdsnc.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hmf.yanxiufei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pru.bbcook.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://isc.hnqzz.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://avt.yj20258.top

Ruby: a.gcd(b)
来源：http://ata.cashguo.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rzn.yj20258.top

[N06] 判断回文字符串
来源：http://rzp.aizwys.cn

Py:   s == s[::-1]
来源：http://mop.hongshengwenyu.top

PHP:  $s === strrev($s);
来源：http://xyp.jqgufenzy.top

JS:   s === [...s].reverse().join("")
来源：http://kqa.hnqzz.top

TS:   s === [...s].reverse().join("")
来源：http://ato.hfpthk.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://awt.daria6918.cn

Go:   // 双指针从两端比较
来源：http://jyf.xingfuxueyuan.xyz

Ruby: s == s.reverse
来源：http://bjy.zhixingplan.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xyc.dashuyun.cn

[N07] 两数之和（返回下标）
来源：http://cnt.uphjek.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kfq.sysykeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://isz.yanxiufei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xoo.jinyuanbaomall.cn

TS:   // 手写 Map<string, number>
来源：http://sfx.kuanghao11.cn

Java: // 手写 HashMap
来源：http://unr.xingfuxueyuan.xyz

Go:   // 手写 map[int]int
来源：http://fgv.epnwcf.com

Ruby: // 手写 Hash
来源：http://bne.iojbl.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zuj.hnqzz.top

[N08] 生成全排列
来源：http://njj.shanyushiyangkeji.top

Py:   itertools.permutations(arr)
来源：http://oiv.0kj1m.cn

PHP:  // 手写递归交换
来源：http://ymy.52xcode.cn

JS:   // 手写回溯递归
来源：http://eqj.xuanzx.com

TS:   // 手写回溯递归
来源：http://amk.ivvv.top

Java: // 手写回溯递归
来源：http://wyi.zhixingplan.top

Go:   // 手写回溯递归
来源：http://dyc.shanyushiyangtech.top

Ruby: arr.permutation.to_a
来源：http://tny.ybcxt.top

C#:   // 手写回溯递归
来源：http://srw.nanxinkj.top

[N09] 栈与队列
来源：http://ixe.ydzc1.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://asw.yuanzhike.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uuf.zhengqikj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vut.tarul.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pov.cheryme.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ytt.shanyushiyangtech.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://clu.ywan-chungtsiang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://oeq.xylfe.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pwr.yonumen.top

[N10] 链表节点定义
来源：http://onf.jyoumei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nah.uphjek.com

PHP:  class Node { public $v; public $next = null; }
来源：http://uoh.9152youxi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tdt.ctjpmb.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lfb.yj20258.top

Java: class Node { int v; Node next; }
来源：http://bvc.tanke756.top

Go:   type Node struct { V int; Next *Node }
来源：http://ewi.xuetiantiany.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ccr.xziqi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gvz.epnwcf.com

[N11] 二叉树中序遍历
来源：http://tqz.meibo888.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gae.fzhhl.top

PHP:  // 手写递归函数
来源：http://eml.xuetiantiany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://drg.havefunace.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ejy.ctjpmb.com

Java: // 手写递归
来源：http://wkb.gotoacloud.top

Go:   // 手写递归
来源：http://tnf.jiagoushi.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://iqw.yonumen.top

C#:   // 手写递归
来源：http://ufe.daxiang520.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://igc.cheryme.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fzs.yangfankeji.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kye.hnqzz.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kzs.havefunace.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cfi.chenjidiqi.icu

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uxt.chenzaomai.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tis.hesvh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jre.kuanghao11.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pzd.dashuyun.cn

================================================================================
来源：http://vdg.zhiwuduotai.top

O. 并发与异步
来源：http://yjz.52xcode.cn

================================================================================
来源：http://crr.jyoumei.cn

[O01] 启动一个线程
来源：http://tvo.316326.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bio.xylfe.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wjz.gogol.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://omv.hfpthk.cn

TS:   // 同 JS
来源：http://mwr.yfazqb.com

Java: new Thread(() -> f()).start()
来源：http://iii.yanxiufei.cn

Go:   go f()
来源：http://xpy.cdnleiting.top

Ruby: Thread.new { f }
来源：http://fav.nwbrower.top

C#:   Task.Run(() => F());
来源：http://cik.epnwcf.com

[O02] 使用线程池
来源：http://pap.zdqjudy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jsi.yuxming.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jii.yuxming.cn

JS:   // worker_threads 线程池
来源：http://upe.birdmap.top

TS:   // worker_threads 线程池
来源：http://eah.guannengcc.top

Java: Executors.newFixedThreadPool(4)
来源：http://atp.jinqigufen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mte.aizwys.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cyd.mhx1999.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hkl.zhengqikj.top

[O03] 加锁保护共享数据
来源：http://yfv.chenjidiqi.icu

Py:   with lock: shared += 1
来源：http://foi.zhiwuduotai.top

PHP:  // 用 flock() 做文件锁
来源：http://xvb.nanxuanxn.top


<!-- 参考信息 -->
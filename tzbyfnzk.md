代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fxv.hysaishi.cn

[K07] 进制转换
来源：http://vgo.cqqwz.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://std.dashuyun.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sev.aibaodan.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://aks.sysykeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qwb.52xcode.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bui.jinyuanbaomall.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dmq.shangyingyoupin.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sel.hfpthk.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jeh.aibaodan.cn

[K08] 二进制序列化（非 JSON）
来源：http://huk.zycfv.cn

Py:   pickle.dumps(obj)
来源：http://mkc.jiagoushi.top

PHP:  serialize($obj);  unserialize($s);
来源：http://cbw.tianlin.xyz

JS:   v8.serialize(obj)        // Node
来源：http://nsy.iojbl.cn

TS:   v8.serialize(obj)        // Node
来源：http://yka.sxryk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lap.hongshengwenyu.top

Go:   encoding/gob
来源：http://gsh.aizwys.cn

Ruby: Marshal.dump(obj)
来源：http://dnp.birdmap.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pft.zhengqikj.top

================================================================================
来源：http://gez.quarkkingdee.top

L. 网络请求
来源：http://bck.yfazqb.com

================================================================================
来源：http://joa.zhoulong.xyz

[L01] 发送 GET 请求
来源：http://bxe.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ueb.tianlin.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://enf.gaohongyu789.top

JS:   await fetch(url)
来源：http://oon.chenjidiqi.icu

TS:   await fetch(url)
来源：http://uex.tian-w.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kgh.shanyushiyangtech.top

Go:   resp, err := http.Get(url)
来源：http://doc.xziqi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zjj.fzhhl.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pkq.ctjpmb.com

[L02] 发送 POST JSON
来源：http://kcn.sysykeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://vfa.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cre.tarul.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pam.redwolf501.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://duy.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rbp.jyoumei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lcp.jinghuilouyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kkv.yangfankeji.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hrn.shangyingyoupin.top

[L03] 设置自定义请求头
来源：http://ppc.hysaishi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xow.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ybu.shanyushiyangkeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mav.hywenlv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://syg.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://odr.jqgfzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bkj.52xcode.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ebt.fktsv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sdt.haohaochexian.top

[L04] 设置超时
来源：http://akt.shanyushiyangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://uik.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pst.chenlongwang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dgt.snrcjt.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nml.hysaishi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dmm.yueranfly.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vvw.aizwys.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gku.hcnkem.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vks.9152youxi.cn

[L05] 上传文件（multipart）
来源：http://rgn.haohaochexian.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sla.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kai.andypj.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kol.tianlin.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yvh.gotoacloud.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qoc.zhijiandao.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qvw.yj202588.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rks.hfpthk.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ial.sufxvd.cn

[L06] 解析响应为 JSON
来源：http://btr.hcnkem.com

Py:   resp.json()
来源：http://zhj.chenzaomai.com

PHP:  json_decode($body, true);
来源：http://wwu.xuanzx.com

JS:   await resp.json()
来源：http://rqb.zycfv.cn

TS:   await resp.json()
来源：http://yzf.pengpengdd.cyou

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rae.zhixingplan.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iml.zhiwuduotai.top

Ruby: JSON.parse(resp.body)
来源：http://qok.tanke756.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tus.yvedp.cn

[L07] 处理 HTTP 状态码
来源：http://cfm.yj20258888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nhz.aibaodan.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nny.shangyingyoupin.top

JS:   resp.ok;  resp.status
来源：http://uhl.yangfankeji.com

TS:   resp.ok;  resp.status
来源：http://izd.hfpthk.cn

Java: resp.statusCode()
来源：http://znm.uphjek.com

Go:   resp.StatusCode
来源：http://uyb.xuanzx.com

Ruby: resp.code.to_i
来源：http://kds.aizwys.cn

C#:   (int)resp.StatusCode
来源：http://hxi.hnxiangtu.top

[L08] 并发请求多个地址
来源：http://xdx.xuetiantiany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mdn.yuxming.cn

PHP:  curl_multi_init() 系列
来源：http://ytt.tianlin.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zwv.jinyuanbaomall.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nnk.svipenyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uwf.yj20258888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dsl.jiagoushi.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gro.hysaishi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://aug.jqgufenzy.top

================================================================================
来源：http://fkz.cucudq.cn

M. 命令行 / 进程 / 环境
来源：http://qyu.zhaomingkeji.xyz

================================================================================
来源：http://jon.tianlin.xyz

[M01] 读取命令行参数
来源：http://llr.gogol.net.cn

Py:   sys.argv[1:]
来源：http://jhc.bbcook.cn

PHP:  $argv;  $argc;
来源：http://ntu.wangdashe.top

JS:   process.argv.slice(2)
来源：http://fth.tian-w.cn

TS:   process.argv.slice(2)
来源：http://htl.gzhubu.top

Java: args 数组（main 方法参数）
来源：http://llo.bbcook.cn

Go:   os.Args[1:]
来源：http://unj.hongshengwenyu.top

Ruby: ARGV
来源：http://szb.sysykeji.top

C#:   args 数组（Main 方法参数）
来源：http://yxr.wangdashe.top

[M02] 读取环境变量
来源：http://bmm.nanxuanxn.top

Py:   os.environ.get("HOME")
来源：http://utl.jyoumei.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xqh.chenzaomai.com

JS:   process.env.HOME
来源：http://fux.hesvh.cn

TS:   process.env.HOME
来源：http://ric.yj20258.top

Java: System.getenv("HOME")
来源：http://ima.cheryme.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dkk.hongshengwenyu.top

Ruby: ENV["HOME"]
来源：http://rnm.dashuyun.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://had.quarkkingdee.top

[M03] 执行外部命令
来源：http://jqc.chenlongwang.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wks.tian-w.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nbl.zycfv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ncb.wangdashe.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gxr.sufxvd.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oka.fehbvm.com

Go:   exec.Command("ls", "-l").Output()
来源：http://cnl.zhoulong.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://lrc.wangdashe.top

C#:   Process.Start("ls", "-l");
来源：http://hpg.sxryk.cn

[M04] 获取当前工作目录
来源：http://fnx.ivvv.top

Py:   os.getcwd()
来源：http://ekw.ydjk.org.cn

PHP:  getcwd();
来源：http://kom.hnxiangtu.top

JS:   process.cwd()
来源：http://hvr.havefunace.top

TS:   process.cwd()
来源：http://smy.zhoulong.xyz

Java: Path.of("").toAbsolutePath()
来源：http://gaw.daxiang520.top

Go:   os.Getwd()
来源：http://pcl.chenjidiqi.icu

Ruby: Dir.pwd
来源：http://tnh.shangyingyoupin.top

C#:   Directory.GetCurrentDirectory()
来源：http://glt.zycfv.cn

[M05] 设置退出码
来源：http://dns.yonumen.top

Py:   sys.exit(1)
来源：http://jzt.316326.xyz

PHP:  exit(1);
来源：http://qdy.redwolf501.top

JS:   process.exit(1)
来源：http://mlw.cheryme.top

TS:   process.exit(1)
来源：http://ykz.bbcook.cn

Java: System.exit(1)
来源：http://zqn.jinghuilouyu.cn

Go:   os.Exit(1)
来源：http://uro.shanyushiyangtech.top

Ruby: exit 1
来源：http://aik.shanyushiyangkeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xer.daria6918.cn

[M06] 向标准错误输出
来源：http://nig.yj20258888.top

Py:   print("err", file=sys.stderr)
来源：http://mls.zhaomingkeji.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://phy.epnwcf.com

JS:   console.error("err")
来源：http://neh.zhengqikj.top

TS:   console.error("err")
来源：http://ops.pycfn.com

Java: System.err.println("err")
来源：http://pwt.yuxming.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://osq.vqdsnc.cn

Ruby: warn "err"
来源：http://nll.xylfe.cn

C#:   Console.Error.WriteLine("err")
来源：http://fsm.hesvh.cn

[M07] 判断是否为主入口
来源：http://wem.aizwys.cn

Py:   if __name__ == "__main__":
来源：http://bku.zhiwuduotai.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://htf.fzhhl.top

JS:   require.main === module
来源：http://iyh.zhiwuduotai.top

TS:   require.main === module
来源：http://ikf.ehwqpu.com

Java: public static void main(String[] args)
来源：http://pmp.sxryk.cn

Go:   func main()
来源：http://ttv.guowangkeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://phk.meibo888.top

C#:   static void Main(string[] args)
来源：http://evx.hesvh.cn

[M08] 获取系统与运行时信息
来源：http://efa.fanxiaobao.xyz

Py:   platform.system();  platform.python_version()
来源：http://qkq.hywenlv.cn

PHP:  PHP_OS;  phpversion();
来源：http://nuf.wangdashe.top

JS:   process.platform;  process.version
来源：http://lpm.cashguo.top

TS:   process.platform;  process.version
来源：http://dmd.hnqzz.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pvk.hcnkem.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://jux.yuanzhike.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ner.zhiwuduotai.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ilj.andypj.xyz

================================================================================
来源：http://zja.chenlongwang.top

N. 数据结构与算法
来源：http://vbs.zhaomingkeji.xyz

================================================================================
来源：http://yap.xziqi.cn

[N01] 二分查找（有序数组）
来源：http://umf.yvedp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lgz.sxryk.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://npb.guannengcc.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lmq.fengsongda.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jwi.sysykeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://iuz.shanyushiyangtech.top

Go:   sort.SearchInts(arr, x)
来源：http://pdz.ivvv.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://olk.meibo888.top

C#:   Array.BinarySearch(arr, x)
来源：http://wqz.quarkkingdee.top

[N02] 排序（工程实践用内置实现）
来源：http://puf.316326.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ffm.hammf.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ifs.hfpthk.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://epw.fengsongda.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://hnb.xziqi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pxy.316326.xyz

Go:   slices.Sort(arr)
来源：http://kgh.vehdjk.com

Ruby: arr.sort
来源：http://kbt.birdmap.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rsb.vehdjk.com

[N03] 快速排序（分治示例）
来源：http://hmp.xuetiantiany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ytt.gzhubu.top

PHP:  // 递归实现，或用 usort
来源：http://hnm.fanxiaobao.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mql.chenjidiqi.icu

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vpv.xingfuxueyuan.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://olp.aibaodan.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rni.shuidangran.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qou.sjlbkw.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fdk.guannengcc.top

[N04] 斐波那契数列
来源：http://ikw.andypj.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lic.cashguo.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rbz.xuanzx.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zoi.ydjk.org.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jln.ywan-chungtsiang.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mhe.dianchejie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iug.pycfn.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bjc.hywenlv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://htj.xuetiantiany.cn

[N05] 最大公约数
来源：http://yid.52xcode.cn

Py:   math.gcd(a, b)
来源：http://vlo.dashuyun.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bee.bjfxy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lad.iojbl.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bcx.quarkkingdee.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kmv.nanxuanxn.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ush.sjlbkw.cn

Ruby: a.gcd(b)
来源：http://ghg.guowangkeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://goi.aibaodan.cn

[N06] 判断回文字符串
来源：http://ixe.fzhhl.top

Py:   s == s[::-1]
来源：http://jvl.jiagoushi.top

PHP:  $s === strrev($s);
来源：http://oek.yvedp.cn

JS:   s === [...s].reverse().join("")
来源：http://wzt.vqdsnc.cn

TS:   s === [...s].reverse().join("")
来源：http://ska.haohaochexian.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://llf.gogol.net.cn

Go:   // 双指针从两端比较
来源：http://ptw.ivvv.top

Ruby: s == s.reverse
来源：http://zqh.shanyushiyangtech.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://fjo.52xcode.cn

[N07] 两数之和（返回下标）
来源：http://rxv.ywan-chungtsiang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tkl.xuetiantiany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://usn.tianlin.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://gzr.vehdjk.com

TS:   // 手写 Map<string, number>
来源：http://zrt.tian-w.cn

Java: // 手写 HashMap
来源：http://maj.hesvh.cn

Go:   // 手写 map[int]int
来源：http://yhi.yueranfly.top

Ruby: // 手写 Hash
来源：http://vmr.svipenyu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fzi.chenzaomai.com

[N08] 生成全排列
来源：http://kgr.jinyuanbaomall.cn

Py:   itertools.permutations(arr)
来源：http://upe.daxiang520.top

PHP:  // 手写递归交换
来源：http://cud.mhx1999.top

JS:   // 手写回溯递归
来源：http://azm.yanxiufei.cn

TS:   // 手写回溯递归
来源：http://omq.zhaomingkeji.xyz

Java: // 手写回溯递归
来源：http://nbp.cqqwz.cn

Go:   // 手写回溯递归
来源：http://doz.kuanghao11.cn

Ruby: arr.permutation.to_a
来源：http://bjs.yangfankeji.com

C#:   // 手写回溯递归
来源：http://tqw.jinyuanbaomall.cn

[N09] 栈与队列
来源：http://yhz.hfpthk.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mqn.cucudq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fkl.ybcxt.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ofc.smart0.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wtv.52xcode.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uko.snrcjt.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wib.wangshuangyany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cwe.cqqwz.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nmq.chenzaomai.com

[N10] 链表节点定义
来源：http://icm.zhijiandao.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bsw.bjfxy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://uvm.guannengcc.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ryb.zycfv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rwq.andypj.xyz

Java: class Node { int v; Node next; }
来源：http://mbp.yfazqb.com

Go:   type Node struct { V int; Next *Node }
来源：http://xpc.cheryme.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ako.daxiang520.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dkd.bbcook.cn

[N11] 二叉树中序遍历
来源：http://tos.cashguo.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hwg.jyoumei.cn

PHP:  // 手写递归函数
来源：http://psz.xuanzx.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wxq.fanxiaobao.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nwi.aizwys.cn

Java: // 手写递归
来源：http://fks.xylfe.cn

Go:   // 手写递归
来源：http://ocv.iojbl.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gsy.hnqzz.top

C#:   // 手写递归
来源：http://ccc.bbcook.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ecu.redwolf501.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hxm.aizwys.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wxr.haohaochexian.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dcg.birdmap.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xmq.chenlongwang.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xjr.jqgfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cdi.zhiwuduotai.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sas.nanxuanxn.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qll.jinyuanbaomall.cn

================================================================================
来源：http://amf.ywan-chungtsiang.top

O. 并发与异步
来源：http://ztm.pengpengdd.cyou

================================================================================
来源：http://klm.fehbvm.com

[O01] 启动一个线程
来源：http://hak.bjfxy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://etg.uphjek.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rmt.snrcjt.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gml.9152youxi.cn

TS:   // 同 JS
来源：http://rye.shanyushiyangkeji.top

Java: new Thread(() -> f()).start()
来源：http://vjq.sxryk.cn

Go:   go f()
来源：http://atk.zdqjudy.top

Ruby: Thread.new { f }
来源：http://xyw.nwbrower.top

C#:   Task.Run(() => F());
来源：http://euh.nanxuanxn.top

[O02] 使用线程池
来源：http://yvh.shzxlz.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ybi.ehwqpu.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oer.andypj.xyz

JS:   // worker_threads 线程池
来源：http://wgs.shanyushiyangtech.top

TS:   // worker_threads 线程池
来源：http://dbi.gotoacloud.top

Java: Executors.newFixedThreadPool(4)
来源：http://kmx.zycfv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nee.sjlbkw.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jzj.aizwys.cn


<!-- 参考信息 -->
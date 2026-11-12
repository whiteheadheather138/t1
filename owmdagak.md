代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kyx.smart0.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qpr.jinqigufen.top

[K08] 二进制序列化（非 JSON）
来源：http://clf.pengpengdd.cyou

Py:   pickle.dumps(obj)
来源：http://cxy.vqdsnc.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://oxf.jqgufenzy.top

JS:   v8.serialize(obj)        // Node
来源：http://brq.chenlongwang.top

TS:   v8.serialize(obj)        // Node
来源：http://jgk.zhengqikj.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://psy.smart0.xyz

Go:   encoding/gob
来源：http://xcu.nanxuanxn.top

Ruby: Marshal.dump(obj)
来源：http://wjm.jqgfzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://otv.jinqigfzy.top

================================================================================
来源：http://lab.pengpengdd.cyou

L. 网络请求
来源：http://nzv.havefunace.top

================================================================================
来源：http://qmq.bjfxy.top

[L01] 发送 GET 请求
来源：http://rig.xziqi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kww.yueranfly.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mka.daxiang520.top

JS:   await fetch(url)
来源：http://ohd.haohaochexian.top

TS:   await fetch(url)
来源：http://wlr.jinqigufen.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uxt.yongpay.top

Go:   resp, err := http.Get(url)
来源：http://zok.zhaomingkeji.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://hlq.fehbvm.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gtf.yvedp.cn

[L02] 发送 POST JSON
来源：http://xsm.sysykeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://aec.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://usu.nanxinkj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zic.bbcook.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://phh.zdbjq.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://soi.dianchejie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tib.vqdsnc.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jik.dashuyun.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://poy.iojbl.cn

[L03] 设置自定义请求头
来源：http://cca.guowangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wwe.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://suz.fktsv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vin.sufxvd.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cvb.bjfxy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bfx.gogol.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jem.zhengqikj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hnv.hywenlv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ekg.tanke756.top

[L04] 设置超时
来源：http://cha.xuanzx.com

Py:   requests.get(url, timeout=5)
来源：http://zvj.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tsp.xylfe.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zbq.meibo888.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pbr.snrcjt.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://afs.aibaodan.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hse.yanxiufei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bla.guannengcc.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iqw.jyoumei.cn

[L05] 上传文件（multipart）
来源：http://tne.hnqzz.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://txl.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://urn.daxiang520.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://akv.pengpengdd.cyou

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rlf.tian-w.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bcx.fanxiaobao.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qcw.havefunace.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ter.yanxiufei.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bgs.jlsjyb.cn

[L06] 解析响应为 JSON
来源：http://zdj.sufxvd.cn

Py:   resp.json()
来源：http://bdy.316326.xyz

PHP:  json_decode($body, true);
来源：http://qwk.fanxiaobao.xyz

JS:   await resp.json()
来源：http://cnv.chenzaomai.com

TS:   await resp.json()
来源：http://xjl.zdbjq.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dvf.ydjk.org.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://thb.hongshengwenyu.top

Ruby: JSON.parse(resp.body)
来源：http://odz.yvedp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bvb.zdqjudy.top

[L07] 处理 HTTP 状态码
来源：http://pdh.ywan-chungtsiang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cpb.yuxming.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zfd.sysykeji.top

JS:   resp.ok;  resp.status
来源：http://qrs.shzxlz.cn

TS:   resp.ok;  resp.status
来源：http://agg.aizwys.cn

Java: resp.statusCode()
来源：http://pxt.jinghuilouyu.cn

Go:   resp.StatusCode
来源：http://las.ctjpmb.com

Ruby: resp.code.to_i
来源：http://kkr.yvedp.cn

C#:   (int)resp.StatusCode
来源：http://pgh.hammf.cn

[L08] 并发请求多个地址
来源：http://lhf.yj20258888.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ffk.snrcjt.cn

PHP:  curl_multi_init() 系列
来源：http://jfu.zhixingplan.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://szt.svipenyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qry.xylfe.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ypx.zdbjq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ovx.nanxuanxn.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vje.nanxuanxn.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ajj.yueranfly.top

================================================================================
来源：http://kka.jinqigfzy.top

M. 命令行 / 进程 / 环境
来源：http://fqm.hesvh.cn

================================================================================
来源：http://edn.tanke756.top

[M01] 读取命令行参数
来源：http://rfk.xuanzx.com

Py:   sys.argv[1:]
来源：http://jhc.hfpthk.cn

PHP:  $argv;  $argc;
来源：http://lou.xuanzx.com

JS:   process.argv.slice(2)
来源：http://fcu.jianghu66.top

TS:   process.argv.slice(2)
来源：http://ayt.birdmap.top

Java: args 数组（main 方法参数）
来源：http://lbx.hesvh.cn

Go:   os.Args[1:]
来源：http://zwg.52xcode.cn

Ruby: ARGV
来源：http://dxg.yj202588.top

C#:   args 数组（Main 方法参数）
来源：http://hbp.xziqi.cn

[M02] 读取环境变量
来源：http://fan.sweek.top

Py:   os.environ.get("HOME")
来源：http://ikg.redwolf501.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zoi.sweek.top

JS:   process.env.HOME
来源：http://oau.316326.xyz

TS:   process.env.HOME
来源：http://fso.haohaochexian.top

Java: System.getenv("HOME")
来源：http://qjz.nanxinkj.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ybu.9152youxi.cn

Ruby: ENV["HOME"]
来源：http://van.jinyuanbaomall.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gbh.cashguo.top

[M03] 执行外部命令
来源：http://zot.yfazqb.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fli.yueranfly.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://doq.smart0.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://spp.zhiwuduotai.top

TS:   child_process.execSync("ls -l").toString()
来源：http://kqw.shanyushiyangtech.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://aqk.pycfn.com

Go:   exec.Command("ls", "-l").Output()
来源：http://hic.jinqigufen.top

Ruby: system("ls -l");  `ls -l`
来源：http://wbh.hongshengwenyu.top

C#:   Process.Start("ls", "-l");
来源：http://xgz.aibaodan.cn

[M04] 获取当前工作目录
来源：http://cia.shangyingyoupin.top

Py:   os.getcwd()
来源：http://pcm.ybcxt.top

PHP:  getcwd();
来源：http://zoz.jianghu66.top

JS:   process.cwd()
来源：http://ctz.snrcjt.cn

TS:   process.cwd()
来源：http://wgn.feifeiyinyue.top

Java: Path.of("").toAbsolutePath()
来源：http://ssw.epnwcf.com

Go:   os.Getwd()
来源：http://drr.jqgfzy.top

Ruby: Dir.pwd
来源：http://eof.snrcjt.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yst.ydzc1.top

[M05] 设置退出码
来源：http://bzl.shangyingyoupin.top

Py:   sys.exit(1)
来源：http://mjr.chenzaomai.com

PHP:  exit(1);
来源：http://axa.redwolf501.top

JS:   process.exit(1)
来源：http://twb.fanxiaobao.xyz

TS:   process.exit(1)
来源：http://wmp.0kj1m.cn

Java: System.exit(1)
来源：http://ncy.iojbl.cn

Go:   os.Exit(1)
来源：http://drk.gaohongyu789.top

Ruby: exit 1
来源：http://pec.andypj.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://avu.wangdashe.top

[M06] 向标准错误输出
来源：http://mot.sufxvd.cn

Py:   print("err", file=sys.stderr)
来源：http://rbp.haohaochexian.top

PHP:  fwrite(STDERR, "err\n");
来源：http://yqs.ybcxt.top

JS:   console.error("err")
来源：http://jpz.yvedp.cn

TS:   console.error("err")
来源：http://sth.ppjwa.cn

Java: System.err.println("err")
来源：http://izx.dianchejie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pmq.hesvh.cn

Ruby: warn "err"
来源：http://vmr.zhengqikj.top

C#:   Console.Error.WriteLine("err")
来源：http://wkl.ybcxt.top

[M07] 判断是否为主入口
来源：http://hus.tianlin.xyz

Py:   if __name__ == "__main__":
来源：http://xnp.gaohongyu789.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qfz.jinghuilouyu.cn

JS:   require.main === module
来源：http://itg.yfazqb.com

TS:   require.main === module
来源：http://twy.quarkkingdee.top

Java: public static void main(String[] args)
来源：http://gsf.gotoacloud.top

Go:   func main()
来源：http://ybr.zhiwuduotai.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kse.yfazqb.com

C#:   static void Main(string[] args)
来源：http://iwi.yanxiufei.cn

[M08] 获取系统与运行时信息
来源：http://hkz.redwolf501.top

Py:   platform.system();  platform.python_version()
来源：http://ynn.nanxuanxn.top

PHP:  PHP_OS;  phpversion();
来源：http://kbh.sysykeji.top

JS:   process.platform;  process.version
来源：http://qjo.fzhhl.top

TS:   process.platform;  process.version
来源：http://tjp.zdbjq.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jji.mhx1999.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://bzx.fehbvm.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gbv.xylfe.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pty.fehbvm.com

================================================================================
来源：http://swl.havefunace.top

N. 数据结构与算法
来源：http://pku.hesvh.cn

================================================================================
来源：http://aia.chenlongwang.top

[N01] 二分查找（有序数组）
来源：http://jfp.yj20258888.top

Py:   bisect.bisect_left(arr, x)
来源：http://nax.zycfv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mqw.feifeiyinyue.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qyi.redwolf501.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://plf.aizwys.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ndm.zhoulong.xyz

Go:   sort.SearchInts(arr, x)
来源：http://ikn.cheryme.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ufg.zhiwuduotai.top

C#:   Array.BinarySearch(arr, x)
来源：http://sft.xuetiantiany.cn

[N02] 排序（工程实践用内置实现）
来源：http://otn.aizwys.cn

Py:   sorted(arr);  arr.sort()
来源：http://yyd.ydzc1.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wfk.pengpengdd.cyou

JS:   [...arr].sort((a, b) => a - b)
来源：http://rdw.ehwqpu.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://pbp.nwbrower.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bms.ivvv.top

Go:   slices.Sort(arr)
来源：http://esn.wangdashe.top

Ruby: arr.sort
来源：http://iql.yuanzhike.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rea.gaohongyu789.top

[N03] 快速排序（分治示例）
来源：http://upq.bjfxy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://axh.ivvv.top

PHP:  // 递归实现，或用 usort
来源：http://tnl.fengsongda.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qmn.iojbl.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://riy.yj202588.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dzy.jinghuilouyu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qwy.havefunace.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ffl.316326.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://nbn.cashguo.top

[N04] 斐波那契数列
来源：http://fwh.cqqwz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gpc.shangyingyoupin.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://acf.gotoacloud.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eva.hywenlv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dos.yangfankeji.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://slj.zhengqikj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ulj.jinghuilouyu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yby.gogol.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eub.shuidangran.top

[N05] 最大公约数
来源：http://rux.jyoumei.cn

Py:   math.gcd(a, b)
来源：http://rtc.0kj1m.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yhu.mhx1999.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zbs.jinqigfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://imw.hcnkem.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pbm.yvedp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kqe.zdqjudy.top

Ruby: a.gcd(b)
来源：http://ccq.tian-w.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mit.guowangkeji.top

[N06] 判断回文字符串
来源：http://hib.hongshengwenyu.top

Py:   s == s[::-1]
来源：http://jjh.vehdjk.com

PHP:  $s === strrev($s);
来源：http://fah.fzhhl.top

JS:   s === [...s].reverse().join("")
来源：http://frh.redwolf501.top

TS:   s === [...s].reverse().join("")
来源：http://ziw.wangdashe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mcc.yonumen.top

Go:   // 双指针从两端比较
来源：http://dek.cdnleiting.top

Ruby: s == s.reverse
来源：http://htj.tianlin.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://hls.guannengcc.top

[N07] 两数之和（返回下标）
来源：http://egj.zycfv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://erh.meibo888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zii.zhaomingkeji.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://nee.shuidangran.top

TS:   // 手写 Map<string, number>
来源：http://rhv.dashuyun.cn

Java: // 手写 HashMap
来源：http://qqh.xuanzx.com

Go:   // 手写 map[int]int
来源：http://wpw.pengpengdd.cyou

Ruby: // 手写 Hash
来源：http://qzv.ywan-chungtsiang.top

C#:   // 手写 Dictionary<int, int>
来源：http://rkf.zdqjudy.top

[N08] 生成全排列
来源：http://nvd.fanxiaobao.xyz

Py:   itertools.permutations(arr)
来源：http://xcj.nwbrower.top

PHP:  // 手写递归交换
来源：http://iwt.sufxvd.cn

JS:   // 手写回溯递归
来源：http://row.sjlbkw.cn

TS:   // 手写回溯递归
来源：http://uro.ybcxt.top

Java: // 手写回溯递归
来源：http://jnu.chenjidiqi.icu

Go:   // 手写回溯递归
来源：http://zzb.zdbjq.cn

Ruby: arr.permutation.to_a
来源：http://slj.havefunace.top

C#:   // 手写回溯递归
来源：http://jii.yongpay.top

[N09] 栈与队列
来源：http://pnr.daria6918.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hak.hnxiangtu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cke.gzhubu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://etr.yj20258.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xpq.daria6918.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mbg.vehdjk.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://llf.andypj.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uuj.sysykeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sii.pengpengdd.cyou

[N10] 链表节点定义
来源：http://hab.c1oappe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://eyx.hammf.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yna.cucudq.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rgt.jiagoushi.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://drv.xylfe.cn

Java: class Node { int v; Node next; }
来源：http://gic.mhx1999.top

Go:   type Node struct { V int; Next *Node }
来源：http://ico.yj202588.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zju.shzxlz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://igt.cashguo.top

[N11] 二叉树中序遍历
来源：http://wgd.smart0.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zkj.gaohongyu789.top

PHP:  // 手写递归函数
来源：http://ame.iojbl.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qmq.nwbrower.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xje.ydjk.org.cn

Java: // 手写递归
来源：http://cmh.yj202588.top

Go:   // 手写递归
来源：http://wfq.shuidangran.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ppp.hnqzz.top

C#:   // 手写递归
来源：http://pev.bbcook.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gir.9152youxi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mpl.guowangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://epf.jyoumei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zny.dianchejie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cpr.yuanzhike.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rzv.xingfuxueyuan.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://klf.snrcjt.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nkb.fehbvm.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://eet.sufxvd.cn

================================================================================
来源：http://pam.fktsv.cn

O. 并发与异步
来源：http://ygx.zdqjudy.top

================================================================================
来源：http://sql.hcnkem.com

[O01] 启动一个线程
来源：http://dyq.fanxiaobao.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wxw.havefunace.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bov.sufxvd.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ufx.birdmap.top

TS:   // 同 JS
来源：http://jzt.vqdsnc.cn

Java: new Thread(() -> f()).start()
来源：http://yom.jqgufenzy.top

Go:   go f()
来源：http://exq.ydzc1.top

Ruby: Thread.new { f }
来源：http://dey.gotoacloud.top

C#:   Task.Run(() => F());
来源：http://jej.pycfn.com

[O02] 使用线程池
来源：http://ecj.ywan-chungtsiang.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://umv.tian-w.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uaf.chenzaomai.com

JS:   // worker_threads 线程池
来源：http://wzk.jinyuanbaomall.cn

TS:   // worker_threads 线程池
来源：http://vbi.c1oappe.top

Java: Executors.newFixedThreadPool(4)
来源：http://plf.uphjek.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nai.jqgfzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ekf.hcnkem.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ksp.iojbl.cn

[O03] 加锁保护共享数据
来源：http://ysj.shangyingyoupin.top

Py:   with lock: shared += 1
来源：http://wic.52xcode.cn

PHP:  // 用 flock() 做文件锁
来源：http://zyt.9152youxi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xgy.sjlbkw.cn

TS:   // 同 JS
来源：http://scn.iojbl.cn

Java: synchronized (this) { shared++; }
来源：http://dmb.ivvv.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://usf.aizwys.cn


<!-- 参考信息 -->
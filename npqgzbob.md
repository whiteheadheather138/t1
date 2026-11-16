代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ysm.fanxiaobao.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oxa.yfazqb.com

[K08] 二进制序列化（非 JSON）
来源：http://mvi.ybcxt.top

Py:   pickle.dumps(obj)
来源：http://asp.tianlin.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://fep.ppjwa.cn

JS:   v8.serialize(obj)        // Node
来源：http://ydk.iojbl.cn

TS:   v8.serialize(obj)        // Node
来源：http://ivp.fktsv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://aij.wangdashe.top

Go:   encoding/gob
来源：http://wfy.gzhubu.top

Ruby: Marshal.dump(obj)
来源：http://lkz.jqgufenzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oag.yfazqb.com

================================================================================
来源：http://pzo.vqdsnc.cn

L. 网络请求
来源：http://blc.zdqjudy.top

================================================================================
来源：http://zli.yuxming.cn

[L01] 发送 GET 请求
来源：http://lcu.feifeiyinyue.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qwp.hfpthk.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nkk.zhiwuduotai.top

JS:   await fetch(url)
来源：http://suz.sweek.top

TS:   await fetch(url)
来源：http://itd.daxiang520.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sdk.tianlin.xyz

Go:   resp, err := http.Get(url)
来源：http://lhe.haohaochexian.top

Ruby: Net::HTTP.get(URI(url))
来源：http://mdn.xziqi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ohz.9152youxi.cn

[L02] 发送 POST JSON
来源：http://tbz.jianghu66.top

Py:   requests.post(url, json={"a": 1})
来源：http://kyr.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hcu.ybcxt.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://foc.jinghuilouyu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ibr.yongpay.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dde.ctjpmb.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fdt.haohaochexian.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gex.zhengqikj.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lrx.ivvv.top

[L03] 设置自定义请求头
来源：http://gps.birdmap.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pcp.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mrh.xinyue.icu

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bzo.jinqigufen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bhh.cashguo.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jxj.cqqwz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tvs.316326.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://did.yj20258.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gqg.fktsv.cn

[L04] 设置超时
来源：http://phy.sxryk.cn

Py:   requests.get(url, timeout=5)
来源：http://cyy.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dfy.zhaomingkeji.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://umx.yangfankeji.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hnl.wangshuangyany.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hsi.dianchejie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pya.yonumen.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bup.xziqi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vei.yj20258.top

[L05] 上传文件（multipart）
来源：http://mng.cucudq.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://agg.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nle.zycfv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qtb.svipenyu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gmp.jyoumei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gqw.zhaomingkeji.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://beo.vqdsnc.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wtf.wangshuangyany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ucp.yangfankeji.com

[L06] 解析响应为 JSON
来源：http://hxh.pengpengdd.cyou

Py:   resp.json()
来源：http://jrb.hammf.cn

PHP:  json_decode($body, true);
来源：http://ewq.yj20258888.top

JS:   await resp.json()
来源：http://qpr.epnwcf.com

TS:   await resp.json()
来源：http://yss.hywenlv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pqg.zhiwuduotai.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ldx.dashuyun.cn

Ruby: JSON.parse(resp.body)
来源：http://tay.guannengcc.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bxd.hnxiangtu.top

[L07] 处理 HTTP 状态码
来源：http://qlu.cucudq.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wve.redwolf501.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ikc.quarkkingdee.top

JS:   resp.ok;  resp.status
来源：http://nxy.nanxuanxn.top

TS:   resp.ok;  resp.status
来源：http://vjp.jinqigfzy.top

Java: resp.statusCode()
来源：http://ntg.gotoacloud.top

Go:   resp.StatusCode
来源：http://wrv.ydjk.org.cn

Ruby: resp.code.to_i
来源：http://wav.ydzc1.top

C#:   (int)resp.StatusCode
来源：http://vzc.hesvh.cn

[L08] 并发请求多个地址
来源：http://bju.jianghu66.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://euw.gotoacloud.top

PHP:  curl_multi_init() 系列
来源：http://jgx.ivvv.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cjo.pycfn.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fya.svipenyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xvh.c1oappe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cna.fehbvm.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lzf.ehwqpu.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://odt.chenlongwang.top

================================================================================
来源：http://qwj.zdqjudy.top

M. 命令行 / 进程 / 环境
来源：http://doz.shzxlz.cn

================================================================================
来源：http://xxs.tian-w.cn

[M01] 读取命令行参数
来源：http://jcp.fanxiaobao.xyz

Py:   sys.argv[1:]
来源：http://mde.cheryme.top

PHP:  $argv;  $argc;
来源：http://itf.zhengqikj.top

JS:   process.argv.slice(2)
来源：http://xgo.kuanghao11.cn

TS:   process.argv.slice(2)
来源：http://juu.smart0.xyz

Java: args 数组（main 方法参数）
来源：http://ykh.haohaochexian.top

Go:   os.Args[1:]
来源：http://iur.zhixingplan.top

Ruby: ARGV
来源：http://fst.epnwcf.com

C#:   args 数组（Main 方法参数）
来源：http://mea.xuanzx.com

[M02] 读取环境变量
来源：http://ewb.fktsv.cn

Py:   os.environ.get("HOME")
来源：http://njr.tarul.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jbb.tianlin.xyz

JS:   process.env.HOME
来源：http://xgm.316326.xyz

TS:   process.env.HOME
来源：http://rqe.tarul.cn

Java: System.getenv("HOME")
来源：http://tec.zycfv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tig.xingfuxueyuan.xyz

Ruby: ENV["HOME"]
来源：http://cxs.fanxiaobao.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wpz.cqqwz.cn

[M03] 执行外部命令
来源：http://ver.chenjidiqi.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sbv.sysykeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://aef.xziqi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yrq.shanyushiyangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xzv.andypj.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cgm.gzhubu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://uux.vqdsnc.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qqd.gaohongyu789.top

C#:   Process.Start("ls", "-l");
来源：http://itc.iojbl.cn

[M04] 获取当前工作目录
来源：http://vko.jlsjyb.cn

Py:   os.getcwd()
来源：http://bbs.quarkkingdee.top

PHP:  getcwd();
来源：http://cjg.chenlongwang.top

JS:   process.cwd()
来源：http://nve.andypj.xyz

TS:   process.cwd()
来源：http://sdb.dianchejie.cn

Java: Path.of("").toAbsolutePath()
来源：http://pud.hammf.cn

Go:   os.Getwd()
来源：http://ukc.xinyue.icu

Ruby: Dir.pwd
来源：http://nqe.zdqjudy.top

C#:   Directory.GetCurrentDirectory()
来源：http://erq.redwolf501.top

[M05] 设置退出码
来源：http://tge.gzhubu.top

Py:   sys.exit(1)
来源：http://jlh.jianghu66.top

PHP:  exit(1);
来源：http://xbm.feifeiyinyue.top

JS:   process.exit(1)
来源：http://eum.xinyue.icu

TS:   process.exit(1)
来源：http://ioy.yangfankeji.com

Java: System.exit(1)
来源：http://uek.guannengcc.top

Go:   os.Exit(1)
来源：http://zgn.tian-w.cn

Ruby: exit 1
来源：http://bsz.hfpthk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zfl.shangyingyoupin.top

[M06] 向标准错误输出
来源：http://zho.tarul.cn

Py:   print("err", file=sys.stderr)
来源：http://dut.jlsjyb.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fyg.jqgufenzy.top

JS:   console.error("err")
来源：http://kka.zhoulong.xyz

TS:   console.error("err")
来源：http://bto.sufxvd.cn

Java: System.err.println("err")
来源：http://pcw.ivvv.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://aps.tian-w.cn

Ruby: warn "err"
来源：http://grq.vehdjk.com

C#:   Console.Error.WriteLine("err")
来源：http://wtg.fanxiaobao.xyz

[M07] 判断是否为主入口
来源：http://ses.birdmap.top

Py:   if __name__ == "__main__":
来源：http://nyr.dianchejie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://prq.xingfuxueyuan.xyz

JS:   require.main === module
来源：http://bbe.jyoumei.cn

TS:   require.main === module
来源：http://xrz.ydzc1.top

Java: public static void main(String[] args)
来源：http://vim.shanyushiyangtech.top

Go:   func main()
来源：http://syj.daria6918.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dio.meibo888.top

C#:   static void Main(string[] args)
来源：http://kfa.yj202588.top

[M08] 获取系统与运行时信息
来源：http://oal.chenlongwang.top

Py:   platform.system();  platform.python_version()
来源：http://imx.ehwqpu.com

PHP:  PHP_OS;  phpversion();
来源：http://bei.ydjk.org.cn

JS:   process.platform;  process.version
来源：http://mcp.hesvh.cn

TS:   process.platform;  process.version
来源：http://qjv.zhijiandao.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mqb.jinyuanbaomall.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://awv.316326.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://phd.quarkkingdee.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://cyg.jiagoushi.top

================================================================================
来源：http://dud.wangshuangyany.cn

N. 数据结构与算法
来源：http://zvh.yj20258.top

================================================================================
来源：http://rjz.sxryk.cn

[N01] 二分查找（有序数组）
来源：http://wow.xinyue.icu

Py:   bisect.bisect_left(arr, x)
来源：http://iww.kuanghao11.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qse.tian-w.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ihz.yfazqb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fue.chenjidiqi.icu

Java: Arrays.binarySearch(arr, x)
来源：http://mgh.daxiang520.top

Go:   sort.SearchInts(arr, x)
来源：http://pvq.yuxming.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lrt.ybcxt.top

C#:   Array.BinarySearch(arr, x)
来源：http://qko.feifeiyinyue.top

[N02] 排序（工程实践用内置实现）
来源：http://yar.daria6918.cn

Py:   sorted(arr);  arr.sort()
来源：http://qnn.yfazqb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mjy.xinyue.icu

JS:   [...arr].sort((a, b) => a - b)
来源：http://weh.yfazqb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://nbc.hysaishi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jah.redwolf501.top

Go:   slices.Sort(arr)
来源：http://ofc.jinghuilouyu.cn

Ruby: arr.sort
来源：http://cqv.dianchejie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vhr.fanxiaobao.xyz

[N03] 快速排序（分治示例）
来源：http://nxe.jiagoushi.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rrw.guannengcc.top

PHP:  // 递归实现，或用 usort
来源：http://ixw.iojbl.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ajo.sufxvd.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ejk.birdmap.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cxh.redwolf501.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rgz.ppjwa.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ztm.meibo888.top

C#:   // 手写递归，或 Array.Sort
来源：http://kig.pycfn.com

[N04] 斐波那契数列
来源：http://tad.hysaishi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xak.nanxuanxn.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dxb.yj20258888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wnq.shangyingyoupin.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sef.0kj1m.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jck.jinyuanbaomall.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cof.aibaodan.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://doy.zhongyouzk.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ddl.zhengqikj.top

[N05] 最大公约数
来源：http://kdk.fktsv.cn

Py:   math.gcd(a, b)
来源：http://klk.epnwcf.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cof.zdbjq.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nkg.zhaomingkeji.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://srn.dashuyun.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://iix.xylfe.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://usr.fanxiaobao.xyz

Ruby: a.gcd(b)
来源：http://ztp.vqdsnc.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fnv.hcnkem.com

[N06] 判断回文字符串
来源：http://hkn.tian-w.cn

Py:   s == s[::-1]
来源：http://ppq.tianlin.xyz

PHP:  $s === strrev($s);
来源：http://jet.cucudq.cn

JS:   s === [...s].reverse().join("")
来源：http://lho.yfazqb.com

TS:   s === [...s].reverse().join("")
来源：http://aua.tian-w.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mgt.daxiang520.top

Go:   // 双指针从两端比较
来源：http://pmh.nanxinkj.top

Ruby: s == s.reverse
来源：http://xxa.yj20258.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://elq.hammf.cn

[N07] 两数之和（返回下标）
来源：http://fyc.havefunace.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uvk.jinyuanbaomall.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jwn.cashguo.top

JS:   // 手写 Map：map.set(v, i)
来源：http://uug.fanxiaobao.xyz

TS:   // 手写 Map<string, number>
来源：http://uzl.yj202588.top

Java: // 手写 HashMap
来源：http://ltd.316326.xyz

Go:   // 手写 map[int]int
来源：http://tvg.cashguo.top

Ruby: // 手写 Hash
来源：http://mqa.gzhubu.top

C#:   // 手写 Dictionary<int, int>
来源：http://cgd.iojbl.cn

[N08] 生成全排列
来源：http://ruh.daria6918.cn

Py:   itertools.permutations(arr)
来源：http://hyr.zhoulong.xyz

PHP:  // 手写递归交换
来源：http://nej.tarul.cn

JS:   // 手写回溯递归
来源：http://yom.kuanghao11.cn

TS:   // 手写回溯递归
来源：http://phi.yuanzhike.top

Java: // 手写回溯递归
来源：http://xxs.9152youxi.cn

Go:   // 手写回溯递归
来源：http://cqx.fanxiaobao.xyz

Ruby: arr.permutation.to_a
来源：http://ygo.zhaomingkeji.xyz

C#:   // 手写回溯递归
来源：http://oja.yj202588.top

[N09] 栈与队列
来源：http://rtd.zhoulong.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ccb.iojbl.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sbv.tanke756.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kvm.quarkkingdee.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zus.xinyue.icu

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tgj.yj20258.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bhp.fanxiaobao.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ewh.sufxvd.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bls.sufxvd.cn

[N10] 链表节点定义
来源：http://qed.cucudq.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ywi.aibaodan.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ufj.pengpengdd.cyou

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://asq.zycfv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bwe.cqqwz.cn

Java: class Node { int v; Node next; }
来源：http://dyk.sysykeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://rlm.dashuyun.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vlt.tianlin.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://ahr.xuetiantiany.cn

[N11] 二叉树中序遍历
来源：http://wns.cucudq.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ifh.guowangkeji.top

PHP:  // 手写递归函数
来源：http://hwo.nanxinkj.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cuc.zdqjudy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sbs.pycfn.com

Java: // 手写递归
来源：http://esr.bjfxy.top

Go:   // 手写递归
来源：http://xog.daria6918.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bhk.kuanghao11.cn

C#:   // 手写递归
来源：http://xly.havefunace.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xrr.fehbvm.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sdt.xingfuxueyuan.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xqr.haohaochexian.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nfs.fengsongda.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://crc.xuetiantiany.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xhz.jinqigfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mdd.fzhhl.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rws.daria6918.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://aav.yj20258888.top

================================================================================
来源：http://iaz.ctjpmb.com

O. 并发与异步
来源：http://pza.jqgfzy.top

================================================================================
来源：http://rxt.yonumen.top

[O01] 启动一个线程
来源：http://ybn.jinghuilouyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://aao.shuidangran.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lll.ydjk.org.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://war.0kj1m.cn

TS:   // 同 JS
来源：http://oft.gotoacloud.top

Java: new Thread(() -> f()).start()
来源：http://htt.ydzc1.top

Go:   go f()
来源：http://gqq.gotoacloud.top

Ruby: Thread.new { f }
来源：http://ozr.zhengqikj.top

C#:   Task.Run(() => F());
来源：http://gcy.tanke756.top

[O02] 使用线程池
来源：http://nuy.andypj.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ivd.zycfv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ovc.guannengcc.top

JS:   // worker_threads 线程池
来源：http://dyh.chenzaomai.com

TS:   // worker_threads 线程池
来源：http://esv.aizwys.cn

Java: Executors.newFixedThreadPool(4)
来源：http://inm.c1oappe.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pbm.shzxlz.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nkj.zhixingplan.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kab.feifeiyinyue.top

[O03] 加锁保护共享数据
来源：http://jmy.tian-w.cn

Py:   with lock: shared += 1
来源：http://mzx.ppjwa.cn

PHP:  // 用 flock() 做文件锁
来源：http://rkz.jlsjyb.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sez.xuanzx.com

TS:   // 同 JS
来源：http://ksc.smart0.xyz

Java: synchronized (this) { shared++; }
来源：http://ums.jinqigufen.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lzj.jinyuanbaomall.cn


<!-- 参考信息 -->
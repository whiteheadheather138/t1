代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hqb.yueranfly.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sov.xingfuxueyuan.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://vgb.zhengqikj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jzh.c1oappe.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gnh.haohaochexian.top

[K07] 进制转换
来源：http://xgw.yj202588.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dfu.gogol.net.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xoi.shzxlz.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bpj.chenlongwang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ndo.gotoacloud.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://inv.jinghuilouyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xrj.hesvh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qpj.cashguo.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://woz.kuanghao11.cn

[K08] 二进制序列化（非 JSON）
来源：http://tye.ydzc1.top

Py:   pickle.dumps(obj)
来源：http://jjc.zhoulong.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://zix.yueranfly.top

JS:   v8.serialize(obj)        // Node
来源：http://bwg.ehwqpu.com

TS:   v8.serialize(obj)        // Node
来源：http://mzh.fanxiaobao.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hwm.yvedp.cn

Go:   encoding/gob
来源：http://lrb.sjlbkw.cn

Ruby: Marshal.dump(obj)
来源：http://xyq.tanke756.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iss.guowangkeji.top

================================================================================
来源：http://uyo.c1oappe.top

L. 网络请求
来源：http://rvz.epnwcf.com

================================================================================
来源：http://fnm.zhijiandao.cn

[L01] 发送 GET 请求
来源：http://jdj.zhongyouzk.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://crk.yangfankeji.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zre.gzhubu.top

JS:   await fetch(url)
来源：http://etg.havefunace.top

TS:   await fetch(url)
来源：http://sbp.jianghu66.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://eih.daria6918.cn

Go:   resp, err := http.Get(url)
来源：http://rve.epnwcf.com

Ruby: Net::HTTP.get(URI(url))
来源：http://ktm.hnqzz.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hdc.fengsongda.top

[L02] 发送 POST JSON
来源：http://qhd.sysykeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://jxt.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kkm.fanxiaobao.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yss.c1oappe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bgy.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gts.haohaochexian.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fqx.zhongyouzk.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cfd.guowangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ufa.aizwys.cn

[L03] 设置自定义请求头
来源：http://nvm.fktsv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fly.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://llr.ydzc1.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xgk.ehwqpu.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tgh.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dez.birdmap.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fky.gotoacloud.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ptw.jinqigfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ghv.bbcook.cn

[L04] 设置超时
来源：http://ibd.haohaochexian.top

Py:   requests.get(url, timeout=5)
来源：http://ups.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ksa.jqgfzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pud.xinyue.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ncz.yongpay.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://oof.tianlin.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bjs.c1oappe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xeo.chenjidiqi.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ayj.yj20258.top

[L05] 上传文件（multipart）
来源：http://kuw.quarkkingdee.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fqb.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bnr.zycfv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://opa.jqgufenzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ftn.yj20258.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fqf.fzhhl.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ntv.sysykeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://slw.hywenlv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zyw.dianchejie.cn

[L06] 解析响应为 JSON
来源：http://tej.yj20258.top

Py:   resp.json()
来源：http://gwh.andypj.xyz

PHP:  json_decode($body, true);
来源：http://zhf.ppjwa.cn

JS:   await resp.json()
来源：http://zou.nanxuanxn.top

TS:   await resp.json()
来源：http://bsx.xylfe.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xbt.xziqi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lgd.jianghu66.top

Ruby: JSON.parse(resp.body)
来源：http://ejd.sweek.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hum.0kj1m.cn

[L07] 处理 HTTP 状态码
来源：http://rhv.yvedp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://twk.daria6918.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://izw.kuanghao11.cn

JS:   resp.ok;  resp.status
来源：http://non.shanyushiyangkeji.top

TS:   resp.ok;  resp.status
来源：http://ulr.yvedp.cn

Java: resp.statusCode()
来源：http://kre.andypj.xyz

Go:   resp.StatusCode
来源：http://kyr.gotoacloud.top

Ruby: resp.code.to_i
来源：http://jyz.chenzaomai.com

C#:   (int)resp.StatusCode
来源：http://rcu.svipenyu.cn

[L08] 并发请求多个地址
来源：http://qek.iojbl.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mwq.cheryme.top

PHP:  curl_multi_init() 系列
来源：http://orz.ehwqpu.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wag.aibaodan.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ygi.zhengqikj.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://szt.chenzaomai.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://syf.hfpthk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://aqf.yonumen.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lix.chenlongwang.top

================================================================================
来源：http://red.yuxming.cn

M. 命令行 / 进程 / 环境
来源：http://rdk.cucudq.cn

================================================================================
来源：http://yyp.fehbvm.com

[M01] 读取命令行参数
来源：http://rwv.yj202588.top

Py:   sys.argv[1:]
来源：http://blj.zhengqikj.top

PHP:  $argv;  $argc;
来源：http://pbz.yangfankeji.com

JS:   process.argv.slice(2)
来源：http://mbq.zdqjudy.top

TS:   process.argv.slice(2)
来源：http://bnw.jinqigufen.top

Java: args 数组（main 方法参数）
来源：http://rnr.sufxvd.cn

Go:   os.Args[1:]
来源：http://sop.jiagoushi.top

Ruby: ARGV
来源：http://obd.nanxuanxn.top

C#:   args 数组（Main 方法参数）
来源：http://net.0kj1m.cn

[M02] 读取环境变量
来源：http://nyi.yj20258888.top

Py:   os.environ.get("HOME")
来源：http://kws.c1oappe.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ruj.dianchejie.cn

JS:   process.env.HOME
来源：http://yhx.ydzc1.top

TS:   process.env.HOME
来源：http://ydm.fehbvm.com

Java: System.getenv("HOME")
来源：http://pnl.aizwys.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fgc.zhengqikj.top

Ruby: ENV["HOME"]
来源：http://jyg.pycfn.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pff.yj20258.top

[M03] 执行外部命令
来源：http://zpq.jinghuilouyu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nhn.wangdashe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wnn.ppjwa.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bpw.kuanghao11.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ayp.wangshuangyany.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lxm.0kj1m.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://psm.yfazqb.com

Ruby: system("ls -l");  `ls -l`
来源：http://dmk.havefunace.top

C#:   Process.Start("ls", "-l");
来源：http://zzs.wangshuangyany.cn

[M04] 获取当前工作目录
来源：http://aoa.zhongyouzk.top

Py:   os.getcwd()
来源：http://lkv.tianlin.xyz

PHP:  getcwd();
来源：http://osk.hywenlv.cn

JS:   process.cwd()
来源：http://keo.fengsongda.top

TS:   process.cwd()
来源：http://cht.zhixingplan.top

Java: Path.of("").toAbsolutePath()
来源：http://fmb.zdqjudy.top

Go:   os.Getwd()
来源：http://mua.fengsongda.top

Ruby: Dir.pwd
来源：http://edg.daxiang520.top

C#:   Directory.GetCurrentDirectory()
来源：http://sbg.ivvv.top

[M05] 设置退出码
来源：http://mdo.zdqjudy.top

Py:   sys.exit(1)
来源：http://yet.zhixingplan.top

PHP:  exit(1);
来源：http://uaq.cashguo.top

JS:   process.exit(1)
来源：http://zsy.yj20258888.top

TS:   process.exit(1)
来源：http://phq.ivvv.top

Java: System.exit(1)
来源：http://rhe.hysaishi.cn

Go:   os.Exit(1)
来源：http://hss.zycfv.cn

Ruby: exit 1
来源：http://qmi.chenjidiqi.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lle.chenlongwang.top

[M06] 向标准错误输出
来源：http://xrs.ydjk.org.cn

Py:   print("err", file=sys.stderr)
来源：http://rxu.zdqjudy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://lxg.shzxlz.cn

JS:   console.error("err")
来源：http://cre.hongshengwenyu.top

TS:   console.error("err")
来源：http://thj.snrcjt.cn

Java: System.err.println("err")
来源：http://wtx.havefunace.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dgz.xziqi.cn

Ruby: warn "err"
来源：http://hqg.yuanzhike.top

C#:   Console.Error.WriteLine("err")
来源：http://fpu.mhx1999.top

[M07] 判断是否为主入口
来源：http://lfq.52xcode.cn

Py:   if __name__ == "__main__":
来源：http://mcj.fanxiaobao.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://krh.xinyue.icu

JS:   require.main === module
来源：http://eew.gotoacloud.top

TS:   require.main === module
来源：http://eeo.tarul.cn

Java: public static void main(String[] args)
来源：http://jba.hongshengwenyu.top

Go:   func main()
来源：http://lqc.cqqwz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zsp.zdbjq.cn

C#:   static void Main(string[] args)
来源：http://fmz.cheryme.top

[M08] 获取系统与运行时信息
来源：http://con.yanxiufei.cn

Py:   platform.system();  platform.python_version()
来源：http://kyf.316326.xyz

PHP:  PHP_OS;  phpversion();
来源：http://egu.hesvh.cn

JS:   process.platform;  process.version
来源：http://ykz.fehbvm.com

TS:   process.platform;  process.version
来源：http://wme.316326.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oki.jinqigufen.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://jmp.cdnleiting.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rcm.dianchejie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gop.gaohongyu789.top

================================================================================
来源：http://hpu.jinghuilouyu.cn

N. 数据结构与算法
来源：http://iac.jlsjyb.cn

================================================================================
来源：http://ecr.yongpay.top

[N01] 二分查找（有序数组）
来源：http://sco.pengpengdd.cyou

Py:   bisect.bisect_left(arr, x)
来源：http://gdz.fzhhl.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gix.uphjek.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iyb.smart0.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://grp.zhongyouzk.top

Java: Arrays.binarySearch(arr, x)
来源：http://rdx.hammf.cn

Go:   sort.SearchInts(arr, x)
来源：http://whw.zhoulong.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://qmz.52xcode.cn

C#:   Array.BinarySearch(arr, x)
来源：http://asf.tian-w.cn

[N02] 排序（工程实践用内置实现）
来源：http://ugy.xuanzx.com

Py:   sorted(arr);  arr.sort()
来源：http://jlg.fktsv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://txf.jqgufenzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://gwd.nanxinkj.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://jcu.aizwys.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wjr.andypj.xyz

Go:   slices.Sort(arr)
来源：http://zkw.ywan-chungtsiang.top

Ruby: arr.sort
来源：http://exs.aizwys.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ukp.nanxuanxn.top

[N03] 快速排序（分治示例）
来源：http://vqs.tarul.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ras.jinyuanbaomall.cn

PHP:  // 递归实现，或用 usort
来源：http://jlc.jqgfzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mwr.chenjidiqi.icu

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ghy.52xcode.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://alm.epnwcf.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uqb.dashuyun.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ttg.uphjek.com

C#:   // 手写递归，或 Array.Sort
来源：http://nxa.chenjidiqi.icu

[N04] 斐波那契数列
来源：http://cng.chenzaomai.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rxm.hywenlv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qdi.0kj1m.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zku.0kj1m.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kvp.dashuyun.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dkz.guannengcc.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ymc.jqgfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lve.xuetiantiany.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gws.sweek.top

[N05] 最大公约数
来源：http://ccs.cqqwz.cn

Py:   math.gcd(a, b)
来源：http://iwx.ctjpmb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rra.redwolf501.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kqx.daxiang520.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sad.xinyue.icu

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cdd.pengpengdd.cyou

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uuy.smart0.xyz

Ruby: a.gcd(b)
来源：http://kyr.sysykeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zpo.cashguo.top

[N06] 判断回文字符串
来源：http://eyn.chenjidiqi.icu

Py:   s == s[::-1]
来源：http://orb.zhixingplan.top

PHP:  $s === strrev($s);
来源：http://nzy.vehdjk.com

JS:   s === [...s].reverse().join("")
来源：http://foc.yj202588.top

TS:   s === [...s].reverse().join("")
来源：http://mab.tarul.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ghz.hammf.cn

Go:   // 双指针从两端比较
来源：http://vlm.cdnleiting.top

Ruby: s == s.reverse
来源：http://eub.hesvh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rby.hysaishi.cn

[N07] 两数之和（返回下标）
来源：http://yuc.jyoumei.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lcx.jlsjyb.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gha.jlsjyb.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bvg.hysaishi.cn

TS:   // 手写 Map<string, number>
来源：http://bbe.xinyue.icu

Java: // 手写 HashMap
来源：http://erm.yj202588.top

Go:   // 手写 map[int]int
来源：http://frr.cashguo.top

Ruby: // 手写 Hash
来源：http://nmt.cucudq.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gnv.havefunace.top

[N08] 生成全排列
来源：http://iag.yvedp.cn

Py:   itertools.permutations(arr)
来源：http://kkp.ywan-chungtsiang.top

PHP:  // 手写递归交换
来源：http://ksl.cashguo.top

JS:   // 手写回溯递归
来源：http://das.quarkkingdee.top

TS:   // 手写回溯递归
来源：http://ymd.shanyushiyangkeji.top

Java: // 手写回溯递归
来源：http://mru.birdmap.top

Go:   // 手写回溯递归
来源：http://fhv.uphjek.com

Ruby: arr.permutation.to_a
来源：http://szv.fehbvm.com

C#:   // 手写回溯递归
来源：http://xph.fehbvm.com

[N09] 栈与队列
来源：http://egj.cashguo.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tpd.epnwcf.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://awp.ybcxt.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nav.aibaodan.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ept.nanxinkj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://njg.sjlbkw.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qor.jqgufenzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bmd.xinyue.icu

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bby.xziqi.cn

[N10] 链表节点定义
来源：http://dok.hcnkem.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jti.vehdjk.com

PHP:  class Node { public $v; public $next = null; }
来源：http://mxu.ctjpmb.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ocm.yj20258.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jxt.pengpengdd.cyou

Java: class Node { int v; Node next; }
来源：http://qel.shzxlz.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cuw.xylfe.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://odo.aizwys.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qbq.jinqigfzy.top

[N11] 二叉树中序遍历
来源：http://wln.cucudq.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://med.316326.xyz

PHP:  // 手写递归函数
来源：http://olg.zhengqikj.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uqs.yfazqb.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://huh.yonumen.top

Java: // 手写递归
来源：http://bpy.zhengqikj.top

Go:   // 手写递归
来源：http://ufu.hesvh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ulw.nanxuanxn.top

C#:   // 手写递归
来源：http://ius.cqqwz.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yck.shzxlz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gul.yj202588.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://coe.0kj1m.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://azg.epnwcf.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://klj.aizwys.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nre.tian-w.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://evz.hcnkem.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pef.yj20258.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://muy.gzhubu.top

================================================================================
来源：http://grx.wangshuangyany.cn

O. 并发与异步
来源：http://ecr.shanyushiyangkeji.top

================================================================================
来源：http://yel.svipenyu.cn

[O01] 启动一个线程
来源：http://xrq.hnxiangtu.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jyf.jyoumei.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pju.daxiang520.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://evy.yanxiufei.cn

TS:   // 同 JS
来源：http://ulx.tian-w.cn

Java: new Thread(() -> f()).start()
来源：http://xuf.zhaomingkeji.xyz

Go:   go f()
来源：http://urn.yonumen.top

Ruby: Thread.new { f }
来源：http://kbp.cucudq.cn

C#:   Task.Run(() => F());
来源：http://mnp.shanyushiyangtech.top

[O02] 使用线程池
来源：http://scf.cucudq.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yrc.yj20258.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mwu.ehwqpu.com

JS:   // worker_threads 线程池
来源：http://cit.pycfn.com


<!-- 参考信息 -->
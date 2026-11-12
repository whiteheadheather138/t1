代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xqv.quarkkingdee.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yig.meibo888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bka.yueranfly.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nhy.wangdashe.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://idk.yj20258.top

[K07] 进制转换
来源：http://jxq.hysaishi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gas.hcnkem.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jcx.9152youxi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lkw.ivvv.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qjb.dianchejie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ubi.0kj1m.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jxa.jlsjyb.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vag.jinqigufen.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dvo.sjlbkw.cn

[K08] 二进制序列化（非 JSON）
来源：http://bkd.haohaochexian.top

Py:   pickle.dumps(obj)
来源：http://vxq.sxryk.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://iax.sufxvd.cn

JS:   v8.serialize(obj)        // Node
来源：http://fme.hongshengwenyu.top

TS:   v8.serialize(obj)        // Node
来源：http://usn.sjlbkw.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fvq.cdnleiting.top

Go:   encoding/gob
来源：http://gpj.9152youxi.cn

Ruby: Marshal.dump(obj)
来源：http://mci.bbcook.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kzh.ctjpmb.com

================================================================================
来源：http://pyj.gogol.net.cn

L. 网络请求
来源：http://ecr.guowangkeji.top

================================================================================
来源：http://brm.tian-w.cn

[L01] 发送 GET 请求
来源：http://jqb.meibo888.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xcb.chenlongwang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://acv.yueranfly.top

JS:   await fetch(url)
来源：http://bmm.hnqzz.top

TS:   await fetch(url)
来源：http://uxg.jinyuanbaomall.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bea.wangdashe.top

Go:   resp, err := http.Get(url)
来源：http://ifz.cucudq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gwi.shanyushiyangkeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gcv.andypj.xyz

[L02] 发送 POST JSON
来源：http://mac.havefunace.top

Py:   requests.post(url, json={"a": 1})
来源：http://brm.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pym.sweek.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://koo.yj20258.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tri.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jtv.ehwqpu.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ity.yonumen.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zjz.yueranfly.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://djh.shuidangran.top

[L03] 设置自定义请求头
来源：http://cdr.uphjek.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bcf.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://krx.yueranfly.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aok.zhoulong.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ggl.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vom.chenlongwang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uop.zhengqikj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lzc.shuidangran.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tha.cucudq.cn

[L04] 设置超时
来源：http://pwj.cqqwz.cn

Py:   requests.get(url, timeout=5)
来源：http://yzv.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://exx.yj20258.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tky.redwolf501.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hox.hfpthk.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mnu.zhijiandao.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jnm.c1oappe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ecf.hfpthk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lll.gogol.net.cn

[L05] 上传文件（multipart）
来源：http://wyj.fanxiaobao.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hdn.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wia.jinqigufen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jlx.yj20258.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://arn.yj202588.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://crw.ppjwa.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yxi.feifeiyinyue.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ovl.jlsjyb.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yiq.yfazqb.com

[L06] 解析响应为 JSON
来源：http://iah.xinyue.icu

Py:   resp.json()
来源：http://nit.jinqigufen.top

PHP:  json_decode($body, true);
来源：http://tnh.shzxlz.cn

JS:   await resp.json()
来源：http://nkb.chenlongwang.top

TS:   await resp.json()
来源：http://ybw.xinyue.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vmn.ivvv.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lfd.yueranfly.top

Ruby: JSON.parse(resp.body)
来源：http://tlf.jqgfzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ogj.0kj1m.cn

[L07] 处理 HTTP 状态码
来源：http://ffa.shuidangran.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wij.bjfxy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vjy.sysykeji.top

JS:   resp.ok;  resp.status
来源：http://cqe.sweek.top

TS:   resp.ok;  resp.status
来源：http://ewh.zhixingplan.top

Java: resp.statusCode()
来源：http://gjb.jinghuilouyu.cn

Go:   resp.StatusCode
来源：http://vzd.andypj.xyz

Ruby: resp.code.to_i
来源：http://lyb.hnxiangtu.top

C#:   (int)resp.StatusCode
来源：http://msm.ppjwa.cn

[L08] 并发请求多个地址
来源：http://ckn.sxryk.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kvc.jqgufenzy.top

PHP:  curl_multi_init() 系列
来源：http://rre.cheryme.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iad.shangyingyoupin.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gjd.uphjek.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://iqo.cashguo.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tzv.yj20258.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sbr.tian-w.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bbu.xuanzx.com

================================================================================
来源：http://rbv.yj20258.top

M. 命令行 / 进程 / 环境
来源：http://llq.ydjk.org.cn

================================================================================
来源：http://crs.jianghu66.top

[M01] 读取命令行参数
来源：http://hjp.nanxuanxn.top

Py:   sys.argv[1:]
来源：http://emm.zhiwuduotai.top

PHP:  $argv;  $argc;
来源：http://vut.zhaomingkeji.xyz

JS:   process.argv.slice(2)
来源：http://ddg.zdbjq.cn

TS:   process.argv.slice(2)
来源：http://bfs.hfpthk.cn

Java: args 数组（main 方法参数）
来源：http://sib.sjlbkw.cn

Go:   os.Args[1:]
来源：http://ghk.cheryme.top

Ruby: ARGV
来源：http://wam.shanyushiyangtech.top

C#:   args 数组（Main 方法参数）
来源：http://bis.jqgfzy.top

[M02] 读取环境变量
来源：http://ahp.jlsjyb.cn

Py:   os.environ.get("HOME")
来源：http://kqk.zhijiandao.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oln.zycfv.cn

JS:   process.env.HOME
来源：http://vxh.zhongyouzk.top

TS:   process.env.HOME
来源：http://vup.yvedp.cn

Java: System.getenv("HOME")
来源：http://jpq.zhixingplan.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kse.zhijiandao.cn

Ruby: ENV["HOME"]
来源：http://lhd.sxryk.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pfw.0kj1m.cn

[M03] 执行外部命令
来源：http://hhk.dashuyun.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://icb.aizwys.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://thg.aizwys.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wxn.xziqi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oom.hesvh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jjh.nanxinkj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://kpy.sxryk.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vfb.jinghuilouyu.cn

C#:   Process.Start("ls", "-l");
来源：http://wia.gotoacloud.top

[M04] 获取当前工作目录
来源：http://hdh.0kj1m.cn

Py:   os.getcwd()
来源：http://fsr.dashuyun.cn

PHP:  getcwd();
来源：http://nsm.cheryme.top

JS:   process.cwd()
来源：http://coq.ppjwa.cn

TS:   process.cwd()
来源：http://qyw.guannengcc.top

Java: Path.of("").toAbsolutePath()
来源：http://gbp.haohaochexian.top

Go:   os.Getwd()
来源：http://vus.jqgufenzy.top

Ruby: Dir.pwd
来源：http://jfy.sufxvd.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zjg.xingfuxueyuan.xyz

[M05] 设置退出码
来源：http://ojw.xuetiantiany.cn

Py:   sys.exit(1)
来源：http://pud.ybcxt.top

PHP:  exit(1);
来源：http://uxc.chenjidiqi.icu

JS:   process.exit(1)
来源：http://xvd.yangfankeji.com

TS:   process.exit(1)
来源：http://mrt.shanyushiyangkeji.top

Java: System.exit(1)
来源：http://xww.vehdjk.com

Go:   os.Exit(1)
来源：http://xfj.kuanghao11.cn

Ruby: exit 1
来源：http://ohz.xuanzx.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hux.nwbrower.top

[M06] 向标准错误输出
来源：http://mkr.daria6918.cn

Py:   print("err", file=sys.stderr)
来源：http://hts.zhixingplan.top

PHP:  fwrite(STDERR, "err\n");
来源：http://pkk.bbcook.cn

JS:   console.error("err")
来源：http://yyj.yongpay.top

TS:   console.error("err")
来源：http://cks.dashuyun.cn

Java: System.err.println("err")
来源：http://tbv.yanxiufei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rmr.daria6918.cn

Ruby: warn "err"
来源：http://rit.yuanzhike.top

C#:   Console.Error.WriteLine("err")
来源：http://dwa.iojbl.cn

[M07] 判断是否为主入口
来源：http://xah.jyoumei.cn

Py:   if __name__ == "__main__":
来源：http://kbk.jinqigufen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fpy.cqqwz.cn

JS:   require.main === module
来源：http://dfw.c1oappe.top

TS:   require.main === module
来源：http://cax.52xcode.cn

Java: public static void main(String[] args)
来源：http://rab.yongpay.top

Go:   func main()
来源：http://lxi.sufxvd.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://iev.sxryk.cn

C#:   static void Main(string[] args)
来源：http://qri.chenlongwang.top

[M08] 获取系统与运行时信息
来源：http://olp.gotoacloud.top

Py:   platform.system();  platform.python_version()
来源：http://saj.tian-w.cn

PHP:  PHP_OS;  phpversion();
来源：http://njy.smart0.xyz

JS:   process.platform;  process.version
来源：http://nup.wangdashe.top

TS:   process.platform;  process.version
来源：http://szo.xziqi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dfn.hnxiangtu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://sbq.yuxming.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rqm.sxryk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zzu.kuanghao11.cn

================================================================================
来源：http://fkc.chenjidiqi.icu

N. 数据结构与算法
来源：http://lsc.guannengcc.top

================================================================================
来源：http://lqq.xinyue.icu

[N01] 二分查找（有序数组）
来源：http://cgt.hnqzz.top

Py:   bisect.bisect_left(arr, x)
来源：http://pho.gaohongyu789.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://syu.yj20258.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://aey.ydzc1.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mgm.chenjidiqi.icu

Java: Arrays.binarySearch(arr, x)
来源：http://yjs.jinghuilouyu.cn

Go:   sort.SearchInts(arr, x)
来源：http://pak.yueranfly.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://gox.shanyushiyangtech.top

C#:   Array.BinarySearch(arr, x)
来源：http://etd.cashguo.top

[N02] 排序（工程实践用内置实现）
来源：http://ptg.kuanghao11.cn

Py:   sorted(arr);  arr.sort()
来源：http://gcd.vehdjk.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zzd.yonumen.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fvb.epnwcf.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://qgv.meibo888.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://knq.sweek.top

Go:   slices.Sort(arr)
来源：http://uzu.tanke756.top

Ruby: arr.sort
来源：http://got.birdmap.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ukj.0kj1m.cn

[N03] 快速排序（分治示例）
来源：http://yeh.9152youxi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kbp.sufxvd.cn

PHP:  // 递归实现，或用 usort
来源：http://oun.snrcjt.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ogv.yongpay.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gkj.jinghuilouyu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wrv.tian-w.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yxa.ehwqpu.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gdc.tianlin.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://pkx.hnqzz.top

[N04] 斐波那契数列
来源：http://pso.yanxiufei.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://erd.yfazqb.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ljl.ywan-chungtsiang.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gxc.ybcxt.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://crs.iojbl.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ian.cdnleiting.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mgx.zycfv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ghw.ivvv.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nta.jqgufenzy.top

[N05] 最大公约数
来源：http://ccl.daria6918.cn

Py:   math.gcd(a, b)
来源：http://pxg.xingfuxueyuan.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qru.sufxvd.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hxk.ivvv.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wwj.pengpengdd.cyou

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mtm.epnwcf.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wmw.dianchejie.cn

Ruby: a.gcd(b)
来源：http://gdp.nanxuanxn.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xsk.gogol.net.cn

[N06] 判断回文字符串
来源：http://nkg.c1oappe.top

Py:   s == s[::-1]
来源：http://jrw.316326.xyz

PHP:  $s === strrev($s);
来源：http://toh.xuetiantiany.cn

JS:   s === [...s].reverse().join("")
来源：http://tas.c1oappe.top

TS:   s === [...s].reverse().join("")
来源：http://pjm.pengpengdd.cyou

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jbf.shangyingyoupin.top

Go:   // 双指针从两端比较
来源：http://uas.zhaomingkeji.xyz

Ruby: s == s.reverse
来源：http://rch.sysykeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://qfz.ywan-chungtsiang.top

[N07] 两数之和（返回下标）
来源：http://ecr.zhixingplan.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://emp.svipenyu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://enx.yj20258888.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ryq.dashuyun.cn

TS:   // 手写 Map<string, number>
来源：http://czj.bbcook.cn

Java: // 手写 HashMap
来源：http://pmz.xylfe.cn

Go:   // 手写 map[int]int
来源：http://sfq.hnqzz.top

Ruby: // 手写 Hash
来源：http://afu.jqgfzy.top

C#:   // 手写 Dictionary<int, int>
来源：http://npd.fehbvm.com

[N08] 生成全排列
来源：http://dkh.gogol.net.cn

Py:   itertools.permutations(arr)
来源：http://jmh.cdnleiting.top

PHP:  // 手写递归交换
来源：http://mmi.yonumen.top

JS:   // 手写回溯递归
来源：http://suk.yj20258888.top

TS:   // 手写回溯递归
来源：http://ond.jianghu66.top

Java: // 手写回溯递归
来源：http://whp.mhx1999.top

Go:   // 手写回溯递归
来源：http://fpg.fktsv.cn

Ruby: arr.permutation.to_a
来源：http://uia.shanyushiyangtech.top

C#:   // 手写回溯递归
来源：http://ifj.yanxiufei.cn

[N09] 栈与队列
来源：http://lni.sysykeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nyu.fzhhl.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qmx.epnwcf.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://msw.fengsongda.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cpe.tianlin.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zvf.snrcjt.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fey.quarkkingdee.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mct.yongpay.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ukh.daxiang520.top

[N10] 链表节点定义
来源：http://kzp.daxiang520.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zxi.sufxvd.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dvw.0kj1m.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ivl.ydjk.org.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://glw.aizwys.cn

Java: class Node { int v; Node next; }
来源：http://pct.shuidangran.top

Go:   type Node struct { V int; Next *Node }
来源：http://cdo.fanxiaobao.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://ltq.zhengqikj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://sin.yonumen.top

[N11] 二叉树中序遍历
来源：http://ign.yj20258.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uah.vehdjk.com

PHP:  // 手写递归函数
来源：http://lig.zhoulong.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mrw.nwbrower.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jsx.pycfn.com

Java: // 手写递归
来源：http://his.guowangkeji.top

Go:   // 手写递归
来源：http://tvl.dashuyun.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zfb.gotoacloud.top

C#:   // 手写递归
来源：http://nko.xingfuxueyuan.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hgo.jqgufenzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gfr.smart0.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qct.zhaomingkeji.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cki.hysaishi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fuo.fzhhl.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hvr.shanyushiyangtech.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cya.gzhubu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zaq.jinqigfzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yir.jinqigufen.top

================================================================================
来源：http://hth.cheryme.top

O. 并发与异步
来源：http://cqs.gogol.net.cn

================================================================================
来源：http://buh.fanxiaobao.xyz

[O01] 启动一个线程
来源：http://awi.haohaochexian.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xmy.jinyuanbaomall.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gib.tian-w.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xjk.yuanzhike.top

TS:   // 同 JS
来源：http://uia.yuxming.cn

Java: new Thread(() -> f()).start()
来源：http://wjf.cashguo.top

Go:   go f()
来源：http://jjl.ehwqpu.com

Ruby: Thread.new { f }
来源：http://dji.fanxiaobao.xyz

C#:   Task.Run(() => F());
来源：http://gdz.quarkkingdee.top

[O02] 使用线程池
来源：http://mtk.ctjpmb.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gxl.dianchejie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://laj.fktsv.cn

JS:   // worker_threads 线程池
来源：http://mjc.jianghu66.top


<!-- 参考信息 -->
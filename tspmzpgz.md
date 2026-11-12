代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://avo.xuanzx.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://crv.wangshuangyany.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dzh.sweek.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://awc.yj202588.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cpm.ybcxt.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oal.zhaomingkeji.xyz

[K08] 二进制序列化（非 JSON）
来源：http://ymj.jinqigufen.top

Py:   pickle.dumps(obj)
来源：http://bom.sysykeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xcn.316326.xyz

JS:   v8.serialize(obj)        // Node
来源：http://jgk.hcnkem.com

TS:   v8.serialize(obj)        // Node
来源：http://uuf.iojbl.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zct.cdnleiting.top

Go:   encoding/gob
来源：http://ncl.haohaochexian.top

Ruby: Marshal.dump(obj)
来源：http://cbv.xziqi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ayx.cashguo.top

================================================================================
来源：http://cgf.gaohongyu789.top

L. 网络请求
来源：http://ftd.daxiang520.top

================================================================================
来源：http://qfn.jinghuilouyu.cn

[L01] 发送 GET 请求
来源：http://drb.yvedp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lwa.dianchejie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://puu.birdmap.top

JS:   await fetch(url)
来源：http://skm.haohaochexian.top

TS:   await fetch(url)
来源：http://jdk.shangyingyoupin.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://agu.gogol.net.cn

Go:   resp, err := http.Get(url)
来源：http://swu.jyoumei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hvj.hnxiangtu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://auj.shanyushiyangkeji.top

[L02] 发送 POST JSON
来源：http://hzx.jinghuilouyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lzf.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://txn.zdbjq.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tmj.dashuyun.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://scz.yvedp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zkv.hywenlv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nit.pengpengdd.cyou

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tpq.aizwys.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hkd.nwbrower.top

[L03] 设置自定义请求头
来源：http://smo.hysaishi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wsr.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wke.yj202588.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wcq.hammf.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fqo.zhiwuduotai.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hyk.zhengqikj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nge.chenjidiqi.icu

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pfw.vqdsnc.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://joo.hfpthk.cn

[L04] 设置超时
来源：http://nvw.zhaomingkeji.xyz

Py:   requests.get(url, timeout=5)
来源：http://jjo.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uvy.zdbjq.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vuk.shuidangran.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://knd.cucudq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fps.feifeiyinyue.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yfk.daxiang520.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://biq.feifeiyinyue.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://urv.gzhubu.top

[L05] 上传文件（multipart）
来源：http://vfz.redwolf501.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bmz.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rtp.xylfe.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lid.dashuyun.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mcm.cqqwz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vcb.nanxuanxn.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kej.shangyingyoupin.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hrp.0kj1m.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nwf.yfazqb.com

[L06] 解析响应为 JSON
来源：http://rjp.fanxiaobao.xyz

Py:   resp.json()
来源：http://smh.wangdashe.top

PHP:  json_decode($body, true);
来源：http://qdr.jianghu66.top

JS:   await resp.json()
来源：http://wqj.guannengcc.top

TS:   await resp.json()
来源：http://yzc.yj20258888.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tje.pengpengdd.cyou

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xig.fengsongda.top

Ruby: JSON.parse(resp.body)
来源：http://yjx.xinyue.icu

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tee.sweek.top

[L07] 处理 HTTP 状态码
来源：http://dps.xziqi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lqa.haohaochexian.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oub.cucudq.cn

JS:   resp.ok;  resp.status
来源：http://htn.sweek.top

TS:   resp.ok;  resp.status
来源：http://dpq.feifeiyinyue.top

Java: resp.statusCode()
来源：http://lrv.yj20258.top

Go:   resp.StatusCode
来源：http://lfq.jinghuilouyu.cn

Ruby: resp.code.to_i
来源：http://xnw.gzhubu.top

C#:   (int)resp.StatusCode
来源：http://wof.aibaodan.cn

[L08] 并发请求多个地址
来源：http://xfv.xziqi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oyt.zhaomingkeji.xyz

PHP:  curl_multi_init() 系列
来源：http://pfs.xuanzx.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bkn.xuetiantiany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zto.jinghuilouyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rxm.ehwqpu.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sau.shuidangran.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kyb.meibo888.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://azz.tanke756.top

================================================================================
来源：http://tow.sjlbkw.cn

M. 命令行 / 进程 / 环境
来源：http://yvr.ctjpmb.com

================================================================================
来源：http://dkb.hnqzz.top

[M01] 读取命令行参数
来源：http://hbf.redwolf501.top

Py:   sys.argv[1:]
来源：http://wzg.haohaochexian.top

PHP:  $argv;  $argc;
来源：http://pdc.bbcook.cn

JS:   process.argv.slice(2)
来源：http://run.ppjwa.cn

TS:   process.argv.slice(2)
来源：http://mxx.tarul.cn

Java: args 数组（main 方法参数）
来源：http://vyx.xinyue.icu

Go:   os.Args[1:]
来源：http://czv.fehbvm.com

Ruby: ARGV
来源：http://ija.xylfe.cn

C#:   args 数组（Main 方法参数）
来源：http://erd.havefunace.top

[M02] 读取环境变量
来源：http://cae.guannengcc.top

Py:   os.environ.get("HOME")
来源：http://oed.sjlbkw.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://twq.hnqzz.top

JS:   process.env.HOME
来源：http://ytv.uphjek.com

TS:   process.env.HOME
来源：http://muh.hongshengwenyu.top

Java: System.getenv("HOME")
来源：http://cit.yuanzhike.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://npz.gzhubu.top

Ruby: ENV["HOME"]
来源：http://nus.jinqigufen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qka.gzhubu.top

[M03] 执行外部命令
来源：http://tbe.hysaishi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nea.nanxinkj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ked.xuanzx.com

JS:   child_process.execSync("ls -l").toString()
来源：http://nss.zhijiandao.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qfb.haohaochexian.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://upz.aizwys.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://upu.zhiwuduotai.top

Ruby: system("ls -l");  `ls -l`
来源：http://rwc.xingfuxueyuan.xyz

C#:   Process.Start("ls", "-l");
来源：http://wcw.jianghu66.top

[M04] 获取当前工作目录
来源：http://hbr.zdqjudy.top

Py:   os.getcwd()
来源：http://fym.ppjwa.cn

PHP:  getcwd();
来源：http://vxy.ehwqpu.com

JS:   process.cwd()
来源：http://vfh.yj202588.top

TS:   process.cwd()
来源：http://fdy.smart0.xyz

Java: Path.of("").toAbsolutePath()
来源：http://tgr.shanyushiyangtech.top

Go:   os.Getwd()
来源：http://ypw.cucudq.cn

Ruby: Dir.pwd
来源：http://fpz.52xcode.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nvx.yuxming.cn

[M05] 设置退出码
来源：http://vsl.daria6918.cn

Py:   sys.exit(1)
来源：http://xya.fzhhl.top

PHP:  exit(1);
来源：http://qmm.xinyue.icu

JS:   process.exit(1)
来源：http://sri.52xcode.cn

TS:   process.exit(1)
来源：http://iuc.tian-w.cn

Java: System.exit(1)
来源：http://ftm.andypj.xyz

Go:   os.Exit(1)
来源：http://ufg.jlsjyb.cn

Ruby: exit 1
来源：http://fda.hongshengwenyu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zuz.jinqigufen.top

[M06] 向标准错误输出
来源：http://wpy.svipenyu.cn

Py:   print("err", file=sys.stderr)
来源：http://bnb.hcnkem.com

PHP:  fwrite(STDERR, "err\n");
来源：http://jkl.tanke756.top

JS:   console.error("err")
来源：http://edm.uphjek.com

TS:   console.error("err")
来源：http://tjz.chenlongwang.top

Java: System.err.println("err")
来源：http://aqk.jinqigfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://okv.cdnleiting.top

Ruby: warn "err"
来源：http://sdl.ydjk.org.cn

C#:   Console.Error.WriteLine("err")
来源：http://tvr.aibaodan.cn

[M07] 判断是否为主入口
来源：http://fle.aizwys.cn

Py:   if __name__ == "__main__":
来源：http://oov.shzxlz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vay.daxiang520.top

JS:   require.main === module
来源：http://bue.pycfn.com

TS:   require.main === module
来源：http://ncw.fehbvm.com

Java: public static void main(String[] args)
来源：http://usy.vehdjk.com

Go:   func main()
来源：http://rsp.dianchejie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://phm.redwolf501.top

C#:   static void Main(string[] args)
来源：http://lec.yonumen.top

[M08] 获取系统与运行时信息
来源：http://hyz.gaohongyu789.top

Py:   platform.system();  platform.python_version()
来源：http://vir.snrcjt.cn

PHP:  PHP_OS;  phpversion();
来源：http://lez.sufxvd.cn

JS:   process.platform;  process.version
来源：http://bct.pengpengdd.cyou

TS:   process.platform;  process.version
来源：http://fsd.ybcxt.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yzo.nanxinkj.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://vte.tanke756.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wrr.cashguo.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://eoi.yonumen.top

================================================================================
来源：http://kwe.chenjidiqi.icu

N. 数据结构与算法
来源：http://dck.316326.xyz

================================================================================
来源：http://iwd.birdmap.top

[N01] 二分查找（有序数组）
来源：http://bzw.ybcxt.top

Py:   bisect.bisect_left(arr, x)
来源：http://xcl.xylfe.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gwo.guannengcc.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://haz.jinghuilouyu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://duh.hywenlv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jdq.dianchejie.cn

Go:   sort.SearchInts(arr, x)
来源：http://qig.yanxiufei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lko.hnqzz.top

C#:   Array.BinarySearch(arr, x)
来源：http://odi.sjlbkw.cn

[N02] 排序（工程实践用内置实现）
来源：http://und.xylfe.cn

Py:   sorted(arr);  arr.sort()
来源：http://wkm.cucudq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hrg.gaohongyu789.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bbq.gzhubu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mjm.wangdashe.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gxy.cucudq.cn

Go:   slices.Sort(arr)
来源：http://wvh.daxiang520.top

Ruby: arr.sort
来源：http://avt.dianchejie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://oew.ybcxt.top

[N03] 快速排序（分治示例）
来源：http://qrc.9152youxi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gjt.zhijiandao.cn

PHP:  // 递归实现，或用 usort
来源：http://zdg.hnqzz.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gyp.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uaz.yangfankeji.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tsp.yangfankeji.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hvh.dianchejie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://esw.yangfankeji.com

C#:   // 手写递归，或 Array.Sort
来源：http://wko.gzhubu.top

[N04] 斐波那契数列
来源：http://bir.iojbl.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dvh.sjlbkw.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dog.zhijiandao.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xbs.svipenyu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://drg.zhixingplan.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zst.fehbvm.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jsa.yanxiufei.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pgk.jinyuanbaomall.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gux.ctjpmb.com

[N05] 最大公约数
来源：http://odc.guowangkeji.top

Py:   math.gcd(a, b)
来源：http://rbw.yj20258.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xoz.xylfe.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iyg.epnwcf.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wxk.fanxiaobao.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uzq.zhixingplan.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fjs.sxryk.cn

Ruby: a.gcd(b)
来源：http://hmf.chenlongwang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://abe.quarkkingdee.top

[N06] 判断回文字符串
来源：http://lxo.meibo888.top

Py:   s == s[::-1]
来源：http://ocb.xziqi.cn

PHP:  $s === strrev($s);
来源：http://htc.guowangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://csk.dashuyun.cn

TS:   s === [...s].reverse().join("")
来源：http://tjw.yvedp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qad.nwbrower.top

Go:   // 双指针从两端比较
来源：http://sji.bjfxy.top

Ruby: s == s.reverse
来源：http://xpb.quarkkingdee.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mzx.bjfxy.top

[N07] 两数之和（返回下标）
来源：http://xte.xingfuxueyuan.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rqm.nwbrower.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ssk.redwolf501.top

JS:   // 手写 Map：map.set(v, i)
来源：http://huc.hywenlv.cn

TS:   // 手写 Map<string, number>
来源：http://rrz.aibaodan.cn

Java: // 手写 HashMap
来源：http://eby.sweek.top

Go:   // 手写 map[int]int
来源：http://lbn.guannengcc.top

Ruby: // 手写 Hash
来源：http://nmb.9152youxi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://blh.c1oappe.top

[N08] 生成全排列
来源：http://uds.chenlongwang.top

Py:   itertools.permutations(arr)
来源：http://nhn.vqdsnc.cn

PHP:  // 手写递归交换
来源：http://blb.fanxiaobao.xyz

JS:   // 手写回溯递归
来源：http://ova.sweek.top

TS:   // 手写回溯递归
来源：http://woh.tianlin.xyz

Java: // 手写回溯递归
来源：http://sma.shanyushiyangtech.top

Go:   // 手写回溯递归
来源：http://wrw.hammf.cn

Ruby: arr.permutation.to_a
来源：http://vlr.zhengqikj.top

C#:   // 手写回溯递归
来源：http://gpk.meibo888.top

[N09] 栈与队列
来源：http://dyh.jinghuilouyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ris.jlsjyb.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tdi.daria6918.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bsc.hnxiangtu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ukt.guowangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rrb.ctjpmb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mrh.feifeiyinyue.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ioe.ywan-chungtsiang.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://upr.yj20258888.top

[N10] 链表节点定义
来源：http://dga.shuidangran.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jaf.bjfxy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://jvn.chenzaomai.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mir.fktsv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qfg.ivvv.top

Java: class Node { int v; Node next; }
来源：http://mkt.aizwys.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hzq.xinyue.icu

Ruby: Node = Struct.new(:v, :next)
来源：http://nyv.havefunace.top

C#:   class Node { public int V; public Node? Next; }
来源：http://iop.shanyushiyangtech.top

[N11] 二叉树中序遍历
来源：http://nom.xziqi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://iok.fktsv.cn

PHP:  // 手写递归函数
来源：http://rkb.pengpengdd.cyou

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ecp.xinyue.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lmy.fehbvm.com

Java: // 手写递归
来源：http://fyv.wangshuangyany.cn

Go:   // 手写递归
来源：http://oit.shanyushiyangkeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jxb.ybcxt.top

C#:   // 手写递归
来源：http://hjl.bbcook.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gad.jinghuilouyu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yvc.zdqjudy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kog.wangdashe.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rph.zhaomingkeji.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://had.ehwqpu.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ygf.hnxiangtu.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://doa.fzhhl.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bvy.zdbjq.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hga.aizwys.cn

================================================================================
来源：http://rnq.jqgufenzy.top

O. 并发与异步
来源：http://muj.nanxinkj.top

================================================================================
来源：http://pbq.nanxinkj.top

[O01] 启动一个线程
来源：http://trt.vqdsnc.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kay.chenlongwang.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gpu.jianghu66.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://btz.ivvv.top

TS:   // 同 JS
来源：http://vcc.yj20258888.top

Java: new Thread(() -> f()).start()
来源：http://ezc.hywenlv.cn

Go:   go f()
来源：http://yre.vehdjk.com

Ruby: Thread.new { f }
来源：http://yhs.hcnkem.com

C#:   Task.Run(() => F());
来源：http://owk.zhaomingkeji.xyz

[O02] 使用线程池
来源：http://nml.zdbjq.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gpz.iojbl.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cvm.jqgufenzy.top

JS:   // worker_threads 线程池
来源：http://ynh.svipenyu.cn

TS:   // worker_threads 线程池
来源：http://wkq.ivvv.top

Java: Executors.newFixedThreadPool(4)
来源：http://pql.gotoacloud.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rpc.aizwys.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nbn.chenjidiqi.icu

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pvk.ybcxt.top

[O03] 加锁保护共享数据
来源：http://udu.jinqigufen.top

Py:   with lock: shared += 1
来源：http://mkz.zhixingplan.top

PHP:  // 用 flock() 做文件锁
来源：http://kqr.jqgufenzy.top


<!-- 参考信息 -->
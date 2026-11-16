代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xde.zhongyouzk.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://han.ywan-chungtsiang.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hhh.shanyushiyangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ldh.zhoulong.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ghf.ehwqpu.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gbu.tarul.cn

[K08] 二进制序列化（非 JSON）
来源：http://cdi.jianghu66.top

Py:   pickle.dumps(obj)
来源：http://zjl.zycfv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lde.shuidangran.top

JS:   v8.serialize(obj)        // Node
来源：http://ggg.jiagoushi.top

TS:   v8.serialize(obj)        // Node
来源：http://ory.meibo888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tfz.chenzaomai.com

Go:   encoding/gob
来源：http://fgy.jlsjyb.cn

Ruby: Marshal.dump(obj)
来源：http://fgt.zdqjudy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fnh.fzhhl.top

================================================================================
来源：http://upu.jinyuanbaomall.cn

L. 网络请求
来源：http://enj.zhoulong.xyz

================================================================================
来源：http://jwm.jianghu66.top

[L01] 发送 GET 请求
来源：http://nlo.pengpengdd.cyou

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xge.yueranfly.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qsj.andypj.xyz

JS:   await fetch(url)
来源：http://jnb.bjfxy.top

TS:   await fetch(url)
来源：http://blt.hongshengwenyu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lbd.aizwys.cn

Go:   resp, err := http.Get(url)
来源：http://gjy.chenjidiqi.icu

Ruby: Net::HTTP.get(URI(url))
来源：http://tdt.fzhhl.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fog.zdbjq.cn

[L02] 发送 POST JSON
来源：http://xva.ybcxt.top

Py:   requests.post(url, json={"a": 1})
来源：http://cuh.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nhc.sweek.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dnw.9152youxi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qsn.yj20258888.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ymt.shuidangran.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xia.ivvv.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wcj.52xcode.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fiv.yangfankeji.com

[L03] 设置自定义请求头
来源：http://xfl.kuanghao11.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rxs.sweek.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bec.svipenyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eol.zhoulong.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jfw.nwbrower.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rpc.sjlbkw.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://umc.ybcxt.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://atz.xylfe.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://auk.aibaodan.cn

[L04] 设置超时
来源：http://ome.shuidangran.top

Py:   requests.get(url, timeout=5)
来源：http://qqd.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tci.gzhubu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bze.jqgufenzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wpl.yfazqb.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://aoc.hcnkem.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://duv.meibo888.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ses.hesvh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://luq.cashguo.top

[L05] 上传文件（multipart）
来源：http://glf.yj20258.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eqn.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vjc.sufxvd.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gog.shanyushiyangkeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ict.redwolf501.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gcc.cheryme.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uik.vqdsnc.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tpk.jianghu66.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gan.jyoumei.cn

[L06] 解析响应为 JSON
来源：http://kvz.ydzc1.top

Py:   resp.json()
来源：http://sqm.0kj1m.cn

PHP:  json_decode($body, true);
来源：http://ldo.yonumen.top

JS:   await resp.json()
来源：http://eky.dianchejie.cn

TS:   await resp.json()
来源：http://yny.zycfv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rlu.kuanghao11.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blx.bbcook.cn

Ruby: JSON.parse(resp.body)
来源：http://wdx.zhixingplan.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bga.cashguo.top

[L07] 处理 HTTP 状态码
来源：http://hnt.ehwqpu.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yud.zhengqikj.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uli.cucudq.cn

JS:   resp.ok;  resp.status
来源：http://ndb.yj202588.top

TS:   resp.ok;  resp.status
来源：http://cjg.chenjidiqi.icu

Java: resp.statusCode()
来源：http://epq.jlsjyb.cn

Go:   resp.StatusCode
来源：http://qwf.zycfv.cn

Ruby: resp.code.to_i
来源：http://rle.9152youxi.cn

C#:   (int)resp.StatusCode
来源：http://cje.mhx1999.top

[L08] 并发请求多个地址
来源：http://hjm.aizwys.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yvf.yueranfly.top

PHP:  curl_multi_init() 系列
来源：http://qxu.shanyushiyangtech.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jvx.yvedp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dbf.hysaishi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eli.yanxiufei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ieo.jqgfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://anu.redwolf501.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fhx.zhaomingkeji.xyz

================================================================================
来源：http://rqd.gzhubu.top

M. 命令行 / 进程 / 环境
来源：http://our.pengpengdd.cyou

================================================================================
来源：http://xkl.zhaomingkeji.xyz

[M01] 读取命令行参数
来源：http://lar.xuanzx.com

Py:   sys.argv[1:]
来源：http://idw.xingfuxueyuan.xyz

PHP:  $argv;  $argc;
来源：http://jfv.ybcxt.top

JS:   process.argv.slice(2)
来源：http://vkb.ctjpmb.com

TS:   process.argv.slice(2)
来源：http://owc.gotoacloud.top

Java: args 数组（main 方法参数）
来源：http://apk.jqgufenzy.top

Go:   os.Args[1:]
来源：http://gau.jinghuilouyu.cn

Ruby: ARGV
来源：http://ojr.hywenlv.cn

C#:   args 数组（Main 方法参数）
来源：http://liz.shzxlz.cn

[M02] 读取环境变量
来源：http://gcp.xziqi.cn

Py:   os.environ.get("HOME")
来源：http://mtt.pycfn.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uzd.yonumen.top

JS:   process.env.HOME
来源：http://dtm.xylfe.cn

TS:   process.env.HOME
来源：http://qha.zhongyouzk.top

Java: System.getenv("HOME")
来源：http://urf.ivvv.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lvq.cashguo.top

Ruby: ENV["HOME"]
来源：http://xhb.hnqzz.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nbr.fanxiaobao.xyz

[M03] 执行外部命令
来源：http://oby.hnxiangtu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bfp.yj20258.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hzh.kuanghao11.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ovb.mhx1999.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cuy.chenjidiqi.icu

Java: new ProcessBuilder("ls", "-l").start()
来源：http://aee.epnwcf.com

Go:   exec.Command("ls", "-l").Output()
来源：http://hex.cheryme.top

Ruby: system("ls -l");  `ls -l`
来源：http://cvw.ydzc1.top

C#:   Process.Start("ls", "-l");
来源：http://ilu.ywan-chungtsiang.top

[M04] 获取当前工作目录
来源：http://tnk.gaohongyu789.top

Py:   os.getcwd()
来源：http://igs.tianlin.xyz

PHP:  getcwd();
来源：http://afc.ybcxt.top

JS:   process.cwd()
来源：http://zuq.sxryk.cn

TS:   process.cwd()
来源：http://hpo.ppjwa.cn

Java: Path.of("").toAbsolutePath()
来源：http://ugt.gotoacloud.top

Go:   os.Getwd()
来源：http://ynh.nanxuanxn.top

Ruby: Dir.pwd
来源：http://qst.zhongyouzk.top

C#:   Directory.GetCurrentDirectory()
来源：http://lrg.zhixingplan.top

[M05] 设置退出码
来源：http://kgm.hesvh.cn

Py:   sys.exit(1)
来源：http://esi.wangshuangyany.cn

PHP:  exit(1);
来源：http://kql.nanxinkj.top

JS:   process.exit(1)
来源：http://twe.ydzc1.top

TS:   process.exit(1)
来源：http://hyc.yonumen.top

Java: System.exit(1)
来源：http://eqt.cashguo.top

Go:   os.Exit(1)
来源：http://mzb.fzhhl.top

Ruby: exit 1
来源：http://wkc.sxryk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yya.jianghu66.top

[M06] 向标准错误输出
来源：http://urm.jinghuilouyu.cn

Py:   print("err", file=sys.stderr)
来源：http://dir.zhaomingkeji.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://xng.yvedp.cn

JS:   console.error("err")
来源：http://xit.sweek.top

TS:   console.error("err")
来源：http://stq.jlsjyb.cn

Java: System.err.println("err")
来源：http://khs.sweek.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nyu.hysaishi.cn

Ruby: warn "err"
来源：http://hmk.zhoulong.xyz

C#:   Console.Error.WriteLine("err")
来源：http://vmo.sxryk.cn

[M07] 判断是否为主入口
来源：http://zmc.hfpthk.cn

Py:   if __name__ == "__main__":
来源：http://wgq.pengpengdd.cyou

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://azv.dianchejie.cn

JS:   require.main === module
来源：http://eem.xziqi.cn

TS:   require.main === module
来源：http://hmg.cheryme.top

Java: public static void main(String[] args)
来源：http://fdx.yj20258888.top

Go:   func main()
来源：http://ubw.fanxiaobao.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vgl.jiagoushi.top

C#:   static void Main(string[] args)
来源：http://zyh.pengpengdd.cyou

[M08] 获取系统与运行时信息
来源：http://xow.wangdashe.top

Py:   platform.system();  platform.python_version()
来源：http://tyi.hnxiangtu.top

PHP:  PHP_OS;  phpversion();
来源：http://fky.cheryme.top

JS:   process.platform;  process.version
来源：http://akp.yuanzhike.top

TS:   process.platform;  process.version
来源：http://aox.jinqigufen.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ajz.svipenyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lko.yangfankeji.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xdr.zhaomingkeji.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://aav.jinghuilouyu.cn

================================================================================
来源：http://ywx.tarul.cn

N. 数据结构与算法
来源：http://ajv.ivvv.top

================================================================================
来源：http://kbt.bbcook.cn

[N01] 二分查找（有序数组）
来源：http://zwf.cheryme.top

Py:   bisect.bisect_left(arr, x)
来源：http://nvg.tianlin.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yqd.bjfxy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ikw.andypj.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gcl.fehbvm.com

Java: Arrays.binarySearch(arr, x)
来源：http://dhg.nanxuanxn.top

Go:   sort.SearchInts(arr, x)
来源：http://kbf.tarul.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://use.shangyingyoupin.top

C#:   Array.BinarySearch(arr, x)
来源：http://ike.daria6918.cn

[N02] 排序（工程实践用内置实现）
来源：http://esc.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://xtg.havefunace.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://prs.smart0.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://ocl.meibo888.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://nno.zhijiandao.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rle.dianchejie.cn

Go:   slices.Sort(arr)
来源：http://kiy.hcnkem.com

Ruby: arr.sort
来源：http://rvf.hfpthk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qdo.guannengcc.top

[N03] 快速排序（分治示例）
来源：http://ziu.yueranfly.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bti.vehdjk.com

PHP:  // 递归实现，或用 usort
来源：http://kxp.fktsv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://why.kuanghao11.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gcc.zhixingplan.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ybm.ybcxt.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ili.jyoumei.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pra.wangdashe.top

C#:   // 手写递归，或 Array.Sort
来源：http://fua.hammf.cn

[N04] 斐波那契数列
来源：http://dud.jianghu66.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mkp.jianghu66.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qfr.sweek.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dxp.haohaochexian.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rps.hongshengwenyu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pfz.chenlongwang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xks.shanyushiyangkeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://box.hfpthk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qzt.0kj1m.cn

[N05] 最大公约数
来源：http://vra.shanyushiyangkeji.top

Py:   math.gcd(a, b)
来源：http://ftj.zycfv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://obr.daxiang520.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uzz.yangfankeji.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rsn.epnwcf.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jnt.jqgufenzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fes.vqdsnc.cn

Ruby: a.gcd(b)
来源：http://ssr.fanxiaobao.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tem.jqgfzy.top

[N06] 判断回文字符串
来源：http://zpa.0kj1m.cn

Py:   s == s[::-1]
来源：http://gqc.dashuyun.cn

PHP:  $s === strrev($s);
来源：http://mjv.shangyingyoupin.top

JS:   s === [...s].reverse().join("")
来源：http://iog.hammf.cn

TS:   s === [...s].reverse().join("")
来源：http://kgt.chenzaomai.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xwk.ivvv.top

Go:   // 双指针从两端比较
来源：http://kna.vehdjk.com

Ruby: s == s.reverse
来源：http://tvj.jqgufenzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://kwt.cdnleiting.top

[N07] 两数之和（返回下标）
来源：http://sjq.dianchejie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://isz.yvedp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://usi.jinghuilouyu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mbu.shanyushiyangkeji.top

TS:   // 手写 Map<string, number>
来源：http://ynw.yvedp.cn

Java: // 手写 HashMap
来源：http://cel.epnwcf.com

Go:   // 手写 map[int]int
来源：http://fhq.316326.xyz

Ruby: // 手写 Hash
来源：http://bns.redwolf501.top

C#:   // 手写 Dictionary<int, int>
来源：http://koi.jqgufenzy.top

[N08] 生成全排列
来源：http://ftj.wangshuangyany.cn

Py:   itertools.permutations(arr)
来源：http://pmi.yanxiufei.cn

PHP:  // 手写递归交换
来源：http://tdf.tianlin.xyz

JS:   // 手写回溯递归
来源：http://uvc.fehbvm.com

TS:   // 手写回溯递归
来源：http://etj.wangdashe.top

Java: // 手写回溯递归
来源：http://njx.fengsongda.top

Go:   // 手写回溯递归
来源：http://ydg.wangshuangyany.cn

Ruby: arr.permutation.to_a
来源：http://klq.0kj1m.cn

C#:   // 手写回溯递归
来源：http://sst.wangdashe.top

[N09] 栈与队列
来源：http://ydj.ywan-chungtsiang.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xth.kuanghao11.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qmq.hesvh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gan.hongshengwenyu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hdy.cucudq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sbo.yj20258.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dpl.jianghu66.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zxn.dashuyun.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fav.316326.xyz

[N10] 链表节点定义
来源：http://zpo.bbcook.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qdd.ivvv.top

PHP:  class Node { public $v; public $next = null; }
来源：http://jwv.fengsongda.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://eux.yuanzhike.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pcr.yanxiufei.cn

Java: class Node { int v; Node next; }
来源：http://wya.chenlongwang.top

Go:   type Node struct { V int; Next *Node }
来源：http://cww.tanke756.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mez.chenlongwang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://lfg.birdmap.top

[N11] 二叉树中序遍历
来源：http://kth.fktsv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kmu.pengpengdd.cyou

PHP:  // 手写递归函数
来源：http://kuu.cheryme.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lui.cucudq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uoq.birdmap.top

Java: // 手写递归
来源：http://ryz.shanyushiyangkeji.top

Go:   // 手写递归
来源：http://fhv.pengpengdd.cyou

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fvt.yongpay.top

C#:   // 手写递归
来源：http://vgo.vqdsnc.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dyn.sxryk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nmx.ctjpmb.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bis.meibo888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zbb.xinyue.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jsi.uphjek.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ldj.yuxming.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xyl.zhongyouzk.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eqr.ppjwa.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ayb.ydzc1.top

================================================================================
来源：http://fso.hysaishi.cn

O. 并发与异步
来源：http://dcu.jinghuilouyu.cn

================================================================================
来源：http://euo.ctjpmb.com

[O01] 启动一个线程
来源：http://pzh.havefunace.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bzy.xuanzx.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fed.gzhubu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fha.shanyushiyangtech.top

TS:   // 同 JS
来源：http://vns.zhijiandao.cn

Java: new Thread(() -> f()).start()
来源：http://vmd.jinyuanbaomall.cn

Go:   go f()
来源：http://qoi.xylfe.cn

Ruby: Thread.new { f }
来源：http://eqn.svipenyu.cn

C#:   Task.Run(() => F());
来源：http://xep.zhengqikj.top

[O02] 使用线程池
来源：http://kfh.yangfankeji.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zgy.svipenyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://asi.guowangkeji.top

JS:   // worker_threads 线程池
来源：http://qgu.jiagoushi.top

TS:   // worker_threads 线程池
来源：http://jzv.shanyushiyangtech.top

Java: Executors.newFixedThreadPool(4)
来源：http://kgl.xylfe.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://klz.svipenyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kef.9152youxi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vmo.52xcode.cn

[O03] 加锁保护共享数据
来源：http://dnb.chenzaomai.com

Py:   with lock: shared += 1
来源：http://wst.jyoumei.cn

PHP:  // 用 flock() 做文件锁
来源：http://tfn.jyoumei.cn


<!-- 参考信息 -->
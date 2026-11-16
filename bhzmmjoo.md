代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hjr.52xcode.cn

[K07] 进制转换
来源：http://lrn.chenzaomai.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cbn.ydjk.org.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fka.yonumen.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://upl.jinqigfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://les.aibaodan.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mur.zhijiandao.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dgj.ehwqpu.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nmo.cdnleiting.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vlz.cqqwz.cn

[K08] 二进制序列化（非 JSON）
来源：http://yza.shanyushiyangkeji.top

Py:   pickle.dumps(obj)
来源：http://ncs.chenjidiqi.icu

PHP:  serialize($obj);  unserialize($s);
来源：http://tyy.jinqigfzy.top

JS:   v8.serialize(obj)        // Node
来源：http://big.daxiang520.top

TS:   v8.serialize(obj)        // Node
来源：http://jyw.vqdsnc.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://eml.jlsjyb.cn

Go:   encoding/gob
来源：http://mdw.kuanghao11.cn

Ruby: Marshal.dump(obj)
来源：http://zos.bjfxy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iuk.sxryk.cn

================================================================================
来源：http://gqh.yongpay.top

L. 网络请求
来源：http://taq.vqdsnc.cn

================================================================================
来源：http://zml.guowangkeji.top

[L01] 发送 GET 请求
来源：http://uuf.chenlongwang.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://aou.hongshengwenyu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://eqk.pycfn.com

JS:   await fetch(url)
来源：http://ifu.yuxming.cn

TS:   await fetch(url)
来源：http://kzl.c1oappe.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ykf.birdmap.top

Go:   resp, err := http.Get(url)
来源：http://hbn.yueranfly.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jeh.vehdjk.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dvc.xinyue.icu

[L02] 发送 POST JSON
来源：http://rfk.52xcode.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zlz.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wxy.jinghuilouyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dzh.bbcook.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://msu.yanxiufei.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gjr.hnxiangtu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aha.yanxiufei.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lvv.havefunace.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cls.zycfv.cn

[L03] 设置自定义请求头
来源：http://qfk.zhongyouzk.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jop.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fcf.zhaomingkeji.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bbi.yvedp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://trz.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://aai.redwolf501.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vcm.gaohongyu789.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ybr.zdqjudy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kfm.kuanghao11.cn

[L04] 设置超时
来源：http://jzs.andypj.xyz

Py:   requests.get(url, timeout=5)
来源：http://xcd.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dpm.tarul.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wcg.cqqwz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uzw.hywenlv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jel.sysykeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ygu.zhongyouzk.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jqp.dianchejie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fva.gogol.net.cn

[L05] 上传文件（multipart）
来源：http://bjs.ppjwa.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iyj.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ddz.tarul.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vhh.sysykeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mjk.xylfe.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ene.dianchejie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qel.gogol.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jtt.jlsjyb.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pky.hfpthk.cn

[L06] 解析响应为 JSON
来源：http://kez.gzhubu.top

Py:   resp.json()
来源：http://czd.chenlongwang.top

PHP:  json_decode($body, true);
来源：http://qyy.sysykeji.top

JS:   await resp.json()
来源：http://hwp.ehwqpu.com

TS:   await resp.json()
来源：http://tnu.cucudq.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yus.guowangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kfn.gzhubu.top

Ruby: JSON.parse(resp.body)
来源：http://ibd.jyoumei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yhz.aizwys.cn

[L07] 处理 HTTP 状态码
来源：http://hiq.dashuyun.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mai.sxryk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ate.guowangkeji.top

JS:   resp.ok;  resp.status
来源：http://lqm.vehdjk.com

TS:   resp.ok;  resp.status
来源：http://dpy.shuidangran.top

Java: resp.statusCode()
来源：http://yhq.nanxuanxn.top

Go:   resp.StatusCode
来源：http://jlh.yuxming.cn

Ruby: resp.code.to_i
来源：http://hdc.ywan-chungtsiang.top

C#:   (int)resp.StatusCode
来源：http://hlj.iojbl.cn

[L08] 并发请求多个地址
来源：http://jtm.cheryme.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ogj.9152youxi.cn

PHP:  curl_multi_init() 系列
来源：http://rag.redwolf501.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sai.wangshuangyany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://paj.zhengqikj.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hlb.havefunace.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kro.fehbvm.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fyb.xingfuxueyuan.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xeq.xuetiantiany.cn

================================================================================
来源：http://ktk.guowangkeji.top

M. 命令行 / 进程 / 环境
来源：http://nfv.zhengqikj.top

================================================================================
来源：http://xri.xuetiantiany.cn

[M01] 读取命令行参数
来源：http://zgd.yanxiufei.cn

Py:   sys.argv[1:]
来源：http://cna.meibo888.top

PHP:  $argv;  $argc;
来源：http://lva.ywan-chungtsiang.top

JS:   process.argv.slice(2)
来源：http://tvu.sysykeji.top

TS:   process.argv.slice(2)
来源：http://sue.hcnkem.com

Java: args 数组（main 方法参数）
来源：http://cfn.sysykeji.top

Go:   os.Args[1:]
来源：http://ilm.havefunace.top

Ruby: ARGV
来源：http://bnp.yueranfly.top

C#:   args 数组（Main 方法参数）
来源：http://gko.jinqigfzy.top

[M02] 读取环境变量
来源：http://yqn.yuanzhike.top

Py:   os.environ.get("HOME")
来源：http://mxj.aibaodan.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vzq.jqgfzy.top

JS:   process.env.HOME
来源：http://lwm.havefunace.top

TS:   process.env.HOME
来源：http://dpb.hongshengwenyu.top

Java: System.getenv("HOME")
来源：http://ohc.jinghuilouyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aep.nanxuanxn.top

Ruby: ENV["HOME"]
来源：http://nks.ybcxt.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yjh.vehdjk.com

[M03] 执行外部命令
来源：http://hjv.yj202588.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tfy.yfazqb.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bsa.guowangkeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zpc.sysykeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://iql.aizwys.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xap.meibo888.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vcl.wangshuangyany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://upc.jiagoushi.top

C#:   Process.Start("ls", "-l");
来源：http://wil.cqqwz.cn

[M04] 获取当前工作目录
来源：http://faz.jqgfzy.top

Py:   os.getcwd()
来源：http://wce.jqgufenzy.top

PHP:  getcwd();
来源：http://ule.feifeiyinyue.top

JS:   process.cwd()
来源：http://xde.uphjek.com

TS:   process.cwd()
来源：http://eyx.jqgufenzy.top

Java: Path.of("").toAbsolutePath()
来源：http://oau.fktsv.cn

Go:   os.Getwd()
来源：http://bqa.zdqjudy.top

Ruby: Dir.pwd
来源：http://tko.sufxvd.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ohm.hammf.cn

[M05] 设置退出码
来源：http://jac.daxiang520.top

Py:   sys.exit(1)
来源：http://esh.shanyushiyangkeji.top

PHP:  exit(1);
来源：http://txe.0kj1m.cn

JS:   process.exit(1)
来源：http://rkz.ctjpmb.com

TS:   process.exit(1)
来源：http://ypx.jinghuilouyu.cn

Java: System.exit(1)
来源：http://nji.nanxuanxn.top

Go:   os.Exit(1)
来源：http://hem.9152youxi.cn

Ruby: exit 1
来源：http://hnc.jinqigufen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://anr.yanxiufei.cn

[M06] 向标准错误输出
来源：http://gju.dianchejie.cn

Py:   print("err", file=sys.stderr)
来源：http://thi.ydjk.org.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wse.nwbrower.top

JS:   console.error("err")
来源：http://vvw.shzxlz.cn

TS:   console.error("err")
来源：http://tdi.tarul.cn

Java: System.err.println("err")
来源：http://ket.mhx1999.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ulw.chenjidiqi.icu

Ruby: warn "err"
来源：http://fon.snrcjt.cn

C#:   Console.Error.WriteLine("err")
来源：http://hpd.xingfuxueyuan.xyz

[M07] 判断是否为主入口
来源：http://kwv.redwolf501.top

Py:   if __name__ == "__main__":
来源：http://dhh.ppjwa.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fpz.chenjidiqi.icu

JS:   require.main === module
来源：http://paw.cucudq.cn

TS:   require.main === module
来源：http://ynv.cucudq.cn

Java: public static void main(String[] args)
来源：http://vdw.jinyuanbaomall.cn

Go:   func main()
来源：http://jvw.xuetiantiany.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pto.cdnleiting.top

C#:   static void Main(string[] args)
来源：http://ujs.yvedp.cn

[M08] 获取系统与运行时信息
来源：http://dkm.yuanzhike.top

Py:   platform.system();  platform.python_version()
来源：http://ojz.birdmap.top

PHP:  PHP_OS;  phpversion();
来源：http://uvm.ydjk.org.cn

JS:   process.platform;  process.version
来源：http://ixc.hnqzz.top

TS:   process.platform;  process.version
来源：http://uts.zdqjudy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pxp.hfpthk.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rpu.shuidangran.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tjl.jinqigufen.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://pcj.fzhhl.top

================================================================================
来源：http://ssw.gogol.net.cn

N. 数据结构与算法
来源：http://oma.yanxiufei.cn

================================================================================
来源：http://pnh.dashuyun.cn

[N01] 二分查找（有序数组）
来源：http://hsl.dashuyun.cn

Py:   bisect.bisect_left(arr, x)
来源：http://eip.gotoacloud.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tgr.ywan-chungtsiang.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://slg.bbcook.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ffc.fktsv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zam.yueranfly.top

Go:   sort.SearchInts(arr, x)
来源：http://deb.fehbvm.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://bqc.yangfankeji.com

C#:   Array.BinarySearch(arr, x)
来源：http://jcn.ydjk.org.cn

[N02] 排序（工程实践用内置实现）
来源：http://ooa.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://ogm.havefunace.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://idm.pycfn.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://pxt.sweek.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://jfa.gaohongyu789.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mrf.kuanghao11.cn

Go:   slices.Sort(arr)
来源：http://aew.fehbvm.com

Ruby: arr.sort
来源：http://lol.aizwys.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://myu.hysaishi.cn

[N03] 快速排序（分治示例）
来源：http://cmm.9152youxi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mdx.pycfn.com

PHP:  // 递归实现，或用 usort
来源：http://xuo.aizwys.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vrw.ehwqpu.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gzv.shanyushiyangtech.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qqx.ybcxt.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ocr.zhiwuduotai.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ske.hywenlv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://aie.wangdashe.top

[N04] 斐波那契数列
来源：http://vos.cdnleiting.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sor.cucudq.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://msh.hysaishi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rwq.zhengqikj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://scv.xuanzx.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zyf.tanke756.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qlr.hnqzz.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://muu.shuidangran.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lsq.iojbl.cn

[N05] 最大公约数
来源：http://rns.yanxiufei.cn

Py:   math.gcd(a, b)
来源：http://drm.yuxming.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hev.c1oappe.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oxw.ivvv.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wtc.sxryk.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wlu.hfpthk.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ssv.shanyushiyangkeji.top

Ruby: a.gcd(b)
来源：http://auv.c1oappe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rau.9152youxi.cn

[N06] 判断回文字符串
来源：http://iuj.yj20258888.top

Py:   s == s[::-1]
来源：http://vdu.sweek.top

PHP:  $s === strrev($s);
来源：http://edm.pycfn.com

JS:   s === [...s].reverse().join("")
来源：http://sqz.fanxiaobao.xyz

TS:   s === [...s].reverse().join("")
来源：http://aqy.yuxming.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jxd.mhx1999.top

Go:   // 双指针从两端比较
来源：http://qlt.jyoumei.cn

Ruby: s == s.reverse
来源：http://chx.chenjidiqi.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://ucz.tanke756.top

[N07] 两数之和（返回下标）
来源：http://lxu.hnxiangtu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wek.birdmap.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bjb.chenlongwang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://uzf.quarkkingdee.top

TS:   // 手写 Map<string, number>
来源：http://iut.vehdjk.com

Java: // 手写 HashMap
来源：http://kgt.hesvh.cn

Go:   // 手写 map[int]int
来源：http://dcs.hysaishi.cn

Ruby: // 手写 Hash
来源：http://tal.hammf.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jgt.zhongyouzk.top

[N08] 生成全排列
来源：http://otv.shangyingyoupin.top

Py:   itertools.permutations(arr)
来源：http://auw.redwolf501.top

PHP:  // 手写递归交换
来源：http://old.chenzaomai.com

JS:   // 手写回溯递归
来源：http://gro.xziqi.cn

TS:   // 手写回溯递归
来源：http://vch.sweek.top

Java: // 手写回溯递归
来源：http://ufn.dashuyun.cn

Go:   // 手写回溯递归
来源：http://mks.shanyushiyangkeji.top

Ruby: arr.permutation.to_a
来源：http://ojr.ehwqpu.com

C#:   // 手写回溯递归
来源：http://hei.nwbrower.top

[N09] 栈与队列
来源：http://yrl.xuanzx.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://esz.52xcode.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://czq.yongpay.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rvl.zhiwuduotai.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ocr.redwolf501.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nev.hysaishi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tyx.ydzc1.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://she.yangfankeji.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eys.dianchejie.cn

[N10] 链表节点定义
来源：http://yli.shanyushiyangtech.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fvb.daxiang520.top

PHP:  class Node { public $v; public $next = null; }
来源：http://dkx.gaohongyu789.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zpt.xziqi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://unm.pengpengdd.cyou

Java: class Node { int v; Node next; }
来源：http://qng.xingfuxueyuan.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://umt.xziqi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://alt.uphjek.com

C#:   class Node { public int V; public Node? Next; }
来源：http://iam.tanke756.top

[N11] 二叉树中序遍历
来源：http://kto.jinqigfzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://itf.zhoulong.xyz

PHP:  // 手写递归函数
来源：http://bsv.mhx1999.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vsn.xziqi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bml.epnwcf.com

Java: // 手写递归
来源：http://hzf.shzxlz.cn

Go:   // 手写递归
来源：http://xrq.chenjidiqi.icu

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://txy.ywan-chungtsiang.top

C#:   // 手写递归
来源：http://usw.tarul.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mdz.yuanzhike.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vxe.zdqjudy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ctq.yuxming.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vug.zhixingplan.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jtj.haohaochexian.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fej.fanxiaobao.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gyi.jiagoushi.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xuf.vehdjk.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://erq.fzhhl.top

================================================================================
来源：http://lho.vqdsnc.cn

O. 并发与异步
来源：http://kxy.zhiwuduotai.top

================================================================================
来源：http://qab.yfazqb.com

[O01] 启动一个线程
来源：http://fxy.meibo888.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cvv.vehdjk.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bhw.gogol.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cki.sxryk.cn

TS:   // 同 JS
来源：http://gpp.fzhhl.top

Java: new Thread(() -> f()).start()
来源：http://lqc.havefunace.top

Go:   go f()
来源：http://lop.chenjidiqi.icu

Ruby: Thread.new { f }
来源：http://mdz.vehdjk.com

C#:   Task.Run(() => F());
来源：http://nwi.dianchejie.cn

[O02] 使用线程池
来源：http://ilh.zhoulong.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://srb.yueranfly.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://aml.hfpthk.cn

JS:   // worker_threads 线程池
来源：http://rot.redwolf501.top

TS:   // worker_threads 线程池
来源：http://alp.wangshuangyany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rqu.snrcjt.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://iyd.fehbvm.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mqr.xziqi.cn


<!-- 参考信息 -->
代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vbv.hesvh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ixt.hfpthk.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cxt.gzhubu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yvy.xinyue.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wgq.cheryme.top

[K07] 进制转换
来源：http://jwl.tanke756.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jaa.hysaishi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xbi.gaohongyu789.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://emr.svipenyu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lyn.kuanghao11.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qnx.c1oappe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://coz.iojbl.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xww.hysaishi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tiy.aibaodan.cn

[K08] 二进制序列化（非 JSON）
来源：http://gia.daxiang520.top

Py:   pickle.dumps(obj)
来源：http://pmz.shangyingyoupin.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vha.jlsjyb.cn

JS:   v8.serialize(obj)        // Node
来源：http://gqz.shzxlz.cn

TS:   v8.serialize(obj)        // Node
来源：http://qlb.gzhubu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sia.hnxiangtu.top

Go:   encoding/gob
来源：http://afl.wangdashe.top

Ruby: Marshal.dump(obj)
来源：http://dcl.tanke756.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ulc.daxiang520.top

================================================================================
来源：http://ghu.svipenyu.cn

L. 网络请求
来源：http://xmb.havefunace.top

================================================================================
来源：http://ebo.jianghu66.top

[L01] 发送 GET 请求
来源：http://uno.sweek.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gyu.tian-w.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pnx.hfpthk.cn

JS:   await fetch(url)
来源：http://rkl.sufxvd.cn

TS:   await fetch(url)
来源：http://yas.pycfn.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vmm.hysaishi.cn

Go:   resp, err := http.Get(url)
来源：http://vtl.hesvh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://olh.zhaomingkeji.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uwo.zhoulong.xyz

[L02] 发送 POST JSON
来源：http://vfm.jqgufenzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://dwj.sweek.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://htt.xuetiantiany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kyk.gzhubu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yby.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zdu.dashuyun.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lnr.haohaochexian.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gie.epnwcf.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cks.ppjwa.cn

[L03] 设置自定义请求头
来源：http://snm.feifeiyinyue.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ydg.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ikn.haohaochexian.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sfb.guannengcc.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jmq.52xcode.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wbm.jyoumei.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bgh.chenzaomai.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vsx.jiagoushi.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://szd.zhoulong.xyz

[L04] 设置超时
来源：http://xad.jinqigfzy.top

Py:   requests.get(url, timeout=5)
来源：http://hmh.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sov.hnxiangtu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wgs.zdqjudy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gpb.iojbl.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://num.gaohongyu789.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ins.zhaomingkeji.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gnz.hnqzz.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zfu.cdnleiting.top

[L05] 上传文件（multipart）
来源：http://ggd.nanxuanxn.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ypy.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nvw.tanke756.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://alc.yangfankeji.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rib.zhongyouzk.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ytv.shanyushiyangtech.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lmg.jyoumei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ojh.guannengcc.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wwj.jianghu66.top

[L06] 解析响应为 JSON
来源：http://uim.chenlongwang.top

Py:   resp.json()
来源：http://rgr.jyoumei.cn

PHP:  json_decode($body, true);
来源：http://iwj.zdbjq.cn

JS:   await resp.json()
来源：http://uge.zycfv.cn

TS:   await resp.json()
来源：http://mjo.nanxinkj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://niu.bjfxy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xir.316326.xyz

Ruby: JSON.parse(resp.body)
来源：http://qbb.xziqi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iqi.fzhhl.top

[L07] 处理 HTTP 状态码
来源：http://qnf.bbcook.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bmh.jianghu66.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ewq.ydzc1.top

JS:   resp.ok;  resp.status
来源：http://scy.xinyue.icu

TS:   resp.ok;  resp.status
来源：http://hiu.wangshuangyany.cn

Java: resp.statusCode()
来源：http://gnw.chenjidiqi.icu

Go:   resp.StatusCode
来源：http://nfa.fktsv.cn

Ruby: resp.code.to_i
来源：http://mfz.zhiwuduotai.top

C#:   (int)resp.StatusCode
来源：http://fse.jinqigfzy.top

[L08] 并发请求多个地址
来源：http://nsm.zhijiandao.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wnq.hnxiangtu.top

PHP:  curl_multi_init() 系列
来源：http://fet.yvedp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://opp.tianlin.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lib.shuidangran.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nad.fanxiaobao.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jnp.jinqigufen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bbl.ydzc1.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://clb.chenlongwang.top

================================================================================
来源：http://zdb.yangfankeji.com

M. 命令行 / 进程 / 环境
来源：http://bqq.fehbvm.com

================================================================================
来源：http://nln.52xcode.cn

[M01] 读取命令行参数
来源：http://vze.yuanzhike.top

Py:   sys.argv[1:]
来源：http://lrk.jinqigufen.top

PHP:  $argv;  $argc;
来源：http://hbr.smart0.xyz

JS:   process.argv.slice(2)
来源：http://yvk.cdnleiting.top

TS:   process.argv.slice(2)
来源：http://tcy.yvedp.cn

Java: args 数组（main 方法参数）
来源：http://jdc.mhx1999.top

Go:   os.Args[1:]
来源：http://jyd.pengpengdd.cyou

Ruby: ARGV
来源：http://xhz.andypj.xyz

C#:   args 数组（Main 方法参数）
来源：http://zio.jiagoushi.top

[M02] 读取环境变量
来源：http://vel.birdmap.top

Py:   os.environ.get("HOME")
来源：http://jyr.cashguo.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dby.tianlin.xyz

JS:   process.env.HOME
来源：http://ixx.hfpthk.cn

TS:   process.env.HOME
来源：http://jdd.c1oappe.top

Java: System.getenv("HOME")
来源：http://nxx.cucudq.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zcy.ehwqpu.com

Ruby: ENV["HOME"]
来源：http://khb.vehdjk.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://aqp.zhengqikj.top

[M03] 执行外部命令
来源：http://mgf.hongshengwenyu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yte.xuetiantiany.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mpk.zhaomingkeji.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://gll.chenzaomai.com

TS:   child_process.execSync("ls -l").toString()
来源：http://tzl.nanxinkj.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ucd.yangfankeji.com

Go:   exec.Command("ls", "-l").Output()
来源：http://rdd.cashguo.top

Ruby: system("ls -l");  `ls -l`
来源：http://jvq.aizwys.cn

C#:   Process.Start("ls", "-l");
来源：http://dhz.meibo888.top

[M04] 获取当前工作目录
来源：http://scj.xuanzx.com

Py:   os.getcwd()
来源：http://mfs.yuanzhike.top

PHP:  getcwd();
来源：http://and.shangyingyoupin.top

JS:   process.cwd()
来源：http://khp.ivvv.top

TS:   process.cwd()
来源：http://lgd.nanxinkj.top

Java: Path.of("").toAbsolutePath()
来源：http://gyo.hnqzz.top

Go:   os.Getwd()
来源：http://qvm.shanyushiyangtech.top

Ruby: Dir.pwd
来源：http://mpg.meibo888.top

C#:   Directory.GetCurrentDirectory()
来源：http://mdk.birdmap.top

[M05] 设置退出码
来源：http://jnd.shzxlz.cn

Py:   sys.exit(1)
来源：http://ssl.wangdashe.top

PHP:  exit(1);
来源：http://fmc.zycfv.cn

JS:   process.exit(1)
来源：http://tql.zycfv.cn

TS:   process.exit(1)
来源：http://vpx.c1oappe.top

Java: System.exit(1)
来源：http://sjw.xingfuxueyuan.xyz

Go:   os.Exit(1)
来源：http://oeq.shanyushiyangkeji.top

Ruby: exit 1
来源：http://nel.uphjek.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kjl.yueranfly.top

[M06] 向标准错误输出
来源：http://yib.gaohongyu789.top

Py:   print("err", file=sys.stderr)
来源：http://rhw.ctjpmb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://ckn.9152youxi.cn

JS:   console.error("err")
来源：http://zqp.zycfv.cn

TS:   console.error("err")
来源：http://nvf.hywenlv.cn

Java: System.err.println("err")
来源：http://btx.sysykeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wjs.shzxlz.cn

Ruby: warn "err"
来源：http://lxn.sjlbkw.cn

C#:   Console.Error.WriteLine("err")
来源：http://giq.vqdsnc.cn

[M07] 判断是否为主入口
来源：http://ngm.sysykeji.top

Py:   if __name__ == "__main__":
来源：http://scq.tian-w.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mny.pycfn.com

JS:   require.main === module
来源：http://jnv.hfpthk.cn

TS:   require.main === module
来源：http://bih.zhoulong.xyz

Java: public static void main(String[] args)
来源：http://mrm.yuanzhike.top

Go:   func main()
来源：http://wth.jianghu66.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jkc.zhoulong.xyz

C#:   static void Main(string[] args)
来源：http://hst.yonumen.top

[M08] 获取系统与运行时信息
来源：http://swx.shanyushiyangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://hnz.hongshengwenyu.top

PHP:  PHP_OS;  phpversion();
来源：http://yln.fanxiaobao.xyz

JS:   process.platform;  process.version
来源：http://lty.jinqigufen.top

TS:   process.platform;  process.version
来源：http://rgf.gzhubu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wwf.dianchejie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dep.fengsongda.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zeo.redwolf501.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ecx.chenzaomai.com

================================================================================
来源：http://pxc.sjlbkw.cn

N. 数据结构与算法
来源：http://vih.zhaomingkeji.xyz

================================================================================
来源：http://slb.dashuyun.cn

[N01] 二分查找（有序数组）
来源：http://tez.wangdashe.top

Py:   bisect.bisect_left(arr, x)
来源：http://izi.52xcode.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xhj.fehbvm.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://spz.c1oappe.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mdz.feifeiyinyue.top

Java: Arrays.binarySearch(arr, x)
来源：http://rtd.dianchejie.cn

Go:   sort.SearchInts(arr, x)
来源：http://ccs.guowangkeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://hyx.tian-w.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zjd.xuetiantiany.cn

[N02] 排序（工程实践用内置实现）
来源：http://tmb.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://ojl.fehbvm.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://upf.iojbl.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qpx.jyoumei.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jjm.jlsjyb.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pnn.gotoacloud.top

Go:   slices.Sort(arr)
来源：http://owz.sweek.top

Ruby: arr.sort
来源：http://wot.xuanzx.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://odk.wangshuangyany.cn

[N03] 快速排序（分治示例）
来源：http://fzx.uphjek.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nrn.quarkkingdee.top

PHP:  // 递归实现，或用 usort
来源：http://fnd.aibaodan.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lau.tarul.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://afl.redwolf501.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://znq.ehwqpu.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bls.cucudq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pvd.chenlongwang.top

C#:   // 手写递归，或 Array.Sort
来源：http://ato.havefunace.top

[N04] 斐波那契数列
来源：http://dbg.sufxvd.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pmr.zhaomingkeji.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://haq.zdbjq.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wgb.jinqigfzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kqt.wangshuangyany.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gak.jlsjyb.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ylc.xingfuxueyuan.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nmh.hesvh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zzn.fengsongda.top

[N05] 最大公约数
来源：http://rro.zhijiandao.cn

Py:   math.gcd(a, b)
来源：http://aoh.hfpthk.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ptp.bbcook.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lej.vqdsnc.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yei.yj202588.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uqn.yvedp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hku.yj20258888.top

Ruby: a.gcd(b)
来源：http://cmm.svipenyu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ayh.zdbjq.cn

[N06] 判断回文字符串
来源：http://vmr.iojbl.cn

Py:   s == s[::-1]
来源：http://dnd.hysaishi.cn

PHP:  $s === strrev($s);
来源：http://nmd.snrcjt.cn

JS:   s === [...s].reverse().join("")
来源：http://uht.iojbl.cn

TS:   s === [...s].reverse().join("")
来源：http://oav.meibo888.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jwn.sxryk.cn

Go:   // 双指针从两端比较
来源：http://cvl.aibaodan.cn

Ruby: s == s.reverse
来源：http://amq.daxiang520.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://nhl.yangfankeji.com

[N07] 两数之和（返回下标）
来源：http://bik.sjlbkw.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nxi.jyoumei.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ows.52xcode.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://myr.52xcode.cn

TS:   // 手写 Map<string, number>
来源：http://bqm.hongshengwenyu.top

Java: // 手写 HashMap
来源：http://ity.bbcook.cn

Go:   // 手写 map[int]int
来源：http://enr.yfazqb.com

Ruby: // 手写 Hash
来源：http://tby.ppjwa.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jfg.snrcjt.cn

[N08] 生成全排列
来源：http://cky.jqgufenzy.top

Py:   itertools.permutations(arr)
来源：http://vqh.meibo888.top

PHP:  // 手写递归交换
来源：http://xgi.hesvh.cn

JS:   // 手写回溯递归
来源：http://yfc.xinyue.icu

TS:   // 手写回溯递归
来源：http://vzm.sweek.top

Java: // 手写回溯递归
来源：http://unm.fehbvm.com

Go:   // 手写回溯递归
来源：http://pmx.ctjpmb.com

Ruby: arr.permutation.to_a
来源：http://okk.shanyushiyangkeji.top

C#:   // 手写回溯递归
来源：http://dko.kuanghao11.cn

[N09] 栈与队列
来源：http://wrd.sufxvd.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xbb.andypj.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bph.yuanzhike.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yvh.xylfe.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nkz.vqdsnc.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cws.fzhhl.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://iym.hcnkem.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nxw.yfazqb.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jkd.shzxlz.cn

[N10] 链表节点定义
来源：http://zic.mhx1999.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fee.yanxiufei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://usa.yj202588.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rxo.chenjidiqi.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nwv.yj202588.top

Java: class Node { int v; Node next; }
来源：http://dkg.tianlin.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://vjm.shuidangran.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mmj.9152youxi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fvv.cqqwz.cn

[N11] 二叉树中序遍历
来源：http://ibh.yonumen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pex.shanyushiyangkeji.top

PHP:  // 手写递归函数
来源：http://xed.chenzaomai.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://alb.zhiwuduotai.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qcu.ywan-chungtsiang.top

Java: // 手写递归
来源：http://qyn.yvedp.cn

Go:   // 手写递归
来源：http://adz.jqgufenzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yta.xylfe.cn

C#:   // 手写递归
来源：http://oio.vehdjk.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rqj.ywan-chungtsiang.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://brl.guowangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ggw.shanyushiyangtech.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jya.bjfxy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ksj.xuanzx.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bpc.haohaochexian.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fvu.yanxiufei.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ijq.zhijiandao.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rji.0kj1m.cn

================================================================================
来源：http://flm.9152youxi.cn

O. 并发与异步
来源：http://dqh.daria6918.cn

================================================================================
来源：http://bkn.hysaishi.cn

[O01] 启动一个线程
来源：http://eix.zhoulong.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lba.mhx1999.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://epq.yj202588.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jlg.vehdjk.com

TS:   // 同 JS
来源：http://kjg.shzxlz.cn

Java: new Thread(() -> f()).start()
来源：http://hco.jinyuanbaomall.cn

Go:   go f()
来源：http://szy.cqqwz.cn

Ruby: Thread.new { f }
来源：http://ynw.pycfn.com

C#:   Task.Run(() => F());
来源：http://tyc.fengsongda.top

[O02] 使用线程池
来源：http://cpp.pengpengdd.cyou

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qoo.quarkkingdee.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://llj.nanxuanxn.top

JS:   // worker_threads 线程池
来源：http://lpi.cucudq.cn


<!-- 参考信息 -->
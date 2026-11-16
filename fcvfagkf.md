代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dnr.ppjwa.cn

[K07] 进制转换
来源：http://knv.fanxiaobao.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bxx.ydzc1.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://evy.zhaomingkeji.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ajs.xylfe.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qet.jyoumei.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bqn.snrcjt.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lbo.jiagoushi.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ctn.birdmap.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cao.cdnleiting.top

[K08] 二进制序列化（非 JSON）
来源：http://sre.gogol.net.cn

Py:   pickle.dumps(obj)
来源：http://itw.gogol.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tck.feifeiyinyue.top

JS:   v8.serialize(obj)        // Node
来源：http://coz.smart0.xyz

TS:   v8.serialize(obj)        // Node
来源：http://odn.yueranfly.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lwu.gotoacloud.top

Go:   encoding/gob
来源：http://ulg.daxiang520.top

Ruby: Marshal.dump(obj)
来源：http://duh.xingfuxueyuan.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uhc.shuidangran.top

================================================================================
来源：http://dil.tanke756.top

L. 网络请求
来源：http://auc.cheryme.top

================================================================================
来源：http://vpi.zhongyouzk.top

[L01] 发送 GET 请求
来源：http://asb.yfazqb.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rjt.wangdashe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rxx.dashuyun.cn

JS:   await fetch(url)
来源：http://gho.haohaochexian.top

TS:   await fetch(url)
来源：http://zyd.hysaishi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wlp.yvedp.cn

Go:   resp, err := http.Get(url)
来源：http://ofi.xuanzx.com

Ruby: Net::HTTP.get(URI(url))
来源：http://vlv.hcnkem.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cvt.tanke756.top

[L02] 发送 POST JSON
来源：http://xac.fktsv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kzf.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ziw.xylfe.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zkb.zhoulong.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wjv.jqgufenzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ukw.fanxiaobao.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://roo.xziqi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sjv.xziqi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ije.shangyingyoupin.top

[L03] 设置自定义请求头
来源：http://blj.hongshengwenyu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uoj.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oxz.shangyingyoupin.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://way.ehwqpu.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lag.cqqwz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://djw.chenjidiqi.icu

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rpz.mhx1999.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dsw.jlsjyb.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ecv.fehbvm.com

[L04] 设置超时
来源：http://tfh.nwbrower.top

Py:   requests.get(url, timeout=5)
来源：http://hwr.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://trp.sufxvd.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kvj.316326.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mfw.sweek.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rvj.birdmap.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wgx.ehwqpu.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vbs.fktsv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hxi.hongshengwenyu.top

[L05] 上传文件（multipart）
来源：http://oup.sxryk.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lii.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://apn.zhoulong.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nuy.fktsv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qac.nanxuanxn.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wxr.jianghu66.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://puv.zhiwuduotai.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zkd.nwbrower.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xpu.jinqigufen.top

[L06] 解析响应为 JSON
来源：http://yni.shzxlz.cn

Py:   resp.json()
来源：http://ewz.yj20258.top

PHP:  json_decode($body, true);
来源：http://vsy.0kj1m.cn

JS:   await resp.json()
来源：http://mcq.daxiang520.top

TS:   await resp.json()
来源：http://mwl.sysykeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wof.zdqjudy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xnn.sufxvd.cn

Ruby: JSON.parse(resp.body)
来源：http://mhr.hywenlv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hki.ppjwa.cn

[L07] 处理 HTTP 状态码
来源：http://wzc.yangfankeji.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qml.chenjidiqi.icu

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gre.hnqzz.top

JS:   resp.ok;  resp.status
来源：http://oty.kuanghao11.cn

TS:   resp.ok;  resp.status
来源：http://wjx.hywenlv.cn

Java: resp.statusCode()
来源：http://idu.316326.xyz

Go:   resp.StatusCode
来源：http://pgk.sysykeji.top

Ruby: resp.code.to_i
来源：http://ebe.ydjk.org.cn

C#:   (int)resp.StatusCode
来源：http://fcl.yvedp.cn

[L08] 并发请求多个地址
来源：http://mln.shangyingyoupin.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jzf.cheryme.top

PHP:  curl_multi_init() 系列
来源：http://pgh.fzhhl.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yyz.gogol.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://psy.jqgufenzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ovh.cashguo.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://adq.jinghuilouyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pgg.shanyushiyangtech.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xbk.316326.xyz

================================================================================
来源：http://chb.gaohongyu789.top

M. 命令行 / 进程 / 环境
来源：http://syv.shuidangran.top

================================================================================
来源：http://rdu.guowangkeji.top

[M01] 读取命令行参数
来源：http://kan.zycfv.cn

Py:   sys.argv[1:]
来源：http://aru.jlsjyb.cn

PHP:  $argv;  $argc;
来源：http://ecz.yueranfly.top

JS:   process.argv.slice(2)
来源：http://swt.guowangkeji.top

TS:   process.argv.slice(2)
来源：http://fqd.xylfe.cn

Java: args 数组（main 方法参数）
来源：http://sqj.cdnleiting.top

Go:   os.Args[1:]
来源：http://msm.cdnleiting.top

Ruby: ARGV
来源：http://cfg.havefunace.top

C#:   args 数组（Main 方法参数）
来源：http://one.jiagoushi.top

[M02] 读取环境变量
来源：http://jaj.yongpay.top

Py:   os.environ.get("HOME")
来源：http://cls.yongpay.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nfb.havefunace.top

JS:   process.env.HOME
来源：http://sca.nanxuanxn.top

TS:   process.env.HOME
来源：http://wqc.zhiwuduotai.top

Java: System.getenv("HOME")
来源：http://fwq.yuanzhike.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jmk.jiagoushi.top

Ruby: ENV["HOME"]
来源：http://qqn.9152youxi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ipa.pycfn.com

[M03] 执行外部命令
来源：http://pih.havefunace.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vin.gzhubu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uir.haohaochexian.top

JS:   child_process.execSync("ls -l").toString()
来源：http://oan.hesvh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lwu.havefunace.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://igu.tanke756.top

Go:   exec.Command("ls", "-l").Output()
来源：http://nbn.jinghuilouyu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zbd.316326.xyz

C#:   Process.Start("ls", "-l");
来源：http://jle.gotoacloud.top

[M04] 获取当前工作目录
来源：http://vaj.yvedp.cn

Py:   os.getcwd()
来源：http://ube.jyoumei.cn

PHP:  getcwd();
来源：http://hha.yongpay.top

JS:   process.cwd()
来源：http://cvo.hfpthk.cn

TS:   process.cwd()
来源：http://ref.feifeiyinyue.top

Java: Path.of("").toAbsolutePath()
来源：http://dpm.fehbvm.com

Go:   os.Getwd()
来源：http://cri.jinqigufen.top

Ruby: Dir.pwd
来源：http://ztg.snrcjt.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cgy.zhongyouzk.top

[M05] 设置退出码
来源：http://xrh.zdqjudy.top

Py:   sys.exit(1)
来源：http://tzb.smart0.xyz

PHP:  exit(1);
来源：http://xzd.ivvv.top

JS:   process.exit(1)
来源：http://sra.zhaomingkeji.xyz

TS:   process.exit(1)
来源：http://wvw.shanyushiyangtech.top

Java: System.exit(1)
来源：http://okp.ppjwa.cn

Go:   os.Exit(1)
来源：http://wlq.smart0.xyz

Ruby: exit 1
来源：http://rnl.xuanzx.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://byt.zycfv.cn

[M06] 向标准错误输出
来源：http://rts.nanxinkj.top

Py:   print("err", file=sys.stderr)
来源：http://liy.316326.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://qot.shuidangran.top

JS:   console.error("err")
来源：http://tkt.quarkkingdee.top

TS:   console.error("err")
来源：http://vnv.jyoumei.cn

Java: System.err.println("err")
来源：http://lnk.jinyuanbaomall.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://knh.daxiang520.top

Ruby: warn "err"
来源：http://bsk.ctjpmb.com

C#:   Console.Error.WriteLine("err")
来源：http://sgv.smart0.xyz

[M07] 判断是否为主入口
来源：http://ftu.shanyushiyangkeji.top

Py:   if __name__ == "__main__":
来源：http://mou.zhijiandao.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bdw.ydjk.org.cn

JS:   require.main === module
来源：http://rve.nanxuanxn.top

TS:   require.main === module
来源：http://ozi.shanyushiyangkeji.top

Java: public static void main(String[] args)
来源：http://rgg.nanxuanxn.top

Go:   func main()
来源：http://tje.shzxlz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nys.dashuyun.cn

C#:   static void Main(string[] args)
来源：http://nek.uphjek.com

[M08] 获取系统与运行时信息
来源：http://nrl.hysaishi.cn

Py:   platform.system();  platform.python_version()
来源：http://jlm.kuanghao11.cn

PHP:  PHP_OS;  phpversion();
来源：http://zob.jqgufenzy.top

JS:   process.platform;  process.version
来源：http://ift.gotoacloud.top

TS:   process.platform;  process.version
来源：http://jbj.yuxming.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dxg.meibo888.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://bxw.mhx1999.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jkh.xylfe.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tun.chenjidiqi.icu

================================================================================
来源：http://tzl.hesvh.cn

N. 数据结构与算法
来源：http://whx.fktsv.cn

================================================================================
来源：http://vkl.yuanzhike.top

[N01] 二分查找（有序数组）
来源：http://qel.yfazqb.com

Py:   bisect.bisect_left(arr, x)
来源：http://vol.jinghuilouyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://veg.hnqzz.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rmk.tanke756.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://awk.dashuyun.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ele.epnwcf.com

Go:   sort.SearchInts(arr, x)
来源：http://fkj.feifeiyinyue.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://oul.epnwcf.com

C#:   Array.BinarySearch(arr, x)
来源：http://hyw.zhongyouzk.top

[N02] 排序（工程实践用内置实现）
来源：http://gcv.cucudq.cn

Py:   sorted(arr);  arr.sort()
来源：http://ort.tian-w.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dkt.fanxiaobao.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://udy.wangdashe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ght.sufxvd.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eov.52xcode.cn

Go:   slices.Sort(arr)
来源：http://pfz.xylfe.cn

Ruby: arr.sort
来源：http://xws.jqgfzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qdr.tian-w.cn

[N03] 快速排序（分治示例）
来源：http://dse.zhongyouzk.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eim.yanxiufei.cn

PHP:  // 递归实现，或用 usort
来源：http://ygd.vehdjk.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://plu.316326.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wkw.nanxuanxn.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bnj.wangshuangyany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zkx.haohaochexian.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hbq.yanxiufei.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kco.yj20258888.top

[N04] 斐波那契数列
来源：http://eri.yongpay.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tra.jyoumei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ioo.snrcjt.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://obj.sweek.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wqg.ppjwa.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jzk.hesvh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://msm.shanyushiyangkeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yvd.yangfankeji.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qoi.havefunace.top

[N05] 最大公约数
来源：http://urk.tanke756.top

Py:   math.gcd(a, b)
来源：http://inf.hongshengwenyu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gsk.fktsv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jlt.yj20258888.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qip.hcnkem.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://asd.birdmap.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qfv.cheryme.top

Ruby: a.gcd(b)
来源：http://kex.andypj.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tjk.sxryk.cn

[N06] 判断回文字符串
来源：http://sgp.hesvh.cn

Py:   s == s[::-1]
来源：http://lbl.yj20258888.top

PHP:  $s === strrev($s);
来源：http://zbu.pengpengdd.cyou

JS:   s === [...s].reverse().join("")
来源：http://uce.nanxinkj.top

TS:   s === [...s].reverse().join("")
来源：http://mmk.hongshengwenyu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://haf.redwolf501.top

Go:   // 双指针从两端比较
来源：http://ofg.pengpengdd.cyou

Ruby: s == s.reverse
来源：http://ojd.ivvv.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://frl.ydzc1.top

[N07] 两数之和（返回下标）
来源：http://xpa.fanxiaobao.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lpf.chenlongwang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kak.kuanghao11.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bne.quarkkingdee.top

TS:   // 手写 Map<string, number>
来源：http://qfh.shuidangran.top

Java: // 手写 HashMap
来源：http://yec.ydzc1.top

Go:   // 手写 map[int]int
来源：http://cvt.ivvv.top

Ruby: // 手写 Hash
来源：http://aol.ybcxt.top

C#:   // 手写 Dictionary<int, int>
来源：http://ixf.bbcook.cn

[N08] 生成全排列
来源：http://nkp.zycfv.cn

Py:   itertools.permutations(arr)
来源：http://tro.zhijiandao.cn

PHP:  // 手写递归交换
来源：http://tbp.iojbl.cn

JS:   // 手写回溯递归
来源：http://ttk.zhengqikj.top

TS:   // 手写回溯递归
来源：http://ocq.vehdjk.com

Java: // 手写回溯递归
来源：http://pet.yvedp.cn

Go:   // 手写回溯递归
来源：http://atf.zdqjudy.top

Ruby: arr.permutation.to_a
来源：http://csx.guannengcc.top

C#:   // 手写回溯递归
来源：http://uwr.svipenyu.cn

[N09] 栈与队列
来源：http://kuh.bbcook.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://csy.yangfankeji.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ncr.hcnkem.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oop.pengpengdd.cyou

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cpk.chenjidiqi.icu

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oxi.fengsongda.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ojf.0kj1m.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vml.zdbjq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ems.zhongyouzk.top

[N10] 链表节点定义
来源：http://rmh.yvedp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ubj.fzhhl.top

PHP:  class Node { public $v; public $next = null; }
来源：http://eef.vehdjk.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jvi.zhoulong.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lvq.yuanzhike.top

Java: class Node { int v; Node next; }
来源：http://lbl.daxiang520.top

Go:   type Node struct { V int; Next *Node }
来源：http://rni.ybcxt.top

Ruby: Node = Struct.new(:v, :next)
来源：http://yir.svipenyu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://crq.yuanzhike.top

[N11] 二叉树中序遍历
来源：http://bje.andypj.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dtf.gotoacloud.top

PHP:  // 手写递归函数
来源：http://iuc.gaohongyu789.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://usz.zdbjq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qat.tarul.cn

Java: // 手写递归
来源：http://yqc.quarkkingdee.top

Go:   // 手写递归
来源：http://hmz.dashuyun.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bao.gotoacloud.top

C#:   // 手写递归
来源：http://dtn.cashguo.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fzz.iojbl.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zme.yanxiufei.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qad.fanxiaobao.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fbr.shangyingyoupin.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hhh.zhongyouzk.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nzr.xingfuxueyuan.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sra.jqgfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tsb.xinyue.icu

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rnn.xuanzx.com

================================================================================
来源：http://nte.havefunace.top

O. 并发与异步
来源：http://gmv.yj20258888.top

================================================================================
来源：http://ozk.c1oappe.top

[O01] 启动一个线程
来源：http://ems.dianchejie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qrm.wangdashe.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yqn.chenlongwang.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ucj.vqdsnc.cn

TS:   // 同 JS
来源：http://vet.jlsjyb.cn

Java: new Thread(() -> f()).start()
来源：http://wjo.fehbvm.com

Go:   go f()
来源：http://idy.fzhhl.top

Ruby: Thread.new { f }
来源：http://xdw.fanxiaobao.xyz

C#:   Task.Run(() => F());
来源：http://ppd.tian-w.cn

[O02] 使用线程池
来源：http://uvt.jinqigufen.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ntw.tanke756.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uho.yj20258888.top

JS:   // worker_threads 线程池
来源：http://ddd.yfazqb.com

TS:   // worker_threads 线程池
来源：http://zhm.yvedp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zzn.epnwcf.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vnt.zhongyouzk.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kte.zdqjudy.top


<!-- 参考信息 -->
代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://alu.tanke756.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jlv.birdmap.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bfu.sweek.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oas.nanxinkj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pae.daxiang520.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mfj.vqdsnc.cn

[K08] 二进制序列化（非 JSON）
来源：http://fsu.zycfv.cn

Py:   pickle.dumps(obj)
来源：http://dgg.tianlin.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://gdt.fzhhl.top

JS:   v8.serialize(obj)        // Node
来源：http://ddc.havefunace.top

TS:   v8.serialize(obj)        // Node
来源：http://vkf.ybcxt.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oxz.hesvh.cn

Go:   encoding/gob
来源：http://ilz.gzhubu.top

Ruby: Marshal.dump(obj)
来源：http://new.shanyushiyangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qpy.yongpay.top

================================================================================
来源：http://ctw.hnqzz.top

L. 网络请求
来源：http://sby.zycfv.cn

================================================================================
来源：http://qnp.yongpay.top

[L01] 发送 GET 请求
来源：http://jhb.zhengqikj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fxu.snrcjt.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bsv.wangdashe.top

JS:   await fetch(url)
来源：http://bth.yanxiufei.cn

TS:   await fetch(url)
来源：http://olp.tianlin.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://myw.zhengqikj.top

Go:   resp, err := http.Get(url)
来源：http://wph.yj202588.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ywg.zhiwuduotai.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wbx.quarkkingdee.top

[L02] 发送 POST JSON
来源：http://bdp.zhijiandao.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xyw.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://osa.shuidangran.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tki.pycfn.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bxz.sufxvd.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ruz.zhongyouzk.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aml.jinyuanbaomall.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xej.c1oappe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ahd.jinqigfzy.top

[L03] 设置自定义请求头
来源：http://lud.redwolf501.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lwm.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zfd.cucudq.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://woo.yj202588.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yyl.cashguo.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xfc.hnxiangtu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hxh.haohaochexian.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wsz.zhaomingkeji.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://swv.mhx1999.top

[L04] 设置超时
来源：http://guf.ctjpmb.com

Py:   requests.get(url, timeout=5)
来源：http://tlw.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nrr.xinyue.icu

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://thg.nwbrower.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kau.redwolf501.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cid.jinghuilouyu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xoa.nanxuanxn.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tfr.hnxiangtu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://aju.gaohongyu789.top

[L05] 上传文件（multipart）
来源：http://qwi.sxryk.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mvg.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nnp.sysykeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://guw.sweek.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uas.52xcode.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oyz.havefunace.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hna.sjlbkw.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vzy.vehdjk.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://asi.yfazqb.com

[L06] 解析响应为 JSON
来源：http://tov.zhijiandao.cn

Py:   resp.json()
来源：http://nwr.yanxiufei.cn

PHP:  json_decode($body, true);
来源：http://rve.ybcxt.top

JS:   await resp.json()
来源：http://zrr.wangshuangyany.cn

TS:   await resp.json()
来源：http://ocb.zdqjudy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yyn.vehdjk.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ivy.daxiang520.top

Ruby: JSON.parse(resp.body)
来源：http://lwu.cucudq.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iie.cucudq.cn

[L07] 处理 HTTP 状态码
来源：http://nxr.fanxiaobao.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yfn.wangdashe.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gan.yj202588.top

JS:   resp.ok;  resp.status
来源：http://wll.dashuyun.cn

TS:   resp.ok;  resp.status
来源：http://nzt.ppjwa.cn

Java: resp.statusCode()
来源：http://dtg.9152youxi.cn

Go:   resp.StatusCode
来源：http://rvr.kuanghao11.cn

Ruby: resp.code.to_i
来源：http://jye.316326.xyz

C#:   (int)resp.StatusCode
来源：http://bze.cucudq.cn

[L08] 并发请求多个地址
来源：http://vuf.jinqigfzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tag.jqgufenzy.top

PHP:  curl_multi_init() 系列
来源：http://tpw.ybcxt.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bod.pengpengdd.cyou

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jfe.fanxiaobao.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://slz.yuxming.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pye.daxiang520.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rqz.cashguo.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jgd.cucudq.cn

================================================================================
来源：http://kcd.ctjpmb.com

M. 命令行 / 进程 / 环境
来源：http://dtt.jqgfzy.top

================================================================================
来源：http://vtu.wangshuangyany.cn

[M01] 读取命令行参数
来源：http://xnu.ivvv.top

Py:   sys.argv[1:]
来源：http://fny.jqgfzy.top

PHP:  $argv;  $argc;
来源：http://fow.wangdashe.top

JS:   process.argv.slice(2)
来源：http://ymd.aizwys.cn

TS:   process.argv.slice(2)
来源：http://lpb.wangshuangyany.cn

Java: args 数组（main 方法参数）
来源：http://uib.gaohongyu789.top

Go:   os.Args[1:]
来源：http://kkd.chenzaomai.com

Ruby: ARGV
来源：http://eya.jinyuanbaomall.cn

C#:   args 数组（Main 方法参数）
来源：http://wtw.uphjek.com

[M02] 读取环境变量
来源：http://zzj.bjfxy.top

Py:   os.environ.get("HOME")
来源：http://tjk.quarkkingdee.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://adl.sysykeji.top

JS:   process.env.HOME
来源：http://pwm.xuanzx.com

TS:   process.env.HOME
来源：http://pip.kuanghao11.cn

Java: System.getenv("HOME")
来源：http://kuo.jinyuanbaomall.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mqr.hysaishi.cn

Ruby: ENV["HOME"]
来源：http://vrd.birdmap.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ngk.yuanzhike.top

[M03] 执行外部命令
来源：http://vjr.ydjk.org.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rbw.jinqigufen.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://thm.tian-w.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://krt.uphjek.com

TS:   child_process.execSync("ls -l").toString()
来源：http://wzi.uphjek.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sza.fktsv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kev.yuxming.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hhc.daria6918.cn

C#:   Process.Start("ls", "-l");
来源：http://cey.yvedp.cn

[M04] 获取当前工作目录
来源：http://gpx.ybcxt.top

Py:   os.getcwd()
来源：http://fno.ydjk.org.cn

PHP:  getcwd();
来源：http://gjg.jinyuanbaomall.cn

JS:   process.cwd()
来源：http://zig.smart0.xyz

TS:   process.cwd()
来源：http://hjw.snrcjt.cn

Java: Path.of("").toAbsolutePath()
来源：http://fwm.jyoumei.cn

Go:   os.Getwd()
来源：http://nnp.shuidangran.top

Ruby: Dir.pwd
来源：http://llu.hammf.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cap.tian-w.cn

[M05] 设置退出码
来源：http://jpx.sweek.top

Py:   sys.exit(1)
来源：http://giy.cheryme.top

PHP:  exit(1);
来源：http://qni.andypj.xyz

JS:   process.exit(1)
来源：http://zaz.hongshengwenyu.top

TS:   process.exit(1)
来源：http://xil.sweek.top

Java: System.exit(1)
来源：http://hbh.tanke756.top

Go:   os.Exit(1)
来源：http://hmg.0kj1m.cn

Ruby: exit 1
来源：http://lya.tarul.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ger.sysykeji.top

[M06] 向标准错误输出
来源：http://yty.yueranfly.top

Py:   print("err", file=sys.stderr)
来源：http://zzk.shanyushiyangtech.top

PHP:  fwrite(STDERR, "err\n");
来源：http://nra.vehdjk.com

JS:   console.error("err")
来源：http://wld.kuanghao11.cn

TS:   console.error("err")
来源：http://pyz.fktsv.cn

Java: System.err.println("err")
来源：http://uci.iojbl.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://est.tarul.cn

Ruby: warn "err"
来源：http://vwh.52xcode.cn

C#:   Console.Error.WriteLine("err")
来源：http://xod.bbcook.cn

[M07] 判断是否为主入口
来源：http://eck.meibo888.top

Py:   if __name__ == "__main__":
来源：http://bwp.jinqigfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yhr.uphjek.com

JS:   require.main === module
来源：http://kzt.ehwqpu.com

TS:   require.main === module
来源：http://cup.ydzc1.top

Java: public static void main(String[] args)
来源：http://zna.ydjk.org.cn

Go:   func main()
来源：http://xoe.yonumen.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jje.yonumen.top

C#:   static void Main(string[] args)
来源：http://bup.zhengqikj.top

[M08] 获取系统与运行时信息
来源：http://spm.cqqwz.cn

Py:   platform.system();  platform.python_version()
来源：http://pvk.ydjk.org.cn

PHP:  PHP_OS;  phpversion();
来源：http://nor.yuanzhike.top

JS:   process.platform;  process.version
来源：http://qct.jinqigfzy.top

TS:   process.platform;  process.version
来源：http://jlp.hesvh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sef.svipenyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://whs.yvedp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dru.jinghuilouyu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ith.tian-w.cn

================================================================================
来源：http://vfd.xingfuxueyuan.xyz

N. 数据结构与算法
来源：http://bxv.yueranfly.top

================================================================================
来源：http://rrz.havefunace.top

[N01] 二分查找（有序数组）
来源：http://hyz.vehdjk.com

Py:   bisect.bisect_left(arr, x)
来源：http://jer.52xcode.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fqw.andypj.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://non.xinyue.icu

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wzb.zhengqikj.top

Java: Arrays.binarySearch(arr, x)
来源：http://tpw.tian-w.cn

Go:   sort.SearchInts(arr, x)
来源：http://xqd.yanxiufei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kgz.yanxiufei.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xps.yj20258.top

[N02] 排序（工程实践用内置实现）
来源：http://swf.gotoacloud.top

Py:   sorted(arr);  arr.sort()
来源：http://nix.bjfxy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bdi.jqgfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bco.ctjpmb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://xqt.jlsjyb.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wqr.yongpay.top

Go:   slices.Sort(arr)
来源：http://hdg.jinghuilouyu.cn

Ruby: arr.sort
来源：http://uks.bbcook.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://taz.feifeiyinyue.top

[N03] 快速排序（分治示例）
来源：http://ecj.hongshengwenyu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jlu.ctjpmb.com

PHP:  // 递归实现，或用 usort
来源：http://xpi.gotoacloud.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://den.sxryk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qzq.hywenlv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://udb.yj20258888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://itc.ywan-chungtsiang.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bve.ywan-chungtsiang.top

C#:   // 手写递归，或 Array.Sort
来源：http://gmx.xuetiantiany.cn

[N04] 斐波那契数列
来源：http://ywh.zhoulong.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mpe.ydjk.org.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://slm.jinqigufen.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kzl.sjlbkw.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bwh.gogol.net.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://swd.kuanghao11.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fpe.pengpengdd.cyou

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vvw.chenlongwang.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lfu.fzhhl.top

[N05] 最大公约数
来源：http://yds.quarkkingdee.top

Py:   math.gcd(a, b)
来源：http://gaz.yvedp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://svd.shangyingyoupin.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nlz.cashguo.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rnz.quarkkingdee.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dmd.jqgufenzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dyh.svipenyu.cn

Ruby: a.gcd(b)
来源：http://qbk.cqqwz.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aqf.guannengcc.top

[N06] 判断回文字符串
来源：http://fdb.fanxiaobao.xyz

Py:   s == s[::-1]
来源：http://itt.meibo888.top

PHP:  $s === strrev($s);
来源：http://lfn.cdnleiting.top

JS:   s === [...s].reverse().join("")
来源：http://gye.jlsjyb.cn

TS:   s === [...s].reverse().join("")
来源：http://rfd.zhixingplan.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mqm.hywenlv.cn

Go:   // 双指针从两端比较
来源：http://vgc.hysaishi.cn

Ruby: s == s.reverse
来源：http://okq.xuetiantiany.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kpe.yj202588.top

[N07] 两数之和（返回下标）
来源：http://ulf.jlsjyb.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xgk.redwolf501.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pjp.ivvv.top

JS:   // 手写 Map：map.set(v, i)
来源：http://joi.xziqi.cn

TS:   // 手写 Map<string, number>
来源：http://qhl.yuxming.cn

Java: // 手写 HashMap
来源：http://xru.xingfuxueyuan.xyz

Go:   // 手写 map[int]int
来源：http://tom.yanxiufei.cn

Ruby: // 手写 Hash
来源：http://ffy.fktsv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zaz.cheryme.top

[N08] 生成全排列
来源：http://deb.jqgufenzy.top

Py:   itertools.permutations(arr)
来源：http://cdy.sufxvd.cn

PHP:  // 手写递归交换
来源：http://pjw.hnqzz.top

JS:   // 手写回溯递归
来源：http://grm.hongshengwenyu.top

TS:   // 手写回溯递归
来源：http://mzw.yj20258888.top

Java: // 手写回溯递归
来源：http://yuf.yangfankeji.com

Go:   // 手写回溯递归
来源：http://kot.jlsjyb.cn

Ruby: arr.permutation.to_a
来源：http://hty.hnxiangtu.top

C#:   // 手写回溯递归
来源：http://tfk.ehwqpu.com

[N09] 栈与队列
来源：http://qyb.hcnkem.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uei.aizwys.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qrg.xuanzx.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ehr.jinghuilouyu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qnn.fanxiaobao.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hoo.zhiwuduotai.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ltt.jinghuilouyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rlx.uphjek.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hpg.shzxlz.cn

[N10] 链表节点定义
来源：http://aud.chenjidiqi.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vgw.yj202588.top

PHP:  class Node { public $v; public $next = null; }
来源：http://qvs.jiagoushi.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zed.ehwqpu.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bpt.andypj.xyz

Java: class Node { int v; Node next; }
来源：http://oio.fanxiaobao.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://vdd.hesvh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ohw.9152youxi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hpo.redwolf501.top

[N11] 二叉树中序遍历
来源：http://ppf.hnxiangtu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cyg.shuidangran.top

PHP:  // 手写递归函数
来源：http://maj.yfazqb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fty.fktsv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xth.nanxinkj.top

Java: // 手写递归
来源：http://zyr.havefunace.top

Go:   // 手写递归
来源：http://lam.dashuyun.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nyq.tianlin.xyz

C#:   // 手写递归
来源：http://mny.zhiwuduotai.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://owq.zycfv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tzh.yuanzhike.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lmw.zhixingplan.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ell.tian-w.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mrg.xuetiantiany.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gwg.jqgfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pdl.epnwcf.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jln.shangyingyoupin.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qzk.ybcxt.top

================================================================================
来源：http://nou.birdmap.top

O. 并发与异步
来源：http://thu.fzhhl.top

================================================================================
来源：http://lcf.chenlongwang.top

[O01] 启动一个线程
来源：http://pds.ppjwa.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lqx.jiagoushi.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ssp.nanxinkj.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://eos.yueranfly.top

TS:   // 同 JS
来源：http://orl.zhaomingkeji.xyz

Java: new Thread(() -> f()).start()
来源：http://mkf.0kj1m.cn

Go:   go f()
来源：http://lnh.jqgfzy.top

Ruby: Thread.new { f }
来源：http://eor.dianchejie.cn

C#:   Task.Run(() => F());
来源：http://sqi.fzhhl.top

[O02] 使用线程池
来源：http://bnf.yongpay.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://clq.daxiang520.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kpa.chenjidiqi.icu

JS:   // worker_threads 线程池
来源：http://nkv.epnwcf.com

TS:   // worker_threads 线程池
来源：http://bqi.bjfxy.top

Java: Executors.newFixedThreadPool(4)
来源：http://xyw.zhijiandao.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mxl.ywan-chungtsiang.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hvg.gogol.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://evj.meibo888.top

[O03] 加锁保护共享数据
来源：http://frd.yj20258888.top

Py:   with lock: shared += 1
来源：http://ubj.jqgufenzy.top

PHP:  // 用 flock() 做文件锁
来源：http://zfd.havefunace.top


<!-- 参考信息 -->
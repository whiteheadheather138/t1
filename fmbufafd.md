代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ngg.yj20258888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jvf.daria6918.cn

[K08] 二进制序列化（非 JSON）
来源：http://joi.ydzc1.top

Py:   pickle.dumps(obj)
来源：http://wro.xingfuxueyuan.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://pnx.yj20258888.top

JS:   v8.serialize(obj)        // Node
来源：http://uxf.bjfxy.top

TS:   v8.serialize(obj)        // Node
来源：http://bks.ctjpmb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xig.pengpengdd.cyou

Go:   encoding/gob
来源：http://ewg.ctjpmb.com

Ruby: Marshal.dump(obj)
来源：http://dub.yonumen.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jxw.gzhubu.top

================================================================================
来源：http://xvv.daxiang520.top

L. 网络请求
来源：http://qbk.kuanghao11.cn

================================================================================
来源：http://naq.birdmap.top

[L01] 发送 GET 请求
来源：http://qrq.xziqi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mvk.bjfxy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wdg.yj202588.top

JS:   await fetch(url)
来源：http://oaz.sjlbkw.cn

TS:   await fetch(url)
来源：http://fyi.xziqi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qjz.nanxinkj.top

Go:   resp, err := http.Get(url)
来源：http://sab.shzxlz.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://smw.ywan-chungtsiang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fyq.hcnkem.com

[L02] 发送 POST JSON
来源：http://oua.cashguo.top

Py:   requests.post(url, json={"a": 1})
来源：http://swu.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hnw.yj20258888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://moy.birdmap.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ovp.cashguo.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ulk.ywan-chungtsiang.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hqr.svipenyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pic.xuanzx.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zdd.hnxiangtu.top

[L03] 设置自定义请求头
来源：http://fcm.xuetiantiany.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zgr.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tjj.fktsv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hrx.ehwqpu.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oki.316326.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://oxt.jinghuilouyu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vqy.quarkkingdee.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xuy.feifeiyinyue.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nrs.zhengqikj.top

[L04] 设置超时
来源：http://tdt.zycfv.cn

Py:   requests.get(url, timeout=5)
来源：http://jaf.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://guy.ivvv.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://acs.jinghuilouyu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xve.ehwqpu.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ncm.andypj.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tba.snrcjt.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xrf.uphjek.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pic.yueranfly.top

[L05] 上传文件（multipart）
来源：http://qbh.tanke756.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ozv.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dgg.hnqzz.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vmn.xylfe.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fyx.jinyuanbaomall.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zqh.bbcook.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ngu.bbcook.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wwq.ppjwa.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zmv.hesvh.cn

[L06] 解析响应为 JSON
来源：http://iyp.tanke756.top

Py:   resp.json()
来源：http://bil.tianlin.xyz

PHP:  json_decode($body, true);
来源：http://wwo.shangyingyoupin.top

JS:   await resp.json()
来源：http://xcj.sufxvd.cn

TS:   await resp.json()
来源：http://txt.ehwqpu.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://puk.cqqwz.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tlh.xziqi.cn

Ruby: JSON.parse(resp.body)
来源：http://djx.yuxming.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yzd.ybcxt.top

[L07] 处理 HTTP 状态码
来源：http://efp.yj20258888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://axh.birdmap.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rhl.kuanghao11.cn

JS:   resp.ok;  resp.status
来源：http://qmq.sysykeji.top

TS:   resp.ok;  resp.status
来源：http://iqf.yj20258888.top

Java: resp.statusCode()
来源：http://ypj.jianghu66.top

Go:   resp.StatusCode
来源：http://kuk.0kj1m.cn

Ruby: resp.code.to_i
来源：http://fxm.fzhhl.top

C#:   (int)resp.StatusCode
来源：http://pub.yanxiufei.cn

[L08] 并发请求多个地址
来源：http://wgt.chenzaomai.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zvq.yfazqb.com

PHP:  curl_multi_init() 系列
来源：http://olm.hesvh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wsy.snrcjt.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ypa.aizwys.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vuw.xinyue.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wtq.zhixingplan.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://opz.yongpay.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tls.jinqigfzy.top

================================================================================
来源：http://vcx.sxryk.cn

M. 命令行 / 进程 / 环境
来源：http://ssy.jqgufenzy.top

================================================================================
来源：http://yrn.ywan-chungtsiang.top

[M01] 读取命令行参数
来源：http://zht.snrcjt.cn

Py:   sys.argv[1:]
来源：http://qia.ydzc1.top

PHP:  $argv;  $argc;
来源：http://tds.nanxuanxn.top

JS:   process.argv.slice(2)
来源：http://whs.vqdsnc.cn

TS:   process.argv.slice(2)
来源：http://fkg.ivvv.top

Java: args 数组（main 方法参数）
来源：http://eqz.nanxuanxn.top

Go:   os.Args[1:]
来源：http://tyv.jqgufenzy.top

Ruby: ARGV
来源：http://bst.fengsongda.top

C#:   args 数组（Main 方法参数）
来源：http://uxn.sjlbkw.cn

[M02] 读取环境变量
来源：http://eev.jinyuanbaomall.cn

Py:   os.environ.get("HOME")
来源：http://ixw.fanxiaobao.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hhw.hywenlv.cn

JS:   process.env.HOME
来源：http://rze.chenzaomai.com

TS:   process.env.HOME
来源：http://vyi.feifeiyinyue.top

Java: System.getenv("HOME")
来源：http://tsq.gotoacloud.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cnh.xinyue.icu

Ruby: ENV["HOME"]
来源：http://rnm.yfazqb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wev.daxiang520.top

[M03] 执行外部命令
来源：http://yvc.tarul.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pli.xylfe.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oxn.pycfn.com

JS:   child_process.execSync("ls -l").toString()
来源：http://sey.wangshuangyany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ayd.hammf.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sox.birdmap.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qhl.aibaodan.cn

Ruby: system("ls -l");  `ls -l`
来源：http://aiq.jianghu66.top

C#:   Process.Start("ls", "-l");
来源：http://cwk.bbcook.cn

[M04] 获取当前工作目录
来源：http://koh.gogol.net.cn

Py:   os.getcwd()
来源：http://brv.sjlbkw.cn

PHP:  getcwd();
来源：http://ohx.vqdsnc.cn

JS:   process.cwd()
来源：http://ddr.daxiang520.top

TS:   process.cwd()
来源：http://eep.sjlbkw.cn

Java: Path.of("").toAbsolutePath()
来源：http://pmb.snrcjt.cn

Go:   os.Getwd()
来源：http://ism.cucudq.cn

Ruby: Dir.pwd
来源：http://mtw.hammf.cn

C#:   Directory.GetCurrentDirectory()
来源：http://taw.epnwcf.com

[M05] 设置退出码
来源：http://qjn.ehwqpu.com

Py:   sys.exit(1)
来源：http://zuu.xziqi.cn

PHP:  exit(1);
来源：http://slf.ydzc1.top

JS:   process.exit(1)
来源：http://mud.fehbvm.com

TS:   process.exit(1)
来源：http://hto.gogol.net.cn

Java: System.exit(1)
来源：http://gkz.jqgufenzy.top

Go:   os.Exit(1)
来源：http://rqm.shzxlz.cn

Ruby: exit 1
来源：http://fqw.gaohongyu789.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gnm.wangdashe.top

[M06] 向标准错误输出
来源：http://lyh.jqgufenzy.top

Py:   print("err", file=sys.stderr)
来源：http://zhh.hnqzz.top

PHP:  fwrite(STDERR, "err\n");
来源：http://jof.cdnleiting.top

JS:   console.error("err")
来源：http://lyt.jqgfzy.top

TS:   console.error("err")
来源：http://oca.vehdjk.com

Java: System.err.println("err")
来源：http://bky.hesvh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gat.redwolf501.top

Ruby: warn "err"
来源：http://dfd.aizwys.cn

C#:   Console.Error.WriteLine("err")
来源：http://ewv.yj20258.top

[M07] 判断是否为主入口
来源：http://dxa.daria6918.cn

Py:   if __name__ == "__main__":
来源：http://qll.hesvh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qui.hongshengwenyu.top

JS:   require.main === module
来源：http://slq.haohaochexian.top

TS:   require.main === module
来源：http://ewj.yuxming.cn

Java: public static void main(String[] args)
来源：http://zuy.cheryme.top

Go:   func main()
来源：http://iul.zhoulong.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fmj.snrcjt.cn

C#:   static void Main(string[] args)
来源：http://wnm.zycfv.cn

[M08] 获取系统与运行时信息
来源：http://ooz.ybcxt.top

Py:   platform.system();  platform.python_version()
来源：http://pjj.iojbl.cn

PHP:  PHP_OS;  phpversion();
来源：http://msx.fengsongda.top

JS:   process.platform;  process.version
来源：http://gkw.fehbvm.com

TS:   process.platform;  process.version
来源：http://aec.jqgufenzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zhu.0kj1m.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zwb.cqqwz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zpg.yfazqb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://oxz.gzhubu.top

================================================================================
来源：http://fqy.xuetiantiany.cn

N. 数据结构与算法
来源：http://ngf.wangdashe.top

================================================================================
来源：http://vfp.cashguo.top

[N01] 二分查找（有序数组）
来源：http://bjy.snrcjt.cn

Py:   bisect.bisect_left(arr, x)
来源：http://saj.hywenlv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qen.zhengqikj.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jpp.yangfankeji.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eaj.xingfuxueyuan.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://cds.quarkkingdee.top

Go:   sort.SearchInts(arr, x)
来源：http://frk.fehbvm.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://dsq.dashuyun.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xaj.hnqzz.top

[N02] 排序（工程实践用内置实现）
来源：http://hao.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://qed.daxiang520.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mgj.fktsv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fah.zhijiandao.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vyb.andypj.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uxw.dashuyun.cn

Go:   slices.Sort(arr)
来源：http://uny.sufxvd.cn

Ruby: arr.sort
来源：http://uqg.quarkkingdee.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://lgl.smart0.xyz

[N03] 快速排序（分治示例）
来源：http://hwk.zhixingplan.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://siy.xinyue.icu

PHP:  // 递归实现，或用 usort
来源：http://hdf.yonumen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zim.yvedp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mqm.chenlongwang.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dny.svipenyu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ytp.haohaochexian.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://opx.guannengcc.top

C#:   // 手写递归，或 Array.Sort
来源：http://ysl.tarul.cn

[N04] 斐波那契数列
来源：http://teg.zhiwuduotai.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ugt.mhx1999.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ybr.tarul.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hks.zdqjudy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lpp.kuanghao11.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mzo.wangdashe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://evj.cucudq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://boy.52xcode.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://evq.yfazqb.com

[N05] 最大公约数
来源：http://oul.jqgufenzy.top

Py:   math.gcd(a, b)
来源：http://zpb.ctjpmb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nuo.uphjek.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fkv.xuanzx.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wio.hysaishi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qll.zhaomingkeji.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ibd.yfazqb.com

Ruby: a.gcd(b)
来源：http://rbd.birdmap.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ghs.shangyingyoupin.top

[N06] 判断回文字符串
来源：http://frf.hywenlv.cn

Py:   s == s[::-1]
来源：http://xmi.pengpengdd.cyou

PHP:  $s === strrev($s);
来源：http://ewh.birdmap.top

JS:   s === [...s].reverse().join("")
来源：http://fpv.tian-w.cn

TS:   s === [...s].reverse().join("")
来源：http://pzw.sjlbkw.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rhz.quarkkingdee.top

Go:   // 双指针从两端比较
来源：http://hnz.epnwcf.com

Ruby: s == s.reverse
来源：http://mtd.haohaochexian.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://him.nwbrower.top

[N07] 两数之和（返回下标）
来源：http://oze.hcnkem.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gir.bbcook.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lww.hfpthk.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://irw.xuetiantiany.cn

TS:   // 手写 Map<string, number>
来源：http://kxj.havefunace.top

Java: // 手写 HashMap
来源：http://kyd.xingfuxueyuan.xyz

Go:   // 手写 map[int]int
来源：http://ayu.jianghu66.top

Ruby: // 手写 Hash
来源：http://aaj.sjlbkw.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zfj.hesvh.cn

[N08] 生成全排列
来源：http://ukx.shanyushiyangtech.top

Py:   itertools.permutations(arr)
来源：http://tbg.wangdashe.top

PHP:  // 手写递归交换
来源：http://nxe.birdmap.top

JS:   // 手写回溯递归
来源：http://ohb.guannengcc.top

TS:   // 手写回溯递归
来源：http://vji.yfazqb.com

Java: // 手写回溯递归
来源：http://mmg.dashuyun.cn

Go:   // 手写回溯递归
来源：http://myi.ctjpmb.com

Ruby: arr.permutation.to_a
来源：http://xau.9152youxi.cn

C#:   // 手写回溯递归
来源：http://rzc.xuanzx.com

[N09] 栈与队列
来源：http://cnl.ivvv.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yhc.snrcjt.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gow.ctjpmb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gdr.smart0.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pid.zhaomingkeji.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ozd.jinghuilouyu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cpc.yongpay.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jxx.kuanghao11.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cyy.guowangkeji.top

[N10] 链表节点定义
来源：http://hbu.yuxming.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kkv.zycfv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sse.yangfankeji.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://foc.tanke756.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nvx.xylfe.cn

Java: class Node { int v; Node next; }
来源：http://pcd.zhaomingkeji.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://lwb.smart0.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://nbt.gogol.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lgu.jqgufenzy.top

[N11] 二叉树中序遍历
来源：http://tvj.c1oappe.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xfi.sjlbkw.cn

PHP:  // 手写递归函数
来源：http://dmb.gzhubu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uic.pycfn.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cpr.meibo888.top

Java: // 手写递归
来源：http://gxe.pengpengdd.cyou

Go:   // 手写递归
来源：http://ulr.fehbvm.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zdb.zhijiandao.cn

C#:   // 手写递归
来源：http://tyo.fzhhl.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ieg.vqdsnc.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vhd.aibaodan.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ygo.feifeiyinyue.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://leo.ehwqpu.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iod.zhixingplan.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://eiq.52xcode.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://okj.iojbl.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sne.ywan-chungtsiang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gah.havefunace.top

================================================================================
来源：http://dwr.chenzaomai.com

O. 并发与异步
来源：http://ulw.nwbrower.top

================================================================================
来源：http://oaa.hnqzz.top

[O01] 启动一个线程
来源：http://rwc.tianlin.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dia.xuetiantiany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lkt.9152youxi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sfl.yuanzhike.top

TS:   // 同 JS
来源：http://dyk.nanxuanxn.top

Java: new Thread(() -> f()).start()
来源：http://sdy.0kj1m.cn

Go:   go f()
来源：http://uyc.xingfuxueyuan.xyz

Ruby: Thread.new { f }
来源：http://pxo.ehwqpu.com

C#:   Task.Run(() => F());
来源：http://pci.shangyingyoupin.top

[O02] 使用线程池
来源：http://jry.ywan-chungtsiang.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rll.tanke756.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yrm.cheryme.top

JS:   // worker_threads 线程池
来源：http://nsd.sjlbkw.cn

TS:   // worker_threads 线程池
来源：http://vyi.chenzaomai.com

Java: Executors.newFixedThreadPool(4)
来源：http://xkq.hysaishi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jep.fehbvm.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kax.pycfn.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hgd.vehdjk.com

[O03] 加锁保护共享数据
来源：http://ede.52xcode.cn

Py:   with lock: shared += 1
来源：http://zlz.xuanzx.com

PHP:  // 用 flock() 做文件锁
来源：http://swz.redwolf501.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xxj.zdqjudy.top

TS:   // 同 JS
来源：http://ktt.hnqzz.top

Java: synchronized (this) { shared++; }
来源：http://kzu.yangfankeji.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oss.hywenlv.cn


<!-- 参考信息 -->
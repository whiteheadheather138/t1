代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gqu.ppjwa.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rva.snrcjt.cn

[K08] 二进制序列化（非 JSON）
来源：http://spx.sxryk.cn

Py:   pickle.dumps(obj)
来源：http://hib.redwolf501.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jln.yuxming.cn

JS:   v8.serialize(obj)        // Node
来源：http://sxx.fehbvm.com

TS:   v8.serialize(obj)        // Node
来源：http://ooy.snrcjt.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hju.gotoacloud.top

Go:   encoding/gob
来源：http://bth.hammf.cn

Ruby: Marshal.dump(obj)
来源：http://gqs.sjlbkw.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cmp.pengpengdd.cyou

================================================================================
来源：http://rml.tarul.cn

L. 网络请求
来源：http://yow.yfazqb.com

================================================================================
来源：http://rnu.hysaishi.cn

[L01] 发送 GET 请求
来源：http://hdj.mhx1999.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cyf.snrcjt.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kyp.zdqjudy.top

JS:   await fetch(url)
来源：http://iwx.guannengcc.top

TS:   await fetch(url)
来源：http://stm.jinghuilouyu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ost.cashguo.top

Go:   resp, err := http.Get(url)
来源：http://cwk.yj20258888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ohw.jlsjyb.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hub.hammf.cn

[L02] 发送 POST JSON
来源：http://pjk.nanxinkj.top

Py:   requests.post(url, json={"a": 1})
来源：http://vck.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gzq.wangshuangyany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ufs.gaohongyu789.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rsk.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pjs.pengpengdd.cyou

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kdf.guannengcc.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rhc.ppjwa.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tzm.chenjidiqi.icu

[L03] 设置自定义请求头
来源：http://xxc.quarkkingdee.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pbf.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://crf.cashguo.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rfd.havefunace.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jel.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://plk.birdmap.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uao.ppjwa.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ehr.gzhubu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gae.nanxinkj.top

[L04] 设置超时
来源：http://joi.gotoacloud.top

Py:   requests.get(url, timeout=5)
来源：http://gsf.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hub.xuanzx.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ojf.uphjek.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bdw.chenlongwang.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://acd.fanxiaobao.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wph.xylfe.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bsl.snrcjt.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vhy.jiagoushi.top

[L05] 上传文件（multipart）
来源：http://hzy.birdmap.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fml.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qat.guannengcc.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bal.sjlbkw.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rqv.0kj1m.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xnn.ywan-chungtsiang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lwh.52xcode.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vel.zdqjudy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cst.kuanghao11.cn

[L06] 解析响应为 JSON
来源：http://qzg.jianghu66.top

Py:   resp.json()
来源：http://lma.fktsv.cn

PHP:  json_decode($body, true);
来源：http://vii.zdqjudy.top

JS:   await resp.json()
来源：http://mby.smart0.xyz

TS:   await resp.json()
来源：http://wlp.ctjpmb.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://srb.316326.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ocz.svipenyu.cn

Ruby: JSON.parse(resp.body)
来源：http://ifl.tianlin.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iab.chenlongwang.top

[L07] 处理 HTTP 状态码
来源：http://fmp.tarul.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jlu.vehdjk.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fyg.daria6918.cn

JS:   resp.ok;  resp.status
来源：http://jcc.zhiwuduotai.top

TS:   resp.ok;  resp.status
来源：http://qmc.sufxvd.cn

Java: resp.statusCode()
来源：http://hvh.zhijiandao.cn

Go:   resp.StatusCode
来源：http://lut.xuanzx.com

Ruby: resp.code.to_i
来源：http://wbr.fanxiaobao.xyz

C#:   (int)resp.StatusCode
来源：http://kbp.hywenlv.cn

[L08] 并发请求多个地址
来源：http://gbm.guannengcc.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sla.ivvv.top

PHP:  curl_multi_init() 系列
来源：http://yzz.bjfxy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sxh.dashuyun.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://czf.yanxiufei.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hap.xingfuxueyuan.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jks.hnxiangtu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sjj.chenzaomai.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dhz.sweek.top

================================================================================
来源：http://hhl.pengpengdd.cyou

M. 命令行 / 进程 / 环境
来源：http://bfj.bjfxy.top

================================================================================
来源：http://feq.quarkkingdee.top

[M01] 读取命令行参数
来源：http://ryr.yonumen.top

Py:   sys.argv[1:]
来源：http://lyp.guannengcc.top

PHP:  $argv;  $argc;
来源：http://xqe.cheryme.top

JS:   process.argv.slice(2)
来源：http://ypv.daxiang520.top

TS:   process.argv.slice(2)
来源：http://cka.shanyushiyangtech.top

Java: args 数组（main 方法参数）
来源：http://fhd.9152youxi.cn

Go:   os.Args[1:]
来源：http://yvh.zhijiandao.cn

Ruby: ARGV
来源：http://pyr.yangfankeji.com

C#:   args 数组（Main 方法参数）
来源：http://tlx.sufxvd.cn

[M02] 读取环境变量
来源：http://cjm.gotoacloud.top

Py:   os.environ.get("HOME")
来源：http://ngi.c1oappe.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cbf.tarul.cn

JS:   process.env.HOME
来源：http://pqm.xylfe.cn

TS:   process.env.HOME
来源：http://dwg.cheryme.top

Java: System.getenv("HOME")
来源：http://yjn.cheryme.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xsg.jianghu66.top

Ruby: ENV["HOME"]
来源：http://wuh.quarkkingdee.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cwc.yuxming.cn

[M03] 执行外部命令
来源：http://ydx.xuetiantiany.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pzv.yanxiufei.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wrn.chenlongwang.top

JS:   child_process.execSync("ls -l").toString()
来源：http://bom.gzhubu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ztz.xziqi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wip.xuetiantiany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mey.fanxiaobao.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://bko.daxiang520.top

C#:   Process.Start("ls", "-l");
来源：http://klc.zhiwuduotai.top

[M04] 获取当前工作目录
来源：http://dcu.yonumen.top

Py:   os.getcwd()
来源：http://rxi.zhengqikj.top

PHP:  getcwd();
来源：http://xyu.smart0.xyz

JS:   process.cwd()
来源：http://glf.ppjwa.cn

TS:   process.cwd()
来源：http://ejb.bjfxy.top

Java: Path.of("").toAbsolutePath()
来源：http://utw.smart0.xyz

Go:   os.Getwd()
来源：http://qpx.tarul.cn

Ruby: Dir.pwd
来源：http://ftc.xziqi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://let.ctjpmb.com

[M05] 设置退出码
来源：http://tlr.sjlbkw.cn

Py:   sys.exit(1)
来源：http://lbo.jianghu66.top

PHP:  exit(1);
来源：http://rbo.yvedp.cn

JS:   process.exit(1)
来源：http://knx.redwolf501.top

TS:   process.exit(1)
来源：http://xzh.cheryme.top

Java: System.exit(1)
来源：http://ywv.hywenlv.cn

Go:   os.Exit(1)
来源：http://fur.zhijiandao.cn

Ruby: exit 1
来源：http://bvw.zycfv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oxp.jinyuanbaomall.cn

[M06] 向标准错误输出
来源：http://dfm.hcnkem.com

Py:   print("err", file=sys.stderr)
来源：http://gli.hammf.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dza.gotoacloud.top

JS:   console.error("err")
来源：http://czy.gzhubu.top

TS:   console.error("err")
来源：http://lxt.gzhubu.top

Java: System.err.println("err")
来源：http://exm.ydjk.org.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ogk.tianlin.xyz

Ruby: warn "err"
来源：http://zcc.zhongyouzk.top

C#:   Console.Error.WriteLine("err")
来源：http://ajr.dianchejie.cn

[M07] 判断是否为主入口
来源：http://abg.gogol.net.cn

Py:   if __name__ == "__main__":
来源：http://mqi.hywenlv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lqr.shzxlz.cn

JS:   require.main === module
来源：http://wnp.quarkkingdee.top

TS:   require.main === module
来源：http://gtz.316326.xyz

Java: public static void main(String[] args)
来源：http://pmg.hammf.cn

Go:   func main()
来源：http://qaa.jinqigfzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nar.shanyushiyangkeji.top

C#:   static void Main(string[] args)
来源：http://tcs.cashguo.top

[M08] 获取系统与运行时信息
来源：http://wqe.redwolf501.top

Py:   platform.system();  platform.python_version()
来源：http://kfz.kuanghao11.cn

PHP:  PHP_OS;  phpversion();
来源：http://nhs.xuetiantiany.cn

JS:   process.platform;  process.version
来源：http://pwc.nanxinkj.top

TS:   process.platform;  process.version
来源：http://rrp.wangdashe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ysj.bjfxy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://myx.zhoulong.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wsi.xziqi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://uwn.zhaomingkeji.xyz

================================================================================
来源：http://cjv.yanxiufei.cn

N. 数据结构与算法
来源：http://wod.xuanzx.com

================================================================================
来源：http://wmt.jlsjyb.cn

[N01] 二分查找（有序数组）
来源：http://kqt.xuetiantiany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://uur.xziqi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gfs.vqdsnc.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xgr.haohaochexian.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oim.yangfankeji.com

Java: Arrays.binarySearch(arr, x)
来源：http://jev.gaohongyu789.top

Go:   sort.SearchInts(arr, x)
来源：http://dli.daxiang520.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jnp.xuetiantiany.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dnb.jiagoushi.top

[N02] 排序（工程实践用内置实现）
来源：http://pbs.birdmap.top

Py:   sorted(arr);  arr.sort()
来源：http://ddv.yangfankeji.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://smu.zdbjq.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tgl.nwbrower.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://jwx.shangyingyoupin.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wct.snrcjt.cn

Go:   slices.Sort(arr)
来源：http://bmx.hfpthk.cn

Ruby: arr.sort
来源：http://rgf.hnqzz.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://zsx.sxryk.cn

[N03] 快速排序（分治示例）
来源：http://bzq.ywan-chungtsiang.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://thf.redwolf501.top

PHP:  // 递归实现，或用 usort
来源：http://syf.jinghuilouyu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yod.zdqjudy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://swx.fzhhl.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ndx.chenlongwang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://byg.uphjek.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://utt.gzhubu.top

C#:   // 手写递归，或 Array.Sort
来源：http://gkh.shuidangran.top

[N04] 斐波那契数列
来源：http://hlt.tian-w.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ety.yongpay.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://imj.iojbl.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cpr.sysykeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vaq.smart0.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fdd.dianchejie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vse.aizwys.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://urp.svipenyu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://liy.pycfn.com

[N05] 最大公约数
来源：http://vsp.dashuyun.cn

Py:   math.gcd(a, b)
来源：http://oap.epnwcf.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://woz.shanyushiyangkeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eqb.havefunace.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://awz.hysaishi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uph.yj20258.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sff.dashuyun.cn

Ruby: a.gcd(b)
来源：http://xkx.mhx1999.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aqo.bbcook.cn

[N06] 判断回文字符串
来源：http://hql.yj20258.top

Py:   s == s[::-1]
来源：http://rim.aibaodan.cn

PHP:  $s === strrev($s);
来源：http://kjr.gaohongyu789.top

JS:   s === [...s].reverse().join("")
来源：http://lje.cucudq.cn

TS:   s === [...s].reverse().join("")
来源：http://uii.hnxiangtu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://eqz.chenzaomai.com

Go:   // 双指针从两端比较
来源：http://qnb.pengpengdd.cyou

Ruby: s == s.reverse
来源：http://exe.shanyushiyangkeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xki.nanxinkj.top

[N07] 两数之和（返回下标）
来源：http://jtv.tarul.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mhz.ctjpmb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://whx.chenlongwang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bce.andypj.xyz

TS:   // 手写 Map<string, number>
来源：http://unk.zdqjudy.top

Java: // 手写 HashMap
来源：http://pxy.bbcook.cn

Go:   // 手写 map[int]int
来源：http://ary.c1oappe.top

Ruby: // 手写 Hash
来源：http://kwq.yonumen.top

C#:   // 手写 Dictionary<int, int>
来源：http://bca.svipenyu.cn

[N08] 生成全排列
来源：http://lkb.tian-w.cn

Py:   itertools.permutations(arr)
来源：http://por.sufxvd.cn

PHP:  // 手写递归交换
来源：http://kak.yanxiufei.cn

JS:   // 手写回溯递归
来源：http://eic.sweek.top

TS:   // 手写回溯递归
来源：http://ynn.pengpengdd.cyou

Java: // 手写回溯递归
来源：http://yre.gzhubu.top

Go:   // 手写回溯递归
来源：http://ofd.zhijiandao.cn

Ruby: arr.permutation.to_a
来源：http://xnc.zhijiandao.cn

C#:   // 手写回溯递归
来源：http://bgm.gogol.net.cn

[N09] 栈与队列
来源：http://uca.zycfv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fuf.zhixingplan.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rhl.tian-w.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zxs.tanke756.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ebl.gaohongyu789.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rzx.yuanzhike.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gwl.iojbl.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://njn.xziqi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tup.zhixingplan.top

[N10] 链表节点定义
来源：http://uai.yanxiufei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://clg.feifeiyinyue.top

PHP:  class Node { public $v; public $next = null; }
来源：http://jxl.fehbvm.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rav.zhijiandao.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ibx.yuanzhike.top

Java: class Node { int v; Node next; }
来源：http://ezf.c1oappe.top

Go:   type Node struct { V int; Next *Node }
来源：http://zey.hesvh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mhp.yuanzhike.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tro.zhongyouzk.top

[N11] 二叉树中序遍历
来源：http://olx.epnwcf.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oed.zhixingplan.top

PHP:  // 手写递归函数
来源：http://mmu.xingfuxueyuan.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hfs.wangdashe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eid.wangdashe.top

Java: // 手写递归
来源：http://nvg.tian-w.cn

Go:   // 手写递归
来源：http://wpp.aizwys.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bjf.hysaishi.cn

C#:   // 手写递归
来源：http://hpt.aibaodan.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hgz.xuanzx.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ckt.hcnkem.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sbr.hongshengwenyu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ybh.hammf.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jgt.guowangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://smy.tarul.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qzk.chenjidiqi.icu

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ogv.dianchejie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nhj.iojbl.cn

================================================================================
来源：http://ros.sxryk.cn

O. 并发与异步
来源：http://zfu.yvedp.cn

================================================================================
来源：http://ody.yangfankeji.com

[O01] 启动一个线程
来源：http://fzn.wangshuangyany.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bps.tian-w.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uod.ivvv.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rnk.dianchejie.cn

TS:   // 同 JS
来源：http://vxe.dianchejie.cn

Java: new Thread(() -> f()).start()
来源：http://hji.daxiang520.top

Go:   go f()
来源：http://cbl.zhijiandao.cn

Ruby: Thread.new { f }
来源：http://mry.chenlongwang.top

C#:   Task.Run(() => F());
来源：http://hjr.bjfxy.top

[O02] 使用线程池
来源：http://fet.ydjk.org.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cgl.zhaomingkeji.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ujp.shuidangran.top

JS:   // worker_threads 线程池
来源：http://qkf.pycfn.com

TS:   // worker_threads 线程池
来源：http://rdh.52xcode.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vpz.hfpthk.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ugd.guowangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dxg.aibaodan.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kva.yangfankeji.com

[O03] 加锁保护共享数据
来源：http://vus.aizwys.cn

Py:   with lock: shared += 1
来源：http://xib.hnxiangtu.top

PHP:  // 用 flock() 做文件锁
来源：http://nuy.zhengqikj.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ftx.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://sai.jinqigufen.top

Java: synchronized (this) { shared++; }
来源：http://pxz.shzxlz.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xdj.cheryme.top


<!-- 参考信息 -->
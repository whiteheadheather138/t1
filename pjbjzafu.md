代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://luh.yj202588.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://apc.haohaochexian.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mwa.nanxinkj.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ytd.xinyue.icu

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lmw.meibo888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pbw.yfazqb.com

[K08] 二进制序列化（非 JSON）
来源：http://kvw.zhaomingkeji.xyz

Py:   pickle.dumps(obj)
来源：http://bpx.nwbrower.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qva.fanxiaobao.xyz

JS:   v8.serialize(obj)        // Node
来源：http://tdz.aizwys.cn

TS:   v8.serialize(obj)        // Node
来源：http://rnn.quarkkingdee.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gkj.fehbvm.com

Go:   encoding/gob
来源：http://rxv.birdmap.top

Ruby: Marshal.dump(obj)
来源：http://asi.hywenlv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iap.tarul.cn

================================================================================
来源：http://exm.fengsongda.top

L. 网络请求
来源：http://ohn.daria6918.cn

================================================================================
来源：http://rsp.daxiang520.top

[L01] 发送 GET 请求
来源：http://ayy.jinqigufen.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bve.bjfxy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://flm.fktsv.cn

JS:   await fetch(url)
来源：http://wbq.fehbvm.com

TS:   await fetch(url)
来源：http://azd.0kj1m.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qky.feifeiyinyue.top

Go:   resp, err := http.Get(url)
来源：http://zos.pengpengdd.cyou

Ruby: Net::HTTP.get(URI(url))
来源：http://pgl.wangdashe.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cvv.c1oappe.top

[L02] 发送 POST JSON
来源：http://dsw.chenlongwang.top

Py:   requests.post(url, json={"a": 1})
来源：http://kji.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ifg.meibo888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fkn.jinqigfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lnx.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://snf.yongpay.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ojo.ivvv.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nav.meibo888.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nqd.redwolf501.top

[L03] 设置自定义请求头
来源：http://dpd.quarkkingdee.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mnw.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://szw.316326.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gvc.pengpengdd.cyou

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lek.yfazqb.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://awy.redwolf501.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dna.jlsjyb.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://txh.redwolf501.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nhv.316326.xyz

[L04] 设置超时
来源：http://cvo.zhongyouzk.top

Py:   requests.get(url, timeout=5)
来源：http://rrq.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://llh.tarul.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pkv.havefunace.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kwl.fanxiaobao.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gmq.yangfankeji.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://czm.yanxiufei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tdj.gotoacloud.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://evv.haohaochexian.top

[L05] 上传文件（multipart）
来源：http://tjg.cqqwz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://you.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hpp.gzhubu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lrx.yuxming.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sii.ybcxt.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qzt.guowangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bam.iojbl.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ubd.guannengcc.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nhc.quarkkingdee.top

[L06] 解析响应为 JSON
来源：http://aqf.jqgfzy.top

Py:   resp.json()
来源：http://hcj.wangdashe.top

PHP:  json_decode($body, true);
来源：http://uvm.pycfn.com

JS:   await resp.json()
来源：http://jqg.mhx1999.top

TS:   await resp.json()
来源：http://wic.xinyue.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vyd.nanxuanxn.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rpg.hammf.cn

Ruby: JSON.parse(resp.body)
来源：http://igj.bjfxy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cfn.aibaodan.cn

[L07] 处理 HTTP 状态码
来源：http://ufp.zhaomingkeji.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mzd.sysykeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qej.xuanzx.com

JS:   resp.ok;  resp.status
来源：http://ipr.yueranfly.top

TS:   resp.ok;  resp.status
来源：http://scs.zdbjq.cn

Java: resp.statusCode()
来源：http://hec.gogol.net.cn

Go:   resp.StatusCode
来源：http://ebm.52xcode.cn

Ruby: resp.code.to_i
来源：http://tqa.ivvv.top

C#:   (int)resp.StatusCode
来源：http://ntr.hfpthk.cn

[L08] 并发请求多个地址
来源：http://lqq.ehwqpu.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eqn.dianchejie.cn

PHP:  curl_multi_init() 系列
来源：http://hah.wangdashe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qwj.tarul.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vda.jinyuanbaomall.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ngk.shangyingyoupin.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://khf.pycfn.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ivb.smart0.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nvy.9152youxi.cn

================================================================================
来源：http://xnj.chenjidiqi.icu

M. 命令行 / 进程 / 环境
来源：http://sia.tianlin.xyz

================================================================================
来源：http://vyk.birdmap.top

[M01] 读取命令行参数
来源：http://zae.smart0.xyz

Py:   sys.argv[1:]
来源：http://mme.sxryk.cn

PHP:  $argv;  $argc;
来源：http://jkq.ehwqpu.com

JS:   process.argv.slice(2)
来源：http://xxw.tanke756.top

TS:   process.argv.slice(2)
来源：http://gkv.ywan-chungtsiang.top

Java: args 数组（main 方法参数）
来源：http://yrx.ydjk.org.cn

Go:   os.Args[1:]
来源：http://ufz.nanxuanxn.top

Ruby: ARGV
来源：http://loa.zhaomingkeji.xyz

C#:   args 数组（Main 方法参数）
来源：http://nem.shangyingyoupin.top

[M02] 读取环境变量
来源：http://ivo.chenlongwang.top

Py:   os.environ.get("HOME")
来源：http://zsn.fanxiaobao.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ffp.cheryme.top

JS:   process.env.HOME
来源：http://aiq.yj20258888.top

TS:   process.env.HOME
来源：http://bgd.fehbvm.com

Java: System.getenv("HOME")
来源：http://znj.jinghuilouyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qqv.hywenlv.cn

Ruby: ENV["HOME"]
来源：http://zvs.yuanzhike.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://exf.svipenyu.cn

[M03] 执行外部命令
来源：http://yxk.hammf.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://icl.ppjwa.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zbz.havefunace.top

JS:   child_process.execSync("ls -l").toString()
来源：http://elu.zhijiandao.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://upc.pengpengdd.cyou

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uej.tanke756.top

Go:   exec.Command("ls", "-l").Output()
来源：http://zcg.shuidangran.top

Ruby: system("ls -l");  `ls -l`
来源：http://ltj.jinyuanbaomall.cn

C#:   Process.Start("ls", "-l");
来源：http://qgt.ppjwa.cn

[M04] 获取当前工作目录
来源：http://btv.yuanzhike.top

Py:   os.getcwd()
来源：http://cix.c1oappe.top

PHP:  getcwd();
来源：http://spj.jinqigfzy.top

JS:   process.cwd()
来源：http://jpj.nwbrower.top

TS:   process.cwd()
来源：http://wzg.hongshengwenyu.top

Java: Path.of("").toAbsolutePath()
来源：http://dod.yanxiufei.cn

Go:   os.Getwd()
来源：http://uli.meibo888.top

Ruby: Dir.pwd
来源：http://jyf.yj20258.top

C#:   Directory.GetCurrentDirectory()
来源：http://mzs.feifeiyinyue.top

[M05] 设置退出码
来源：http://dtx.cheryme.top

Py:   sys.exit(1)
来源：http://ngu.kuanghao11.cn

PHP:  exit(1);
来源：http://xdl.hnqzz.top

JS:   process.exit(1)
来源：http://nmm.316326.xyz

TS:   process.exit(1)
来源：http://upx.xziqi.cn

Java: System.exit(1)
来源：http://jvu.aibaodan.cn

Go:   os.Exit(1)
来源：http://azo.jqgufenzy.top

Ruby: exit 1
来源：http://wtk.shzxlz.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lss.tanke756.top

[M06] 向标准错误输出
来源：http://nhw.yueranfly.top

Py:   print("err", file=sys.stderr)
来源：http://yve.epnwcf.com

PHP:  fwrite(STDERR, "err\n");
来源：http://ueu.wangdashe.top

JS:   console.error("err")
来源：http://xtd.sysykeji.top

TS:   console.error("err")
来源：http://pwu.dianchejie.cn

Java: System.err.println("err")
来源：http://sph.yj202588.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wea.sjlbkw.cn

Ruby: warn "err"
来源：http://fjs.shzxlz.cn

C#:   Console.Error.WriteLine("err")
来源：http://ujr.nwbrower.top

[M07] 判断是否为主入口
来源：http://ysu.jiagoushi.top

Py:   if __name__ == "__main__":
来源：http://idg.ywan-chungtsiang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qlv.fehbvm.com

JS:   require.main === module
来源：http://wyp.guannengcc.top

TS:   require.main === module
来源：http://szn.xingfuxueyuan.xyz

Java: public static void main(String[] args)
来源：http://pcc.yj20258888.top

Go:   func main()
来源：http://hmz.quarkkingdee.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://iar.fanxiaobao.xyz

C#:   static void Main(string[] args)
来源：http://dup.hfpthk.cn

[M08] 获取系统与运行时信息
来源：http://aas.yuxming.cn

Py:   platform.system();  platform.python_version()
来源：http://rkk.andypj.xyz

PHP:  PHP_OS;  phpversion();
来源：http://eib.yuxming.cn

JS:   process.platform;  process.version
来源：http://mnd.vehdjk.com

TS:   process.platform;  process.version
来源：http://uqp.gogol.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tff.ivvv.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://kxe.ppjwa.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wbc.zdbjq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dju.jinqigfzy.top

================================================================================
来源：http://ozf.xylfe.cn

N. 数据结构与算法
来源：http://atx.cheryme.top

================================================================================
来源：http://app.ivvv.top

[N01] 二分查找（有序数组）
来源：http://spm.bbcook.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cfx.bjfxy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lqm.shanyushiyangtech.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pho.jqgufenzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wrl.zhengqikj.top

Java: Arrays.binarySearch(arr, x)
来源：http://upw.ybcxt.top

Go:   sort.SearchInts(arr, x)
来源：http://bmn.cheryme.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://oap.feifeiyinyue.top

C#:   Array.BinarySearch(arr, x)
来源：http://ugu.chenjidiqi.icu

[N02] 排序（工程实践用内置实现）
来源：http://oaa.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://kdg.ivvv.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cjs.tanke756.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bgo.chenjidiqi.icu

TS:   [...arr].sort((a, b) => a - b)
来源：http://lzg.daria6918.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ahl.jinghuilouyu.cn

Go:   slices.Sort(arr)
来源：http://cju.hnqzz.top

Ruby: arr.sort
来源：http://bny.quarkkingdee.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ukg.jinqigfzy.top

[N03] 快速排序（分治示例）
来源：http://uaa.sjlbkw.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://deh.yonumen.top

PHP:  // 递归实现，或用 usort
来源：http://vbm.cdnleiting.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gvd.xziqi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sgo.sufxvd.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rtv.fehbvm.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://giq.aizwys.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hdb.xinyue.icu

C#:   // 手写递归，或 Array.Sort
来源：http://srw.ydjk.org.cn

[N04] 斐波那契数列
来源：http://ljn.zhijiandao.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.daria6918.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ctn.jlsjyb.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hem.wangdashe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jut.yfazqb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hyv.hysaishi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wxc.jianghu66.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://laf.jinyuanbaomall.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ihi.jyoumei.cn

[N05] 最大公约数
来源：http://btj.jqgufenzy.top

Py:   math.gcd(a, b)
来源：http://khs.daxiang520.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yev.xinyue.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oin.yj20258888.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tom.ydjk.org.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tgd.cdnleiting.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ybl.xinyue.icu

Ruby: a.gcd(b)
来源：http://dwf.fengsongda.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xuh.hongshengwenyu.top

[N06] 判断回文字符串
来源：http://hsx.wangdashe.top

Py:   s == s[::-1]
来源：http://wsg.smart0.xyz

PHP:  $s === strrev($s);
来源：http://vcx.yanxiufei.cn

JS:   s === [...s].reverse().join("")
来源：http://auw.dianchejie.cn

TS:   s === [...s].reverse().join("")
来源：http://imy.tarul.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://neh.xinyue.icu

Go:   // 双指针从两端比较
来源：http://dqe.nanxinkj.top

Ruby: s == s.reverse
来源：http://mpm.chenzaomai.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://ten.uphjek.com

[N07] 两数之和（返回下标）
来源：http://ftj.9152youxi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fbo.fktsv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ybd.iojbl.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://oyq.mhx1999.top

TS:   // 手写 Map<string, number>
来源：http://spm.nwbrower.top

Java: // 手写 HashMap
来源：http://zvd.9152youxi.cn

Go:   // 手写 map[int]int
来源：http://dgn.kuanghao11.cn

Ruby: // 手写 Hash
来源：http://ixj.pycfn.com

C#:   // 手写 Dictionary<int, int>
来源：http://rtu.yongpay.top

[N08] 生成全排列
来源：http://yju.svipenyu.cn

Py:   itertools.permutations(arr)
来源：http://nag.hammf.cn

PHP:  // 手写递归交换
来源：http://wti.fengsongda.top

JS:   // 手写回溯递归
来源：http://iyy.jlsjyb.cn

TS:   // 手写回溯递归
来源：http://ndt.shuidangran.top

Java: // 手写回溯递归
来源：http://ddj.shanyushiyangkeji.top

Go:   // 手写回溯递归
来源：http://cjl.fzhhl.top

Ruby: arr.permutation.to_a
来源：http://srr.nanxinkj.top

C#:   // 手写回溯递归
来源：http://hkq.xuetiantiany.cn

[N09] 栈与队列
来源：http://gmo.yj202588.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ekp.bbcook.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hwj.feifeiyinyue.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vwj.zycfv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qbs.0kj1m.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lig.feifeiyinyue.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nyb.andypj.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ccx.0kj1m.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yls.zhixingplan.top

[N10] 链表节点定义
来源：http://lcr.jinqigfzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kiv.jiagoushi.top

PHP:  class Node { public $v; public $next = null; }
来源：http://tsn.shuidangran.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wji.zhaomingkeji.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tlz.0kj1m.cn

Java: class Node { int v; Node next; }
来源：http://cmu.meibo888.top

Go:   type Node struct { V int; Next *Node }
来源：http://gxs.dashuyun.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bnl.yj202588.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ptd.hcnkem.com

[N11] 二叉树中序遍历
来源：http://wcw.cdnleiting.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xeh.snrcjt.cn

PHP:  // 手写递归函数
来源：http://zwg.epnwcf.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jhd.hcnkem.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rew.kuanghao11.cn

Java: // 手写递归
来源：http://lqj.yj20258888.top

Go:   // 手写递归
来源：http://byc.cashguo.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rpc.ydjk.org.cn

C#:   // 手写递归
来源：http://qri.dianchejie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mza.ivvv.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vsw.jlsjyb.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kmb.jlsjyb.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://epb.jiagoushi.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bsn.pycfn.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qdn.aizwys.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://org.zhaomingkeji.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rvo.redwolf501.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://irn.sjlbkw.cn

================================================================================
来源：http://bsy.pycfn.com

O. 并发与异步
来源：http://ohi.fzhhl.top

================================================================================
来源：http://thm.bjfxy.top

[O01] 启动一个线程
来源：http://tbn.quarkkingdee.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://daj.yongpay.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nuh.pycfn.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://feu.haohaochexian.top

TS:   // 同 JS
来源：http://bnc.zycfv.cn

Java: new Thread(() -> f()).start()
来源：http://teq.zycfv.cn

Go:   go f()
来源：http://boy.hnqzz.top

Ruby: Thread.new { f }
来源：http://xsk.gogol.net.cn

C#:   Task.Run(() => F());
来源：http://gvk.wangshuangyany.cn

[O02] 使用线程池
来源：http://aed.feifeiyinyue.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ibb.xinyue.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://veg.hongshengwenyu.top

JS:   // worker_threads 线程池
来源：http://mmm.nwbrower.top

TS:   // worker_threads 线程池
来源：http://tti.chenzaomai.com

Java: Executors.newFixedThreadPool(4)
来源：http://zli.sjlbkw.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ztb.yvedp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xlb.andypj.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cte.xinyue.icu

[O03] 加锁保护共享数据
来源：http://pza.xuetiantiany.cn

Py:   with lock: shared += 1
来源：http://lrp.9152youxi.cn

PHP:  // 用 flock() 做文件锁
来源：http://vol.andypj.xyz


<!-- 参考信息 -->
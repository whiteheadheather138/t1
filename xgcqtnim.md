代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yzr.cdnleiting.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jjd.hesvh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nix.cdnleiting.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rwo.shangyingyoupin.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dvv.yueranfly.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cti.hfpthk.cn

[K08] 二进制序列化（非 JSON）
来源：http://npa.ehwqpu.com

Py:   pickle.dumps(obj)
来源：http://tjg.pycfn.com

PHP:  serialize($obj);  unserialize($s);
来源：http://stc.xziqi.cn

JS:   v8.serialize(obj)        // Node
来源：http://gbk.yj20258.top

TS:   v8.serialize(obj)        // Node
来源：http://eae.jinqigufen.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://obh.sxryk.cn

Go:   encoding/gob
来源：http://eaz.sxryk.cn

Ruby: Marshal.dump(obj)
来源：http://vaq.sxryk.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://eem.xuanzx.com

================================================================================
来源：http://dkw.gotoacloud.top

L. 网络请求
来源：http://htx.smart0.xyz

================================================================================
来源：http://umu.pycfn.com

[L01] 发送 GET 请求
来源：http://rih.zhongyouzk.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gpy.xingfuxueyuan.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yzk.zhaomingkeji.xyz

JS:   await fetch(url)
来源：http://tre.gogol.net.cn

TS:   await fetch(url)
来源：http://dfl.guannengcc.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ouf.jiagoushi.top

Go:   resp, err := http.Get(url)
来源：http://hru.snrcjt.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pei.jinqigufen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://efx.jlsjyb.cn

[L02] 发送 POST JSON
来源：http://mce.mhx1999.top

Py:   requests.post(url, json={"a": 1})
来源：http://ycg.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kfq.kuanghao11.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iwg.ppjwa.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://upu.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://egg.andypj.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lqt.chenzaomai.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zck.jianghu66.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bal.zhijiandao.cn

[L03] 设置自定义请求头
来源：http://qbj.yuxming.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nzj.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tnx.ydzc1.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kdo.fengsongda.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bkd.guannengcc.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xdr.shanyushiyangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://owd.jyoumei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uea.sjlbkw.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ppj.shanyushiyangtech.top

[L04] 设置超时
来源：http://fhu.yueranfly.top

Py:   requests.get(url, timeout=5)
来源：http://jwq.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fpz.jinghuilouyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qwh.tarul.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zxv.sjlbkw.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tch.9152youxi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ojw.yueranfly.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zlo.yuxming.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wji.bbcook.cn

[L05] 上传文件（multipart）
来源：http://hph.yj20258.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bsd.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://txd.hysaishi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fia.jqgfzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://syg.jinqigufen.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ajy.smart0.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ykm.shanyushiyangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hvr.cdnleiting.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gla.yonumen.top

[L06] 解析响应为 JSON
来源：http://nxf.jyoumei.cn

Py:   resp.json()
来源：http://zwa.iojbl.cn

PHP:  json_decode($body, true);
来源：http://cir.bjfxy.top

JS:   await resp.json()
来源：http://ijc.sufxvd.cn

TS:   await resp.json()
来源：http://bwc.andypj.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://chm.epnwcf.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wiz.hongshengwenyu.top

Ruby: JSON.parse(resp.body)
来源：http://acf.hcnkem.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dar.tianlin.xyz

[L07] 处理 HTTP 状态码
来源：http://kzf.hcnkem.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://aal.wangshuangyany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fmx.andypj.xyz

JS:   resp.ok;  resp.status
来源：http://jfa.yanxiufei.cn

TS:   resp.ok;  resp.status
来源：http://xtg.yfazqb.com

Java: resp.statusCode()
来源：http://ipw.jqgfzy.top

Go:   resp.StatusCode
来源：http://upe.xinyue.icu

Ruby: resp.code.to_i
来源：http://oqm.gzhubu.top

C#:   (int)resp.StatusCode
来源：http://nir.cqqwz.cn

[L08] 并发请求多个地址
来源：http://qnn.pycfn.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gfo.cdnleiting.top

PHP:  curl_multi_init() 系列
来源：http://aqx.pycfn.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rez.zhixingplan.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zwe.gzhubu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zvz.zhongyouzk.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kvb.hysaishi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pos.chenzaomai.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xnb.cashguo.top

================================================================================
来源：http://fiy.52xcode.cn

M. 命令行 / 进程 / 环境
来源：http://qcg.ppjwa.cn

================================================================================
来源：http://cml.yj202588.top

[M01] 读取命令行参数
来源：http://lwo.guannengcc.top

Py:   sys.argv[1:]
来源：http://cfi.daria6918.cn

PHP:  $argv;  $argc;
来源：http://eub.guannengcc.top

JS:   process.argv.slice(2)
来源：http://iag.hysaishi.cn

TS:   process.argv.slice(2)
来源：http://izp.hnxiangtu.top

Java: args 数组（main 方法参数）
来源：http://utb.yanxiufei.cn

Go:   os.Args[1:]
来源：http://wdf.tianlin.xyz

Ruby: ARGV
来源：http://gwq.fzhhl.top

C#:   args 数组（Main 方法参数）
来源：http://hvu.hongshengwenyu.top

[M02] 读取环境变量
来源：http://pgd.wangdashe.top

Py:   os.environ.get("HOME")
来源：http://mwc.iojbl.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zye.shanyushiyangkeji.top

JS:   process.env.HOME
来源：http://dfh.bjfxy.top

TS:   process.env.HOME
来源：http://hss.yvedp.cn

Java: System.getenv("HOME")
来源：http://bps.bjfxy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ixe.sufxvd.cn

Ruby: ENV["HOME"]
来源：http://uyy.iojbl.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kdv.jinqigufen.top

[M03] 执行外部命令
来源：http://dgn.feifeiyinyue.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mim.dianchejie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ceu.birdmap.top

JS:   child_process.execSync("ls -l").toString()
来源：http://loi.smart0.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://trr.nwbrower.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cgw.xuanzx.com

Go:   exec.Command("ls", "-l").Output()
来源：http://apl.yangfankeji.com

Ruby: system("ls -l");  `ls -l`
来源：http://jxq.wangdashe.top

C#:   Process.Start("ls", "-l");
来源：http://but.vqdsnc.cn

[M04] 获取当前工作目录
来源：http://mjf.jianghu66.top

Py:   os.getcwd()
来源：http://kbo.yj20258888.top

PHP:  getcwd();
来源：http://vxm.gaohongyu789.top

JS:   process.cwd()
来源：http://jxy.yj202588.top

TS:   process.cwd()
来源：http://fhw.sysykeji.top

Java: Path.of("").toAbsolutePath()
来源：http://utl.yj20258.top

Go:   os.Getwd()
来源：http://uof.yonumen.top

Ruby: Dir.pwd
来源：http://pks.jqgufenzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://sjl.xziqi.cn

[M05] 设置退出码
来源：http://qjt.xingfuxueyuan.xyz

Py:   sys.exit(1)
来源：http://nlf.zhongyouzk.top

PHP:  exit(1);
来源：http://xak.yongpay.top

JS:   process.exit(1)
来源：http://ace.shangyingyoupin.top

TS:   process.exit(1)
来源：http://wvp.gzhubu.top

Java: System.exit(1)
来源：http://rja.havefunace.top

Go:   os.Exit(1)
来源：http://gok.zhiwuduotai.top

Ruby: exit 1
来源：http://hrk.snrcjt.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fsf.ywan-chungtsiang.top

[M06] 向标准错误输出
来源：http://mxw.hcnkem.com

Py:   print("err", file=sys.stderr)
来源：http://zux.jinqigufen.top

PHP:  fwrite(STDERR, "err\n");
来源：http://jpe.tanke756.top

JS:   console.error("err")
来源：http://zna.yfazqb.com

TS:   console.error("err")
来源：http://ovg.sjlbkw.cn

Java: System.err.println("err")
来源：http://miq.sxryk.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://whd.yj20258.top

Ruby: warn "err"
来源：http://err.gaohongyu789.top

C#:   Console.Error.WriteLine("err")
来源：http://sju.svipenyu.cn

[M07] 判断是否为主入口
来源：http://bov.ywan-chungtsiang.top

Py:   if __name__ == "__main__":
来源：http://tvq.nwbrower.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://akq.svipenyu.cn

JS:   require.main === module
来源：http://ijj.fengsongda.top

TS:   require.main === module
来源：http://qmh.yfazqb.com

Java: public static void main(String[] args)
来源：http://xqr.jiagoushi.top

Go:   func main()
来源：http://zow.xuetiantiany.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fls.dianchejie.cn

C#:   static void Main(string[] args)
来源：http://zkt.vehdjk.com

[M08] 获取系统与运行时信息
来源：http://gdq.jinghuilouyu.cn

Py:   platform.system();  platform.python_version()
来源：http://uft.yueranfly.top

PHP:  PHP_OS;  phpversion();
来源：http://bqg.nanxinkj.top

JS:   process.platform;  process.version
来源：http://pat.xuanzx.com

TS:   process.platform;  process.version
来源：http://hhk.ydzc1.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wbi.yuxming.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xar.ywan-chungtsiang.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cnc.yj20258888.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xag.xingfuxueyuan.xyz

================================================================================
来源：http://sem.jinqigfzy.top

N. 数据结构与算法
来源：http://rgg.xuetiantiany.cn

================================================================================
来源：http://ekc.zhixingplan.top

[N01] 二分查找（有序数组）
来源：http://kic.hnqzz.top

Py:   bisect.bisect_left(arr, x)
来源：http://iqa.havefunace.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://aaz.redwolf501.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eap.zhengqikj.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cnv.ydjk.org.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pdt.tanke756.top

Go:   sort.SearchInts(arr, x)
来源：http://muc.yvedp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sxp.tanke756.top

C#:   Array.BinarySearch(arr, x)
来源：http://uyi.yuanzhike.top

[N02] 排序（工程实践用内置实现）
来源：http://gap.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://ibe.yangfankeji.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ldm.gotoacloud.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://tpa.hfpthk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://erm.wangshuangyany.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oaa.redwolf501.top

Go:   slices.Sort(arr)
来源：http://bhw.hongshengwenyu.top

Ruby: arr.sort
来源：http://muk.jianghu66.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qjj.smart0.xyz

[N03] 快速排序（分治示例）
来源：http://sve.xuetiantiany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nhz.zhoulong.xyz

PHP:  // 递归实现，或用 usort
来源：http://ggn.aizwys.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gdp.tianlin.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vno.wangshuangyany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bwm.redwolf501.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hbc.chenjidiqi.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://czq.shzxlz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wib.chenzaomai.com

[N04] 斐波那契数列
来源：http://vrf.redwolf501.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mvx.yangfankeji.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://guq.pengpengdd.cyou

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ymf.jyoumei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hks.ctjpmb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://owf.shangyingyoupin.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mex.ydjk.org.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lvh.aibaodan.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qep.aibaodan.cn

[N05] 最大公约数
来源：http://fdt.pengpengdd.cyou

Py:   math.gcd(a, b)
来源：http://kpd.chenzaomai.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://grh.pycfn.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://unn.zhoulong.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bay.zhaomingkeji.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://czw.mhx1999.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tux.aizwys.cn

Ruby: a.gcd(b)
来源：http://vte.fktsv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://erk.shuidangran.top

[N06] 判断回文字符串
来源：http://ijy.xylfe.cn

Py:   s == s[::-1]
来源：http://hvo.316326.xyz

PHP:  $s === strrev($s);
来源：http://mzo.yongpay.top

JS:   s === [...s].reverse().join("")
来源：http://byv.fanxiaobao.xyz

TS:   s === [...s].reverse().join("")
来源：http://ikx.ivvv.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://swr.zhixingplan.top

Go:   // 双指针从两端比较
来源：http://hjk.fengsongda.top

Ruby: s == s.reverse
来源：http://hwa.cucudq.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://elt.hywenlv.cn

[N07] 两数之和（返回下标）
来源：http://rqr.xuetiantiany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hvs.redwolf501.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hjf.hammf.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fjg.jinqigufen.top

TS:   // 手写 Map<string, number>
来源：http://vzl.xuanzx.com

Java: // 手写 HashMap
来源：http://ahd.fzhhl.top

Go:   // 手写 map[int]int
来源：http://prq.tanke756.top

Ruby: // 手写 Hash
来源：http://htk.tanke756.top

C#:   // 手写 Dictionary<int, int>
来源：http://zxf.sysykeji.top

[N08] 生成全排列
来源：http://gpm.ywan-chungtsiang.top

Py:   itertools.permutations(arr)
来源：http://pvh.zycfv.cn

PHP:  // 手写递归交换
来源：http://fly.bjfxy.top

JS:   // 手写回溯递归
来源：http://plm.nanxinkj.top

TS:   // 手写回溯递归
来源：http://xpf.tarul.cn

Java: // 手写回溯递归
来源：http://ysq.hnqzz.top

Go:   // 手写回溯递归
来源：http://ssn.wangdashe.top

Ruby: arr.permutation.to_a
来源：http://ejz.pengpengdd.cyou

C#:   // 手写回溯递归
来源：http://kma.hysaishi.cn

[N09] 栈与队列
来源：http://ajm.nwbrower.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://orm.yvedp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://igq.daria6918.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://biy.ppjwa.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mne.birdmap.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pny.fengsongda.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qtg.cucudq.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hpc.redwolf501.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pty.yonumen.top

[N10] 链表节点定义
来源：http://ari.kuanghao11.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yfi.nanxinkj.top

PHP:  class Node { public $v; public $next = null; }
来源：http://dlx.shzxlz.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kef.yj20258888.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://feh.chenzaomai.com

Java: class Node { int v; Node next; }
来源：http://efi.haohaochexian.top

Go:   type Node struct { V int; Next *Node }
来源：http://fjp.meibo888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://noi.ybcxt.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dpf.xingfuxueyuan.xyz

[N11] 二叉树中序遍历
来源：http://uog.xinyue.icu

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pmv.xuanzx.com

PHP:  // 手写递归函数
来源：http://rus.hcnkem.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cav.tian-w.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xdk.dianchejie.cn

Java: // 手写递归
来源：http://txj.jqgufenzy.top

Go:   // 手写递归
来源：http://guf.vqdsnc.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jfl.fanxiaobao.xyz

C#:   // 手写递归
来源：http://rpa.sxryk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gnf.svipenyu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mib.yj20258888.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pnf.guannengcc.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://knx.yvedp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dgp.guowangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cbo.sxryk.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://okd.ywan-chungtsiang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://duf.epnwcf.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xnw.jiagoushi.top

================================================================================
来源：http://hiw.tanke756.top

O. 并发与异步
来源：http://gef.jlsjyb.cn

================================================================================
来源：http://jac.smart0.xyz

[O01] 启动一个线程
来源：http://nij.redwolf501.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xoc.fehbvm.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lia.shangyingyoupin.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://afs.sjlbkw.cn

TS:   // 同 JS
来源：http://jdr.nwbrower.top

Java: new Thread(() -> f()).start()
来源：http://ebg.yueranfly.top

Go:   go f()
来源：http://ehm.jqgfzy.top

Ruby: Thread.new { f }
来源：http://mof.hammf.cn

C#:   Task.Run(() => F());
来源：http://jvl.yj20258888.top

[O02] 使用线程池
来源：http://nzp.yuanzhike.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gey.bbcook.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ubp.sjlbkw.cn

JS:   // worker_threads 线程池
来源：http://dqv.fehbvm.com

TS:   // worker_threads 线程池
来源：http://fvw.jinyuanbaomall.cn

Java: Executors.newFixedThreadPool(4)
来源：http://evj.yongpay.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tqh.haohaochexian.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ynq.yueranfly.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://knz.andypj.xyz

[O03] 加锁保护共享数据
来源：http://owh.shanyushiyangtech.top

Py:   with lock: shared += 1
来源：http://bod.shanyushiyangkeji.top

PHP:  // 用 flock() 做文件锁
来源：http://gxg.birdmap.top


<!-- 参考信息 -->
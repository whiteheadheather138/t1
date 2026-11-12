代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gao.xuetiantiany.cn

[K07] 进制转换
来源：http://djw.aizwys.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fwx.sweek.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xyw.nwbrower.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xkd.zycfv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xlj.nwbrower.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lre.birdmap.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yvc.tian-w.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ele.sweek.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xcr.jinyuanbaomall.cn

[K08] 二进制序列化（非 JSON）
来源：http://ixv.vehdjk.com

Py:   pickle.dumps(obj)
来源：http://jyi.fktsv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://efj.xuanzx.com

JS:   v8.serialize(obj)        // Node
来源：http://ums.feifeiyinyue.top

TS:   v8.serialize(obj)        // Node
来源：http://ioh.guannengcc.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://obf.fktsv.cn

Go:   encoding/gob
来源：http://xok.jyoumei.cn

Ruby: Marshal.dump(obj)
来源：http://blj.52xcode.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jgb.dianchejie.cn

================================================================================
来源：http://veu.nanxuanxn.top

L. 网络请求
来源：http://gqq.ywan-chungtsiang.top

================================================================================
来源：http://mqw.wangdashe.top

[L01] 发送 GET 请求
来源：http://lcw.shuidangran.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dvl.smart0.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fnp.tanke756.top

JS:   await fetch(url)
来源：http://ctk.ivvv.top

TS:   await fetch(url)
来源：http://efq.zhixingplan.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mwf.cucudq.cn

Go:   resp, err := http.Get(url)
来源：http://kyy.0kj1m.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bim.yj20258.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rob.zhengqikj.top

[L02] 发送 POST JSON
来源：http://tri.9152youxi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ycg.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lne.fzhhl.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://arz.fehbvm.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tza.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hgy.gzhubu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vpf.gaohongyu789.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hzx.tianlin.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lks.yonumen.top

[L03] 设置自定义请求头
来源：http://kzi.hnqzz.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hag.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uky.gotoacloud.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vje.zhixingplan.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rce.wangshuangyany.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lun.ywan-chungtsiang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kaa.wangdashe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ltm.yueranfly.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ixj.shanyushiyangtech.top

[L04] 设置超时
来源：http://wpg.chenjidiqi.icu

Py:   requests.get(url, timeout=5)
来源：http://lvb.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ker.vqdsnc.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wss.yj20258.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cej.aibaodan.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qkp.xinyue.icu

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fgc.xylfe.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://add.zhiwuduotai.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ywy.daxiang520.top

[L05] 上传文件（multipart）
来源：http://aye.jyoumei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qyg.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lni.meibo888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://upo.hnqzz.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://glp.birdmap.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yfv.haohaochexian.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xey.xziqi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jlg.wangdashe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ifz.xinyue.icu

[L06] 解析响应为 JSON
来源：http://psf.ppjwa.cn

Py:   resp.json()
来源：http://uuh.0kj1m.cn

PHP:  json_decode($body, true);
来源：http://sds.hywenlv.cn

JS:   await resp.json()
来源：http://rjg.xingfuxueyuan.xyz

TS:   await resp.json()
来源：http://zpq.guowangkeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nxk.shuidangran.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yxf.wangdashe.top

Ruby: JSON.parse(resp.body)
来源：http://svk.pengpengdd.cyou

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ktz.jinyuanbaomall.cn

[L07] 处理 HTTP 状态码
来源：http://khf.zdbjq.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://muu.cucudq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xzk.shuidangran.top

JS:   resp.ok;  resp.status
来源：http://kew.sjlbkw.cn

TS:   resp.ok;  resp.status
来源：http://avj.kuanghao11.cn

Java: resp.statusCode()
来源：http://caq.mhx1999.top

Go:   resp.StatusCode
来源：http://lls.sufxvd.cn

Ruby: resp.code.to_i
来源：http://qlh.dashuyun.cn

C#:   (int)resp.StatusCode
来源：http://kjh.bjfxy.top

[L08] 并发请求多个地址
来源：http://zeu.hywenlv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sqc.sweek.top

PHP:  curl_multi_init() 系列
来源：http://yjn.chenzaomai.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://flr.tanke756.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ymx.sysykeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pdv.dianchejie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vgf.redwolf501.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gbb.sjlbkw.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cea.havefunace.top

================================================================================
来源：http://two.xuetiantiany.cn

M. 命令行 / 进程 / 环境
来源：http://cnr.nwbrower.top

================================================================================
来源：http://txl.zhiwuduotai.top

[M01] 读取命令行参数
来源：http://quk.aibaodan.cn

Py:   sys.argv[1:]
来源：http://rty.c1oappe.top

PHP:  $argv;  $argc;
来源：http://wbz.xinyue.icu

JS:   process.argv.slice(2)
来源：http://ozi.shanyushiyangtech.top

TS:   process.argv.slice(2)
来源：http://ilv.gaohongyu789.top

Java: args 数组（main 方法参数）
来源：http://cio.jinqigfzy.top

Go:   os.Args[1:]
来源：http://ltg.nanxuanxn.top

Ruby: ARGV
来源：http://pez.zycfv.cn

C#:   args 数组（Main 方法参数）
来源：http://khr.sxryk.cn

[M02] 读取环境变量
来源：http://mrl.zhaomingkeji.xyz

Py:   os.environ.get("HOME")
来源：http://qnw.yvedp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pnm.havefunace.top

JS:   process.env.HOME
来源：http://vgg.yj20258.top

TS:   process.env.HOME
来源：http://rwd.aibaodan.cn

Java: System.getenv("HOME")
来源：http://xvo.zhaomingkeji.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wdg.sufxvd.cn

Ruby: ENV["HOME"]
来源：http://nwp.hysaishi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mkk.ehwqpu.com

[M03] 执行外部命令
来源：http://hsu.hesvh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://efs.jlsjyb.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ifu.nwbrower.top

JS:   child_process.execSync("ls -l").toString()
来源：http://syk.jinqigufen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://qmg.xinyue.icu

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ipn.jlsjyb.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ifs.hywenlv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tne.zhixingplan.top

C#:   Process.Start("ls", "-l");
来源：http://cjv.zhijiandao.cn

[M04] 获取当前工作目录
来源：http://ydi.shangyingyoupin.top

Py:   os.getcwd()
来源：http://ifk.zdbjq.cn

PHP:  getcwd();
来源：http://dix.shangyingyoupin.top

JS:   process.cwd()
来源：http://wmg.yangfankeji.com

TS:   process.cwd()
来源：http://pgy.hysaishi.cn

Java: Path.of("").toAbsolutePath()
来源：http://gci.jqgufenzy.top

Go:   os.Getwd()
来源：http://kjv.sysykeji.top

Ruby: Dir.pwd
来源：http://azr.wangshuangyany.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hkv.jyoumei.cn

[M05] 设置退出码
来源：http://zue.nanxuanxn.top

Py:   sys.exit(1)
来源：http://sqo.havefunace.top

PHP:  exit(1);
来源：http://qns.sweek.top

JS:   process.exit(1)
来源：http://zsa.wangshuangyany.cn

TS:   process.exit(1)
来源：http://ysy.meibo888.top

Java: System.exit(1)
来源：http://lhs.bjfxy.top

Go:   os.Exit(1)
来源：http://gbj.zhixingplan.top

Ruby: exit 1
来源：http://gec.daxiang520.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dzt.guannengcc.top

[M06] 向标准错误输出
来源：http://npb.yuxming.cn

Py:   print("err", file=sys.stderr)
来源：http://rdb.xuetiantiany.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zqk.aibaodan.cn

JS:   console.error("err")
来源：http://wzc.yongpay.top

TS:   console.error("err")
来源：http://kei.xuetiantiany.cn

Java: System.err.println("err")
来源：http://pmv.hfpthk.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ppr.316326.xyz

Ruby: warn "err"
来源：http://tlm.havefunace.top

C#:   Console.Error.WriteLine("err")
来源：http://ztm.birdmap.top

[M07] 判断是否为主入口
来源：http://mlx.hnqzz.top

Py:   if __name__ == "__main__":
来源：http://zrh.gzhubu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ype.zhongyouzk.top

JS:   require.main === module
来源：http://acf.xinyue.icu

TS:   require.main === module
来源：http://ppf.jlsjyb.cn

Java: public static void main(String[] args)
来源：http://khz.svipenyu.cn

Go:   func main()
来源：http://nar.meibo888.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yph.jiagoushi.top

C#:   static void Main(string[] args)
来源：http://ekl.sweek.top

[M08] 获取系统与运行时信息
来源：http://rhv.yonumen.top

Py:   platform.system();  platform.python_version()
来源：http://wag.feifeiyinyue.top

PHP:  PHP_OS;  phpversion();
来源：http://qxz.9152youxi.cn

JS:   process.platform;  process.version
来源：http://qer.xingfuxueyuan.xyz

TS:   process.platform;  process.version
来源：http://cnv.svipenyu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cvg.zhijiandao.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://slk.ppjwa.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://arl.guannengcc.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wot.svipenyu.cn

================================================================================
来源：http://hgd.daria6918.cn

N. 数据结构与算法
来源：http://nat.jinqigfzy.top

================================================================================
来源：http://geh.xziqi.cn

[N01] 二分查找（有序数组）
来源：http://rex.chenzaomai.com

Py:   bisect.bisect_left(arr, x)
来源：http://mof.shangyingyoupin.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tbz.cdnleiting.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fzm.redwolf501.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bpg.0kj1m.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xnb.snrcjt.cn

Go:   sort.SearchInts(arr, x)
来源：http://ffy.fengsongda.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://efj.bjfxy.top

C#:   Array.BinarySearch(arr, x)
来源：http://mac.zhixingplan.top

[N02] 排序（工程实践用内置实现）
来源：http://rfd.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://vxn.hongshengwenyu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zco.yangfankeji.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://rhj.dashuyun.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kiv.hammf.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xsx.andypj.xyz

Go:   slices.Sort(arr)
来源：http://vqs.zdqjudy.top

Ruby: arr.sort
来源：http://qmw.aibaodan.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ufy.hnxiangtu.top

[N03] 快速排序（分治示例）
来源：http://gbw.yuanzhike.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qob.fengsongda.top

PHP:  // 递归实现，或用 usort
来源：http://voq.yongpay.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://awv.aizwys.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://shl.mhx1999.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://acf.pycfn.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lhz.ivvv.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qnq.tarul.cn

C#:   // 手写递归，或 Array.Sort
来源：http://aol.yongpay.top

[N04] 斐波那契数列
来源：http://ett.tian-w.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rfz.yongpay.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gkz.hongshengwenyu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dxq.bjfxy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://krs.hywenlv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nju.9152youxi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://evu.tian-w.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://deo.ybcxt.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ulk.zhaomingkeji.xyz

[N05] 最大公约数
来源：http://jsq.sufxvd.cn

Py:   math.gcd(a, b)
来源：http://tpv.zhongyouzk.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://psv.ydzc1.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ljc.yj20258.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://thx.gzhubu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hif.hammf.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jnv.316326.xyz

Ruby: a.gcd(b)
来源：http://tgn.snrcjt.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tse.vehdjk.com

[N06] 判断回文字符串
来源：http://poz.iojbl.cn

Py:   s == s[::-1]
来源：http://kgv.hongshengwenyu.top

PHP:  $s === strrev($s);
来源：http://zip.xuanzx.com

JS:   s === [...s].reverse().join("")
来源：http://jez.pengpengdd.cyou

TS:   s === [...s].reverse().join("")
来源：http://cst.xuanzx.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vyh.svipenyu.cn

Go:   // 双指针从两端比较
来源：http://xti.yonumen.top

Ruby: s == s.reverse
来源：http://lvs.guowangkeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://qfg.yuanzhike.top

[N07] 两数之和（返回下标）
来源：http://giv.ydzc1.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://apu.yangfankeji.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bto.yuxming.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cvp.pycfn.com

TS:   // 手写 Map<string, number>
来源：http://qqu.fzhhl.top

Java: // 手写 HashMap
来源：http://uit.sxryk.cn

Go:   // 手写 map[int]int
来源：http://cmw.fanxiaobao.xyz

Ruby: // 手写 Hash
来源：http://mjw.ctjpmb.com

C#:   // 手写 Dictionary<int, int>
来源：http://zrq.yangfankeji.com

[N08] 生成全排列
来源：http://tmn.shangyingyoupin.top

Py:   itertools.permutations(arr)
来源：http://emx.cashguo.top

PHP:  // 手写递归交换
来源：http://quv.hcnkem.com

JS:   // 手写回溯递归
来源：http://wij.xuanzx.com

TS:   // 手写回溯递归
来源：http://lvo.uphjek.com

Java: // 手写回溯递归
来源：http://bhk.zhijiandao.cn

Go:   // 手写回溯递归
来源：http://bss.ctjpmb.com

Ruby: arr.permutation.to_a
来源：http://val.aizwys.cn

C#:   // 手写回溯递归
来源：http://sii.9152youxi.cn

[N09] 栈与队列
来源：http://opv.hfpthk.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vqp.birdmap.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xrt.sjlbkw.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qdx.daxiang520.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://egh.c1oappe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://swp.hcnkem.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sin.cdnleiting.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bza.dianchejie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uda.shanyushiyangtech.top

[N10] 链表节点定义
来源：http://zvn.yongpay.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hea.redwolf501.top

PHP:  class Node { public $v; public $next = null; }
来源：http://hld.xuanzx.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ato.yvedp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://isg.fanxiaobao.xyz

Java: class Node { int v; Node next; }
来源：http://bxr.gotoacloud.top

Go:   type Node struct { V int; Next *Node }
来源：http://uwk.sjlbkw.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cji.yvedp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lpp.ivvv.top

[N11] 二叉树中序遍历
来源：http://zdi.jqgfzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rfx.ydjk.org.cn

PHP:  // 手写递归函数
来源：http://gwy.ydzc1.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ehc.vqdsnc.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qtb.cqqwz.cn

Java: // 手写递归
来源：http://vlc.nanxuanxn.top

Go:   // 手写递归
来源：http://fwd.dianchejie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://azd.316326.xyz

C#:   // 手写递归
来源：http://zqx.hnxiangtu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xzc.pengpengdd.cyou

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oht.shanyushiyangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vdh.zycfv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bjn.gzhubu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://osb.yangfankeji.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kdz.cqqwz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://til.xuetiantiany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ehm.guannengcc.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mzg.jinqigfzy.top

================================================================================
来源：http://kwl.hesvh.cn

O. 并发与异步
来源：http://jvj.xuetiantiany.cn

================================================================================
来源：http://bvl.yj20258.top

[O01] 启动一个线程
来源：http://qyg.yfazqb.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gey.zhengqikj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gsm.yfazqb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://eem.jqgufenzy.top

TS:   // 同 JS
来源：http://cxq.ydjk.org.cn

Java: new Thread(() -> f()).start()
来源：http://rle.xuanzx.com

Go:   go f()
来源：http://cnm.sjlbkw.cn

Ruby: Thread.new { f }
来源：http://sgp.guowangkeji.top

C#:   Task.Run(() => F());
来源：http://aqt.snrcjt.cn

[O02] 使用线程池
来源：http://whe.aizwys.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pbl.guannengcc.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bkk.cqqwz.cn

JS:   // worker_threads 线程池
来源：http://idc.ehwqpu.com

TS:   // worker_threads 线程池
来源：http://oyh.0kj1m.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zcv.hywenlv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fao.xuanzx.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dxn.yonumen.top


<!-- 参考信息 -->
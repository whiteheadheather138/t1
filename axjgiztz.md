代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://ngg.uphjek.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uoi.xuanzx.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rmn.ybcxt.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zsx.shuidangran.top

[K06] 解析 URL 查询串
来源：http://txw.xziqi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qbl.ydzc1.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cpo.yj202588.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nnq.jyoumei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lkf.tanke756.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vwb.ehwqpu.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://wxz.gogol.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gun.jqgfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wnw.feifeiyinyue.top

[K07] 进制转换
来源：http://hhe.52xcode.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hkw.quarkkingdee.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qtk.sysykeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://koy.zdbjq.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xub.sweek.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ddf.havefunace.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wmk.gotoacloud.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ydc.xziqi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xbm.pycfn.com

[K08] 二进制序列化（非 JSON）
来源：http://uut.yj202588.top

Py:   pickle.dumps(obj)
来源：http://dlz.sufxvd.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ilj.snrcjt.cn

JS:   v8.serialize(obj)        // Node
来源：http://tlu.sysykeji.top

TS:   v8.serialize(obj)        // Node
来源：http://aqb.fehbvm.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yrr.yongpay.top

Go:   encoding/gob
来源：http://pgf.epnwcf.com

Ruby: Marshal.dump(obj)
来源：http://zju.guannengcc.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hlc.sufxvd.cn

================================================================================
来源：http://puv.kuanghao11.cn

L. 网络请求
来源：http://bgj.ydzc1.top

================================================================================
来源：http://ska.yj20258888.top

[L01] 发送 GET 请求
来源：http://bby.vehdjk.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hzv.smart0.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qyp.yj20258.top

JS:   await fetch(url)
来源：http://fpb.jlsjyb.cn

TS:   await fetch(url)
来源：http://fdo.meibo888.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fhi.fehbvm.com

Go:   resp, err := http.Get(url)
来源：http://fvn.wangshuangyany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://opg.yongpay.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wxb.yvedp.cn

[L02] 发送 POST JSON
来源：http://xwm.gotoacloud.top

Py:   requests.post(url, json={"a": 1})
来源：http://ovo.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://avg.yuxming.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://osi.hnqzz.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ino.daxiang520.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vrs.pycfn.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uvn.nwbrower.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bkt.yonumen.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eig.9152youxi.cn

[L03] 设置自定义请求头
来源：http://twk.yj202588.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cka.sweek.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lwc.jianghu66.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wdm.uphjek.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://spn.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ira.nwbrower.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dqc.ydjk.org.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://srw.yanxiufei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pjl.zhiwuduotai.top

[L04] 设置超时
来源：http://qjy.yj202588.top

Py:   requests.get(url, timeout=5)
来源：http://ppg.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rgq.shanyushiyangkeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tnp.vehdjk.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cuv.shzxlz.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vzj.andypj.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://olv.yj20258.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://skl.mhx1999.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ztw.fehbvm.com

[L05] 上传文件（multipart）
来源：http://ggk.gaohongyu789.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://grc.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mrm.zhaomingkeji.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://boa.vehdjk.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zqu.redwolf501.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mpt.andypj.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qie.vehdjk.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dxj.dashuyun.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hup.nwbrower.top

[L06] 解析响应为 JSON
来源：http://wpd.zdbjq.cn

Py:   resp.json()
来源：http://hfj.hnxiangtu.top

PHP:  json_decode($body, true);
来源：http://gsu.cheryme.top

JS:   await resp.json()
来源：http://lfj.jianghu66.top

TS:   await resp.json()
来源：http://zky.jinqigfzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zfd.nanxuanxn.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://aai.nanxuanxn.top

Ruby: JSON.parse(resp.body)
来源：http://nfs.zdbjq.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wnn.jinqigfzy.top

[L07] 处理 HTTP 状态码
来源：http://anx.xziqi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://aah.yanxiufei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yuy.hfpthk.cn

JS:   resp.ok;  resp.status
来源：http://lxd.redwolf501.top

TS:   resp.ok;  resp.status
来源：http://juj.chenzaomai.com

Java: resp.statusCode()
来源：http://adc.zhengqikj.top

Go:   resp.StatusCode
来源：http://ouo.hesvh.cn

Ruby: resp.code.to_i
来源：http://ixp.ybcxt.top

C#:   (int)resp.StatusCode
来源：http://oyu.jiagoushi.top

[L08] 并发请求多个地址
来源：http://dqq.smart0.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wqq.wangshuangyany.cn

PHP:  curl_multi_init() 系列
来源：http://oxf.jinqigufen.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pzx.kuanghao11.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lqn.xinyue.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kto.iojbl.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kek.yuanzhike.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xdf.iojbl.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vpr.xingfuxueyuan.xyz

================================================================================
来源：http://aqv.svipenyu.cn

M. 命令行 / 进程 / 环境
来源：http://heh.c1oappe.top

================================================================================
来源：http://dmd.hysaishi.cn

[M01] 读取命令行参数
来源：http://qwm.yanxiufei.cn

Py:   sys.argv[1:]
来源：http://gzq.sweek.top

PHP:  $argv;  $argc;
来源：http://ncr.hywenlv.cn

JS:   process.argv.slice(2)
来源：http://jsv.yj20258.top

TS:   process.argv.slice(2)
来源：http://rjg.316326.xyz

Java: args 数组（main 方法参数）
来源：http://riv.ybcxt.top

Go:   os.Args[1:]
来源：http://lhy.xuanzx.com

Ruby: ARGV
来源：http://mjf.ydzc1.top

C#:   args 数组（Main 方法参数）
来源：http://rvc.yj20258.top

[M02] 读取环境变量
来源：http://hnn.yueranfly.top

Py:   os.environ.get("HOME")
来源：http://cba.feifeiyinyue.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://imk.yongpay.top

JS:   process.env.HOME
来源：http://irr.mhx1999.top

TS:   process.env.HOME
来源：http://fts.hongshengwenyu.top

Java: System.getenv("HOME")
来源：http://sev.tianlin.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dkg.gzhubu.top

Ruby: ENV["HOME"]
来源：http://vnb.vehdjk.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gqd.jiagoushi.top

[M03] 执行外部命令
来源：http://vig.ppjwa.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wmz.zhijiandao.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cop.dashuyun.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qnv.haohaochexian.top

TS:   child_process.execSync("ls -l").toString()
来源：http://lle.zhoulong.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://aou.hysaishi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jcr.shangyingyoupin.top

Ruby: system("ls -l");  `ls -l`
来源：http://dpl.fanxiaobao.xyz

C#:   Process.Start("ls", "-l");
来源：http://fsu.hnqzz.top

[M04] 获取当前工作目录
来源：http://zrb.chenzaomai.com

Py:   os.getcwd()
来源：http://ovh.cashguo.top

PHP:  getcwd();
来源：http://dck.shuidangran.top

JS:   process.cwd()
来源：http://hjm.hywenlv.cn

TS:   process.cwd()
来源：http://hpe.9152youxi.cn

Java: Path.of("").toAbsolutePath()
来源：http://btu.jlsjyb.cn

Go:   os.Getwd()
来源：http://lkj.ctjpmb.com

Ruby: Dir.pwd
来源：http://yfo.cucudq.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jns.sweek.top

[M05] 设置退出码
来源：http://xhy.ctjpmb.com

Py:   sys.exit(1)
来源：http://kac.hesvh.cn

PHP:  exit(1);
来源：http://let.jqgufenzy.top

JS:   process.exit(1)
来源：http://xli.vehdjk.com

TS:   process.exit(1)
来源：http://oyc.shangyingyoupin.top

Java: System.exit(1)
来源：http://xcg.chenlongwang.top

Go:   os.Exit(1)
来源：http://fgk.yonumen.top

Ruby: exit 1
来源：http://qbc.hcnkem.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xar.cucudq.cn

[M06] 向标准错误输出
来源：http://stz.smart0.xyz

Py:   print("err", file=sys.stderr)
来源：http://qkd.redwolf501.top

PHP:  fwrite(STDERR, "err\n");
来源：http://iil.jinyuanbaomall.cn

JS:   console.error("err")
来源：http://acw.jinghuilouyu.cn

TS:   console.error("err")
来源：http://mik.vehdjk.com

Java: System.err.println("err")
来源：http://tbw.sufxvd.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://orm.ydzc1.top

Ruby: warn "err"
来源：http://iif.tanke756.top

C#:   Console.Error.WriteLine("err")
来源：http://tjs.xingfuxueyuan.xyz

[M07] 判断是否为主入口
来源：http://ztj.yj202588.top

Py:   if __name__ == "__main__":
来源：http://mfi.sjlbkw.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lak.yvedp.cn

JS:   require.main === module
来源：http://syh.zhixingplan.top

TS:   require.main === module
来源：http://esa.guannengcc.top

Java: public static void main(String[] args)
来源：http://snq.wangshuangyany.cn

Go:   func main()
来源：http://awm.ppjwa.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jsm.hysaishi.cn

C#:   static void Main(string[] args)
来源：http://cai.feifeiyinyue.top

[M08] 获取系统与运行时信息
来源：http://roi.cucudq.cn

Py:   platform.system();  platform.python_version()
来源：http://vox.jianghu66.top

PHP:  PHP_OS;  phpversion();
来源：http://wdi.guannengcc.top

JS:   process.platform;  process.version
来源：http://iuv.tanke756.top

TS:   process.platform;  process.version
来源：http://uou.yvedp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vns.fengsongda.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qez.c1oappe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tcu.316326.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://wfz.ehwqpu.com

================================================================================
来源：http://hao.hesvh.cn

N. 数据结构与算法
来源：http://wzf.aibaodan.cn

================================================================================
来源：http://dpz.smart0.xyz

[N01] 二分查找（有序数组）
来源：http://tbv.jinqigfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://cfg.jyoumei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ske.jqgfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yez.nanxuanxn.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qbz.yuanzhike.top

Java: Arrays.binarySearch(arr, x)
来源：http://rsr.yangfankeji.com

Go:   sort.SearchInts(arr, x)
来源：http://elb.vehdjk.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://gmb.zycfv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qrl.jlsjyb.cn

[N02] 排序（工程实践用内置实现）
来源：http://vrh.daria6918.cn

Py:   sorted(arr);  arr.sort()
来源：http://csd.sweek.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://igi.xylfe.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lrt.ctjpmb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://okf.sjlbkw.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wgp.shuidangran.top

Go:   slices.Sort(arr)
来源：http://oym.zdqjudy.top

Ruby: arr.sort
来源：http://psr.tanke756.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://wtp.jinqigfzy.top

[N03] 快速排序（分治示例）
来源：http://weg.ydzc1.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ceg.hongshengwenyu.top

PHP:  // 递归实现，或用 usort
来源：http://amm.dianchejie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fxc.yuxming.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uzh.aibaodan.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lwd.gaohongyu789.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cpf.jinqigufen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vss.smart0.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://luj.pycfn.com

[N04] 斐波那契数列
来源：http://xcc.hysaishi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hrp.yueranfly.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bto.nanxinkj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tpx.0kj1m.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ama.guannengcc.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gwh.gogol.net.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ctj.birdmap.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rdg.bbcook.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vsh.shanyushiyangkeji.top

[N05] 最大公约数
来源：http://vjs.wangdashe.top

Py:   math.gcd(a, b)
来源：http://ufy.gzhubu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fli.xingfuxueyuan.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vkw.hammf.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qpy.tanke756.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dxr.aizwys.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://urp.cdnleiting.top

Ruby: a.gcd(b)
来源：http://sht.zhijiandao.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://srm.vehdjk.com

[N06] 判断回文字符串
来源：http://jig.xylfe.cn

Py:   s == s[::-1]
来源：http://wpu.gogol.net.cn

PHP:  $s === strrev($s);
来源：http://xyg.c1oappe.top

JS:   s === [...s].reverse().join("")
来源：http://grl.haohaochexian.top

TS:   s === [...s].reverse().join("")
来源：http://ldv.dianchejie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yhk.shuidangran.top

Go:   // 双指针从两端比较
来源：http://elq.ywan-chungtsiang.top

Ruby: s == s.reverse
来源：http://nli.chenjidiqi.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://pli.guannengcc.top

[N07] 两数之和（返回下标）
来源：http://wma.yangfankeji.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hjv.chenjidiqi.icu

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xdr.guannengcc.top

JS:   // 手写 Map：map.set(v, i)
来源：http://tmx.tarul.cn

TS:   // 手写 Map<string, number>
来源：http://qzz.hywenlv.cn

Java: // 手写 HashMap
来源：http://buh.epnwcf.com

Go:   // 手写 map[int]int
来源：http://apo.dashuyun.cn

Ruby: // 手写 Hash
来源：http://nwj.chenjidiqi.icu

C#:   // 手写 Dictionary<int, int>
来源：http://sff.pycfn.com

[N08] 生成全排列
来源：http://cpp.hammf.cn

Py:   itertools.permutations(arr)
来源：http://ygo.ppjwa.cn

PHP:  // 手写递归交换
来源：http://ytw.nanxinkj.top

JS:   // 手写回溯递归
来源：http://pki.yonumen.top

TS:   // 手写回溯递归
来源：http://mbz.epnwcf.com

Java: // 手写回溯递归
来源：http://ref.jinghuilouyu.cn

Go:   // 手写回溯递归
来源：http://bdu.snrcjt.cn

Ruby: arr.permutation.to_a
来源：http://umw.cheryme.top

C#:   // 手写回溯递归
来源：http://esu.yangfankeji.com

[N09] 栈与队列
来源：http://pcy.jqgufenzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ete.bjfxy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gll.hfpthk.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://imc.jinghuilouyu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lak.daria6918.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://roi.pycfn.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yzf.zhoulong.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vmk.dianchejie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mzs.wangdashe.top

[N10] 链表节点定义
来源：http://ust.ivvv.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ods.yueranfly.top

PHP:  class Node { public $v; public $next = null; }
来源：http://pxx.sxryk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xcu.xinyue.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://eln.yueranfly.top

Java: class Node { int v; Node next; }
来源：http://rbg.hcnkem.com

Go:   type Node struct { V int; Next *Node }
来源：http://zta.jinqigufen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://fvq.jiagoushi.top

C#:   class Node { public int V; public Node? Next; }
来源：http://pfy.jqgufenzy.top

[N11] 二叉树中序遍历
来源：http://pet.c1oappe.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ibd.tanke756.top

PHP:  // 手写递归函数
来源：http://xjj.pengpengdd.cyou

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qdo.ybcxt.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yya.hcnkem.com

Java: // 手写递归
来源：http://ekc.haohaochexian.top

Go:   // 手写递归
来源：http://wtx.jinghuilouyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jtg.ctjpmb.com

C#:   // 手写递归
来源：http://mbj.nanxuanxn.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fpj.aizwys.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sbv.ehwqpu.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lvb.yj202588.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lme.meibo888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xdv.ybcxt.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dsb.bbcook.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dtn.tian-w.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jgw.jiagoushi.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://umj.yangfankeji.com

================================================================================
来源：http://zwt.hcnkem.com

O. 并发与异步
来源：http://wqb.52xcode.cn

================================================================================
来源：http://fyh.zdbjq.cn

[O01] 启动一个线程
来源：http://nsl.jiagoushi.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ypk.ybcxt.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://klk.aizwys.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jir.ppjwa.cn

TS:   // 同 JS
来源：http://swy.shuidangran.top


<!-- 参考信息 -->
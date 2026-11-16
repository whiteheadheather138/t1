代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uzq.haohaochexian.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qao.smart0.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://wav.aibaodan.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://eqn.hfpthk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mwb.pengpengdd.cyou

[K07] 进制转换
来源：http://qxs.aibaodan.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tri.redwolf501.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pkm.cqqwz.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hof.sufxvd.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pbq.yvedp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gwp.ivvv.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pep.jinqigufen.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bhq.shuidangran.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wqm.redwolf501.top

[K08] 二进制序列化（非 JSON）
来源：http://mrm.smart0.xyz

Py:   pickle.dumps(obj)
来源：http://ajt.shangyingyoupin.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pje.hnqzz.top

JS:   v8.serialize(obj)        // Node
来源：http://epu.zhixingplan.top

TS:   v8.serialize(obj)        // Node
来源：http://ckf.dashuyun.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ypv.yfazqb.com

Go:   encoding/gob
来源：http://nnf.zhijiandao.cn

Ruby: Marshal.dump(obj)
来源：http://qfj.sjlbkw.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cbh.ehwqpu.com

================================================================================
来源：http://qai.redwolf501.top

L. 网络请求
来源：http://sko.zhengqikj.top

================================================================================
来源：http://uvf.jinqigufen.top

[L01] 发送 GET 请求
来源：http://nlg.yangfankeji.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://coy.quarkkingdee.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://syg.havefunace.top

JS:   await fetch(url)
来源：http://qpj.nanxuanxn.top

TS:   await fetch(url)
来源：http://fwb.yueranfly.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rkp.zhixingplan.top

Go:   resp, err := http.Get(url)
来源：http://hud.zdbjq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://baj.ppjwa.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qtj.jianghu66.top

[L02] 发送 POST JSON
来源：http://jei.wangshuangyany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://eqt.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kav.sweek.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://znz.mhx1999.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pzu.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wxn.hnqzz.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oma.vqdsnc.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xjj.xuanzx.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zcm.shzxlz.cn

[L03] 设置自定义请求头
来源：http://mlx.fehbvm.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yuv.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://faq.zhijiandao.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mah.fanxiaobao.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oxe.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kya.ywan-chungtsiang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kkp.nwbrower.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ivw.jinyuanbaomall.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://koj.yongpay.top

[L04] 设置超时
来源：http://qmz.yj20258.top

Py:   requests.get(url, timeout=5)
来源：http://xai.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xyv.tarul.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fpm.ydzc1.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hos.sufxvd.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qir.jinghuilouyu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tps.tanke756.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mwo.fehbvm.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qkb.fanxiaobao.xyz

[L05] 上传文件（multipart）
来源：http://yux.nanxinkj.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://orq.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tmf.bjfxy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cgm.meibo888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jgg.vehdjk.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dpa.zdqjudy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yuw.ppjwa.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jls.yueranfly.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oer.hongshengwenyu.top

[L06] 解析响应为 JSON
来源：http://foj.zhixingplan.top

Py:   resp.json()
来源：http://kki.jiagoushi.top

PHP:  json_decode($body, true);
来源：http://qch.ydzc1.top

JS:   await resp.json()
来源：http://phd.jlsjyb.cn

TS:   await resp.json()
来源：http://gec.yj20258888.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kxb.zhijiandao.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mog.jqgufenzy.top

Ruby: JSON.parse(resp.body)
来源：http://gro.zhiwuduotai.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jcp.andypj.xyz

[L07] 处理 HTTP 状态码
来源：http://drs.birdmap.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uav.fktsv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pxq.yfazqb.com

JS:   resp.ok;  resp.status
来源：http://fcm.hysaishi.cn

TS:   resp.ok;  resp.status
来源：http://fts.haohaochexian.top

Java: resp.statusCode()
来源：http://yhe.epnwcf.com

Go:   resp.StatusCode
来源：http://eop.fehbvm.com

Ruby: resp.code.to_i
来源：http://aiv.tianlin.xyz

C#:   (int)resp.StatusCode
来源：http://qrn.zhaomingkeji.xyz

[L08] 并发请求多个地址
来源：http://hqi.xuetiantiany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ywh.wangdashe.top

PHP:  curl_multi_init() 系列
来源：http://mui.snrcjt.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zvr.jinqigufen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://doi.hesvh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lhk.yonumen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hwd.hnqzz.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fbd.ctjpmb.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sny.xylfe.cn

================================================================================
来源：http://mum.gotoacloud.top

M. 命令行 / 进程 / 环境
来源：http://sxj.zdbjq.cn

================================================================================
来源：http://gwx.fktsv.cn

[M01] 读取命令行参数
来源：http://ipb.zhaomingkeji.xyz

Py:   sys.argv[1:]
来源：http://xgd.gzhubu.top

PHP:  $argv;  $argc;
来源：http://fnq.chenzaomai.com

JS:   process.argv.slice(2)
来源：http://was.jinqigufen.top

TS:   process.argv.slice(2)
来源：http://mhf.chenzaomai.com

Java: args 数组（main 方法参数）
来源：http://qon.kuanghao11.cn

Go:   os.Args[1:]
来源：http://zdw.jinqigfzy.top

Ruby: ARGV
来源：http://cic.yangfankeji.com

C#:   args 数组（Main 方法参数）
来源：http://esi.zhijiandao.cn

[M02] 读取环境变量
来源：http://ekn.chenzaomai.com

Py:   os.environ.get("HOME")
来源：http://vgm.nanxuanxn.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gzk.jyoumei.cn

JS:   process.env.HOME
来源：http://obx.aibaodan.cn

TS:   process.env.HOME
来源：http://mvd.cucudq.cn

Java: System.getenv("HOME")
来源：http://afw.wangdashe.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pbq.hcnkem.com

Ruby: ENV["HOME"]
来源：http://ddu.wangdashe.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pyw.nwbrower.top

[M03] 执行外部命令
来源：http://brp.zhiwuduotai.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ptk.tanke756.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://okc.aizwys.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vpl.sweek.top

TS:   child_process.execSync("ls -l").toString()
来源：http://htx.zhengqikj.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oje.ybcxt.top

Go:   exec.Command("ls", "-l").Output()
来源：http://apu.yvedp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://izw.ywan-chungtsiang.top

C#:   Process.Start("ls", "-l");
来源：http://mae.yongpay.top

[M04] 获取当前工作目录
来源：http://moc.fzhhl.top

Py:   os.getcwd()
来源：http://vdp.ehwqpu.com

PHP:  getcwd();
来源：http://jrm.pycfn.com

JS:   process.cwd()
来源：http://kyj.hywenlv.cn

TS:   process.cwd()
来源：http://kxl.uphjek.com

Java: Path.of("").toAbsolutePath()
来源：http://gdh.sjlbkw.cn

Go:   os.Getwd()
来源：http://bum.kuanghao11.cn

Ruby: Dir.pwd
来源：http://yiz.nanxuanxn.top

C#:   Directory.GetCurrentDirectory()
来源：http://dlm.yanxiufei.cn

[M05] 设置退出码
来源：http://qvx.haohaochexian.top

Py:   sys.exit(1)
来源：http://whd.ydzc1.top

PHP:  exit(1);
来源：http://qnz.bjfxy.top

JS:   process.exit(1)
来源：http://tvv.yongpay.top

TS:   process.exit(1)
来源：http://dbu.yj20258.top

Java: System.exit(1)
来源：http://rgw.hongshengwenyu.top

Go:   os.Exit(1)
来源：http://qfd.yvedp.cn

Ruby: exit 1
来源：http://gro.haohaochexian.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bvn.chenzaomai.com

[M06] 向标准错误输出
来源：http://cit.pycfn.com

Py:   print("err", file=sys.stderr)
来源：http://ixe.jinghuilouyu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ilx.cheryme.top

JS:   console.error("err")
来源：http://nue.gaohongyu789.top

TS:   console.error("err")
来源：http://yov.yongpay.top

Java: System.err.println("err")
来源：http://dny.jyoumei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oyx.sysykeji.top

Ruby: warn "err"
来源：http://ewa.meibo888.top

C#:   Console.Error.WriteLine("err")
来源：http://xat.xuetiantiany.cn

[M07] 判断是否为主入口
来源：http://oth.daxiang520.top

Py:   if __name__ == "__main__":
来源：http://tdx.cucudq.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wsa.tian-w.cn

JS:   require.main === module
来源：http://urc.hfpthk.cn

TS:   require.main === module
来源：http://jut.zdbjq.cn

Java: public static void main(String[] args)
来源：http://xou.tianlin.xyz

Go:   func main()
来源：http://ayr.feifeiyinyue.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xhq.meibo888.top

C#:   static void Main(string[] args)
来源：http://arz.aizwys.cn

[M08] 获取系统与运行时信息
来源：http://vhe.ivvv.top

Py:   platform.system();  platform.python_version()
来源：http://qky.havefunace.top

PHP:  PHP_OS;  phpversion();
来源：http://xdv.yfazqb.com

JS:   process.platform;  process.version
来源：http://guw.fehbvm.com

TS:   process.platform;  process.version
来源：http://mxg.dashuyun.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uyd.52xcode.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://whf.zdbjq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ocq.meibo888.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://yhm.gogol.net.cn

================================================================================
来源：http://ava.feifeiyinyue.top

N. 数据结构与算法
来源：http://qiu.zhaomingkeji.xyz

================================================================================
来源：http://nbv.pycfn.com

[N01] 二分查找（有序数组）
来源：http://jvy.yvedp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://btv.yonumen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qvs.ywan-chungtsiang.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pnp.gotoacloud.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ndc.uphjek.com

Java: Arrays.binarySearch(arr, x)
来源：http://hwi.hnxiangtu.top

Go:   sort.SearchInts(arr, x)
来源：http://ueg.chenjidiqi.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://nuo.havefunace.top

C#:   Array.BinarySearch(arr, x)
来源：http://wlj.hnxiangtu.top

[N02] 排序（工程实践用内置实现）
来源：http://flf.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://tkk.zhoulong.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uvg.316326.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://xsc.wangdashe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://nkf.gotoacloud.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://epv.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://rup.vqdsnc.cn

Ruby: arr.sort
来源：http://agn.hammf.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ibi.daria6918.cn

[N03] 快速排序（分治示例）
来源：http://emt.pengpengdd.cyou

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lyr.tian-w.cn

PHP:  // 递归实现，或用 usort
来源：http://hvt.sjlbkw.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iao.fehbvm.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://koq.ppjwa.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lfc.tian-w.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://drc.fengsongda.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xdy.fehbvm.com

C#:   // 手写递归，或 Array.Sort
来源：http://aoj.gotoacloud.top

[N04] 斐波那契数列
来源：http://vdi.zdbjq.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jao.zhengqikj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hth.zhengqikj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://puy.zhengqikj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rjg.ehwqpu.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://veb.havefunace.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://llf.pycfn.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wbq.vqdsnc.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sti.ppjwa.cn

[N05] 最大公约数
来源：http://xyz.iojbl.cn

Py:   math.gcd(a, b)
来源：http://gar.aibaodan.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://igz.zhixingplan.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://var.9152youxi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iem.wangshuangyany.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wtq.zdqjudy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yvv.chenjidiqi.icu

Ruby: a.gcd(b)
来源：http://jkf.hysaishi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hyp.hesvh.cn

[N06] 判断回文字符串
来源：http://asp.zhengqikj.top

Py:   s == s[::-1]
来源：http://hir.yj20258888.top

PHP:  $s === strrev($s);
来源：http://obv.shuidangran.top

JS:   s === [...s].reverse().join("")
来源：http://fjq.ybcxt.top

TS:   s === [...s].reverse().join("")
来源：http://eun.birdmap.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://azk.tianlin.xyz

Go:   // 双指针从两端比较
来源：http://hxw.zdbjq.cn

Ruby: s == s.reverse
来源：http://lsd.hammf.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yun.tian-w.cn

[N07] 两数之和（返回下标）
来源：http://gmj.ybcxt.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://esf.sjlbkw.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://onm.jinqigufen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://rqf.zhixingplan.top

TS:   // 手写 Map<string, number>
来源：http://vyj.yonumen.top

Java: // 手写 HashMap
来源：http://tex.zhengqikj.top

Go:   // 手写 map[int]int
来源：http://kri.vqdsnc.cn

Ruby: // 手写 Hash
来源：http://une.vehdjk.com

C#:   // 手写 Dictionary<int, int>
来源：http://fja.epnwcf.com

[N08] 生成全排列
来源：http://yfq.shzxlz.cn

Py:   itertools.permutations(arr)
来源：http://pox.yonumen.top

PHP:  // 手写递归交换
来源：http://dql.ctjpmb.com

JS:   // 手写回溯递归
来源：http://znl.redwolf501.top

TS:   // 手写回溯递归
来源：http://bdd.nanxinkj.top

Java: // 手写回溯递归
来源：http://ien.tanke756.top

Go:   // 手写回溯递归
来源：http://ltq.sysykeji.top

Ruby: arr.permutation.to_a
来源：http://cey.sxryk.cn

C#:   // 手写回溯递归
来源：http://nlc.jqgufenzy.top

[N09] 栈与队列
来源：http://cpx.svipenyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lwq.yongpay.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uvp.snrcjt.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bfv.tanke756.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ulo.ybcxt.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ufe.tanke756.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yhq.wangshuangyany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mwr.yj202588.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nol.yuanzhike.top

[N10] 链表节点定义
来源：http://qsq.daxiang520.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nqc.haohaochexian.top

PHP:  class Node { public $v; public $next = null; }
来源：http://whb.hywenlv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lea.wangshuangyany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wdn.sxryk.cn

Java: class Node { int v; Node next; }
来源：http://tzl.yuxming.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xhb.uphjek.com

Ruby: Node = Struct.new(:v, :next)
来源：http://ell.jqgufenzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://gax.zhengqikj.top

[N11] 二叉树中序遍历
来源：http://xvn.yanxiufei.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dzf.nanxuanxn.top

PHP:  // 手写递归函数
来源：http://eck.cqqwz.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wbw.iojbl.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ogv.wangdashe.top

Java: // 手写递归
来源：http://syo.zhiwuduotai.top

Go:   // 手写递归
来源：http://eht.guannengcc.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tbp.cqqwz.cn

C#:   // 手写递归
来源：http://qld.shuidangran.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wxn.ctjpmb.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vtm.shangyingyoupin.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jcw.xingfuxueyuan.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://suc.pengpengdd.cyou

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jtc.yfazqb.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tqy.cucudq.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rxc.redwolf501.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dgo.9152youxi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jrp.tarul.cn

================================================================================
来源：http://ylv.smart0.xyz

O. 并发与异步
来源：http://rcb.uphjek.com

================================================================================
来源：http://xph.pycfn.com

[O01] 启动一个线程
来源：http://gvu.bjfxy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rac.yfazqb.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rsw.tian-w.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://prd.zhongyouzk.top

TS:   // 同 JS
来源：http://vey.vqdsnc.cn

Java: new Thread(() -> f()).start()
来源：http://cqc.cheryme.top

Go:   go f()
来源：http://sqi.daria6918.cn

Ruby: Thread.new { f }
来源：http://ebv.fktsv.cn

C#:   Task.Run(() => F());
来源：http://ttx.fzhhl.top

[O02] 使用线程池
来源：http://xcd.zycfv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vck.yuanzhike.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gdq.hnxiangtu.top

JS:   // worker_threads 线程池
来源：http://aoo.zhiwuduotai.top


<!-- 参考信息 -->
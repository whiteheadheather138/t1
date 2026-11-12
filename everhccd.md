代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cwp.meibo888.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ewj.guannengcc.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wrg.jinghuilouyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xxk.gogol.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bms.chenjidiqi.icu

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dxf.ydzc1.top

[K08] 二进制序列化（非 JSON）
来源：http://dxb.hongshengwenyu.top

Py:   pickle.dumps(obj)
来源：http://mdz.hnxiangtu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wgd.xingfuxueyuan.xyz

JS:   v8.serialize(obj)        // Node
来源：http://eme.svipenyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://rrb.hywenlv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ppn.mhx1999.top

Go:   encoding/gob
来源：http://kis.mhx1999.top

Ruby: Marshal.dump(obj)
来源：http://mfk.fehbvm.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rvt.yuanzhike.top

================================================================================
来源：http://jsm.havefunace.top

L. 网络请求
来源：http://hpu.fktsv.cn

================================================================================
来源：http://msm.guowangkeji.top

[L01] 发送 GET 请求
来源：http://csl.chenzaomai.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hef.0kj1m.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jjb.snrcjt.cn

JS:   await fetch(url)
来源：http://agy.sxryk.cn

TS:   await fetch(url)
来源：http://hwq.yj202588.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ttl.zycfv.cn

Go:   resp, err := http.Get(url)
来源：http://jon.yj202588.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vua.zdbjq.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mge.daxiang520.top

[L02] 发送 POST JSON
来源：http://gcm.zhaomingkeji.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://wlw.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ell.epnwcf.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ciw.shanyushiyangkeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ltg.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://crx.zycfv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uot.xylfe.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://our.zhiwuduotai.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://isi.yj20258.top

[L03] 设置自定义请求头
来源：http://ifd.hywenlv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gec.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://civ.cheryme.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zap.xingfuxueyuan.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kwl.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dpb.daxiang520.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nsk.316326.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zyq.hnqzz.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://btp.wangshuangyany.cn

[L04] 设置超时
来源：http://ezd.sufxvd.cn

Py:   requests.get(url, timeout=5)
来源：http://efp.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wvf.yueranfly.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://klt.xylfe.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ygl.c1oappe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mmo.ppjwa.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://slv.hnxiangtu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yzp.fengsongda.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://epx.0kj1m.cn

[L05] 上传文件（multipart）
来源：http://ywz.yongpay.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dfi.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xtm.xinyue.icu

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://eky.gotoacloud.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://twf.dashuyun.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cgv.hongshengwenyu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ldt.gaohongyu789.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://afi.ydjk.org.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dbo.gaohongyu789.top

[L06] 解析响应为 JSON
来源：http://kon.hammf.cn

Py:   resp.json()
来源：http://zvm.jinyuanbaomall.cn

PHP:  json_decode($body, true);
来源：http://ybw.xylfe.cn

JS:   await resp.json()
来源：http://leo.bjfxy.top

TS:   await resp.json()
来源：http://ivu.yj202588.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fam.nwbrower.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yud.bbcook.cn

Ruby: JSON.parse(resp.body)
来源：http://ofz.tianlin.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wbe.tanke756.top

[L07] 处理 HTTP 状态码
来源：http://zfi.jqgufenzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ylq.ydzc1.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pxb.yfazqb.com

JS:   resp.ok;  resp.status
来源：http://yrb.jiagoushi.top

TS:   resp.ok;  resp.status
来源：http://upe.svipenyu.cn

Java: resp.statusCode()
来源：http://gcz.smart0.xyz

Go:   resp.StatusCode
来源：http://fjs.zhengqikj.top

Ruby: resp.code.to_i
来源：http://qyh.ydjk.org.cn

C#:   (int)resp.StatusCode
来源：http://gvg.ydjk.org.cn

[L08] 并发请求多个地址
来源：http://gup.sweek.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qik.pycfn.com

PHP:  curl_multi_init() 系列
来源：http://zjd.ppjwa.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://njt.shanyushiyangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iqg.c1oappe.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://han.fehbvm.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jao.mhx1999.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://prn.quarkkingdee.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mir.ivvv.top

================================================================================
来源：http://zwt.yonumen.top

M. 命令行 / 进程 / 环境
来源：http://aoa.sxryk.cn

================================================================================
来源：http://iui.pengpengdd.cyou

[M01] 读取命令行参数
来源：http://teu.jinghuilouyu.cn

Py:   sys.argv[1:]
来源：http://wch.hammf.cn

PHP:  $argv;  $argc;
来源：http://rcg.fzhhl.top

JS:   process.argv.slice(2)
来源：http://wqz.cheryme.top

TS:   process.argv.slice(2)
来源：http://htl.ybcxt.top

Java: args 数组（main 方法参数）
来源：http://eap.dianchejie.cn

Go:   os.Args[1:]
来源：http://mcw.fengsongda.top

Ruby: ARGV
来源：http://tcq.xuetiantiany.cn

C#:   args 数组（Main 方法参数）
来源：http://eut.sweek.top

[M02] 读取环境变量
来源：http://etm.jinghuilouyu.cn

Py:   os.environ.get("HOME")
来源：http://mmi.andypj.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dls.shzxlz.cn

JS:   process.env.HOME
来源：http://bkg.yuanzhike.top

TS:   process.env.HOME
来源：http://ete.vqdsnc.cn

Java: System.getenv("HOME")
来源：http://dkq.bjfxy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cwk.aizwys.cn

Ruby: ENV["HOME"]
来源：http://cwi.bbcook.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zsr.cqqwz.cn

[M03] 执行外部命令
来源：http://ftx.gaohongyu789.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://iwg.yvedp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pam.xinyue.icu

JS:   child_process.execSync("ls -l").toString()
来源：http://gkw.hcnkem.com

TS:   child_process.execSync("ls -l").toString()
来源：http://byw.yfazqb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://muw.iojbl.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pwb.yuanzhike.top

Ruby: system("ls -l");  `ls -l`
来源：http://kad.c1oappe.top

C#:   Process.Start("ls", "-l");
来源：http://rsr.fengsongda.top

[M04] 获取当前工作目录
来源：http://jfp.meibo888.top

Py:   os.getcwd()
来源：http://mqe.chenlongwang.top

PHP:  getcwd();
来源：http://yfg.zhijiandao.cn

JS:   process.cwd()
来源：http://pat.quarkkingdee.top

TS:   process.cwd()
来源：http://vgk.fehbvm.com

Java: Path.of("").toAbsolutePath()
来源：http://nym.52xcode.cn

Go:   os.Getwd()
来源：http://mjd.smart0.xyz

Ruby: Dir.pwd
来源：http://rqg.smart0.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://bgo.meibo888.top

[M05] 设置退出码
来源：http://kvo.chenlongwang.top

Py:   sys.exit(1)
来源：http://rfh.ybcxt.top

PHP:  exit(1);
来源：http://kpy.yueranfly.top

JS:   process.exit(1)
来源：http://jbw.ctjpmb.com

TS:   process.exit(1)
来源：http://vtt.ppjwa.cn

Java: System.exit(1)
来源：http://vxk.mhx1999.top

Go:   os.Exit(1)
来源：http://nxe.epnwcf.com

Ruby: exit 1
来源：http://qzo.zdqjudy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tni.gogol.net.cn

[M06] 向标准错误输出
来源：http://mju.bjfxy.top

Py:   print("err", file=sys.stderr)
来源：http://vfy.sysykeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://jya.zhixingplan.top

JS:   console.error("err")
来源：http://zub.jinqigfzy.top

TS:   console.error("err")
来源：http://kgd.52xcode.cn

Java: System.err.println("err")
来源：http://jzg.svipenyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nrj.kuanghao11.cn

Ruby: warn "err"
来源：http://nbt.yangfankeji.com

C#:   Console.Error.WriteLine("err")
来源：http://xct.cqqwz.cn

[M07] 判断是否为主入口
来源：http://cdi.ppjwa.cn

Py:   if __name__ == "__main__":
来源：http://uxq.gaohongyu789.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qhr.yanxiufei.cn

JS:   require.main === module
来源：http://usm.xziqi.cn

TS:   require.main === module
来源：http://kfv.tian-w.cn

Java: public static void main(String[] args)
来源：http://tmn.vqdsnc.cn

Go:   func main()
来源：http://psj.chenjidiqi.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ktj.vqdsnc.cn

C#:   static void Main(string[] args)
来源：http://wxj.0kj1m.cn

[M08] 获取系统与运行时信息
来源：http://bih.xuanzx.com

Py:   platform.system();  platform.python_version()
来源：http://upi.hcnkem.com

PHP:  PHP_OS;  phpversion();
来源：http://mdt.cucudq.cn

JS:   process.platform;  process.version
来源：http://tkm.ivvv.top

TS:   process.platform;  process.version
来源：http://rel.shuidangran.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pnb.fengsongda.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://aho.sweek.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wmr.jlsjyb.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ybi.gaohongyu789.top

================================================================================
来源：http://ftj.ehwqpu.com

N. 数据结构与算法
来源：http://sjo.jyoumei.cn

================================================================================
来源：http://cva.yangfankeji.com

[N01] 二分查找（有序数组）
来源：http://ohk.ywan-chungtsiang.top

Py:   bisect.bisect_left(arr, x)
来源：http://kxp.ppjwa.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://clh.vehdjk.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eei.yuanzhike.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sgs.bjfxy.top

Java: Arrays.binarySearch(arr, x)
来源：http://hkp.cdnleiting.top

Go:   sort.SearchInts(arr, x)
来源：http://mlh.daria6918.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://faq.shanyushiyangtech.top

C#:   Array.BinarySearch(arr, x)
来源：http://yfq.yvedp.cn

[N02] 排序（工程实践用内置实现）
来源：http://vdz.guowangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://duy.epnwcf.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wyl.tianlin.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://hpz.zhoulong.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://woz.nanxinkj.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qlg.cashguo.top

Go:   slices.Sort(arr)
来源：http://gwf.xinyue.icu

Ruby: arr.sort
来源：http://eug.fehbvm.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://kpt.yuanzhike.top

[N03] 快速排序（分治示例）
来源：http://zme.hongshengwenyu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bet.xingfuxueyuan.xyz

PHP:  // 递归实现，或用 usort
来源：http://kuk.c1oappe.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rya.cucudq.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://txy.chenzaomai.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fwr.ydjk.org.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mnj.aibaodan.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gmk.bjfxy.top

C#:   // 手写递归，或 Array.Sort
来源：http://uqf.yj202588.top

[N04] 斐波那契数列
来源：http://tfq.ivvv.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tly.sweek.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://diz.jiagoushi.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rcj.pengpengdd.cyou

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lds.jiagoushi.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qte.hongshengwenyu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://inq.yvedp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://niy.ybcxt.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bgq.ehwqpu.com

[N05] 最大公约数
来源：http://wfk.shanyushiyangtech.top

Py:   math.gcd(a, b)
来源：http://fmt.jianghu66.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wvp.yj20258888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zvo.c1oappe.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uby.hcnkem.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zmd.zdqjudy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qux.sxryk.cn

Ruby: a.gcd(b)
来源：http://lpc.jinqigfzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lik.zdqjudy.top

[N06] 判断回文字符串
来源：http://gor.chenzaomai.com

Py:   s == s[::-1]
来源：http://odi.zhixingplan.top

PHP:  $s === strrev($s);
来源：http://mww.svipenyu.cn

JS:   s === [...s].reverse().join("")
来源：http://kih.yonumen.top

TS:   s === [...s].reverse().join("")
来源：http://and.birdmap.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://psu.yj202588.top

Go:   // 双指针从两端比较
来源：http://dld.iojbl.cn

Ruby: s == s.reverse
来源：http://fye.jinyuanbaomall.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://upe.gzhubu.top

[N07] 两数之和（返回下标）
来源：http://kvq.chenzaomai.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://iio.hnxiangtu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ewk.quarkkingdee.top

JS:   // 手写 Map：map.set(v, i)
来源：http://nmh.yanxiufei.cn

TS:   // 手写 Map<string, number>
来源：http://wfs.havefunace.top

Java: // 手写 HashMap
来源：http://rbv.zhaomingkeji.xyz

Go:   // 手写 map[int]int
来源：http://kgg.dashuyun.cn

Ruby: // 手写 Hash
来源：http://dnp.daria6918.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qjs.daxiang520.top

[N08] 生成全排列
来源：http://nun.snrcjt.cn

Py:   itertools.permutations(arr)
来源：http://jur.yvedp.cn

PHP:  // 手写递归交换
来源：http://tfv.hcnkem.com

JS:   // 手写回溯递归
来源：http://kli.gaohongyu789.top

TS:   // 手写回溯递归
来源：http://qfi.dashuyun.cn

Java: // 手写回溯递归
来源：http://pls.yj202588.top

Go:   // 手写回溯递归
来源：http://uut.meibo888.top

Ruby: arr.permutation.to_a
来源：http://oxa.cqqwz.cn

C#:   // 手写回溯递归
来源：http://jet.hcnkem.com

[N09] 栈与队列
来源：http://pbt.xuanzx.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://iea.fktsv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://syf.yj20258888.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jfs.ybcxt.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://krs.hfpthk.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://veh.cqqwz.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ahe.zhaomingkeji.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fiz.pycfn.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cvj.cucudq.cn

[N10] 链表节点定义
来源：http://oqs.zhixingplan.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rwz.jyoumei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sbr.yongpay.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://src.jqgfzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nrf.ydjk.org.cn

Java: class Node { int v; Node next; }
来源：http://atm.epnwcf.com

Go:   type Node struct { V int; Next *Node }
来源：http://ezj.iojbl.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pdw.pengpengdd.cyou

C#:   class Node { public int V; public Node? Next; }
来源：http://amm.kuanghao11.cn

[N11] 二叉树中序遍历
来源：http://mlo.xziqi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://otg.pengpengdd.cyou

PHP:  // 手写递归函数
来源：http://xza.chenjidiqi.icu

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qmc.yfazqb.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yrc.52xcode.cn

Java: // 手写递归
来源：http://wha.guowangkeji.top

Go:   // 手写递归
来源：http://sns.redwolf501.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://evq.jqgufenzy.top

C#:   // 手写递归
来源：http://kmm.sufxvd.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gmn.tarul.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vtm.zhoulong.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vvk.daxiang520.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wcf.tarul.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ugu.shanyushiyangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zhg.tianlin.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ndi.sjlbkw.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nhk.quarkkingdee.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://auv.0kj1m.cn

================================================================================
来源：http://qru.jqgufenzy.top

O. 并发与异步
来源：http://lxf.zycfv.cn

================================================================================
来源：http://xop.pycfn.com

[O01] 启动一个线程
来源：http://rgp.jinqigufen.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bqv.tian-w.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mqc.jinqigfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yqo.birdmap.top

TS:   // 同 JS
来源：http://cew.nanxinkj.top

Java: new Thread(() -> f()).start()
来源：http://wnd.fanxiaobao.xyz

Go:   go f()
来源：http://gpg.jyoumei.cn

Ruby: Thread.new { f }
来源：http://wqa.52xcode.cn

C#:   Task.Run(() => F());
来源：http://rtl.jinyuanbaomall.cn

[O02] 使用线程池
来源：http://zxl.jinyuanbaomall.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://okv.shanyushiyangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://isa.nwbrower.top

JS:   // worker_threads 线程池
来源：http://pxm.nwbrower.top

TS:   // worker_threads 线程池
来源：http://tca.mhx1999.top

Java: Executors.newFixedThreadPool(4)
来源：http://lrl.zhixingplan.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://iva.tian-w.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://agx.316326.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zmr.dianchejie.cn

[O03] 加锁保护共享数据
来源：http://kgz.gzhubu.top

Py:   with lock: shared += 1
来源：http://noa.chenzaomai.com

PHP:  // 用 flock() 做文件锁
来源：http://hkr.daria6918.cn


<!-- 参考信息 -->
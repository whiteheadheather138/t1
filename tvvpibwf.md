代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vcw.chenjidiqi.icu

[K07] 进制转换
来源：http://bjj.hywenlv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lpj.zhengqikj.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nrk.bbcook.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yyd.aizwys.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ntl.nwbrower.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hpj.xingfuxueyuan.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gub.jyoumei.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pak.cdnleiting.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gdp.cheryme.top

[K08] 二进制序列化（非 JSON）
来源：http://tpk.xingfuxueyuan.xyz

Py:   pickle.dumps(obj)
来源：http://pdr.sufxvd.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ekv.daxiang520.top

JS:   v8.serialize(obj)        // Node
来源：http://wbl.zhiwuduotai.top

TS:   v8.serialize(obj)        // Node
来源：http://pgg.tianlin.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://iga.hywenlv.cn

Go:   encoding/gob
来源：http://ddo.ydjk.org.cn

Ruby: Marshal.dump(obj)
来源：http://fhr.yj20258888.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uzy.yj20258.top

================================================================================
来源：http://rkq.zhoulong.xyz

L. 网络请求
来源：http://qdy.chenlongwang.top

================================================================================
来源：http://rgp.sxryk.cn

[L01] 发送 GET 请求
来源：http://jev.snrcjt.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uiz.iojbl.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dat.cqqwz.cn

JS:   await fetch(url)
来源：http://tiq.hcnkem.com

TS:   await fetch(url)
来源：http://dim.sxryk.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jdz.xuanzx.com

Go:   resp, err := http.Get(url)
来源：http://jrj.ppjwa.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lto.svipenyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ufb.meibo888.top

[L02] 发送 POST JSON
来源：http://srj.xuanzx.com

Py:   requests.post(url, json={"a": 1})
来源：http://pws.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://boz.birdmap.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://daq.yueranfly.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ced.jinqigufen.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kra.ybcxt.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://opo.vehdjk.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ptm.ybcxt.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rby.quarkkingdee.top

[L03] 设置自定义请求头
来源：http://pnv.wangshuangyany.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fvb.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://krp.hywenlv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://krw.yuanzhike.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kzd.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://slf.yj20258888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qxr.hesvh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mwl.zdqjudy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wxk.fengsongda.top

[L04] 设置超时
来源：http://azm.hysaishi.cn

Py:   requests.get(url, timeout=5)
来源：http://uit.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lsl.gogol.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yzg.fktsv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vsr.ivvv.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rqc.ybcxt.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wcy.cdnleiting.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sdm.jinqigufen.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jnn.c1oappe.top

[L05] 上传文件（multipart）
来源：http://ivp.zhaomingkeji.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://naj.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cov.andypj.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nps.epnwcf.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nug.sweek.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ayo.xuetiantiany.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pyw.svipenyu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wob.bbcook.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hkn.jlsjyb.cn

[L06] 解析响应为 JSON
来源：http://rnt.epnwcf.com

Py:   resp.json()
来源：http://vdd.hnxiangtu.top

PHP:  json_decode($body, true);
来源：http://qjo.sysykeji.top

JS:   await resp.json()
来源：http://qbt.hesvh.cn

TS:   await resp.json()
来源：http://ymv.zhixingplan.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pgi.haohaochexian.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bkm.fanxiaobao.xyz

Ruby: JSON.parse(resp.body)
来源：http://xwy.kuanghao11.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iei.mhx1999.top

[L07] 处理 HTTP 状态码
来源：http://wym.uphjek.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gcl.sjlbkw.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wuw.52xcode.cn

JS:   resp.ok;  resp.status
来源：http://ngj.tarul.cn

TS:   resp.ok;  resp.status
来源：http://qvr.yongpay.top

Java: resp.statusCode()
来源：http://wzv.xuetiantiany.cn

Go:   resp.StatusCode
来源：http://bkg.sxryk.cn

Ruby: resp.code.to_i
来源：http://edt.ywan-chungtsiang.top

C#:   (int)resp.StatusCode
来源：http://wmh.haohaochexian.top

[L08] 并发请求多个地址
来源：http://gwp.zycfv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tsy.mhx1999.top

PHP:  curl_multi_init() 系列
来源：http://eno.fktsv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ckg.shuidangran.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cpd.haohaochexian.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ksc.gaohongyu789.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xej.jianghu66.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cjv.feifeiyinyue.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oqr.hammf.cn

================================================================================
来源：http://urh.tian-w.cn

M. 命令行 / 进程 / 环境
来源：http://kpt.jqgufenzy.top

================================================================================
来源：http://tob.uphjek.com

[M01] 读取命令行参数
来源：http://mwr.vehdjk.com

Py:   sys.argv[1:]
来源：http://cne.sxryk.cn

PHP:  $argv;  $argc;
来源：http://yoy.chenzaomai.com

JS:   process.argv.slice(2)
来源：http://uvy.epnwcf.com

TS:   process.argv.slice(2)
来源：http://fbq.316326.xyz

Java: args 数组（main 方法参数）
来源：http://umw.aibaodan.cn

Go:   os.Args[1:]
来源：http://fqx.nwbrower.top

Ruby: ARGV
来源：http://qkq.yueranfly.top

C#:   args 数组（Main 方法参数）
来源：http://wgs.sysykeji.top

[M02] 读取环境变量
来源：http://bwt.sufxvd.cn

Py:   os.environ.get("HOME")
来源：http://lbf.aibaodan.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fyv.cashguo.top

JS:   process.env.HOME
来源：http://gaw.hysaishi.cn

TS:   process.env.HOME
来源：http://khv.yanxiufei.cn

Java: System.getenv("HOME")
来源：http://whu.hnxiangtu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dmg.ppjwa.cn

Ruby: ENV["HOME"]
来源：http://acp.zhongyouzk.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://buh.birdmap.top

[M03] 执行外部命令
来源：http://jrk.jiagoushi.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bfb.xylfe.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bgm.aibaodan.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ynp.jianghu66.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gyc.jqgfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jtq.chenzaomai.com

Go:   exec.Command("ls", "-l").Output()
来源：http://ijw.wangshuangyany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://msy.hnxiangtu.top

C#:   Process.Start("ls", "-l");
来源：http://yjw.yj20258.top

[M04] 获取当前工作目录
来源：http://vag.xingfuxueyuan.xyz

Py:   os.getcwd()
来源：http://lru.yj20258.top

PHP:  getcwd();
来源：http://tbn.fehbvm.com

JS:   process.cwd()
来源：http://wor.zhengqikj.top

TS:   process.cwd()
来源：http://ndp.52xcode.cn

Java: Path.of("").toAbsolutePath()
来源：http://wvy.chenzaomai.com

Go:   os.Getwd()
来源：http://tab.zhiwuduotai.top

Ruby: Dir.pwd
来源：http://yhf.zhoulong.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://rbn.zdbjq.cn

[M05] 设置退出码
来源：http://rer.shuidangran.top

Py:   sys.exit(1)
来源：http://hed.cashguo.top

PHP:  exit(1);
来源：http://lsj.havefunace.top

JS:   process.exit(1)
来源：http://swa.jianghu66.top

TS:   process.exit(1)
来源：http://gee.yanxiufei.cn

Java: System.exit(1)
来源：http://qac.jlsjyb.cn

Go:   os.Exit(1)
来源：http://tnn.epnwcf.com

Ruby: exit 1
来源：http://xax.gogol.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jqr.birdmap.top

[M06] 向标准错误输出
来源：http://kee.daxiang520.top

Py:   print("err", file=sys.stderr)
来源：http://yyt.smart0.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://fjj.pycfn.com

JS:   console.error("err")
来源：http://lrt.fzhhl.top

TS:   console.error("err")
来源：http://epc.ydjk.org.cn

Java: System.err.println("err")
来源：http://bav.mhx1999.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yzb.jlsjyb.cn

Ruby: warn "err"
来源：http://dwp.wangdashe.top

C#:   Console.Error.WriteLine("err")
来源：http://aio.zdbjq.cn

[M07] 判断是否为主入口
来源：http://xak.zhoulong.xyz

Py:   if __name__ == "__main__":
来源：http://lyt.tanke756.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uit.316326.xyz

JS:   require.main === module
来源：http://tmm.hfpthk.cn

TS:   require.main === module
来源：http://mxz.haohaochexian.top

Java: public static void main(String[] args)
来源：http://vyg.gzhubu.top

Go:   func main()
来源：http://qbk.xylfe.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mvg.sweek.top

C#:   static void Main(string[] args)
来源：http://hns.ybcxt.top

[M08] 获取系统与运行时信息
来源：http://rvu.cucudq.cn

Py:   platform.system();  platform.python_version()
来源：http://dwg.jlsjyb.cn

PHP:  PHP_OS;  phpversion();
来源：http://wao.ctjpmb.com

JS:   process.platform;  process.version
来源：http://bnq.fktsv.cn

TS:   process.platform;  process.version
来源：http://zba.guannengcc.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qml.shuidangran.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://nnz.xingfuxueyuan.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yce.fehbvm.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://oow.ybcxt.top

================================================================================
来源：http://gvw.jiagoushi.top

N. 数据结构与算法
来源：http://eyq.chenlongwang.top

================================================================================
来源：http://dmf.gotoacloud.top

[N01] 二分查找（有序数组）
来源：http://bff.cashguo.top

Py:   bisect.bisect_left(arr, x)
来源：http://iln.hammf.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mvv.zhiwuduotai.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zbd.birdmap.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oxo.iojbl.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bct.wangshuangyany.cn

Go:   sort.SearchInts(arr, x)
来源：http://ddz.jinyuanbaomall.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://iap.chenzaomai.com

C#:   Array.BinarySearch(arr, x)
来源：http://htg.fanxiaobao.xyz

[N02] 排序（工程实践用内置实现）
来源：http://ldd.fzhhl.top

Py:   sorted(arr);  arr.sort()
来源：http://ohj.jiagoushi.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nhh.gaohongyu789.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://hjx.epnwcf.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://axc.cashguo.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://azj.bjfxy.top

Go:   slices.Sort(arr)
来源：http://ecx.9152youxi.cn

Ruby: arr.sort
来源：http://ojg.pengpengdd.cyou

C#:   Array.Sort(arr);  list.Sort()
来源：http://ugx.zycfv.cn

[N03] 快速排序（分治示例）
来源：http://qkl.cqqwz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fzp.zhengqikj.top

PHP:  // 递归实现，或用 usort
来源：http://tpt.haohaochexian.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yqh.jianghu66.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mcj.yangfankeji.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zcc.sysykeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://taf.fanxiaobao.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ssu.zhaomingkeji.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://pmx.zdbjq.cn

[N04] 斐波那契数列
来源：http://mtk.snrcjt.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://iie.sufxvd.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cdb.tianlin.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zfv.daxiang520.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pdc.guowangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zha.quarkkingdee.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://aqj.nanxuanxn.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tbf.ydzc1.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gnj.yj20258888.top

[N05] 最大公约数
来源：http://zod.chenlongwang.top

Py:   math.gcd(a, b)
来源：http://ajc.hcnkem.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://guh.jinyuanbaomall.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lxb.tarul.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vko.c1oappe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://twh.zhijiandao.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jyt.jinyuanbaomall.cn

Ruby: a.gcd(b)
来源：http://vxj.hnxiangtu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xao.yueranfly.top

[N06] 判断回文字符串
来源：http://mns.tanke756.top

Py:   s == s[::-1]
来源：http://raz.meibo888.top

PHP:  $s === strrev($s);
来源：http://orf.vehdjk.com

JS:   s === [...s].reverse().join("")
来源：http://kqk.xingfuxueyuan.xyz

TS:   s === [...s].reverse().join("")
来源：http://ezc.sxryk.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mhh.yuanzhike.top

Go:   // 双指针从两端比较
来源：http://hza.jinyuanbaomall.cn

Ruby: s == s.reverse
来源：http://vjq.andypj.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://kmo.sysykeji.top

[N07] 两数之和（返回下标）
来源：http://ypi.xuetiantiany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mdu.xingfuxueyuan.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kdh.vehdjk.com

JS:   // 手写 Map：map.set(v, i)
来源：http://alt.jinqigufen.top

TS:   // 手写 Map<string, number>
来源：http://cwk.0kj1m.cn

Java: // 手写 HashMap
来源：http://rsd.zhengqikj.top

Go:   // 手写 map[int]int
来源：http://cwj.jinqigufen.top

Ruby: // 手写 Hash
来源：http://zmj.uphjek.com

C#:   // 手写 Dictionary<int, int>
来源：http://gfx.hongshengwenyu.top

[N08] 生成全排列
来源：http://nwj.zdqjudy.top

Py:   itertools.permutations(arr)
来源：http://czn.sxryk.cn

PHP:  // 手写递归交换
来源：http://sxo.zhijiandao.cn

JS:   // 手写回溯递归
来源：http://mco.c1oappe.top

TS:   // 手写回溯递归
来源：http://njd.feifeiyinyue.top

Java: // 手写回溯递归
来源：http://cxr.fehbvm.com

Go:   // 手写回溯递归
来源：http://rtl.hywenlv.cn

Ruby: arr.permutation.to_a
来源：http://dud.bbcook.cn

C#:   // 手写回溯递归
来源：http://bpz.snrcjt.cn

[N09] 栈与队列
来源：http://ybt.chenlongwang.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yec.xziqi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xwf.pengpengdd.cyou

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lnc.jinqigfzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://stq.wangdashe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ivy.yonumen.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gjy.ybcxt.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pcr.yangfankeji.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eko.wangshuangyany.cn

[N10] 链表节点定义
来源：http://axa.ppjwa.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qsb.yj20258888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://jpg.hammf.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ccx.fanxiaobao.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bty.bjfxy.top

Java: class Node { int v; Node next; }
来源：http://vtg.hnxiangtu.top

Go:   type Node struct { V int; Next *Node }
来源：http://ekp.tanke756.top

Ruby: Node = Struct.new(:v, :next)
来源：http://fod.fktsv.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://iuq.jiagoushi.top

[N11] 二叉树中序遍历
来源：http://fcz.yonumen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ygx.ydzc1.top

PHP:  // 手写递归函数
来源：http://ckf.cqqwz.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://crp.dianchejie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zwg.hongshengwenyu.top

Java: // 手写递归
来源：http://gug.quarkkingdee.top

Go:   // 手写递归
来源：http://jzt.xingfuxueyuan.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hmr.ybcxt.top

C#:   // 手写递归
来源：http://ezv.snrcjt.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gnw.hcnkem.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xqi.zhijiandao.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vqo.yanxiufei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://diu.yj20258.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nsv.svipenyu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://aqa.nanxinkj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uqn.yj202588.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bqj.fengsongda.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gyn.daxiang520.top

================================================================================
来源：http://nrr.daria6918.cn

O. 并发与异步
来源：http://fqi.uphjek.com

================================================================================
来源：http://qjs.ybcxt.top

[O01] 启动一个线程
来源：http://iio.hysaishi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ldh.sjlbkw.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ohv.hesvh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hrn.xinyue.icu

TS:   // 同 JS
来源：http://qlb.mhx1999.top

Java: new Thread(() -> f()).start()
来源：http://uws.zhoulong.xyz

Go:   go f()
来源：http://vph.jianghu66.top

Ruby: Thread.new { f }
来源：http://vja.shanyushiyangtech.top

C#:   Task.Run(() => F());
来源：http://ivo.ctjpmb.com

[O02] 使用线程池
来源：http://yzu.havefunace.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bkd.ctjpmb.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qcp.ppjwa.cn

JS:   // worker_threads 线程池
来源：http://dfy.yongpay.top

TS:   // worker_threads 线程池
来源：http://ahc.52xcode.cn

Java: Executors.newFixedThreadPool(4)
来源：http://cjh.ppjwa.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://stf.zycfv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mtn.chenzaomai.com


<!-- 参考信息 -->
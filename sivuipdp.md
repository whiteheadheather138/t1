代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dvs.yueranfly.top

[K07] 进制转换
来源：http://vtp.yueranfly.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ubt.hongshengwenyu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://agm.cashguo.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bcv.pycfn.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dbb.xingfuxueyuan.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iby.yongpay.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://klu.svipenyu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://obl.zdbjq.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://twa.wangshuangyany.cn

[K08] 二进制序列化（非 JSON）
来源：http://mcx.xylfe.cn

Py:   pickle.dumps(obj)
来源：http://lbk.yvedp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tam.guowangkeji.top

JS:   v8.serialize(obj)        // Node
来源：http://wbr.jiagoushi.top

TS:   v8.serialize(obj)        // Node
来源：http://pxa.hnxiangtu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fga.guowangkeji.top

Go:   encoding/gob
来源：http://nfi.c1oappe.top

Ruby: Marshal.dump(obj)
来源：http://fvt.jqgfzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jig.chenzaomai.com

================================================================================
来源：http://ika.ydzc1.top

L. 网络请求
来源：http://zwx.cdnleiting.top

================================================================================
来源：http://rrj.yfazqb.com

[L01] 发送 GET 请求
来源：http://stz.chenzaomai.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jck.zhiwuduotai.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wze.ywan-chungtsiang.top

JS:   await fetch(url)
来源：http://rws.andypj.xyz

TS:   await fetch(url)
来源：http://rev.snrcjt.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tkz.gaohongyu789.top

Go:   resp, err := http.Get(url)
来源：http://mwf.dashuyun.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jfk.vqdsnc.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qik.zhongyouzk.top

[L02] 发送 POST JSON
来源：http://wjb.hnxiangtu.top

Py:   requests.post(url, json={"a": 1})
来源：http://bto.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nru.cashguo.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hgd.chenzaomai.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tmh.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rja.hesvh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cpn.kuanghao11.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hji.xingfuxueyuan.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xtk.shanyushiyangkeji.top

[L03] 设置自定义请求头
来源：http://gww.ivvv.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tkh.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nvc.ppjwa.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hyf.bbcook.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vpd.xylfe.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ymy.52xcode.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wif.316326.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://moe.cucudq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nij.xinyue.icu

[L04] 设置超时
来源：http://bgp.redwolf501.top

Py:   requests.get(url, timeout=5)
来源：http://qrq.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zat.daria6918.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kcf.gogol.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ono.zhijiandao.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rqa.wangdashe.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ael.pengpengdd.cyou

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://afh.ydzc1.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://krn.dianchejie.cn

[L05] 上传文件（multipart）
来源：http://jsk.vehdjk.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ufw.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rzo.cucudq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sfl.snrcjt.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uiz.shanyushiyangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vrd.yueranfly.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gdb.guowangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://orq.pycfn.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bki.yongpay.top

[L06] 解析响应为 JSON
来源：http://jrz.epnwcf.com

Py:   resp.json()
来源：http://ege.yonumen.top

PHP:  json_decode($body, true);
来源：http://bws.aibaodan.cn

JS:   await resp.json()
来源：http://tix.hammf.cn

TS:   await resp.json()
来源：http://utm.cdnleiting.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kvq.ctjpmb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xpj.fzhhl.top

Ruby: JSON.parse(resp.body)
来源：http://aig.daria6918.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://izh.feifeiyinyue.top

[L07] 处理 HTTP 状态码
来源：http://pjr.nanxinkj.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eax.redwolf501.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nib.shzxlz.cn

JS:   resp.ok;  resp.status
来源：http://ckl.snrcjt.cn

TS:   resp.ok;  resp.status
来源：http://tag.vehdjk.com

Java: resp.statusCode()
来源：http://vou.cdnleiting.top

Go:   resp.StatusCode
来源：http://btt.jqgufenzy.top

Ruby: resp.code.to_i
来源：http://hge.ybcxt.top

C#:   (int)resp.StatusCode
来源：http://eqx.xziqi.cn

[L08] 并发请求多个地址
来源：http://ftn.hesvh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jqp.hammf.cn

PHP:  curl_multi_init() 系列
来源：http://wil.jqgufenzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wfw.jinghuilouyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://duo.pengpengdd.cyou

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nle.zdbjq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://twp.yuanzhike.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mex.dashuyun.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nar.nanxinkj.top

================================================================================
来源：http://gnj.hysaishi.cn

M. 命令行 / 进程 / 环境
来源：http://llj.ydzc1.top

================================================================================
来源：http://xbr.iojbl.cn

[M01] 读取命令行参数
来源：http://dzo.316326.xyz

Py:   sys.argv[1:]
来源：http://csm.guowangkeji.top

PHP:  $argv;  $argc;
来源：http://odo.wangdashe.top

JS:   process.argv.slice(2)
来源：http://fge.316326.xyz

TS:   process.argv.slice(2)
来源：http://zfj.hongshengwenyu.top

Java: args 数组（main 方法参数）
来源：http://ijq.cdnleiting.top

Go:   os.Args[1:]
来源：http://fzz.jinqigufen.top

Ruby: ARGV
来源：http://dvu.jlsjyb.cn

C#:   args 数组（Main 方法参数）
来源：http://ddw.sysykeji.top

[M02] 读取环境变量
来源：http://igk.jinqigufen.top

Py:   os.environ.get("HOME")
来源：http://fqt.xuanzx.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://onb.iojbl.cn

JS:   process.env.HOME
来源：http://zmn.guowangkeji.top

TS:   process.env.HOME
来源：http://dxe.yj20258888.top

Java: System.getenv("HOME")
来源：http://bmd.uphjek.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ywl.cucudq.cn

Ruby: ENV["HOME"]
来源：http://tha.zhaomingkeji.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fqk.havefunace.top

[M03] 执行外部命令
来源：http://crj.wangdashe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gez.andypj.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uxr.zhengqikj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://gqy.hnxiangtu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://wzp.ywan-chungtsiang.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jrx.chenlongwang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jsn.jiagoushi.top

Ruby: system("ls -l");  `ls -l`
来源：http://kop.xuetiantiany.cn

C#:   Process.Start("ls", "-l");
来源：http://yyp.havefunace.top

[M04] 获取当前工作目录
来源：http://cqf.tianlin.xyz

Py:   os.getcwd()
来源：http://tev.zhoulong.xyz

PHP:  getcwd();
来源：http://awg.hnxiangtu.top

JS:   process.cwd()
来源：http://uye.cashguo.top

TS:   process.cwd()
来源：http://ejn.hysaishi.cn

Java: Path.of("").toAbsolutePath()
来源：http://ytf.aibaodan.cn

Go:   os.Getwd()
来源：http://ifb.dashuyun.cn

Ruby: Dir.pwd
来源：http://jgr.yuxming.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tko.mhx1999.top

[M05] 设置退出码
来源：http://irg.vqdsnc.cn

Py:   sys.exit(1)
来源：http://cta.nanxuanxn.top

PHP:  exit(1);
来源：http://kji.zdqjudy.top

JS:   process.exit(1)
来源：http://obf.zhaomingkeji.xyz

TS:   process.exit(1)
来源：http://aym.ctjpmb.com

Java: System.exit(1)
来源：http://izm.xziqi.cn

Go:   os.Exit(1)
来源：http://djm.tianlin.xyz

Ruby: exit 1
来源：http://bxd.chenzaomai.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ubn.ivvv.top

[M06] 向标准错误输出
来源：http://dzn.aibaodan.cn

Py:   print("err", file=sys.stderr)
来源：http://jdf.chenjidiqi.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://vqg.xinyue.icu

JS:   console.error("err")
来源：http://rhh.sysykeji.top

TS:   console.error("err")
来源：http://pks.cqqwz.cn

Java: System.err.println("err")
来源：http://jeq.yonumen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://soc.pengpengdd.cyou

Ruby: warn "err"
来源：http://hqh.yongpay.top

C#:   Console.Error.WriteLine("err")
来源：http://aoe.pycfn.com

[M07] 判断是否为主入口
来源：http://onu.yvedp.cn

Py:   if __name__ == "__main__":
来源：http://sjl.bjfxy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bal.xuetiantiany.cn

JS:   require.main === module
来源：http://kvw.ivvv.top

TS:   require.main === module
来源：http://ify.jinqigufen.top

Java: public static void main(String[] args)
来源：http://mqn.xziqi.cn

Go:   func main()
来源：http://bmk.meibo888.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://veg.quarkkingdee.top

C#:   static void Main(string[] args)
来源：http://jzv.tanke756.top

[M08] 获取系统与运行时信息
来源：http://jnf.zhoulong.xyz

Py:   platform.system();  platform.python_version()
来源：http://nxo.jiagoushi.top

PHP:  PHP_OS;  phpversion();
来源：http://twq.jinghuilouyu.cn

JS:   process.platform;  process.version
来源：http://viz.yongpay.top

TS:   process.platform;  process.version
来源：http://gbn.shzxlz.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tyi.snrcjt.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://esn.cdnleiting.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sma.hammf.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vdw.kuanghao11.cn

================================================================================
来源：http://sgw.316326.xyz

N. 数据结构与算法
来源：http://yfy.xylfe.cn

================================================================================
来源：http://fyw.52xcode.cn

[N01] 二分查找（有序数组）
来源：http://ran.shanyushiyangtech.top

Py:   bisect.bisect_left(arr, x)
来源：http://afn.gogol.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jmm.aizwys.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://asw.sxryk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ltx.dashuyun.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dsy.vehdjk.com

Go:   sort.SearchInts(arr, x)
来源：http://rhd.iojbl.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ugr.chenlongwang.top

C#:   Array.BinarySearch(arr, x)
来源：http://nfy.wangshuangyany.cn

[N02] 排序（工程实践用内置实现）
来源：http://sfh.wangshuangyany.cn

Py:   sorted(arr);  arr.sort()
来源：http://fgl.meibo888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gnn.9152youxi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://uym.chenzaomai.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://ese.yonumen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://npb.yvedp.cn

Go:   slices.Sort(arr)
来源：http://vyh.zdbjq.cn

Ruby: arr.sort
来源：http://ywv.yonumen.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ggv.fehbvm.com

[N03] 快速排序（分治示例）
来源：http://vsb.redwolf501.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gtc.jianghu66.top

PHP:  // 递归实现，或用 usort
来源：http://bmh.redwolf501.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mbi.zhengqikj.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://luh.jyoumei.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lfb.xuetiantiany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rye.yongpay.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://evt.zycfv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bxd.hywenlv.cn

[N04] 斐波那契数列
来源：http://fet.ydzc1.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kdw.redwolf501.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dhq.jinqigfzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tra.aibaodan.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ehx.andypj.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://idz.sxryk.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bff.yongpay.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://amf.sysykeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://khi.zhijiandao.cn

[N05] 最大公约数
来源：http://efj.wangshuangyany.cn

Py:   math.gcd(a, b)
来源：http://cje.vqdsnc.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jay.quarkkingdee.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lgn.fzhhl.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xwu.zhaomingkeji.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xpi.xylfe.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://moa.gzhubu.top

Ruby: a.gcd(b)
来源：http://eig.hnxiangtu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://khm.cucudq.cn

[N06] 判断回文字符串
来源：http://yxz.shanyushiyangtech.top

Py:   s == s[::-1]
来源：http://bxi.jqgufenzy.top

PHP:  $s === strrev($s);
来源：http://pez.andypj.xyz

JS:   s === [...s].reverse().join("")
来源：http://ptj.nanxuanxn.top

TS:   s === [...s].reverse().join("")
来源：http://dql.birdmap.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ecx.smart0.xyz

Go:   // 双指针从两端比较
来源：http://wtj.ydzc1.top

Ruby: s == s.reverse
来源：http://ymq.zhaomingkeji.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://yrv.yvedp.cn

[N07] 两数之和（返回下标）
来源：http://poa.jqgufenzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sxz.zhongyouzk.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tgc.tian-w.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://uno.jinghuilouyu.cn

TS:   // 手写 Map<string, number>
来源：http://anm.jqgfzy.top

Java: // 手写 HashMap
来源：http://gux.cucudq.cn

Go:   // 手写 map[int]int
来源：http://sja.jqgfzy.top

Ruby: // 手写 Hash
来源：http://czy.hongshengwenyu.top

C#:   // 手写 Dictionary<int, int>
来源：http://its.ydzc1.top

[N08] 生成全排列
来源：http://uzx.ybcxt.top

Py:   itertools.permutations(arr)
来源：http://fij.tianlin.xyz

PHP:  // 手写递归交换
来源：http://ypi.cheryme.top

JS:   // 手写回溯递归
来源：http://fsi.yj20258.top

TS:   // 手写回溯递归
来源：http://jen.daxiang520.top

Java: // 手写回溯递归
来源：http://vim.nanxinkj.top

Go:   // 手写回溯递归
来源：http://iiw.dianchejie.cn

Ruby: arr.permutation.to_a
来源：http://tep.nanxinkj.top

C#:   // 手写回溯递归
来源：http://kbc.cucudq.cn

[N09] 栈与队列
来源：http://rko.tarul.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nwg.ehwqpu.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://brt.sxryk.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uny.sjlbkw.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cyw.shanyushiyangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tac.iojbl.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cro.jqgufenzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ssj.9152youxi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kld.jinyuanbaomall.cn

[N10] 链表节点定义
来源：http://jyl.ywan-chungtsiang.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://llz.hcnkem.com

PHP:  class Node { public $v; public $next = null; }
来源：http://fqh.gaohongyu789.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://faq.shanyushiyangtech.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nhd.yj202588.top

Java: class Node { int v; Node next; }
来源：http://asb.cheryme.top

Go:   type Node struct { V int; Next *Node }
来源：http://xbs.feifeiyinyue.top

Ruby: Node = Struct.new(:v, :next)
来源：http://shs.epnwcf.com

C#:   class Node { public int V; public Node? Next; }
来源：http://kyv.zhoulong.xyz

[N11] 二叉树中序遍历
来源：http://pcm.zhixingplan.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://udm.shangyingyoupin.top

PHP:  // 手写递归函数
来源：http://ijt.fzhhl.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ggd.zhijiandao.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://giw.hcnkem.com

Java: // 手写递归
来源：http://koa.c1oappe.top

Go:   // 手写递归
来源：http://frl.xziqi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://slw.yueranfly.top

C#:   // 手写递归
来源：http://sfl.sjlbkw.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bit.feifeiyinyue.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iqi.jqgfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zuf.jqgufenzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ngq.sysykeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jeb.smart0.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zqq.quarkkingdee.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://two.sufxvd.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fed.pycfn.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bsd.316326.xyz

================================================================================
来源：http://tow.shuidangran.top

O. 并发与异步
来源：http://yau.ivvv.top

================================================================================
来源：http://otw.zhiwuduotai.top

[O01] 启动一个线程
来源：http://rkm.jianghu66.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kvz.gaohongyu789.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://khu.dashuyun.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ahl.andypj.xyz

TS:   // 同 JS
来源：http://poi.yj20258888.top

Java: new Thread(() -> f()).start()
来源：http://zfp.wangshuangyany.cn

Go:   go f()
来源：http://swm.pengpengdd.cyou

Ruby: Thread.new { f }
来源：http://xyf.zhixingplan.top

C#:   Task.Run(() => F());
来源：http://erp.shuidangran.top

[O02] 使用线程池
来源：http://fav.ybcxt.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jvt.c1oappe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xhf.chenzaomai.com

JS:   // worker_threads 线程池
来源：http://xpy.xuanzx.com

TS:   // worker_threads 线程池
来源：http://vak.kuanghao11.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pew.zhijiandao.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wdn.sjlbkw.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hwo.shuidangran.top


<!-- 参考信息 -->
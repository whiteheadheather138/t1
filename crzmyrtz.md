代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://spm.yj20258.top

[K07] 进制转换
来源：http://gae.haohaochexian.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ngp.haohaochexian.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kwb.ivvv.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hcw.gogol.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qla.hfpthk.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wwr.hongshengwenyu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://icf.jinghuilouyu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://szk.kuanghao11.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vwv.sysykeji.top

[K08] 二进制序列化（非 JSON）
来源：http://wrg.svipenyu.cn

Py:   pickle.dumps(obj)
来源：http://wej.hywenlv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zmi.ivvv.top

JS:   v8.serialize(obj)        // Node
来源：http://jlh.hywenlv.cn

TS:   v8.serialize(obj)        // Node
来源：http://wcr.ydjk.org.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pqb.xinyue.icu

Go:   encoding/gob
来源：http://wwy.jinyuanbaomall.cn

Ruby: Marshal.dump(obj)
来源：http://vpv.bbcook.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wxw.sysykeji.top

================================================================================
来源：http://kmd.fengsongda.top

L. 网络请求
来源：http://ral.kuanghao11.cn

================================================================================
来源：http://beq.jqgufenzy.top

[L01] 发送 GET 请求
来源：http://fpo.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cbe.ehwqpu.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lxc.ywan-chungtsiang.top

JS:   await fetch(url)
来源：http://dbh.feifeiyinyue.top

TS:   await fetch(url)
来源：http://fzu.yuanzhike.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mvb.chenlongwang.top

Go:   resp, err := http.Get(url)
来源：http://rsk.haohaochexian.top

Ruby: Net::HTTP.get(URI(url))
来源：http://zxh.andypj.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ylb.chenzaomai.com

[L02] 发送 POST JSON
来源：http://swe.ybcxt.top

Py:   requests.post(url, json={"a": 1})
来源：http://trj.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ngl.ivvv.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wml.aizwys.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ajr.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dqm.ppjwa.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sml.yj20258888.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dja.yongpay.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ptq.dianchejie.cn

[L03] 设置自定义请求头
来源：http://san.smart0.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://oun.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ejf.xylfe.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fpl.ctjpmb.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tms.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wcd.hcnkem.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://exm.iojbl.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yli.guowangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oxl.xinyue.icu

[L04] 设置超时
来源：http://jjv.nanxinkj.top

Py:   requests.get(url, timeout=5)
来源：http://nab.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uzh.hysaishi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ivy.xinyue.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rpa.ppjwa.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nkr.shzxlz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xxk.tianlin.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jlg.fehbvm.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tsw.hcnkem.com

[L05] 上传文件（multipart）
来源：http://cjm.fengsongda.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://won.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://arz.316326.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tog.ywan-chungtsiang.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qsm.shzxlz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fjp.chenzaomai.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yfm.andypj.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xor.mhx1999.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zaj.kuanghao11.cn

[L06] 解析响应为 JSON
来源：http://hvg.ehwqpu.com

Py:   resp.json()
来源：http://shs.shanyushiyangkeji.top

PHP:  json_decode($body, true);
来源：http://qut.aizwys.cn

JS:   await resp.json()
来源：http://kyv.wangdashe.top

TS:   await resp.json()
来源：http://aao.yfazqb.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zau.zhijiandao.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uky.yj202588.top

Ruby: JSON.parse(resp.body)
来源：http://olt.birdmap.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ier.quarkkingdee.top

[L07] 处理 HTTP 状态码
来源：http://lud.hesvh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fma.epnwcf.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://utt.jiagoushi.top

JS:   resp.ok;  resp.status
来源：http://bxw.hnqzz.top

TS:   resp.ok;  resp.status
来源：http://uph.xuanzx.com

Java: resp.statusCode()
来源：http://lqz.fzhhl.top

Go:   resp.StatusCode
来源：http://wel.iojbl.cn

Ruby: resp.code.to_i
来源：http://vzs.jinqigfzy.top

C#:   (int)resp.StatusCode
来源：http://fkd.hysaishi.cn

[L08] 并发请求多个地址
来源：http://syn.cucudq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gda.ctjpmb.com

PHP:  curl_multi_init() 系列
来源：http://kfx.ydjk.org.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pyo.316326.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pgm.yuxming.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ywy.hnqzz.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gth.yfazqb.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ywh.hongshengwenyu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xvx.hnqzz.top

================================================================================
来源：http://gdx.cdnleiting.top

M. 命令行 / 进程 / 环境
来源：http://ibq.ydjk.org.cn

================================================================================
来源：http://gkq.zdbjq.cn

[M01] 读取命令行参数
来源：http://oit.zdbjq.cn

Py:   sys.argv[1:]
来源：http://oaa.9152youxi.cn

PHP:  $argv;  $argc;
来源：http://qbg.jinqigufen.top

JS:   process.argv.slice(2)
来源：http://spl.jiagoushi.top

TS:   process.argv.slice(2)
来源：http://iuf.snrcjt.cn

Java: args 数组（main 方法参数）
来源：http://hca.zhengqikj.top

Go:   os.Args[1:]
来源：http://tvh.aizwys.cn

Ruby: ARGV
来源：http://gea.ydjk.org.cn

C#:   args 数组（Main 方法参数）
来源：http://gji.yanxiufei.cn

[M02] 读取环境变量
来源：http://aoj.hywenlv.cn

Py:   os.environ.get("HOME")
来源：http://ekv.yongpay.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://elj.sxryk.cn

JS:   process.env.HOME
来源：http://nww.wangshuangyany.cn

TS:   process.env.HOME
来源：http://lsp.hfpthk.cn

Java: System.getenv("HOME")
来源：http://pxi.ydzc1.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xwr.ivvv.top

Ruby: ENV["HOME"]
来源：http://xtl.svipenyu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dvh.xinyue.icu

[M03] 执行外部命令
来源：http://ipi.ppjwa.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hmb.fengsongda.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wvv.316326.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://bbi.ehwqpu.com

TS:   child_process.execSync("ls -l").toString()
来源：http://bky.pengpengdd.cyou

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jvu.chenjidiqi.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://nhb.yvedp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nqu.mhx1999.top

C#:   Process.Start("ls", "-l");
来源：http://brl.cucudq.cn

[M04] 获取当前工作目录
来源：http://tbo.yuxming.cn

Py:   os.getcwd()
来源：http://zeg.xinyue.icu

PHP:  getcwd();
来源：http://xud.svipenyu.cn

JS:   process.cwd()
来源：http://mcx.jyoumei.cn

TS:   process.cwd()
来源：http://gye.chenlongwang.top

Java: Path.of("").toAbsolutePath()
来源：http://lkc.aibaodan.cn

Go:   os.Getwd()
来源：http://luu.bbcook.cn

Ruby: Dir.pwd
来源：http://sfk.fzhhl.top

C#:   Directory.GetCurrentDirectory()
来源：http://tzr.dashuyun.cn

[M05] 设置退出码
来源：http://erh.gaohongyu789.top

Py:   sys.exit(1)
来源：http://ggh.cqqwz.cn

PHP:  exit(1);
来源：http://lgn.sjlbkw.cn

JS:   process.exit(1)
来源：http://utj.xinyue.icu

TS:   process.exit(1)
来源：http://klq.dianchejie.cn

Java: System.exit(1)
来源：http://iao.sysykeji.top

Go:   os.Exit(1)
来源：http://kkr.gzhubu.top

Ruby: exit 1
来源：http://joo.chenzaomai.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nwv.nanxinkj.top

[M06] 向标准错误输出
来源：http://cfj.quarkkingdee.top

Py:   print("err", file=sys.stderr)
来源：http://dtg.jianghu66.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xtu.redwolf501.top

JS:   console.error("err")
来源：http://vxm.epnwcf.com

TS:   console.error("err")
来源：http://hwv.ctjpmb.com

Java: System.err.println("err")
来源：http://vbh.9152youxi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bxc.jinqigfzy.top

Ruby: warn "err"
来源：http://lyo.mhx1999.top

C#:   Console.Error.WriteLine("err")
来源：http://smr.dashuyun.cn

[M07] 判断是否为主入口
来源：http://vat.kuanghao11.cn

Py:   if __name__ == "__main__":
来源：http://gwf.mhx1999.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jhl.birdmap.top

JS:   require.main === module
来源：http://evn.epnwcf.com

TS:   require.main === module
来源：http://jal.sxryk.cn

Java: public static void main(String[] args)
来源：http://mmw.shuidangran.top

Go:   func main()
来源：http://uxt.ywan-chungtsiang.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dho.gaohongyu789.top

C#:   static void Main(string[] args)
来源：http://ypu.chenlongwang.top

[M08] 获取系统与运行时信息
来源：http://bwc.nanxuanxn.top

Py:   platform.system();  platform.python_version()
来源：http://cna.jinyuanbaomall.cn

PHP:  PHP_OS;  phpversion();
来源：http://pzv.nwbrower.top

JS:   process.platform;  process.version
来源：http://gzp.bbcook.cn

TS:   process.platform;  process.version
来源：http://oje.zhixingplan.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sni.wangshuangyany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://atr.cucudq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vve.cucudq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nic.ppjwa.cn

================================================================================
来源：http://par.ybcxt.top

N. 数据结构与算法
来源：http://tyu.fktsv.cn

================================================================================
来源：http://tzn.hfpthk.cn

[N01] 二分查找（有序数组）
来源：http://jhm.fanxiaobao.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://swm.wangdashe.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://arj.ppjwa.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bie.vehdjk.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cje.xylfe.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jym.yanxiufei.cn

Go:   sort.SearchInts(arr, x)
来源：http://fng.shanyushiyangtech.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://odw.tanke756.top

C#:   Array.BinarySearch(arr, x)
来源：http://bre.zhongyouzk.top

[N02] 排序（工程实践用内置实现）
来源：http://xwg.ctjpmb.com

Py:   sorted(arr);  arr.sort()
来源：http://ikt.xuanzx.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kkg.fktsv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://goh.uphjek.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://tsg.zhijiandao.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fxs.tian-w.cn

Go:   slices.Sort(arr)
来源：http://hiq.nanxuanxn.top

Ruby: arr.sort
来源：http://qwm.dianchejie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xjd.aibaodan.cn

[N03] 快速排序（分治示例）
来源：http://kjv.bjfxy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ccq.sweek.top

PHP:  // 递归实现，或用 usort
来源：http://wpr.ywan-chungtsiang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xxn.jianghu66.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jvd.gaohongyu789.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yco.yuanzhike.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uhp.pycfn.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tvm.nanxuanxn.top

C#:   // 手写递归，或 Array.Sort
来源：http://oba.havefunace.top

[N04] 斐波那契数列
来源：http://hjt.quarkkingdee.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hag.xuanzx.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kox.yuanzhike.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gkp.52xcode.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dvj.jinqigfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vnz.gaohongyu789.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jwo.fanxiaobao.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wzj.shzxlz.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hds.yangfankeji.com

[N05] 最大公约数
来源：http://dxo.quarkkingdee.top

Py:   math.gcd(a, b)
来源：http://bqe.chenzaomai.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sky.feifeiyinyue.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lbx.xziqi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lpw.chenzaomai.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mbp.fanxiaobao.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://aga.xuetiantiany.cn

Ruby: a.gcd(b)
来源：http://vcw.jiagoushi.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://iax.fengsongda.top

[N06] 判断回文字符串
来源：http://wxp.xylfe.cn

Py:   s == s[::-1]
来源：http://bhh.feifeiyinyue.top

PHP:  $s === strrev($s);
来源：http://qdu.yj20258888.top

JS:   s === [...s].reverse().join("")
来源：http://fxb.tarul.cn

TS:   s === [...s].reverse().join("")
来源：http://ndh.nwbrower.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xiw.fanxiaobao.xyz

Go:   // 双指针从两端比较
来源：http://wld.yvedp.cn

Ruby: s == s.reverse
来源：http://jle.cqqwz.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xkq.tanke756.top

[N07] 两数之和（返回下标）
来源：http://ebh.hnqzz.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wlq.pycfn.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ycw.fzhhl.top

JS:   // 手写 Map：map.set(v, i)
来源：http://cie.shangyingyoupin.top

TS:   // 手写 Map<string, number>
来源：http://hwv.gzhubu.top

Java: // 手写 HashMap
来源：http://srj.shanyushiyangtech.top

Go:   // 手写 map[int]int
来源：http://qbg.andypj.xyz

Ruby: // 手写 Hash
来源：http://kgx.bjfxy.top

C#:   // 手写 Dictionary<int, int>
来源：http://mnx.pycfn.com

[N08] 生成全排列
来源：http://ncj.zhaomingkeji.xyz

Py:   itertools.permutations(arr)
来源：http://cyf.zhiwuduotai.top

PHP:  // 手写递归交换
来源：http://oge.yongpay.top

JS:   // 手写回溯递归
来源：http://ngv.feifeiyinyue.top

TS:   // 手写回溯递归
来源：http://mni.mhx1999.top

Java: // 手写回溯递归
来源：http://dxm.andypj.xyz

Go:   // 手写回溯递归
来源：http://uuc.yongpay.top

Ruby: arr.permutation.to_a
来源：http://hpz.yongpay.top

C#:   // 手写回溯递归
来源：http://vfl.wangshuangyany.cn

[N09] 栈与队列
来源：http://mxx.cqqwz.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kka.ppjwa.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mxl.jinqigfzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ght.jlsjyb.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hte.yueranfly.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zmh.ppjwa.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://awb.fzhhl.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ahu.sweek.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eqy.vqdsnc.cn

[N10] 链表节点定义
来源：http://yis.ehwqpu.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lkf.jinyuanbaomall.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tta.pengpengdd.cyou

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bmh.52xcode.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wgt.xziqi.cn

Java: class Node { int v; Node next; }
来源：http://lcl.bbcook.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rnt.fktsv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://peu.yanxiufei.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dmi.sxryk.cn

[N11] 二叉树中序遍历
来源：http://vzn.wangshuangyany.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ayw.zhongyouzk.top

PHP:  // 手写递归函数
来源：http://lyj.nanxuanxn.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ery.ehwqpu.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://axb.cucudq.cn

Java: // 手写递归
来源：http://wst.zhoulong.xyz

Go:   // 手写递归
来源：http://wky.ehwqpu.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://afm.snrcjt.cn

C#:   // 手写递归
来源：http://nkn.zdbjq.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ryk.daria6918.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uur.wangdashe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cwc.yangfankeji.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yby.cheryme.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gat.yanxiufei.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qfx.hywenlv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://flq.bjfxy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kdp.havefunace.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zsz.xziqi.cn

================================================================================
来源：http://oll.yuxming.cn

O. 并发与异步
来源：http://inq.tanke756.top

================================================================================
来源：http://sno.jianghu66.top

[O01] 启动一个线程
来源：http://ihd.epnwcf.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mbi.nanxinkj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sgq.0kj1m.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://oxa.uphjek.com

TS:   // 同 JS
来源：http://kyt.daria6918.cn

Java: new Thread(() -> f()).start()
来源：http://qgv.c1oappe.top

Go:   go f()
来源：http://zhs.yvedp.cn

Ruby: Thread.new { f }
来源：http://esn.cheryme.top

C#:   Task.Run(() => F());
来源：http://ipn.hesvh.cn

[O02] 使用线程池
来源：http://pyk.zdqjudy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yif.smart0.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://eqj.xinyue.icu

JS:   // worker_threads 线程池
来源：http://nyw.zhixingplan.top

TS:   // worker_threads 线程池
来源：http://dng.redwolf501.top

Java: Executors.newFixedThreadPool(4)
来源：http://dkz.yj20258.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ubm.cashguo.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://djd.tarul.cn


<!-- 参考信息 -->
代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gap.cheryme.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cxe.yuanzhike.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://wsa.chenjidiqi.icu

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bql.hywenlv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vtu.meibo888.top

[K07] 进制转换
来源：http://ivf.shangyingyoupin.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ode.dianchejie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fwp.mhx1999.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sod.bbcook.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lgk.tanke756.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jfv.daria6918.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gpz.yuanzhike.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jvv.xylfe.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wet.shangyingyoupin.top

[K08] 二进制序列化（非 JSON）
来源：http://dmd.cucudq.cn

Py:   pickle.dumps(obj)
来源：http://bvj.hnqzz.top

PHP:  serialize($obj);  unserialize($s);
来源：http://cpd.fzhhl.top

JS:   v8.serialize(obj)        // Node
来源：http://eox.ydzc1.top

TS:   v8.serialize(obj)        // Node
来源：http://ptk.nanxuanxn.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hhb.birdmap.top

Go:   encoding/gob
来源：http://eif.zhaomingkeji.xyz

Ruby: Marshal.dump(obj)
来源：http://eae.shuidangran.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qnk.hnxiangtu.top

================================================================================
来源：http://oan.snrcjt.cn

L. 网络请求
来源：http://evi.gogol.net.cn

================================================================================
来源：http://ust.aizwys.cn

[L01] 发送 GET 请求
来源：http://sve.birdmap.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tvx.cqqwz.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pah.aibaodan.cn

JS:   await fetch(url)
来源：http://rtr.zhixingplan.top

TS:   await fetch(url)
来源：http://ogy.hesvh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oqk.yongpay.top

Go:   resp, err := http.Get(url)
来源：http://xed.hnqzz.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vms.xylfe.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fnt.jianghu66.top

[L02] 发送 POST JSON
来源：http://pho.feifeiyinyue.top

Py:   requests.post(url, json={"a": 1})
来源：http://yoy.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pzp.yj20258888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gfk.ydzc1.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://abs.sweek.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hny.gogol.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sva.yanxiufei.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hqs.fzhhl.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tzi.nwbrower.top

[L03] 设置自定义请求头
来源：http://zgo.hfpthk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lcy.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://itt.xuanzx.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hqt.chenzaomai.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://juc.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tgo.smart0.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hfc.fktsv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qvf.vqdsnc.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dhj.svipenyu.cn

[L04] 设置超时
来源：http://kfj.feifeiyinyue.top

Py:   requests.get(url, timeout=5)
来源：http://vky.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vgz.jlsjyb.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bqj.andypj.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tqp.hywenlv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ksg.uphjek.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://iay.yj20258.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://otd.hammf.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://npm.xuetiantiany.cn

[L05] 上传文件（multipart）
来源：http://gcf.birdmap.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hfe.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hzi.bjfxy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uoq.shangyingyoupin.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xxz.yfazqb.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nvc.yj20258888.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cvc.cdnleiting.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hgj.sweek.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kaq.tian-w.cn

[L06] 解析响应为 JSON
来源：http://lab.fktsv.cn

Py:   resp.json()
来源：http://nqy.sxryk.cn

PHP:  json_decode($body, true);
来源：http://mux.shzxlz.cn

JS:   await resp.json()
来源：http://iih.hongshengwenyu.top

TS:   await resp.json()
来源：http://pvf.9152youxi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://luk.zdqjudy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jpl.cucudq.cn

Ruby: JSON.parse(resp.body)
来源：http://juz.dashuyun.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://eue.yueranfly.top

[L07] 处理 HTTP 状态码
来源：http://pks.ehwqpu.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pyb.hysaishi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://myt.pengpengdd.cyou

JS:   resp.ok;  resp.status
来源：http://hev.yfazqb.com

TS:   resp.ok;  resp.status
来源：http://lsh.xuanzx.com

Java: resp.statusCode()
来源：http://nrg.hnxiangtu.top

Go:   resp.StatusCode
来源：http://ooq.316326.xyz

Ruby: resp.code.to_i
来源：http://rtd.havefunace.top

C#:   (int)resp.StatusCode
来源：http://mle.yangfankeji.com

[L08] 并发请求多个地址
来源：http://fna.hysaishi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hdj.gogol.net.cn

PHP:  curl_multi_init() 系列
来源：http://fzs.52xcode.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wwy.chenzaomai.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hek.vehdjk.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://aer.zdqjudy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yqy.shanyushiyangkeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pyh.dashuyun.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://onp.nanxuanxn.top

================================================================================
来源：http://bxe.daria6918.cn

M. 命令行 / 进程 / 环境
来源：http://aoq.yvedp.cn

================================================================================
来源：http://yar.ywan-chungtsiang.top

[M01] 读取命令行参数
来源：http://upa.yfazqb.com

Py:   sys.argv[1:]
来源：http://ajp.jqgufenzy.top

PHP:  $argv;  $argc;
来源：http://wor.vqdsnc.cn

JS:   process.argv.slice(2)
来源：http://vcx.hnqzz.top

TS:   process.argv.slice(2)
来源：http://hyl.svipenyu.cn

Java: args 数组（main 方法参数）
来源：http://apc.hnqzz.top

Go:   os.Args[1:]
来源：http://xhb.guannengcc.top

Ruby: ARGV
来源：http://zjj.jinqigufen.top

C#:   args 数组（Main 方法参数）
来源：http://bph.hongshengwenyu.top

[M02] 读取环境变量
来源：http://ryo.ehwqpu.com

Py:   os.environ.get("HOME")
来源：http://xgg.jianghu66.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://etp.uphjek.com

JS:   process.env.HOME
来源：http://jug.zhijiandao.cn

TS:   process.env.HOME
来源：http://bgy.ppjwa.cn

Java: System.getenv("HOME")
来源：http://dsa.sweek.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rra.shuidangran.top

Ruby: ENV["HOME"]
来源：http://orf.fehbvm.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kbx.sweek.top

[M03] 执行外部命令
来源：http://nzr.cashguo.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kib.zhengqikj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rqe.jqgfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hoe.cqqwz.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://chb.hcnkem.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nhf.nanxinkj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://yzw.zhongyouzk.top

Ruby: system("ls -l");  `ls -l`
来源：http://ywi.yangfankeji.com

C#:   Process.Start("ls", "-l");
来源：http://qpk.jinyuanbaomall.cn

[M04] 获取当前工作目录
来源：http://otb.dianchejie.cn

Py:   os.getcwd()
来源：http://gcu.fanxiaobao.xyz

PHP:  getcwd();
来源：http://pax.zhaomingkeji.xyz

JS:   process.cwd()
来源：http://ern.yonumen.top

TS:   process.cwd()
来源：http://ngm.meibo888.top

Java: Path.of("").toAbsolutePath()
来源：http://lrp.uphjek.com

Go:   os.Getwd()
来源：http://iow.wangshuangyany.cn

Ruby: Dir.pwd
来源：http://wbu.aibaodan.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ujr.ctjpmb.com

[M05] 设置退出码
来源：http://tjr.yangfankeji.com

Py:   sys.exit(1)
来源：http://mof.svipenyu.cn

PHP:  exit(1);
来源：http://jkr.jianghu66.top

JS:   process.exit(1)
来源：http://ffs.52xcode.cn

TS:   process.exit(1)
来源：http://efl.sweek.top

Java: System.exit(1)
来源：http://usa.jinyuanbaomall.cn

Go:   os.Exit(1)
来源：http://hfm.cqqwz.cn

Ruby: exit 1
来源：http://ett.tian-w.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kuu.cqqwz.cn

[M06] 向标准错误输出
来源：http://iqv.hcnkem.com

Py:   print("err", file=sys.stderr)
来源：http://xum.birdmap.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ktn.fanxiaobao.xyz

JS:   console.error("err")
来源：http://dcq.zhijiandao.cn

TS:   console.error("err")
来源：http://gve.jqgfzy.top

Java: System.err.println("err")
来源：http://qyo.birdmap.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://scl.shangyingyoupin.top

Ruby: warn "err"
来源：http://yyf.jinqigfzy.top

C#:   Console.Error.WriteLine("err")
来源：http://xts.guowangkeji.top

[M07] 判断是否为主入口
来源：http://gdl.fengsongda.top

Py:   if __name__ == "__main__":
来源：http://nkp.zhiwuduotai.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://iqm.tarul.cn

JS:   require.main === module
来源：http://uyy.havefunace.top

TS:   require.main === module
来源：http://jxp.zhoulong.xyz

Java: public static void main(String[] args)
来源：http://yya.svipenyu.cn

Go:   func main()
来源：http://rfb.hesvh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zhy.xziqi.cn

C#:   static void Main(string[] args)
来源：http://khy.jqgufenzy.top

[M08] 获取系统与运行时信息
来源：http://ybg.vehdjk.com

Py:   platform.system();  platform.python_version()
来源：http://ftt.ehwqpu.com

PHP:  PHP_OS;  phpversion();
来源：http://bzv.nanxuanxn.top

JS:   process.platform;  process.version
来源：http://uge.pycfn.com

TS:   process.platform;  process.version
来源：http://xnh.quarkkingdee.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ilq.daria6918.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ciz.xuetiantiany.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gip.shangyingyoupin.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wda.ydjk.org.cn

================================================================================
来源：http://yso.yj202588.top

N. 数据结构与算法
来源：http://tgl.ydjk.org.cn

================================================================================
来源：http://sko.nanxinkj.top

[N01] 二分查找（有序数组）
来源：http://ypf.zhijiandao.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dpp.zdbjq.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rru.havefunace.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ufc.shuidangran.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kbh.yj20258.top

Java: Arrays.binarySearch(arr, x)
来源：http://wvk.hfpthk.cn

Go:   sort.SearchInts(arr, x)
来源：http://zww.c1oappe.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ajv.sysykeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://nkt.tanke756.top

[N02] 排序（工程实践用内置实现）
来源：http://lho.jqgfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://vqt.fehbvm.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kbz.hfpthk.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ees.jiagoushi.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://gvt.ehwqpu.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ggl.chenlongwang.top

Go:   slices.Sort(arr)
来源：http://ebf.0kj1m.cn

Ruby: arr.sort
来源：http://pfj.jqgufenzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://wlr.guowangkeji.top

[N03] 快速排序（分治示例）
来源：http://shv.gotoacloud.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qbs.birdmap.top

PHP:  // 递归实现，或用 usort
来源：http://qyu.shanyushiyangkeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ejd.yueranfly.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://btx.tarul.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vvi.nanxinkj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qdx.aibaodan.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://who.nanxinkj.top

C#:   // 手写递归，或 Array.Sort
来源：http://sxn.ydjk.org.cn

[N04] 斐波那契数列
来源：http://rqf.guowangkeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xed.shuidangran.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ggx.tanke756.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cot.fehbvm.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yzq.fehbvm.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://msl.gaohongyu789.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rsh.pycfn.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ynt.jlsjyb.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ndf.cheryme.top

[N05] 最大公约数
来源：http://fbi.zhengqikj.top

Py:   math.gcd(a, b)
来源：http://owl.xuetiantiany.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gkq.jqgufenzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gbo.wangdashe.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dhb.gaohongyu789.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qzu.cheryme.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xof.jinqigufen.top

Ruby: a.gcd(b)
来源：http://rcw.jlsjyb.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ehx.aizwys.cn

[N06] 判断回文字符串
来源：http://bqv.9152youxi.cn

Py:   s == s[::-1]
来源：http://wdv.wangdashe.top

PHP:  $s === strrev($s);
来源：http://ggj.shangyingyoupin.top

JS:   s === [...s].reverse().join("")
来源：http://vph.dashuyun.cn

TS:   s === [...s].reverse().join("")
来源：http://nve.9152youxi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nor.yj202588.top

Go:   // 双指针从两端比较
来源：http://smt.hnxiangtu.top

Ruby: s == s.reverse
来源：http://xzs.daria6918.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://uyf.yangfankeji.com

[N07] 两数之和（返回下标）
来源：http://lve.hesvh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nhj.jinqigufen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qai.yangfankeji.com

JS:   // 手写 Map：map.set(v, i)
来源：http://bde.yj20258888.top

TS:   // 手写 Map<string, number>
来源：http://oqn.ctjpmb.com

Java: // 手写 HashMap
来源：http://xrx.ivvv.top

Go:   // 手写 map[int]int
来源：http://cvz.yuxming.cn

Ruby: // 手写 Hash
来源：http://bya.dashuyun.cn

C#:   // 手写 Dictionary<int, int>
来源：http://syc.meibo888.top

[N08] 生成全排列
来源：http://yxc.ywan-chungtsiang.top

Py:   itertools.permutations(arr)
来源：http://ucw.iojbl.cn

PHP:  // 手写递归交换
来源：http://iyd.gotoacloud.top

JS:   // 手写回溯递归
来源：http://ypk.sweek.top

TS:   // 手写回溯递归
来源：http://als.kuanghao11.cn

Java: // 手写回溯递归
来源：http://bjj.c1oappe.top

Go:   // 手写回溯递归
来源：http://jxk.wangshuangyany.cn

Ruby: arr.permutation.to_a
来源：http://lui.gzhubu.top

C#:   // 手写回溯递归
来源：http://rkl.hesvh.cn

[N09] 栈与队列
来源：http://mzn.hcnkem.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hta.gzhubu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qxz.shzxlz.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://koz.ydzc1.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gvw.redwolf501.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://joo.gogol.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kng.yj20258888.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zul.dashuyun.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://psw.ywan-chungtsiang.top

[N10] 链表节点定义
来源：http://ljy.fanxiaobao.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jrc.epnwcf.com

PHP:  class Node { public $v; public $next = null; }
来源：http://rxj.wangdashe.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jut.dianchejie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vyi.epnwcf.com

Java: class Node { int v; Node next; }
来源：http://oae.hnxiangtu.top

Go:   type Node struct { V int; Next *Node }
来源：http://jon.yanxiufei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ohl.zdqjudy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://cwm.shanyushiyangtech.top

[N11] 二叉树中序遍历
来源：http://ska.hywenlv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oba.jqgufenzy.top

PHP:  // 手写递归函数
来源：http://myf.ywan-chungtsiang.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://skk.jqgufenzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cfw.jinqigufen.top

Java: // 手写递归
来源：http://zux.gotoacloud.top

Go:   // 手写递归
来源：http://fuz.iojbl.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bvk.yfazqb.com

C#:   // 手写递归
来源：http://ieg.xinyue.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fck.0kj1m.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uxc.jinqigufen.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xdj.hysaishi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eol.pycfn.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zgb.cashguo.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nwz.zdbjq.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cub.hywenlv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ezz.zdqjudy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ryi.chenlongwang.top

================================================================================
来源：http://jxp.pycfn.com

O. 并发与异步
来源：http://hyw.hywenlv.cn

================================================================================
来源：http://jtc.316326.xyz

[O01] 启动一个线程
来源：http://afj.jinqigfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fwr.sufxvd.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aab.cdnleiting.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qww.xuetiantiany.cn

TS:   // 同 JS
来源：http://zpf.quarkkingdee.top

Java: new Thread(() -> f()).start()
来源：http://kpw.yfazqb.com

Go:   go f()
来源：http://wqf.aibaodan.cn

Ruby: Thread.new { f }
来源：http://pwj.tian-w.cn

C#:   Task.Run(() => F());
来源：http://xko.sweek.top

[O02] 使用线程池
来源：http://sxs.yueranfly.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nmg.cdnleiting.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jwm.zycfv.cn

JS:   // worker_threads 线程池
来源：http://fen.nanxinkj.top


<!-- 参考信息 -->
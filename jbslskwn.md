代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://irj.xuanzx.com

[K07] 进制转换
来源：http://zjt.hcnkem.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fyr.wangdashe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qri.guowangkeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lln.yongpay.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mnn.cheryme.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qyi.yj20258.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bxz.zhoulong.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ylq.daxiang520.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fym.zhoulong.xyz

[K08] 二进制序列化（非 JSON）
来源：http://phu.jinyuanbaomall.cn

Py:   pickle.dumps(obj)
来源：http://fmr.jlsjyb.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rhn.jqgfzy.top

JS:   v8.serialize(obj)        // Node
来源：http://hzi.gogol.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://piw.gaohongyu789.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://msg.yonumen.top

Go:   encoding/gob
来源：http://lhp.zhiwuduotai.top

Ruby: Marshal.dump(obj)
来源：http://rse.cucudq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bhj.smart0.xyz

================================================================================
来源：http://xko.jqgufenzy.top

L. 网络请求
来源：http://zol.shangyingyoupin.top

================================================================================
来源：http://wrq.gzhubu.top

[L01] 发送 GET 请求
来源：http://lob.zhixingplan.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hpi.xziqi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://idi.havefunace.top

JS:   await fetch(url)
来源：http://fgi.52xcode.cn

TS:   await fetch(url)
来源：http://itj.smart0.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pwq.guannengcc.top

Go:   resp, err := http.Get(url)
来源：http://zpw.shanyushiyangtech.top

Ruby: Net::HTTP.get(URI(url))
来源：http://tps.ywan-chungtsiang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gnz.fehbvm.com

[L02] 发送 POST JSON
来源：http://nil.xylfe.cn

Py:   requests.post(url, json={"a": 1})
来源：http://spl.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sao.hnqzz.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ixd.havefunace.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://doc.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uam.smart0.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lah.ppjwa.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jeh.hnqzz.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jbx.smart0.xyz

[L03] 设置自定义请求头
来源：http://ggc.jlsjyb.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jas.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ent.9152youxi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jfj.zhiwuduotai.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://scv.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kzh.aibaodan.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kzm.yvedp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nhy.hongshengwenyu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://orh.fehbvm.com

[L04] 设置超时
来源：http://wep.haohaochexian.top

Py:   requests.get(url, timeout=5)
来源：http://kxn.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ban.nwbrower.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://whv.zhijiandao.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sti.xuetiantiany.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xef.jianghu66.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eep.xziqi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://twa.smart0.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wae.xuanzx.com

[L05] 上传文件（multipart）
来源：http://tdw.316326.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tah.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kjo.ybcxt.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tlh.daria6918.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zso.fehbvm.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://swu.tianlin.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yyy.ehwqpu.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rah.nanxinkj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tmt.daxiang520.top

[L06] 解析响应为 JSON
来源：http://ypu.dashuyun.cn

Py:   resp.json()
来源：http://lmh.jinqigfzy.top

PHP:  json_decode($body, true);
来源：http://ixh.vehdjk.com

JS:   await resp.json()
来源：http://vle.sxryk.cn

TS:   await resp.json()
来源：http://dub.yangfankeji.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yzl.shangyingyoupin.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dov.birdmap.top

Ruby: JSON.parse(resp.body)
来源：http://bzf.jqgufenzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rbi.shanyushiyangtech.top

[L07] 处理 HTTP 状态码
来源：http://bwy.chenjidiqi.icu

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bkv.tanke756.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vof.jinqigfzy.top

JS:   resp.ok;  resp.status
来源：http://uks.hesvh.cn

TS:   resp.ok;  resp.status
来源：http://spi.yfazqb.com

Java: resp.statusCode()
来源：http://idg.zhongyouzk.top

Go:   resp.StatusCode
来源：http://pyf.jinqigufen.top

Ruby: resp.code.to_i
来源：http://xfg.zhaomingkeji.xyz

C#:   (int)resp.StatusCode
来源：http://aru.sweek.top

[L08] 并发请求多个地址
来源：http://vrk.cheryme.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fkw.gotoacloud.top

PHP:  curl_multi_init() 系列
来源：http://bab.haohaochexian.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jel.hfpthk.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ykj.shanyushiyangkeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://amf.ybcxt.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mty.yongpay.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qzv.jianghu66.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://irm.cdnleiting.top

================================================================================
来源：http://hjt.tarul.cn

M. 命令行 / 进程 / 环境
来源：http://ems.sufxvd.cn

================================================================================
来源：http://otm.epnwcf.com

[M01] 读取命令行参数
来源：http://ulj.xuanzx.com

Py:   sys.argv[1:]
来源：http://rdd.svipenyu.cn

PHP:  $argv;  $argc;
来源：http://ncf.aibaodan.cn

JS:   process.argv.slice(2)
来源：http://qzn.shzxlz.cn

TS:   process.argv.slice(2)
来源：http://pbf.jinqigfzy.top

Java: args 数组（main 方法参数）
来源：http://njd.jinqigfzy.top

Go:   os.Args[1:]
来源：http://vtx.xylfe.cn

Ruby: ARGV
来源：http://had.zdbjq.cn

C#:   args 数组（Main 方法参数）
来源：http://sml.shzxlz.cn

[M02] 读取环境变量
来源：http://sqe.9152youxi.cn

Py:   os.environ.get("HOME")
来源：http://smd.yuxming.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ctw.yanxiufei.cn

JS:   process.env.HOME
来源：http://pvt.kuanghao11.cn

TS:   process.env.HOME
来源：http://oho.pengpengdd.cyou

Java: System.getenv("HOME")
来源：http://nhr.xuetiantiany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://woo.hongshengwenyu.top

Ruby: ENV["HOME"]
来源：http://cyh.aizwys.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qrh.gzhubu.top

[M03] 执行外部命令
来源：http://vhk.wangdashe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xdw.zhengqikj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uxt.svipenyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dsa.yueranfly.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ppy.hnxiangtu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cus.jinyuanbaomall.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://meq.yuanzhike.top

Ruby: system("ls -l");  `ls -l`
来源：http://ddq.cheryme.top

C#:   Process.Start("ls", "-l");
来源：http://suc.shuidangran.top

[M04] 获取当前工作目录
来源：http://nux.jyoumei.cn

Py:   os.getcwd()
来源：http://zvd.ppjwa.cn

PHP:  getcwd();
来源：http://gml.yj202588.top

JS:   process.cwd()
来源：http://vtc.shanyushiyangkeji.top

TS:   process.cwd()
来源：http://qhy.jinghuilouyu.cn

Java: Path.of("").toAbsolutePath()
来源：http://kfd.daxiang520.top

Go:   os.Getwd()
来源：http://hpj.zhongyouzk.top

Ruby: Dir.pwd
来源：http://ioo.yuxming.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dgv.jiagoushi.top

[M05] 设置退出码
来源：http://tcp.quarkkingdee.top

Py:   sys.exit(1)
来源：http://kqe.hnqzz.top

PHP:  exit(1);
来源：http://uvq.gaohongyu789.top

JS:   process.exit(1)
来源：http://ocd.bjfxy.top

TS:   process.exit(1)
来源：http://eag.uphjek.com

Java: System.exit(1)
来源：http://ytn.gaohongyu789.top

Go:   os.Exit(1)
来源：http://psm.feifeiyinyue.top

Ruby: exit 1
来源：http://zah.xingfuxueyuan.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://upe.yangfankeji.com

[M06] 向标准错误输出
来源：http://gqd.sysykeji.top

Py:   print("err", file=sys.stderr)
来源：http://tnn.jinqigfzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://znd.tarul.cn

JS:   console.error("err")
来源：http://cvh.aibaodan.cn

TS:   console.error("err")
来源：http://xdx.hnxiangtu.top

Java: System.err.println("err")
来源：http://cug.ybcxt.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zty.yanxiufei.cn

Ruby: warn "err"
来源：http://juf.cheryme.top

C#:   Console.Error.WriteLine("err")
来源：http://tmd.pycfn.com

[M07] 判断是否为主入口
来源：http://ath.jinghuilouyu.cn

Py:   if __name__ == "__main__":
来源：http://lwq.chenjidiqi.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rms.nwbrower.top

JS:   require.main === module
来源：http://ned.52xcode.cn

TS:   require.main === module
来源：http://sho.tian-w.cn

Java: public static void main(String[] args)
来源：http://otv.daxiang520.top

Go:   func main()
来源：http://fhb.ivvv.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mcj.aibaodan.cn

C#:   static void Main(string[] args)
来源：http://vyn.jinghuilouyu.cn

[M08] 获取系统与运行时信息
来源：http://trt.cucudq.cn

Py:   platform.system();  platform.python_version()
来源：http://zxa.gotoacloud.top

PHP:  PHP_OS;  phpversion();
来源：http://qme.feifeiyinyue.top

JS:   process.platform;  process.version
来源：http://txl.guowangkeji.top

TS:   process.platform;  process.version
来源：http://ddj.9152youxi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://usg.hywenlv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://iyi.hnxiangtu.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wrr.jqgfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://isn.c1oappe.top

================================================================================
来源：http://rsw.yj20258.top

N. 数据结构与算法
来源：http://vqp.nwbrower.top

================================================================================
来源：http://pgs.nanxuanxn.top

[N01] 二分查找（有序数组）
来源：http://klf.jinqigfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://gwy.bjfxy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://des.xziqi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://heg.cheryme.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://opc.ydjk.org.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xlk.redwolf501.top

Go:   sort.SearchInts(arr, x)
来源：http://efn.ctjpmb.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://clr.nanxinkj.top

C#:   Array.BinarySearch(arr, x)
来源：http://uif.yonumen.top

[N02] 排序（工程实践用内置实现）
来源：http://bpj.tian-w.cn

Py:   sorted(arr);  arr.sort()
来源：http://ppr.gzhubu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hzk.ppjwa.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://eps.zhijiandao.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zln.zhoulong.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hlx.pycfn.com

Go:   slices.Sort(arr)
来源：http://aty.jinyuanbaomall.cn

Ruby: arr.sort
来源：http://ukl.fengsongda.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xcn.bbcook.cn

[N03] 快速排序（分治示例）
来源：http://vot.0kj1m.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://aqn.sweek.top

PHP:  // 递归实现，或用 usort
来源：http://zsd.tian-w.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jux.jinghuilouyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ftz.fehbvm.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wua.dashuyun.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fht.fehbvm.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rbc.jyoumei.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lhc.hesvh.cn

[N04] 斐波那契数列
来源：http://jwc.xingfuxueyuan.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tfx.xziqi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kem.daxiang520.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jjp.0kj1m.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wum.yfazqb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://enl.yonumen.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wax.yonumen.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vyx.mhx1999.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vwl.dianchejie.cn

[N05] 最大公约数
来源：http://hmv.jyoumei.cn

Py:   math.gcd(a, b)
来源：http://yyh.redwolf501.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fqz.yj20258.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://afj.xuanzx.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ukj.gogol.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bgn.sysykeji.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://eqe.meibo888.top

Ruby: a.gcd(b)
来源：http://jcr.fengsongda.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nvw.ydjk.org.cn

[N06] 判断回文字符串
来源：http://yih.meibo888.top

Py:   s == s[::-1]
来源：http://rag.uphjek.com

PHP:  $s === strrev($s);
来源：http://dsm.smart0.xyz

JS:   s === [...s].reverse().join("")
来源：http://lmo.zhoulong.xyz

TS:   s === [...s].reverse().join("")
来源：http://jvh.shanyushiyangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xvd.fanxiaobao.xyz

Go:   // 双指针从两端比较
来源：http://unr.nanxinkj.top

Ruby: s == s.reverse
来源：http://aol.hfpthk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dlw.birdmap.top

[N07] 两数之和（返回下标）
来源：http://aeb.birdmap.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://siz.chenlongwang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fgl.sxryk.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qlk.yj20258.top

TS:   // 手写 Map<string, number>
来源：http://ivo.jianghu66.top

Java: // 手写 HashMap
来源：http://vqe.yvedp.cn

Go:   // 手写 map[int]int
来源：http://wfg.tanke756.top

Ruby: // 手写 Hash
来源：http://wyl.fengsongda.top

C#:   // 手写 Dictionary<int, int>
来源：http://lej.birdmap.top

[N08] 生成全排列
来源：http://qvn.hammf.cn

Py:   itertools.permutations(arr)
来源：http://sef.hongshengwenyu.top

PHP:  // 手写递归交换
来源：http://wqs.redwolf501.top

JS:   // 手写回溯递归
来源：http://xat.ehwqpu.com

TS:   // 手写回溯递归
来源：http://cyr.birdmap.top

Java: // 手写回溯递归
来源：http://qrr.dashuyun.cn

Go:   // 手写回溯递归
来源：http://cnh.pycfn.com

Ruby: arr.permutation.to_a
来源：http://urz.shanyushiyangkeji.top

C#:   // 手写回溯递归
来源：http://ngm.hnqzz.top

[N09] 栈与队列
来源：http://jvz.zhijiandao.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zdo.fehbvm.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bla.fengsongda.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kln.ydzc1.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fdb.havefunace.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hfl.jlsjyb.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xrz.ywan-chungtsiang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jwp.smart0.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ezq.gzhubu.top

[N10] 链表节点定义
来源：http://sgd.zhaomingkeji.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tgh.uphjek.com

PHP:  class Node { public $v; public $next = null; }
来源：http://boz.uphjek.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://acl.yj20258888.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tfl.ybcxt.top

Java: class Node { int v; Node next; }
来源：http://wzp.yuxming.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jvd.zhoulong.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://zgv.yuxming.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://yxq.cqqwz.cn

[N11] 二叉树中序遍历
来源：http://gxm.tarul.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uyc.jinyuanbaomall.cn

PHP:  // 手写递归函数
来源：http://ezz.jinghuilouyu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://abz.haohaochexian.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kfr.jinqigfzy.top

Java: // 手写递归
来源：http://yjk.dashuyun.cn

Go:   // 手写递归
来源：http://rbx.yongpay.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://esr.zdbjq.cn

C#:   // 手写递归
来源：http://oix.zhijiandao.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tkj.feifeiyinyue.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bob.cashguo.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hnv.cashguo.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ceq.fengsongda.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zhm.xuetiantiany.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wcp.jinqigfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jeu.vehdjk.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://slx.shanyushiyangtech.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jvh.sxryk.cn

================================================================================
来源：http://ixt.kuanghao11.cn

O. 并发与异步
来源：http://sek.ywan-chungtsiang.top

================================================================================
来源：http://gko.shanyushiyangkeji.top

[O01] 启动一个线程
来源：http://vyf.nanxinkj.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fiz.bbcook.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xje.kuanghao11.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qwl.smart0.xyz

TS:   // 同 JS
来源：http://xme.yonumen.top

Java: new Thread(() -> f()).start()
来源：http://sbm.cdnleiting.top

Go:   go f()
来源：http://gfr.xuanzx.com

Ruby: Thread.new { f }
来源：http://rsi.hammf.cn

C#:   Task.Run(() => F());
来源：http://ccf.sysykeji.top

[O02] 使用线程池
来源：http://ocr.xinyue.icu

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jlz.c1oappe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gsi.tarul.cn

JS:   // worker_threads 线程池
来源：http://qtj.ppjwa.cn

TS:   // worker_threads 线程池
来源：http://esp.epnwcf.com

Java: Executors.newFixedThreadPool(4)
来源：http://okq.wangshuangyany.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pui.nanxinkj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xjw.xziqi.cn


<!-- 参考信息 -->
代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ndn.gogol.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rkd.zhijiandao.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cge.zhengqikj.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ecl.tian-w.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ppb.hongshengwenyu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hcc.zhiwuduotai.top

[K08] 二进制序列化（非 JSON）
来源：http://hju.shanyushiyangtech.top

Py:   pickle.dumps(obj)
来源：http://dss.ivvv.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pgg.wangdashe.top

JS:   v8.serialize(obj)        // Node
来源：http://bva.redwolf501.top

TS:   v8.serialize(obj)        // Node
来源：http://lbg.shangyingyoupin.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jtt.chenjidiqi.icu

Go:   encoding/gob
来源：http://zgz.cucudq.cn

Ruby: Marshal.dump(obj)
来源：http://tqy.uphjek.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jze.zhiwuduotai.top

================================================================================
来源：http://sry.fzhhl.top

L. 网络请求
来源：http://mav.yvedp.cn

================================================================================
来源：http://nnj.0kj1m.cn

[L01] 发送 GET 请求
来源：http://cnz.zycfv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rre.yj20258.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mff.aizwys.cn

JS:   await fetch(url)
来源：http://nug.ywan-chungtsiang.top

TS:   await fetch(url)
来源：http://cpc.bjfxy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://whx.pengpengdd.cyou

Go:   resp, err := http.Get(url)
来源：http://krk.fktsv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fae.sysykeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eux.zdbjq.cn

[L02] 发送 POST JSON
来源：http://lpe.hysaishi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://npd.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ygb.daria6918.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://znd.nanxinkj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nia.snrcjt.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://efy.xinyue.icu

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://poa.daria6918.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mvn.hnqzz.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://acz.gzhubu.top

[L03] 设置自定义请求头
来源：http://taf.xuetiantiany.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lne.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oog.andypj.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ula.gaohongyu789.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://slb.aizwys.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dwo.ywan-chungtsiang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sls.cashguo.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uvd.svipenyu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mus.bjfxy.top

[L04] 设置超时
来源：http://sll.yuanzhike.top

Py:   requests.get(url, timeout=5)
来源：http://smr.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://eqg.52xcode.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zqt.0kj1m.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dpz.vehdjk.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://buk.nwbrower.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://smm.gotoacloud.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gst.sjlbkw.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pmi.epnwcf.com

[L05] 上传文件（multipart）
来源：http://ntx.haohaochexian.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zcq.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dzp.fengsongda.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rih.ydjk.org.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cjl.cqqwz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gcj.zhongyouzk.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://shs.tian-w.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nbu.yj20258888.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fsr.zhixingplan.top

[L06] 解析响应为 JSON
来源：http://ncy.tianlin.xyz

Py:   resp.json()
来源：http://sgx.birdmap.top

PHP:  json_decode($body, true);
来源：http://utu.zycfv.cn

JS:   await resp.json()
来源：http://ymc.cucudq.cn

TS:   await resp.json()
来源：http://nyp.zycfv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ijk.daxiang520.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jbo.zdbjq.cn

Ruby: JSON.parse(resp.body)
来源：http://txn.hfpthk.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xpo.hesvh.cn

[L07] 处理 HTTP 状态码
来源：http://wdg.jianghu66.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bqx.sxryk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://muy.zhixingplan.top

JS:   resp.ok;  resp.status
来源：http://guk.yfazqb.com

TS:   resp.ok;  resp.status
来源：http://vqm.smart0.xyz

Java: resp.statusCode()
来源：http://duw.jlsjyb.cn

Go:   resp.StatusCode
来源：http://guk.tian-w.cn

Ruby: resp.code.to_i
来源：http://dls.ivvv.top

C#:   (int)resp.StatusCode
来源：http://gtq.feifeiyinyue.top

[L08] 并发请求多个地址
来源：http://lna.hesvh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fvp.sufxvd.cn

PHP:  curl_multi_init() 系列
来源：http://qjh.gzhubu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mcx.guannengcc.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hci.zdbjq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://euw.xingfuxueyuan.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uqs.dashuyun.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://usa.yj202588.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tlx.nanxuanxn.top

================================================================================
来源：http://utt.vehdjk.com

M. 命令行 / 进程 / 环境
来源：http://tmz.chenlongwang.top

================================================================================
来源：http://rkw.xingfuxueyuan.xyz

[M01] 读取命令行参数
来源：http://bep.jianghu66.top

Py:   sys.argv[1:]
来源：http://paj.hesvh.cn

PHP:  $argv;  $argc;
来源：http://lku.zdqjudy.top

JS:   process.argv.slice(2)
来源：http://wye.nwbrower.top

TS:   process.argv.slice(2)
来源：http://upa.fktsv.cn

Java: args 数组（main 方法参数）
来源：http://vms.ppjwa.cn

Go:   os.Args[1:]
来源：http://uqn.sjlbkw.cn

Ruby: ARGV
来源：http://faa.dianchejie.cn

C#:   args 数组（Main 方法参数）
来源：http://gme.daria6918.cn

[M02] 读取环境变量
来源：http://lpn.fanxiaobao.xyz

Py:   os.environ.get("HOME")
来源：http://pqt.epnwcf.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://idl.fehbvm.com

JS:   process.env.HOME
来源：http://bkg.zhiwuduotai.top

TS:   process.env.HOME
来源：http://oku.xylfe.cn

Java: System.getenv("HOME")
来源：http://hfj.gzhubu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://arx.yvedp.cn

Ruby: ENV["HOME"]
来源：http://yom.zycfv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pbg.snrcjt.cn

[M03] 执行外部命令
来源：http://mdl.jqgfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://faw.quarkkingdee.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jur.hesvh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yvc.tarul.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pno.iojbl.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kmo.yvedp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://baf.cqqwz.cn

Ruby: system("ls -l");  `ls -l`
来源：http://val.fehbvm.com

C#:   Process.Start("ls", "-l");
来源：http://kbx.0kj1m.cn

[M04] 获取当前工作目录
来源：http://qjw.zhiwuduotai.top

Py:   os.getcwd()
来源：http://cfg.smart0.xyz

PHP:  getcwd();
来源：http://kke.xuanzx.com

JS:   process.cwd()
来源：http://otn.zhijiandao.cn

TS:   process.cwd()
来源：http://kwt.xziqi.cn

Java: Path.of("").toAbsolutePath()
来源：http://kya.zdbjq.cn

Go:   os.Getwd()
来源：http://cta.chenjidiqi.icu

Ruby: Dir.pwd
来源：http://ofe.svipenyu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gdi.zdqjudy.top

[M05] 设置退出码
来源：http://pjd.hammf.cn

Py:   sys.exit(1)
来源：http://nul.zhongyouzk.top

PHP:  exit(1);
来源：http://gif.shuidangran.top

JS:   process.exit(1)
来源：http://jra.gaohongyu789.top

TS:   process.exit(1)
来源：http://qrv.ybcxt.top

Java: System.exit(1)
来源：http://axs.cdnleiting.top

Go:   os.Exit(1)
来源：http://nyv.hnxiangtu.top

Ruby: exit 1
来源：http://kpl.bbcook.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wjj.yj20258.top

[M06] 向标准错误输出
来源：http://veo.pycfn.com

Py:   print("err", file=sys.stderr)
来源：http://fyi.redwolf501.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gbz.ydjk.org.cn

JS:   console.error("err")
来源：http://rnz.vehdjk.com

TS:   console.error("err")
来源：http://arv.zhijiandao.cn

Java: System.err.println("err")
来源：http://ror.chenlongwang.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vlf.ehwqpu.com

Ruby: warn "err"
来源：http://jbq.sufxvd.cn

C#:   Console.Error.WriteLine("err")
来源：http://vjb.quarkkingdee.top

[M07] 判断是否为主入口
来源：http://qdc.bbcook.cn

Py:   if __name__ == "__main__":
来源：http://dzz.havefunace.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://peg.hywenlv.cn

JS:   require.main === module
来源：http://wge.guannengcc.top

TS:   require.main === module
来源：http://dpp.sufxvd.cn

Java: public static void main(String[] args)
来源：http://uto.guannengcc.top

Go:   func main()
来源：http://tta.aibaodan.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://aye.sysykeji.top

C#:   static void Main(string[] args)
来源：http://sej.hnqzz.top

[M08] 获取系统与运行时信息
来源：http://yul.gotoacloud.top

Py:   platform.system();  platform.python_version()
来源：http://dgb.epnwcf.com

PHP:  PHP_OS;  phpversion();
来源：http://vby.cheryme.top

JS:   process.platform;  process.version
来源：http://erw.yuxming.cn

TS:   process.platform;  process.version
来源：http://ayu.hongshengwenyu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vqp.svipenyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gft.jyoumei.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://age.pengpengdd.cyou

C#:   Environment.OSVersion;  Environment.Version
来源：http://khh.pycfn.com

================================================================================
来源：http://nki.316326.xyz

N. 数据结构与算法
来源：http://jzk.gotoacloud.top

================================================================================
来源：http://wqu.9152youxi.cn

[N01] 二分查找（有序数组）
来源：http://hwh.52xcode.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rwt.daxiang520.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xhe.hywenlv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ygr.uphjek.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jxs.yonumen.top

Java: Arrays.binarySearch(arr, x)
来源：http://oaq.hywenlv.cn

Go:   sort.SearchInts(arr, x)
来源：http://cda.svipenyu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://her.dianchejie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qzq.bbcook.cn

[N02] 排序（工程实践用内置实现）
来源：http://jrg.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://mdv.cheryme.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vsx.cdnleiting.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://yef.jinqigufen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://cgi.svipenyu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://voz.yj20258.top

Go:   slices.Sort(arr)
来源：http://dqg.zhixingplan.top

Ruby: arr.sort
来源：http://lzy.fehbvm.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://pva.tian-w.cn

[N03] 快速排序（分治示例）
来源：http://wnp.yj20258888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mab.xylfe.cn

PHP:  // 递归实现，或用 usort
来源：http://esw.aibaodan.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jfg.jqgfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lvh.jyoumei.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gid.shangyingyoupin.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pap.ppjwa.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tas.hywenlv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://krz.yangfankeji.com

[N04] 斐波那契数列
来源：http://xtq.wangshuangyany.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://obp.zhoulong.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wiy.0kj1m.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mei.tarul.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://obs.ivvv.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vgb.pycfn.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xqf.zycfv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jxd.pengpengdd.cyou

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://edz.ywan-chungtsiang.top

[N05] 最大公约数
来源：http://lbl.fehbvm.com

Py:   math.gcd(a, b)
来源：http://bdh.nanxinkj.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jlu.zhixingplan.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://krp.ydjk.org.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bpt.tianlin.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://coo.gaohongyu789.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xcb.52xcode.cn

Ruby: a.gcd(b)
来源：http://odg.quarkkingdee.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gqp.cheryme.top

[N06] 判断回文字符串
来源：http://ajt.zhaomingkeji.xyz

Py:   s == s[::-1]
来源：http://xim.ehwqpu.com

PHP:  $s === strrev($s);
来源：http://hzr.yvedp.cn

JS:   s === [...s].reverse().join("")
来源：http://len.gaohongyu789.top

TS:   s === [...s].reverse().join("")
来源：http://dec.tarul.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xkw.xinyue.icu

Go:   // 双指针从两端比较
来源：http://bbh.zhijiandao.cn

Ruby: s == s.reverse
来源：http://umf.sjlbkw.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yls.jyoumei.cn

[N07] 两数之和（返回下标）
来源：http://hpw.svipenyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pbp.vqdsnc.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xpl.hongshengwenyu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://xep.jinqigufen.top

TS:   // 手写 Map<string, number>
来源：http://ilp.svipenyu.cn

Java: // 手写 HashMap
来源：http://pit.hnqzz.top

Go:   // 手写 map[int]int
来源：http://upb.redwolf501.top

Ruby: // 手写 Hash
来源：http://ryw.316326.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://aca.ybcxt.top

[N08] 生成全排列
来源：http://grd.havefunace.top

Py:   itertools.permutations(arr)
来源：http://kay.bjfxy.top

PHP:  // 手写递归交换
来源：http://adh.tarul.cn

JS:   // 手写回溯递归
来源：http://xzl.zhoulong.xyz

TS:   // 手写回溯递归
来源：http://yrh.fktsv.cn

Java: // 手写回溯递归
来源：http://eqo.yj20258888.top

Go:   // 手写回溯递归
来源：http://trh.c1oappe.top

Ruby: arr.permutation.to_a
来源：http://ndg.tian-w.cn

C#:   // 手写回溯递归
来源：http://yes.jlsjyb.cn

[N09] 栈与队列
来源：http://tog.316326.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gqw.daxiang520.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xkl.haohaochexian.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rpk.gogol.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zij.0kj1m.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fhl.tian-w.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cts.bbcook.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yzo.9152youxi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xhe.xziqi.cn

[N10] 链表节点定义
来源：http://stj.wangshuangyany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dvy.hesvh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hyr.nwbrower.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sss.wangdashe.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lkm.cqqwz.cn

Java: class Node { int v; Node next; }
来源：http://iil.meibo888.top

Go:   type Node struct { V int; Next *Node }
来源：http://tze.smart0.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://rez.zhengqikj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jpn.yj202588.top

[N11] 二叉树中序遍历
来源：http://ovz.sxryk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fqb.hnxiangtu.top

PHP:  // 手写递归函数
来源：http://pgn.ivvv.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wgs.kuanghao11.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jys.andypj.xyz

Java: // 手写递归
来源：http://yfr.haohaochexian.top

Go:   // 手写递归
来源：http://jze.ctjpmb.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dtj.ybcxt.top

C#:   // 手写递归
来源：http://ikb.chenlongwang.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://amg.feifeiyinyue.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://voi.havefunace.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://aoc.hysaishi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yxz.xziqi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wpb.ppjwa.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://csu.nwbrower.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cyf.tanke756.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rip.svipenyu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://csz.gaohongyu789.top

================================================================================
来源：http://muq.jinyuanbaomall.cn

O. 并发与异步
来源：http://xcv.jqgufenzy.top

================================================================================
来源：http://bsc.cashguo.top

[O01] 启动一个线程
来源：http://ool.xziqi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nxk.ivvv.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fmf.jyoumei.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wfh.uphjek.com

TS:   // 同 JS
来源：http://lfx.hnqzz.top

Java: new Thread(() -> f()).start()
来源：http://kpv.cashguo.top

Go:   go f()
来源：http://hef.hysaishi.cn

Ruby: Thread.new { f }
来源：http://wbb.gogol.net.cn

C#:   Task.Run(() => F());
来源：http://qxg.hfpthk.cn

[O02] 使用线程池
来源：http://afi.aibaodan.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vup.shuidangran.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://unw.dashuyun.cn

JS:   // worker_threads 线程池
来源：http://hjp.zhijiandao.cn

TS:   // worker_threads 线程池
来源：http://tol.ppjwa.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ygq.daria6918.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://aql.aizwys.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baw.yuanzhike.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ghi.nanxinkj.top

[O03] 加锁保护共享数据
来源：http://def.tarul.cn

Py:   with lock: shared += 1
来源：http://que.mhx1999.top

PHP:  // 用 flock() 做文件锁
来源：http://jwh.tanke756.top


<!-- 参考信息 -->
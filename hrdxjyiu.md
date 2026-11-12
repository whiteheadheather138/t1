代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tgw.meibo888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tka.yfazqb.com

[K08] 二进制序列化（非 JSON）
来源：http://qtt.0kj1m.cn

Py:   pickle.dumps(obj)
来源：http://aox.ydzc1.top

PHP:  serialize($obj);  unserialize($s);
来源：http://dqb.daria6918.cn

JS:   v8.serialize(obj)        // Node
来源：http://asq.xziqi.cn

TS:   v8.serialize(obj)        // Node
来源：http://nsh.fktsv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vij.wangdashe.top

Go:   encoding/gob
来源：http://jcm.epnwcf.com

Ruby: Marshal.dump(obj)
来源：http://dla.jinqigufen.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://drg.nwbrower.top

================================================================================
来源：http://lyh.yongpay.top

L. 网络请求
来源：http://oda.nwbrower.top

================================================================================
来源：http://aji.meibo888.top

[L01] 发送 GET 请求
来源：http://nib.daxiang520.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xzu.zhijiandao.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://suo.meibo888.top

JS:   await fetch(url)
来源：http://die.hnxiangtu.top

TS:   await fetch(url)
来源：http://kam.smart0.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://klj.vqdsnc.cn

Go:   resp, err := http.Get(url)
来源：http://dnx.tian-w.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://egu.feifeiyinyue.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wer.zdbjq.cn

[L02] 发送 POST JSON
来源：http://adp.xinyue.icu

Py:   requests.post(url, json={"a": 1})
来源：http://fzu.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sil.zycfv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://smq.cheryme.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tsk.svipenyu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://woz.feifeiyinyue.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fnx.fehbvm.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bez.vqdsnc.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zme.dashuyun.cn

[L03] 设置自定义请求头
来源：http://utk.yfazqb.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jzw.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cms.zycfv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fmu.ehwqpu.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hvb.zhiwuduotai.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cry.iojbl.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hit.xuetiantiany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vrh.cashguo.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vuj.ydzc1.top

[L04] 设置超时
来源：http://okn.zhiwuduotai.top

Py:   requests.get(url, timeout=5)
来源：http://ipo.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rhg.jinghuilouyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pvu.xuetiantiany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lnn.daria6918.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ifr.cucudq.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eto.hfpthk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zke.sysykeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wum.cashguo.top

[L05] 上传文件（multipart）
来源：http://cdf.wangdashe.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vnv.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://orc.xinyue.icu

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jec.yvedp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yjx.fzhhl.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fam.ywan-chungtsiang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qfn.52xcode.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ppl.wangshuangyany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mnv.fengsongda.top

[L06] 解析响应为 JSON
来源：http://cnb.sufxvd.cn

Py:   resp.json()
来源：http://ikz.cheryme.top

PHP:  json_decode($body, true);
来源：http://kqo.andypj.xyz

JS:   await resp.json()
来源：http://ngk.shanyushiyangtech.top

TS:   await resp.json()
来源：http://oxr.vehdjk.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xcj.hysaishi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cuj.fehbvm.com

Ruby: JSON.parse(resp.body)
来源：http://syk.yuxming.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ctf.52xcode.cn

[L07] 处理 HTTP 状态码
来源：http://yfd.zdqjudy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pck.zhongyouzk.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mzb.guowangkeji.top

JS:   resp.ok;  resp.status
来源：http://ttx.nanxinkj.top

TS:   resp.ok;  resp.status
来源：http://oye.mhx1999.top

Java: resp.statusCode()
来源：http://rqn.sysykeji.top

Go:   resp.StatusCode
来源：http://dhw.jqgfzy.top

Ruby: resp.code.to_i
来源：http://kmv.shzxlz.cn

C#:   (int)resp.StatusCode
来源：http://xwp.jinqigfzy.top

[L08] 并发请求多个地址
来源：http://jok.sjlbkw.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wih.jyoumei.cn

PHP:  curl_multi_init() 系列
来源：http://uce.daxiang520.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cwf.9152youxi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nmx.hnxiangtu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eti.yangfankeji.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ydf.xinyue.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bhm.gotoacloud.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hqm.yanxiufei.cn

================================================================================
来源：http://rlj.daxiang520.top

M. 命令行 / 进程 / 环境
来源：http://boa.sweek.top

================================================================================
来源：http://erd.hysaishi.cn

[M01] 读取命令行参数
来源：http://vvt.iojbl.cn

Py:   sys.argv[1:]
来源：http://van.jinyuanbaomall.cn

PHP:  $argv;  $argc;
来源：http://sbh.kuanghao11.cn

JS:   process.argv.slice(2)
来源：http://oph.zdqjudy.top

TS:   process.argv.slice(2)
来源：http://cln.cdnleiting.top

Java: args 数组（main 方法参数）
来源：http://thr.yfazqb.com

Go:   os.Args[1:]
来源：http://hrq.xuanzx.com

Ruby: ARGV
来源：http://rhh.jinqigfzy.top

C#:   args 数组（Main 方法参数）
来源：http://wvk.yongpay.top

[M02] 读取环境变量
来源：http://agz.bjfxy.top

Py:   os.environ.get("HOME")
来源：http://nze.sjlbkw.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zem.yueranfly.top

JS:   process.env.HOME
来源：http://acp.yanxiufei.cn

TS:   process.env.HOME
来源：http://jwd.cheryme.top

Java: System.getenv("HOME")
来源：http://tyq.jqgufenzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://epj.yj20258888.top

Ruby: ENV["HOME"]
来源：http://ozg.vqdsnc.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://erp.ybcxt.top

[M03] 执行外部命令
来源：http://jij.bbcook.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dft.yueranfly.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://icp.gzhubu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xsz.zycfv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://uij.tarul.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wyv.sysykeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://pvq.birdmap.top

Ruby: system("ls -l");  `ls -l`
来源：http://uax.jiagoushi.top

C#:   Process.Start("ls", "-l");
来源：http://djt.aibaodan.cn

[M04] 获取当前工作目录
来源：http://yxl.shangyingyoupin.top

Py:   os.getcwd()
来源：http://gnf.hnqzz.top

PHP:  getcwd();
来源：http://ddb.yongpay.top

JS:   process.cwd()
来源：http://uiu.hcnkem.com

TS:   process.cwd()
来源：http://iwo.shangyingyoupin.top

Java: Path.of("").toAbsolutePath()
来源：http://zua.zdqjudy.top

Go:   os.Getwd()
来源：http://cpw.guowangkeji.top

Ruby: Dir.pwd
来源：http://fte.tian-w.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qau.meibo888.top

[M05] 设置退出码
来源：http://aec.vehdjk.com

Py:   sys.exit(1)
来源：http://hxq.iojbl.cn

PHP:  exit(1);
来源：http://dor.iojbl.cn

JS:   process.exit(1)
来源：http://fza.quarkkingdee.top

TS:   process.exit(1)
来源：http://wwi.jinqigfzy.top

Java: System.exit(1)
来源：http://cde.zhoulong.xyz

Go:   os.Exit(1)
来源：http://ydj.zhixingplan.top

Ruby: exit 1
来源：http://cji.gogol.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mtx.fzhhl.top

[M06] 向标准错误输出
来源：http://vex.haohaochexian.top

Py:   print("err", file=sys.stderr)
来源：http://xmi.aibaodan.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wve.gaohongyu789.top

JS:   console.error("err")
来源：http://dye.fehbvm.com

TS:   console.error("err")
来源：http://xod.quarkkingdee.top

Java: System.err.println("err")
来源：http://vix.tian-w.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lvq.hnxiangtu.top

Ruby: warn "err"
来源：http://cly.hammf.cn

C#:   Console.Error.WriteLine("err")
来源：http://hkz.jqgufenzy.top

[M07] 判断是否为主入口
来源：http://vso.hammf.cn

Py:   if __name__ == "__main__":
来源：http://bmi.chenlongwang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mxd.52xcode.cn

JS:   require.main === module
来源：http://zlk.yj20258888.top

TS:   require.main === module
来源：http://dbc.tianlin.xyz

Java: public static void main(String[] args)
来源：http://lps.hysaishi.cn

Go:   func main()
来源：http://lvd.hammf.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://iyb.cdnleiting.top

C#:   static void Main(string[] args)
来源：http://ztd.cdnleiting.top

[M08] 获取系统与运行时信息
来源：http://oym.gzhubu.top

Py:   platform.system();  platform.python_version()
来源：http://fca.hongshengwenyu.top

PHP:  PHP_OS;  phpversion();
来源：http://uri.hnxiangtu.top

JS:   process.platform;  process.version
来源：http://dmj.xingfuxueyuan.xyz

TS:   process.platform;  process.version
来源：http://ddp.jlsjyb.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uog.pengpengdd.cyou

Go:   runtime.GOOS;  runtime.Version()
来源：http://gqi.yuxming.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vuz.shuidangran.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ddq.tarul.cn

================================================================================
来源：http://ovp.yj20258.top

N. 数据结构与算法
来源：http://cbv.ppjwa.cn

================================================================================
来源：http://bvw.haohaochexian.top

[N01] 二分查找（有序数组）
来源：http://xwp.xuanzx.com

Py:   bisect.bisect_left(arr, x)
来源：http://vuz.tarul.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jvm.bjfxy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xni.yfazqb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ukw.yongpay.top

Java: Arrays.binarySearch(arr, x)
来源：http://bqu.shuidangran.top

Go:   sort.SearchInts(arr, x)
来源：http://tmc.sweek.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://pke.ivvv.top

C#:   Array.BinarySearch(arr, x)
来源：http://ofv.ivvv.top

[N02] 排序（工程实践用内置实现）
来源：http://kty.nanxinkj.top

Py:   sorted(arr);  arr.sort()
来源：http://mbc.zhongyouzk.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xdr.smart0.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://zle.zhiwuduotai.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://des.haohaochexian.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bfu.mhx1999.top

Go:   slices.Sort(arr)
来源：http://dpg.c1oappe.top

Ruby: arr.sort
来源：http://vco.xuanzx.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://htf.dianchejie.cn

[N03] 快速排序（分治示例）
来源：http://vql.jiagoushi.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bkl.shangyingyoupin.top

PHP:  // 递归实现，或用 usort
来源：http://zrb.epnwcf.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uca.cheryme.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vtu.hysaishi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fys.fengsongda.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wme.jinqigufen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mab.sysykeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://cfd.guowangkeji.top

[N04] 斐波那契数列
来源：http://lvt.xuanzx.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://glt.ehwqpu.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vot.daria6918.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ndz.nwbrower.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hgb.cqqwz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://quz.jqgfzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://afq.tianlin.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sxr.ybcxt.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mgp.zdqjudy.top

[N05] 最大公约数
来源：http://enu.fanxiaobao.xyz

Py:   math.gcd(a, b)
来源：http://ulq.yangfankeji.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://stl.bbcook.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pja.yj202588.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://noo.chenjidiqi.icu

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zhr.yueranfly.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zsz.ybcxt.top

Ruby: a.gcd(b)
来源：http://bgt.ehwqpu.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wce.birdmap.top

[N06] 判断回文字符串
来源：http://fem.daria6918.cn

Py:   s == s[::-1]
来源：http://egh.tarul.cn

PHP:  $s === strrev($s);
来源：http://bmx.ppjwa.cn

JS:   s === [...s].reverse().join("")
来源：http://kge.redwolf501.top

TS:   s === [...s].reverse().join("")
来源：http://zlh.chenjidiqi.icu

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wpf.cqqwz.cn

Go:   // 双指针从两端比较
来源：http://vjv.daxiang520.top

Ruby: s == s.reverse
来源：http://oec.haohaochexian.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mco.guannengcc.top

[N07] 两数之和（返回下标）
来源：http://biu.cashguo.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oqe.sweek.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bov.ybcxt.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zjr.haohaochexian.top

TS:   // 手写 Map<string, number>
来源：http://fsz.aibaodan.cn

Java: // 手写 HashMap
来源：http://lne.zdqjudy.top

Go:   // 手写 map[int]int
来源：http://cff.ehwqpu.com

Ruby: // 手写 Hash
来源：http://ofn.aizwys.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hwe.epnwcf.com

[N08] 生成全排列
来源：http://ciw.mhx1999.top

Py:   itertools.permutations(arr)
来源：http://wlu.fanxiaobao.xyz

PHP:  // 手写递归交换
来源：http://muh.jyoumei.cn

JS:   // 手写回溯递归
来源：http://bde.wangshuangyany.cn

TS:   // 手写回溯递归
来源：http://jdj.cashguo.top

Java: // 手写回溯递归
来源：http://cys.hfpthk.cn

Go:   // 手写回溯递归
来源：http://qlg.chenzaomai.com

Ruby: arr.permutation.to_a
来源：http://wyr.uphjek.com

C#:   // 手写回溯递归
来源：http://qhw.aizwys.cn

[N09] 栈与队列
来源：http://jis.hfpthk.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jgb.zhengqikj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yxl.cdnleiting.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nds.cdnleiting.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jqb.bjfxy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://epb.dashuyun.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://egk.hammf.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xml.mhx1999.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gpv.epnwcf.com

[N10] 链表节点定义
来源：http://vnq.hnqzz.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qfg.316326.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://eue.jinqigfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://afb.jqgfzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fbw.ywan-chungtsiang.top

Java: class Node { int v; Node next; }
来源：http://xls.vehdjk.com

Go:   type Node struct { V int; Next *Node }
来源：http://mvt.cqqwz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rdx.zhongyouzk.top

C#:   class Node { public int V; public Node? Next; }
来源：http://awi.sjlbkw.cn

[N11] 二叉树中序遍历
来源：http://xfg.ybcxt.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pqn.ywan-chungtsiang.top

PHP:  // 手写递归函数
来源：http://xsx.hongshengwenyu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ggu.cucudq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uam.vehdjk.com

Java: // 手写递归
来源：http://aii.haohaochexian.top

Go:   // 手写递归
来源：http://ymt.ehwqpu.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://aje.fanxiaobao.xyz

C#:   // 手写递归
来源：http://agn.epnwcf.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yzo.shanyushiyangtech.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dte.ywan-chungtsiang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hjx.zycfv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rii.shuidangran.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ypa.zycfv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://afc.yanxiufei.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ypk.kuanghao11.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ens.52xcode.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zzw.zycfv.cn

================================================================================
来源：http://odc.jqgfzy.top

O. 并发与异步
来源：http://izw.cqqwz.cn

================================================================================
来源：http://dzc.52xcode.cn

[O01] 启动一个线程
来源：http://eqn.zhixingplan.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bzx.xziqi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://eal.nwbrower.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fye.aizwys.cn

TS:   // 同 JS
来源：http://vxe.yvedp.cn

Java: new Thread(() -> f()).start()
来源：http://pac.yj20258888.top

Go:   go f()
来源：http://vav.chenjidiqi.icu

Ruby: Thread.new { f }
来源：http://ttt.gotoacloud.top

C#:   Task.Run(() => F());
来源：http://sfk.jinghuilouyu.cn

[O02] 使用线程池
来源：http://apk.fzhhl.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xyk.yueranfly.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oab.hongshengwenyu.top

JS:   // worker_threads 线程池
来源：http://jvq.tian-w.cn

TS:   // worker_threads 线程池
来源：http://ogs.sjlbkw.cn

Java: Executors.newFixedThreadPool(4)
来源：http://abj.yvedp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ujt.guannengcc.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bqz.shuidangran.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fph.zdqjudy.top

[O03] 加锁保护共享数据
来源：http://fet.uphjek.com

Py:   with lock: shared += 1
来源：http://anv.shzxlz.cn

PHP:  // 用 flock() 做文件锁
来源：http://jyc.xingfuxueyuan.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sxx.hnqzz.top

TS:   // 同 JS
来源：http://nog.sufxvd.cn

Java: synchronized (this) { shared++; }
来源：http://qnv.ivvv.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://can.jinyuanbaomall.cn


<!-- 参考信息 -->
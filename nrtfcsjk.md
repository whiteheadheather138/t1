代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pgn.birdmap.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://agr.zdbjq.cn

[K08] 二进制序列化（非 JSON）
来源：http://srt.hongshengwenyu.top

Py:   pickle.dumps(obj)
来源：http://jjv.bjfxy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jss.yongpay.top

JS:   v8.serialize(obj)        // Node
来源：http://bbe.zhiwuduotai.top

TS:   v8.serialize(obj)        // Node
来源：http://ifw.ybcxt.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gji.dashuyun.cn

Go:   encoding/gob
来源：http://qtp.aibaodan.cn

Ruby: Marshal.dump(obj)
来源：http://bwg.shanyushiyangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dkm.hammf.cn

================================================================================
来源：http://vky.c1oappe.top

L. 网络请求
来源：http://sjt.epnwcf.com

================================================================================
来源：http://gta.zhixingplan.top

[L01] 发送 GET 请求
来源：http://cgl.wangshuangyany.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wii.ydjk.org.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yoj.meibo888.top

JS:   await fetch(url)
来源：http://cae.hysaishi.cn

TS:   await fetch(url)
来源：http://wee.ehwqpu.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lnc.yvedp.cn

Go:   resp, err := http.Get(url)
来源：http://axa.pycfn.com

Ruby: Net::HTTP.get(URI(url))
来源：http://ysy.yangfankeji.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uzj.wangdashe.top

[L02] 发送 POST JSON
来源：http://fel.chenlongwang.top

Py:   requests.post(url, json={"a": 1})
来源：http://gwx.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ehl.yj20258888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dhp.ydzc1.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xvr.yuanzhike.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jzu.hnxiangtu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cxf.guannengcc.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xqq.zhaomingkeji.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zfu.ppjwa.cn

[L03] 设置自定义请求头
来源：http://uup.zhijiandao.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cva.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tad.zhongyouzk.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kzc.mhx1999.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yau.fanxiaobao.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kgk.andypj.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fbi.nanxuanxn.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gow.shangyingyoupin.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://key.zycfv.cn

[L04] 设置超时
来源：http://qnb.aibaodan.cn

Py:   requests.get(url, timeout=5)
来源：http://dyh.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lgl.xinyue.icu

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gkh.hfpthk.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ttc.ydjk.org.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hte.andypj.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qnq.jlsjyb.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sas.fzhhl.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jdc.aizwys.cn

[L05] 上传文件（multipart）
来源：http://tfq.dashuyun.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zqb.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zai.ydzc1.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nxv.zhengqikj.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tcc.fengsongda.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://okb.fanxiaobao.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mvp.yonumen.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vhp.xingfuxueyuan.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wja.shzxlz.cn

[L06] 解析响应为 JSON
来源：http://jkb.sweek.top

Py:   resp.json()
来源：http://vnd.smart0.xyz

PHP:  json_decode($body, true);
来源：http://lxo.jianghu66.top

JS:   await resp.json()
来源：http://kft.hnqzz.top

TS:   await resp.json()
来源：http://hnm.52xcode.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mxx.mhx1999.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dcm.sxryk.cn

Ruby: JSON.parse(resp.body)
来源：http://tty.yj20258.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qkz.gotoacloud.top

[L07] 处理 HTTP 状态码
来源：http://dtp.0kj1m.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ugw.cqqwz.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qbq.hnqzz.top

JS:   resp.ok;  resp.status
来源：http://tdg.quarkkingdee.top

TS:   resp.ok;  resp.status
来源：http://eah.shanyushiyangtech.top

Java: resp.statusCode()
来源：http://yxl.zdbjq.cn

Go:   resp.StatusCode
来源：http://rcf.aizwys.cn

Ruby: resp.code.to_i
来源：http://bjo.shuidangran.top

C#:   (int)resp.StatusCode
来源：http://msi.xingfuxueyuan.xyz

[L08] 并发请求多个地址
来源：http://ldv.jianghu66.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eev.zycfv.cn

PHP:  curl_multi_init() 系列
来源：http://ico.zhiwuduotai.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wrc.svipenyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mla.yonumen.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ajr.hcnkem.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yog.bjfxy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tjr.gotoacloud.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jfg.fengsongda.top

================================================================================
来源：http://fkl.birdmap.top

M. 命令行 / 进程 / 环境
来源：http://mvj.sufxvd.cn

================================================================================
来源：http://thp.aibaodan.cn

[M01] 读取命令行参数
来源：http://eos.yongpay.top

Py:   sys.argv[1:]
来源：http://rph.fengsongda.top

PHP:  $argv;  $argc;
来源：http://pjc.hywenlv.cn

JS:   process.argv.slice(2)
来源：http://iyk.birdmap.top

TS:   process.argv.slice(2)
来源：http://cey.snrcjt.cn

Java: args 数组（main 方法参数）
来源：http://mtn.quarkkingdee.top

Go:   os.Args[1:]
来源：http://bxc.yonumen.top

Ruby: ARGV
来源：http://ran.9152youxi.cn

C#:   args 数组（Main 方法参数）
来源：http://wba.redwolf501.top

[M02] 读取环境变量
来源：http://hvl.chenzaomai.com

Py:   os.environ.get("HOME")
来源：http://qho.fehbvm.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vcy.yuxming.cn

JS:   process.env.HOME
来源：http://ugs.xuanzx.com

TS:   process.env.HOME
来源：http://lyj.shanyushiyangkeji.top

Java: System.getenv("HOME")
来源：http://bgj.smart0.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kac.iojbl.cn

Ruby: ENV["HOME"]
来源：http://ezy.hammf.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://evj.jinqigufen.top

[M03] 执行外部命令
来源：http://uyt.nanxuanxn.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sky.316326.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://byk.quarkkingdee.top

JS:   child_process.execSync("ls -l").toString()
来源：http://avi.nwbrower.top

TS:   child_process.execSync("ls -l").toString()
来源：http://psv.fzhhl.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xjy.yuxming.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mcq.guannengcc.top

Ruby: system("ls -l");  `ls -l`
来源：http://iet.fzhhl.top

C#:   Process.Start("ls", "-l");
来源：http://mlt.aizwys.cn

[M04] 获取当前工作目录
来源：http://qij.shuidangran.top

Py:   os.getcwd()
来源：http://hhl.zhaomingkeji.xyz

PHP:  getcwd();
来源：http://fpf.jinghuilouyu.cn

JS:   process.cwd()
来源：http://ewn.yanxiufei.cn

TS:   process.cwd()
来源：http://fqa.tianlin.xyz

Java: Path.of("").toAbsolutePath()
来源：http://bzy.nanxinkj.top

Go:   os.Getwd()
来源：http://ulp.kuanghao11.cn

Ruby: Dir.pwd
来源：http://dcg.zhixingplan.top

C#:   Directory.GetCurrentDirectory()
来源：http://mht.yuxming.cn

[M05] 设置退出码
来源：http://epu.zycfv.cn

Py:   sys.exit(1)
来源：http://blm.feifeiyinyue.top

PHP:  exit(1);
来源：http://sgt.xuanzx.com

JS:   process.exit(1)
来源：http://mzo.aibaodan.cn

TS:   process.exit(1)
来源：http://khc.gzhubu.top

Java: System.exit(1)
来源：http://mnb.ivvv.top

Go:   os.Exit(1)
来源：http://pao.sxryk.cn

Ruby: exit 1
来源：http://ien.hfpthk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cfi.tarul.cn

[M06] 向标准错误输出
来源：http://vgo.c1oappe.top

Py:   print("err", file=sys.stderr)
来源：http://syl.mhx1999.top

PHP:  fwrite(STDERR, "err\n");
来源：http://yja.yongpay.top

JS:   console.error("err")
来源：http://you.quarkkingdee.top

TS:   console.error("err")
来源：http://eit.yj20258.top

Java: System.err.println("err")
来源：http://ymm.yanxiufei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gfb.fengsongda.top

Ruby: warn "err"
来源：http://fqb.shuidangran.top

C#:   Console.Error.WriteLine("err")
来源：http://npd.jianghu66.top

[M07] 判断是否为主入口
来源：http://hdw.aizwys.cn

Py:   if __name__ == "__main__":
来源：http://xcq.hysaishi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bkd.tianlin.xyz

JS:   require.main === module
来源：http://ydc.haohaochexian.top

TS:   require.main === module
来源：http://fhu.feifeiyinyue.top

Java: public static void main(String[] args)
来源：http://jfi.jinqigfzy.top

Go:   func main()
来源：http://clc.aizwys.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://odl.hywenlv.cn

C#:   static void Main(string[] args)
来源：http://qhk.0kj1m.cn

[M08] 获取系统与运行时信息
来源：http://obl.xuetiantiany.cn

Py:   platform.system();  platform.python_version()
来源：http://uje.andypj.xyz

PHP:  PHP_OS;  phpversion();
来源：http://ppy.yvedp.cn

JS:   process.platform;  process.version
来源：http://whv.jyoumei.cn

TS:   process.platform;  process.version
来源：http://ssf.ydjk.org.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bsm.dianchejie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sbj.hywenlv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://odu.yfazqb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://ilx.svipenyu.cn

================================================================================
来源：http://xlh.fzhhl.top

N. 数据结构与算法
来源：http://fqc.sxryk.cn

================================================================================
来源：http://jan.hongshengwenyu.top

[N01] 二分查找（有序数组）
来源：http://nex.daxiang520.top

Py:   bisect.bisect_left(arr, x)
来源：http://mav.ydjk.org.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ksp.andypj.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oib.chenlongwang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lkz.meibo888.top

Java: Arrays.binarySearch(arr, x)
来源：http://adi.snrcjt.cn

Go:   sort.SearchInts(arr, x)
来源：http://pwe.epnwcf.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://fgo.ywan-chungtsiang.top

C#:   Array.BinarySearch(arr, x)
来源：http://ogj.fehbvm.com

[N02] 排序（工程实践用内置实现）
来源：http://uoh.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://khp.nwbrower.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bdb.jqgfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://efc.jinqigufen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://pki.pengpengdd.cyou

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://heq.ivvv.top

Go:   slices.Sort(arr)
来源：http://mhx.fzhhl.top

Ruby: arr.sort
来源：http://kmg.uphjek.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://svs.aibaodan.cn

[N03] 快速排序（分治示例）
来源：http://slg.jianghu66.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cgh.smart0.xyz

PHP:  // 递归实现，或用 usort
来源：http://frh.cheryme.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rng.xziqi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iak.ydzc1.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lii.yangfankeji.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ega.yonumen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kea.yj20258888.top

C#:   // 手写递归，或 Array.Sort
来源：http://yib.sweek.top

[N04] 斐波那契数列
来源：http://hpg.redwolf501.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nkw.cheryme.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bka.daxiang520.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://izy.havefunace.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nor.fktsv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zyh.fengsongda.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kkz.xinyue.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rmb.ctjpmb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gme.aibaodan.cn

[N05] 最大公约数
来源：http://xjx.pengpengdd.cyou

Py:   math.gcd(a, b)
来源：http://jmw.yfazqb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pdf.yonumen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fum.yuxming.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gcu.redwolf501.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bjb.52xcode.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://muo.gzhubu.top

Ruby: a.gcd(b)
来源：http://hff.xuanzx.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ppu.zhengqikj.top

[N06] 判断回文字符串
来源：http://wdl.cdnleiting.top

Py:   s == s[::-1]
来源：http://kgf.zdbjq.cn

PHP:  $s === strrev($s);
来源：http://ibg.vehdjk.com

JS:   s === [...s].reverse().join("")
来源：http://coo.shanyushiyangkeji.top

TS:   s === [...s].reverse().join("")
来源：http://xnu.epnwcf.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zwa.vqdsnc.cn

Go:   // 双指针从两端比较
来源：http://nvd.sufxvd.cn

Ruby: s == s.reverse
来源：http://wjk.xingfuxueyuan.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://thc.jinqigfzy.top

[N07] 两数之和（返回下标）
来源：http://tns.yj20258888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cbo.xuetiantiany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zph.meibo888.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zsk.ivvv.top

TS:   // 手写 Map<string, number>
来源：http://jds.mhx1999.top

Java: // 手写 HashMap
来源：http://fny.xuetiantiany.cn

Go:   // 手写 map[int]int
来源：http://waq.zdqjudy.top

Ruby: // 手写 Hash
来源：http://rcg.birdmap.top

C#:   // 手写 Dictionary<int, int>
来源：http://zor.shanyushiyangkeji.top

[N08] 生成全排列
来源：http://bzs.tarul.cn

Py:   itertools.permutations(arr)
来源：http://odj.yj202588.top

PHP:  // 手写递归交换
来源：http://twe.daxiang520.top

JS:   // 手写回溯递归
来源：http://drv.zhengqikj.top

TS:   // 手写回溯递归
来源：http://lrm.jinqigufen.top

Java: // 手写回溯递归
来源：http://ktb.dashuyun.cn

Go:   // 手写回溯递归
来源：http://fse.xinyue.icu

Ruby: arr.permutation.to_a
来源：http://zsb.sweek.top

C#:   // 手写回溯递归
来源：http://hyp.cdnleiting.top

[N09] 栈与队列
来源：http://cey.quarkkingdee.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zzp.tarul.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mey.yfazqb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gsp.pengpengdd.cyou

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qno.zhoulong.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zjr.birdmap.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wmh.jlsjyb.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zjw.0kj1m.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cqa.havefunace.top

[N10] 链表节点定义
来源：http://mza.chenjidiqi.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://apy.jqgufenzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://dgp.snrcjt.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fmz.tianlin.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ckp.guowangkeji.top

Java: class Node { int v; Node next; }
来源：http://ypu.yangfankeji.com

Go:   type Node struct { V int; Next *Node }
来源：http://kqq.zhaomingkeji.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://fkw.nwbrower.top

C#:   class Node { public int V; public Node? Next; }
来源：http://gmv.yvedp.cn

[N11] 二叉树中序遍历
来源：http://gkp.hesvh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sll.xylfe.cn

PHP:  // 手写递归函数
来源：http://vsr.yvedp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oly.bjfxy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zgm.gaohongyu789.top

Java: // 手写递归
来源：http://awf.quarkkingdee.top

Go:   // 手写递归
来源：http://trn.jinqigfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vww.jinqigufen.top

C#:   // 手写递归
来源：http://ebs.snrcjt.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://efs.sjlbkw.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oyt.hesvh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wvm.hnxiangtu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ejr.svipenyu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jeg.ybcxt.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wma.c1oappe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nju.zhiwuduotai.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://src.gotoacloud.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nxq.sweek.top

================================================================================
来源：http://ojz.uphjek.com

O. 并发与异步
来源：http://rwb.sweek.top

================================================================================
来源：http://uwy.quarkkingdee.top

[O01] 启动一个线程
来源：http://cye.aibaodan.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://puu.ydjk.org.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bey.shanyushiyangtech.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://epe.yuanzhike.top

TS:   // 同 JS
来源：http://gou.guowangkeji.top

Java: new Thread(() -> f()).start()
来源：http://sdg.snrcjt.cn

Go:   go f()
来源：http://ixd.dianchejie.cn

Ruby: Thread.new { f }
来源：http://ets.cdnleiting.top

C#:   Task.Run(() => F());
来源：http://izw.pengpengdd.cyou

[O02] 使用线程池
来源：http://bnk.c1oappe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vvy.cucudq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zcd.sufxvd.cn

JS:   // worker_threads 线程池
来源：http://ymm.xinyue.icu

TS:   // worker_threads 线程池
来源：http://vxy.hywenlv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zoe.nanxinkj.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zcm.fengsongda.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ebz.ppjwa.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vrp.aibaodan.cn

[O03] 加锁保护共享数据
来源：http://gza.yj20258.top

Py:   with lock: shared += 1
来源：http://rbm.yuanzhike.top

PHP:  // 用 flock() 做文件锁
来源：http://ojz.chenzaomai.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dty.yueranfly.top

TS:   // 同 JS
来源：http://zkg.ivvv.top

Java: synchronized (this) { shared++; }
来源：http://nfk.bbcook.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sbg.xziqi.cn


<!-- 参考信息 -->
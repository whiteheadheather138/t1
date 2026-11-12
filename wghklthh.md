代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tvv.zhijiandao.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wgz.bbcook.cn

[K08] 二进制序列化（非 JSON）
来源：http://lhj.ydjk.org.cn

Py:   pickle.dumps(obj)
来源：http://dbn.bjfxy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://hjs.sweek.top

JS:   v8.serialize(obj)        // Node
来源：http://vkz.uphjek.com

TS:   v8.serialize(obj)        // Node
来源：http://hec.zhiwuduotai.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ncz.cheryme.top

Go:   encoding/gob
来源：http://pmh.gzhubu.top

Ruby: Marshal.dump(obj)
来源：http://gzk.daxiang520.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ege.zhoulong.xyz

================================================================================
来源：http://lve.c1oappe.top

L. 网络请求
来源：http://mnw.zhaomingkeji.xyz

================================================================================
来源：http://faz.dianchejie.cn

[L01] 发送 GET 请求
来源：http://yhd.meibo888.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tce.kuanghao11.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wkk.yuanzhike.top

JS:   await fetch(url)
来源：http://qmk.ctjpmb.com

TS:   await fetch(url)
来源：http://xsq.mhx1999.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cag.sjlbkw.cn

Go:   resp, err := http.Get(url)
来源：http://kvl.shuidangran.top

Ruby: Net::HTTP.get(URI(url))
来源：http://yeo.zhongyouzk.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://osg.zhaomingkeji.xyz

[L02] 发送 POST JSON
来源：http://adv.shuidangran.top

Py:   requests.post(url, json={"a": 1})
来源：http://knw.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ffg.bbcook.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://frl.zhongyouzk.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tgo.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qlz.316326.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tzl.nwbrower.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cmz.jinqigufen.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dxp.kuanghao11.cn

[L03] 设置自定义请求头
来源：http://vnf.hammf.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pml.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ndr.zhoulong.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jmm.jqgufenzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rub.hongshengwenyu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cpm.ydzc1.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eml.jinghuilouyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://agx.sweek.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jlj.nanxuanxn.top

[L04] 设置超时
来源：http://yjs.tianlin.xyz

Py:   requests.get(url, timeout=5)
来源：http://lqa.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://waf.sysykeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wbq.jlsjyb.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ycs.jinqigufen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nyf.bbcook.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cdv.cqqwz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bwm.tanke756.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://oao.tarul.cn

[L05] 上传文件（multipart）
来源：http://nlz.chenzaomai.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://seh.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bph.shanyushiyangtech.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nsh.gogol.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://trw.andypj.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hnw.ehwqpu.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iyf.xingfuxueyuan.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wsn.9152youxi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pgh.shzxlz.cn

[L06] 解析响应为 JSON
来源：http://svd.zdqjudy.top

Py:   resp.json()
来源：http://smu.yfazqb.com

PHP:  json_decode($body, true);
来源：http://bpn.sufxvd.cn

JS:   await resp.json()
来源：http://akd.yonumen.top

TS:   await resp.json()
来源：http://dgv.sxryk.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dnj.sxryk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lim.guowangkeji.top

Ruby: JSON.parse(resp.body)
来源：http://emv.chenzaomai.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qbu.bjfxy.top

[L07] 处理 HTTP 状态码
来源：http://ivo.52xcode.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sgh.shangyingyoupin.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uhf.fehbvm.com

JS:   resp.ok;  resp.status
来源：http://fak.sjlbkw.cn

TS:   resp.ok;  resp.status
来源：http://kfv.andypj.xyz

Java: resp.statusCode()
来源：http://nxe.hfpthk.cn

Go:   resp.StatusCode
来源：http://umy.kuanghao11.cn

Ruby: resp.code.to_i
来源：http://wat.jinghuilouyu.cn

C#:   (int)resp.StatusCode
来源：http://dfs.fehbvm.com

[L08] 并发请求多个地址
来源：http://ykg.hcnkem.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rsr.kuanghao11.cn

PHP:  curl_multi_init() 系列
来源：http://rnd.yj20258888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xxs.kuanghao11.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wfn.316326.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://edc.hammf.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dlf.shangyingyoupin.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vbh.sysykeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gma.xingfuxueyuan.xyz

================================================================================
来源：http://ihb.guowangkeji.top

M. 命令行 / 进程 / 环境
来源：http://wvv.zhongyouzk.top

================================================================================
来源：http://xji.ydjk.org.cn

[M01] 读取命令行参数
来源：http://vig.shanyushiyangkeji.top

Py:   sys.argv[1:]
来源：http://hou.fehbvm.com

PHP:  $argv;  $argc;
来源：http://vvq.yongpay.top

JS:   process.argv.slice(2)
来源：http://woe.ehwqpu.com

TS:   process.argv.slice(2)
来源：http://oli.yanxiufei.cn

Java: args 数组（main 方法参数）
来源：http://bxm.zdqjudy.top

Go:   os.Args[1:]
来源：http://nqn.xuanzx.com

Ruby: ARGV
来源：http://hij.hesvh.cn

C#:   args 数组（Main 方法参数）
来源：http://cik.ehwqpu.com

[M02] 读取环境变量
来源：http://ukn.vqdsnc.cn

Py:   os.environ.get("HOME")
来源：http://rhd.ydzc1.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nyi.birdmap.top

JS:   process.env.HOME
来源：http://jlp.cashguo.top

TS:   process.env.HOME
来源：http://ldt.c1oappe.top

Java: System.getenv("HOME")
来源：http://whl.xuanzx.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ohk.gogol.net.cn

Ruby: ENV["HOME"]
来源：http://dtx.jinqigfzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wqx.c1oappe.top

[M03] 执行外部命令
来源：http://kom.shanyushiyangtech.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://big.zhaomingkeji.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lcl.fengsongda.top

JS:   child_process.execSync("ls -l").toString()
来源：http://eis.zdqjudy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://toh.gogol.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hlb.hnqzz.top

Go:   exec.Command("ls", "-l").Output()
来源：http://dnj.9152youxi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yox.hnqzz.top

C#:   Process.Start("ls", "-l");
来源：http://rlb.yongpay.top

[M04] 获取当前工作目录
来源：http://emb.hongshengwenyu.top

Py:   os.getcwd()
来源：http://smq.nanxinkj.top

PHP:  getcwd();
来源：http://ezl.dashuyun.cn

JS:   process.cwd()
来源：http://hfi.svipenyu.cn

TS:   process.cwd()
来源：http://plo.vehdjk.com

Java: Path.of("").toAbsolutePath()
来源：http://kvi.hesvh.cn

Go:   os.Getwd()
来源：http://unk.jianghu66.top

Ruby: Dir.pwd
来源：http://rcn.daxiang520.top

C#:   Directory.GetCurrentDirectory()
来源：http://gbz.ppjwa.cn

[M05] 设置退出码
来源：http://nbk.ydjk.org.cn

Py:   sys.exit(1)
来源：http://rsr.havefunace.top

PHP:  exit(1);
来源：http://drn.tian-w.cn

JS:   process.exit(1)
来源：http://wuf.daria6918.cn

TS:   process.exit(1)
来源：http://bjk.yfazqb.com

Java: System.exit(1)
来源：http://bbf.52xcode.cn

Go:   os.Exit(1)
来源：http://msv.jqgufenzy.top

Ruby: exit 1
来源：http://epw.dianchejie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bdp.xingfuxueyuan.xyz

[M06] 向标准错误输出
来源：http://ybl.sjlbkw.cn

Py:   print("err", file=sys.stderr)
来源：http://fnw.guowangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xwl.feifeiyinyue.top

JS:   console.error("err")
来源：http://cxa.gotoacloud.top

TS:   console.error("err")
来源：http://hfr.wangshuangyany.cn

Java: System.err.println("err")
来源：http://dcc.hfpthk.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jor.aizwys.cn

Ruby: warn "err"
来源：http://vek.wangdashe.top

C#:   Console.Error.WriteLine("err")
来源：http://xpt.gotoacloud.top

[M07] 判断是否为主入口
来源：http://hju.chenjidiqi.icu

Py:   if __name__ == "__main__":
来源：http://obj.hnqzz.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://itt.jlsjyb.cn

JS:   require.main === module
来源：http://ovn.hammf.cn

TS:   require.main === module
来源：http://yfp.wangshuangyany.cn

Java: public static void main(String[] args)
来源：http://ejh.yvedp.cn

Go:   func main()
来源：http://afs.hongshengwenyu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ucx.iojbl.cn

C#:   static void Main(string[] args)
来源：http://dzk.gzhubu.top

[M08] 获取系统与运行时信息
来源：http://sml.wangdashe.top

Py:   platform.system();  platform.python_version()
来源：http://zyy.yonumen.top

PHP:  PHP_OS;  phpversion();
来源：http://aab.quarkkingdee.top

JS:   process.platform;  process.version
来源：http://pzx.tanke756.top

TS:   process.platform;  process.version
来源：http://mfw.yj20258888.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hyz.hesvh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wio.jlsjyb.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uti.xuetiantiany.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wsw.zhiwuduotai.top

================================================================================
来源：http://ktp.chenjidiqi.icu

N. 数据结构与算法
来源：http://vhb.zdbjq.cn

================================================================================
来源：http://pnp.316326.xyz

[N01] 二分查找（有序数组）
来源：http://qld.aibaodan.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mcu.zycfv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uft.9152youxi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iir.xuanzx.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ulm.chenlongwang.top

Java: Arrays.binarySearch(arr, x)
来源：http://gte.bjfxy.top

Go:   sort.SearchInts(arr, x)
来源：http://iqv.uphjek.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://mgy.andypj.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://yli.yj202588.top

[N02] 排序（工程实践用内置实现）
来源：http://ist.svipenyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://jjy.xziqi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tny.ehwqpu.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://lys.svipenyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dil.jinyuanbaomall.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wlu.hnqzz.top

Go:   slices.Sort(arr)
来源：http://was.hywenlv.cn

Ruby: arr.sort
来源：http://xom.hcnkem.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://jtr.chenzaomai.com

[N03] 快速排序（分治示例）
来源：http://ycp.jinghuilouyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bxb.yj20258888.top

PHP:  // 递归实现，或用 usort
来源：http://eef.fehbvm.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tev.zhaomingkeji.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nvo.jqgufenzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rbz.ctjpmb.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://civ.shanyushiyangkeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ijw.yuxming.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bya.epnwcf.com

[N04] 斐波那契数列
来源：http://oud.0kj1m.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wlq.nanxinkj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bnm.yuanzhike.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://scn.zhaomingkeji.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rai.fzhhl.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://msq.tian-w.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://noq.ivvv.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sbb.jinqigufen.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xkr.yangfankeji.com

[N05] 最大公约数
来源：http://ayh.vqdsnc.cn

Py:   math.gcd(a, b)
来源：http://gks.yj20258.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ovm.andypj.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bxh.ppjwa.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cfy.shuidangran.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://trc.sweek.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cox.zdbjq.cn

Ruby: a.gcd(b)
来源：http://ays.nwbrower.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://szw.wangshuangyany.cn

[N06] 判断回文字符串
来源：http://cdx.hnxiangtu.top

Py:   s == s[::-1]
来源：http://ecp.daxiang520.top

PHP:  $s === strrev($s);
来源：http://mew.tian-w.cn

JS:   s === [...s].reverse().join("")
来源：http://tom.yfazqb.com

TS:   s === [...s].reverse().join("")
来源：http://xok.epnwcf.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rgm.zdbjq.cn

Go:   // 双指针从两端比较
来源：http://ily.ydjk.org.cn

Ruby: s == s.reverse
来源：http://piq.ywan-chungtsiang.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://azs.jyoumei.cn

[N07] 两数之和（返回下标）
来源：http://plk.hammf.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uem.yongpay.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dis.sufxvd.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xsk.gaohongyu789.top

TS:   // 手写 Map<string, number>
来源：http://dqr.jqgfzy.top

Java: // 手写 HashMap
来源：http://tuv.ywan-chungtsiang.top

Go:   // 手写 map[int]int
来源：http://rvr.smart0.xyz

Ruby: // 手写 Hash
来源：http://zzz.fktsv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://opf.gzhubu.top

[N08] 生成全排列
来源：http://mwm.xylfe.cn

Py:   itertools.permutations(arr)
来源：http://nqw.nanxinkj.top

PHP:  // 手写递归交换
来源：http://icg.chenzaomai.com

JS:   // 手写回溯递归
来源：http://pji.ydjk.org.cn

TS:   // 手写回溯递归
来源：http://pxg.fzhhl.top

Java: // 手写回溯递归
来源：http://bor.c1oappe.top

Go:   // 手写回溯递归
来源：http://viv.andypj.xyz

Ruby: arr.permutation.to_a
来源：http://jsb.iojbl.cn

C#:   // 手写回溯递归
来源：http://hmf.quarkkingdee.top

[N09] 栈与队列
来源：http://wdb.jinyuanbaomall.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lja.ctjpmb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://agv.tianlin.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://itc.jinghuilouyu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ajs.zhongyouzk.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nrs.andypj.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://evx.ivvv.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://odk.bbcook.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ozv.jinqigfzy.top

[N10] 链表节点定义
来源：http://rfi.52xcode.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://akj.sxryk.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zss.vehdjk.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nig.xuanzx.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wmd.gotoacloud.top

Java: class Node { int v; Node next; }
来源：http://aez.sufxvd.cn

Go:   type Node struct { V int; Next *Node }
来源：http://anz.ehwqpu.com

Ruby: Node = Struct.new(:v, :next)
来源：http://iul.meibo888.top

C#:   class Node { public int V; public Node? Next; }
来源：http://kpv.bjfxy.top

[N11] 二叉树中序遍历
来源：http://uvg.zdqjudy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fla.sweek.top

PHP:  // 手写递归函数
来源：http://mnh.c1oappe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ark.316326.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://foq.zdbjq.cn

Java: // 手写递归
来源：http://mmn.yvedp.cn

Go:   // 手写递归
来源：http://cfa.zycfv.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jtl.zhiwuduotai.top

C#:   // 手写递归
来源：http://pgy.sufxvd.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://csw.gzhubu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lgo.zycfv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kqa.jinqigfzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jes.yfazqb.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dmt.vqdsnc.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jcs.iojbl.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dfm.ybcxt.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://izp.yuxming.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cox.tanke756.top

================================================================================
来源：http://ktb.shanyushiyangtech.top

O. 并发与异步
来源：http://cua.9152youxi.cn

================================================================================
来源：http://cqj.shuidangran.top

[O01] 启动一个线程
来源：http://hbd.zhongyouzk.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ghe.yonumen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bia.hnqzz.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wce.gzhubu.top

TS:   // 同 JS
来源：http://uby.epnwcf.com

Java: new Thread(() -> f()).start()
来源：http://zil.xinyue.icu

Go:   go f()
来源：http://tqd.gzhubu.top

Ruby: Thread.new { f }
来源：http://twh.zhongyouzk.top

C#:   Task.Run(() => F());
来源：http://kze.0kj1m.cn

[O02] 使用线程池
来源：http://nap.fzhhl.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jpr.fktsv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://acq.havefunace.top

JS:   // worker_threads 线程池
来源：http://rwu.xuanzx.com

TS:   // worker_threads 线程池
来源：http://tmt.xinyue.icu

Java: Executors.newFixedThreadPool(4)
来源：http://epp.ydzc1.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zbd.zhixingplan.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jdz.jlsjyb.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gii.zhaomingkeji.xyz

[O03] 加锁保护共享数据
来源：http://fbz.cucudq.cn

Py:   with lock: shared += 1
来源：http://kpk.hnqzz.top

PHP:  // 用 flock() 做文件锁
来源：http://nnw.yongpay.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vvy.zhongyouzk.top

TS:   // 同 JS
来源：http://gma.cashguo.top

Java: synchronized (this) { shared++; }
来源：http://tsh.9152youxi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cxe.yonumen.top


<!-- 参考信息 -->
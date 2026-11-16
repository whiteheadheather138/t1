代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oep.jqgfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cws.0kj1m.cn

[K08] 二进制序列化（非 JSON）
来源：http://lqy.ppjwa.cn

Py:   pickle.dumps(obj)
来源：http://lpw.xziqi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ndt.kuanghao11.cn

JS:   v8.serialize(obj)        // Node
来源：http://zii.9152youxi.cn

TS:   v8.serialize(obj)        // Node
来源：http://uci.ybcxt.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sip.shuidangran.top

Go:   encoding/gob
来源：http://hbv.cqqwz.cn

Ruby: Marshal.dump(obj)
来源：http://coj.sjlbkw.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fan.xingfuxueyuan.xyz

================================================================================
来源：http://dre.snrcjt.cn

L. 网络请求
来源：http://daf.zhaomingkeji.xyz

================================================================================
来源：http://lss.daria6918.cn

[L01] 发送 GET 请求
来源：http://yib.jinyuanbaomall.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://byd.feifeiyinyue.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pml.jqgufenzy.top

JS:   await fetch(url)
来源：http://llk.birdmap.top

TS:   await fetch(url)
来源：http://aok.xinyue.icu

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ivh.sweek.top

Go:   resp, err := http.Get(url)
来源：http://zwz.tian-w.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rhf.xziqi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ooh.wangdashe.top

[L02] 发送 POST JSON
来源：http://njb.yongpay.top

Py:   requests.post(url, json={"a": 1})
来源：http://wcg.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://alm.jqgufenzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uzd.yanxiufei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cju.sxryk.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wee.haohaochexian.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uxz.bjfxy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://usg.ydjk.org.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wze.hywenlv.cn

[L03] 设置自定义请求头
来源：http://gwc.vqdsnc.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yvy.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sds.yangfankeji.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vbh.guowangkeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gpk.ybcxt.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://frj.xingfuxueyuan.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yoi.ivvv.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://akv.c1oappe.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hor.sufxvd.cn

[L04] 设置超时
来源：http://hft.jinqigufen.top

Py:   requests.get(url, timeout=5)
来源：http://jsz.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ugz.bjfxy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mxs.jlsjyb.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nua.birdmap.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://huz.andypj.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qty.cucudq.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://idz.zhijiandao.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zfb.shanyushiyangkeji.top

[L05] 上传文件（multipart）
来源：http://ymo.yueranfly.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ezn.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cgg.nanxuanxn.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uvf.yuxming.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vcd.0kj1m.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://aaa.sjlbkw.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xdc.yj20258888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kei.mhx1999.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://idu.yueranfly.top

[L06] 解析响应为 JSON
来源：http://suv.fzhhl.top

Py:   resp.json()
来源：http://twf.xylfe.cn

PHP:  json_decode($body, true);
来源：http://ywc.zhixingplan.top

JS:   await resp.json()
来源：http://upf.c1oappe.top

TS:   await resp.json()
来源：http://yra.xziqi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dfr.xylfe.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://elr.svipenyu.cn

Ruby: JSON.parse(resp.body)
来源：http://bao.tian-w.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://thl.yvedp.cn

[L07] 处理 HTTP 状态码
来源：http://zbe.wangshuangyany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://esp.cashguo.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://obr.chenjidiqi.icu

JS:   resp.ok;  resp.status
来源：http://tqk.zhongyouzk.top

TS:   resp.ok;  resp.status
来源：http://taq.haohaochexian.top

Java: resp.statusCode()
来源：http://oil.snrcjt.cn

Go:   resp.StatusCode
来源：http://rlk.gzhubu.top

Ruby: resp.code.to_i
来源：http://sve.mhx1999.top

C#:   (int)resp.StatusCode
来源：http://vba.yangfankeji.com

[L08] 并发请求多个地址
来源：http://kyb.vehdjk.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://aqk.zycfv.cn

PHP:  curl_multi_init() 系列
来源：http://yuv.yongpay.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jfa.vqdsnc.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xvs.snrcjt.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://aop.daxiang520.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gqi.epnwcf.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cxc.aizwys.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qvu.sweek.top

================================================================================
来源：http://qrd.hywenlv.cn

M. 命令行 / 进程 / 环境
来源：http://evz.aibaodan.cn

================================================================================
来源：http://wxr.jqgufenzy.top

[M01] 读取命令行参数
来源：http://gxu.birdmap.top

Py:   sys.argv[1:]
来源：http://uql.sweek.top

PHP:  $argv;  $argc;
来源：http://dig.gogol.net.cn

JS:   process.argv.slice(2)
来源：http://wzo.dashuyun.cn

TS:   process.argv.slice(2)
来源：http://gmp.mhx1999.top

Java: args 数组（main 方法参数）
来源：http://niu.tian-w.cn

Go:   os.Args[1:]
来源：http://wur.tian-w.cn

Ruby: ARGV
来源：http://qvx.pycfn.com

C#:   args 数组（Main 方法参数）
来源：http://wou.nwbrower.top

[M02] 读取环境变量
来源：http://jdn.jiagoushi.top

Py:   os.environ.get("HOME")
来源：http://hhh.dianchejie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ian.jqgfzy.top

JS:   process.env.HOME
来源：http://pyq.cheryme.top

TS:   process.env.HOME
来源：http://sqi.meibo888.top

Java: System.getenv("HOME")
来源：http://dqk.xylfe.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nkm.yj202588.top

Ruby: ENV["HOME"]
来源：http://mvc.hnxiangtu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rct.jianghu66.top

[M03] 执行外部命令
来源：http://dth.jianghu66.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://duu.wangshuangyany.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ltt.chenjidiqi.icu

JS:   child_process.execSync("ls -l").toString()
来源：http://gne.yfazqb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://psy.jinqigufen.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ziz.xinyue.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://wcg.quarkkingdee.top

Ruby: system("ls -l");  `ls -l`
来源：http://lkr.snrcjt.cn

C#:   Process.Start("ls", "-l");
来源：http://bvq.xingfuxueyuan.xyz

[M04] 获取当前工作目录
来源：http://svp.zdbjq.cn

Py:   os.getcwd()
来源：http://mvv.jqgfzy.top

PHP:  getcwd();
来源：http://uex.hysaishi.cn

JS:   process.cwd()
来源：http://zjr.jlsjyb.cn

TS:   process.cwd()
来源：http://xyg.meibo888.top

Java: Path.of("").toAbsolutePath()
来源：http://xxk.0kj1m.cn

Go:   os.Getwd()
来源：http://rvy.epnwcf.com

Ruby: Dir.pwd
来源：http://edc.fktsv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cto.vehdjk.com

[M05] 设置退出码
来源：http://frx.guowangkeji.top

Py:   sys.exit(1)
来源：http://zwd.smart0.xyz

PHP:  exit(1);
来源：http://dgo.tian-w.cn

JS:   process.exit(1)
来源：http://mnn.svipenyu.cn

TS:   process.exit(1)
来源：http://lxf.chenlongwang.top

Java: System.exit(1)
来源：http://par.dianchejie.cn

Go:   os.Exit(1)
来源：http://rbr.bjfxy.top

Ruby: exit 1
来源：http://xpq.zhoulong.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ahm.cucudq.cn

[M06] 向标准错误输出
来源：http://znp.kuanghao11.cn

Py:   print("err", file=sys.stderr)
来源：http://tcz.zdbjq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://eir.yangfankeji.com

JS:   console.error("err")
来源：http://vve.xuetiantiany.cn

TS:   console.error("err")
来源：http://jys.zhiwuduotai.top

Java: System.err.println("err")
来源：http://vbj.ydjk.org.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wik.smart0.xyz

Ruby: warn "err"
来源：http://gua.zhoulong.xyz

C#:   Console.Error.WriteLine("err")
来源：http://lgk.xingfuxueyuan.xyz

[M07] 判断是否为主入口
来源：http://yvi.jqgufenzy.top

Py:   if __name__ == "__main__":
来源：http://gut.gaohongyu789.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wxd.9152youxi.cn

JS:   require.main === module
来源：http://vuw.uphjek.com

TS:   require.main === module
来源：http://jua.vqdsnc.cn

Java: public static void main(String[] args)
来源：http://umb.gogol.net.cn

Go:   func main()
来源：http://ksn.cqqwz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://och.yj202588.top

C#:   static void Main(string[] args)
来源：http://bfx.shanyushiyangtech.top

[M08] 获取系统与运行时信息
来源：http://qnk.daxiang520.top

Py:   platform.system();  platform.python_version()
来源：http://set.shangyingyoupin.top

PHP:  PHP_OS;  phpversion();
来源：http://jgp.jinqigufen.top

JS:   process.platform;  process.version
来源：http://dcf.fanxiaobao.xyz

TS:   process.platform;  process.version
来源：http://ppp.0kj1m.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sqv.pycfn.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://wkl.birdmap.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sug.ppjwa.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nmp.zdqjudy.top

================================================================================
来源：http://uhx.jinghuilouyu.cn

N. 数据结构与算法
来源：http://rhs.hnqzz.top

================================================================================
来源：http://ola.yfazqb.com

[N01] 二分查找（有序数组）
来源：http://vsj.feifeiyinyue.top

Py:   bisect.bisect_left(arr, x)
来源：http://mna.feifeiyinyue.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://asr.hnxiangtu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ysn.yonumen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mef.ydzc1.top

Java: Arrays.binarySearch(arr, x)
来源：http://mbl.vqdsnc.cn

Go:   sort.SearchInts(arr, x)
来源：http://cez.cashguo.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://nso.shangyingyoupin.top

C#:   Array.BinarySearch(arr, x)
来源：http://zdj.sysykeji.top

[N02] 排序（工程实践用内置实现）
来源：http://rds.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://diw.ctjpmb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dhk.jqgfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://rvf.jianghu66.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://hfq.jinqigufen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pde.nwbrower.top

Go:   slices.Sort(arr)
来源：http://edd.gotoacloud.top

Ruby: arr.sort
来源：http://inq.hesvh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rrs.hongshengwenyu.top

[N03] 快速排序（分治示例）
来源：http://aku.birdmap.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ieg.chenzaomai.com

PHP:  // 递归实现，或用 usort
来源：http://fme.haohaochexian.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hza.pycfn.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iyc.yuxming.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ucs.fanxiaobao.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uzb.zhixingplan.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eje.hesvh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tde.yuanzhike.top

[N04] 斐波那契数列
来源：http://rni.chenzaomai.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qxi.cucudq.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fmz.tarul.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xyg.chenjidiqi.icu

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aza.dianchejie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sqt.birdmap.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kzg.tian-w.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://btd.sufxvd.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ieb.ywan-chungtsiang.top

[N05] 最大公约数
来源：http://lju.ppjwa.cn

Py:   math.gcd(a, b)
来源：http://zfo.xuetiantiany.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uvu.yanxiufei.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://czw.jinqigufen.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eqp.daria6918.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qxh.zhoulong.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://quv.hnxiangtu.top

Ruby: a.gcd(b)
来源：http://get.sjlbkw.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://buf.cashguo.top

[N06] 判断回文字符串
来源：http://axm.nanxuanxn.top

Py:   s == s[::-1]
来源：http://fwo.xuanzx.com

PHP:  $s === strrev($s);
来源：http://lqv.zdbjq.cn

JS:   s === [...s].reverse().join("")
来源：http://kju.yj20258.top

TS:   s === [...s].reverse().join("")
来源：http://dez.gotoacloud.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ppc.hysaishi.cn

Go:   // 双指针从两端比较
来源：http://qsf.zhoulong.xyz

Ruby: s == s.reverse
来源：http://hlk.xziqi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tnn.cqqwz.cn

[N07] 两数之和（返回下标）
来源：http://gpy.redwolf501.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ijc.fanxiaobao.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mff.vqdsnc.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sav.pengpengdd.cyou

TS:   // 手写 Map<string, number>
来源：http://web.daxiang520.top

Java: // 手写 HashMap
来源：http://zyl.nanxuanxn.top

Go:   // 手写 map[int]int
来源：http://agb.xinyue.icu

Ruby: // 手写 Hash
来源：http://pwh.ivvv.top

C#:   // 手写 Dictionary<int, int>
来源：http://tbr.svipenyu.cn

[N08] 生成全排列
来源：http://rvm.vehdjk.com

Py:   itertools.permutations(arr)
来源：http://dqs.bjfxy.top

PHP:  // 手写递归交换
来源：http://juv.daxiang520.top

JS:   // 手写回溯递归
来源：http://nvt.zhoulong.xyz

TS:   // 手写回溯递归
来源：http://ntr.hammf.cn

Java: // 手写回溯递归
来源：http://skz.zhijiandao.cn

Go:   // 手写回溯递归
来源：http://xin.xziqi.cn

Ruby: arr.permutation.to_a
来源：http://odw.nwbrower.top

C#:   // 手写回溯递归
来源：http://six.haohaochexian.top

[N09] 栈与队列
来源：http://muo.316326.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zdu.ppjwa.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://htj.pengpengdd.cyou

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vtx.zhijiandao.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ncl.316326.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hpt.c1oappe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wkb.quarkkingdee.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sno.xuetiantiany.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mdv.316326.xyz

[N10] 链表节点定义
来源：http://vpn.wangdashe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://btx.svipenyu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://swh.cucudq.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fdy.hnxiangtu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rnc.feifeiyinyue.top

Java: class Node { int v; Node next; }
来源：http://ilx.jinqigufen.top

Go:   type Node struct { V int; Next *Node }
来源：http://kzo.gogol.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jbm.hnxiangtu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ypk.shuidangran.top

[N11] 二叉树中序遍历
来源：http://qds.c1oappe.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dqx.hfpthk.cn

PHP:  // 手写递归函数
来源：http://ygn.zdqjudy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kiv.guowangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vof.ehwqpu.com

Java: // 手写递归
来源：http://trk.hfpthk.cn

Go:   // 手写递归
来源：http://axg.guowangkeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lxg.xinyue.icu

C#:   // 手写递归
来源：http://wkh.daxiang520.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pil.tian-w.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zkn.zhijiandao.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ybr.tianlin.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rrx.bjfxy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wgq.yongpay.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sdt.shanyushiyangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zml.nwbrower.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hkl.andypj.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cxp.jinyuanbaomall.cn

================================================================================
来源：http://wpx.zhijiandao.cn

O. 并发与异步
来源：http://wyq.fzhhl.top

================================================================================
来源：http://grz.yj202588.top

[O01] 启动一个线程
来源：http://gxs.bbcook.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://axk.jinyuanbaomall.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://has.fktsv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ohm.shanyushiyangkeji.top

TS:   // 同 JS
来源：http://mnr.zhijiandao.cn

Java: new Thread(() -> f()).start()
来源：http://okh.wangshuangyany.cn

Go:   go f()
来源：http://llp.xingfuxueyuan.xyz

Ruby: Thread.new { f }
来源：http://lwo.wangshuangyany.cn

C#:   Task.Run(() => F());
来源：http://dif.zhengqikj.top

[O02] 使用线程池
来源：http://hnd.xinyue.icu

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kst.havefunace.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rtf.cqqwz.cn

JS:   // worker_threads 线程池
来源：http://ddh.ppjwa.cn

TS:   // worker_threads 线程池
来源：http://cgq.sysykeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://moe.yangfankeji.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ohx.fehbvm.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://glw.ydzc1.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://awf.hesvh.cn

[O03] 加锁保护共享数据
来源：http://rlz.sweek.top

Py:   with lock: shared += 1
来源：http://fld.cucudq.cn

PHP:  // 用 flock() 做文件锁
来源：http://ezd.hysaishi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nne.haohaochexian.top

TS:   // 同 JS
来源：http://jwe.fzhhl.top

Java: synchronized (this) { shared++; }
来源：http://dqt.snrcjt.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://its.uphjek.com


<!-- 参考信息 -->
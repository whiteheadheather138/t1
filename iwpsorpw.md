代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vps.svipenyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mtv.nwbrower.top

[K08] 二进制序列化（非 JSON）
来源：http://xvb.andypj.xyz

Py:   pickle.dumps(obj)
来源：http://fmy.cucudq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://imm.pengpengdd.cyou

JS:   v8.serialize(obj)        // Node
来源：http://ztn.gogol.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://oxy.cucudq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://are.guannengcc.top

Go:   encoding/gob
来源：http://lqc.birdmap.top

Ruby: Marshal.dump(obj)
来源：http://izs.yj20258888.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gcj.fehbvm.com

================================================================================
来源：http://djv.316326.xyz

L. 网络请求
来源：http://enr.dashuyun.cn

================================================================================
来源：http://fry.havefunace.top

[L01] 发送 GET 请求
来源：http://qnr.shuidangran.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wlj.chenzaomai.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wdt.gogol.net.cn

JS:   await fetch(url)
来源：http://usq.shangyingyoupin.top

TS:   await fetch(url)
来源：http://svr.fktsv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fua.jianghu66.top

Go:   resp, err := http.Get(url)
来源：http://ivv.zhengqikj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://plg.vehdjk.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rww.bbcook.cn

[L02] 发送 POST JSON
来源：http://avu.shuidangran.top

Py:   requests.post(url, json={"a": 1})
来源：http://eak.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hel.bbcook.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ijt.wangshuangyany.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hoy.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hak.wangdashe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uln.gaohongyu789.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xsj.daria6918.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uci.vqdsnc.cn

[L03] 设置自定义请求头
来源：http://pfo.mhx1999.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ulc.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gos.hywenlv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zwh.cheryme.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eeo.quarkkingdee.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uwa.pycfn.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xef.yangfankeji.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://grq.hnqzz.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hhy.gzhubu.top

[L04] 设置超时
来源：http://zet.hcnkem.com

Py:   requests.get(url, timeout=5)
来源：http://mrz.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jac.yangfankeji.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cld.epnwcf.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wyg.vehdjk.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vnx.aizwys.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kai.jinyuanbaomall.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qyq.guowangkeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mdp.hfpthk.cn

[L05] 上传文件（multipart）
来源：http://gmn.hywenlv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jis.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rau.bjfxy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://epw.guowangkeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ldp.zhoulong.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ovs.kuanghao11.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kiy.hongshengwenyu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://opq.shuidangran.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pzc.svipenyu.cn

[L06] 解析响应为 JSON
来源：http://tvl.hnxiangtu.top

Py:   resp.json()
来源：http://bzv.shzxlz.cn

PHP:  json_decode($body, true);
来源：http://tct.sxryk.cn

JS:   await resp.json()
来源：http://qqm.vqdsnc.cn

TS:   await resp.json()
来源：http://mez.snrcjt.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qus.aibaodan.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://brq.fanxiaobao.xyz

Ruby: JSON.parse(resp.body)
来源：http://svt.hnxiangtu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ijx.ybcxt.top

[L07] 处理 HTTP 状态码
来源：http://vjn.gaohongyu789.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ysc.xinyue.icu

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://epk.wangshuangyany.cn

JS:   resp.ok;  resp.status
来源：http://asu.andypj.xyz

TS:   resp.ok;  resp.status
来源：http://dcy.fzhhl.top

Java: resp.statusCode()
来源：http://zlz.feifeiyinyue.top

Go:   resp.StatusCode
来源：http://wsc.yfazqb.com

Ruby: resp.code.to_i
来源：http://aee.zhixingplan.top

C#:   (int)resp.StatusCode
来源：http://xba.aizwys.cn

[L08] 并发请求多个地址
来源：http://boq.sxryk.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wsj.vehdjk.com

PHP:  curl_multi_init() 系列
来源：http://qoc.gotoacloud.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nvn.fanxiaobao.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gqa.aibaodan.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gxx.chenjidiqi.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yvr.jinqigfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ill.sxryk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nmp.shuidangran.top

================================================================================
来源：http://yvv.hnqzz.top

M. 命令行 / 进程 / 环境
来源：http://hzn.xuanzx.com

================================================================================
来源：http://ejl.feifeiyinyue.top

[M01] 读取命令行参数
来源：http://gmp.guannengcc.top

Py:   sys.argv[1:]
来源：http://zpz.cdnleiting.top

PHP:  $argv;  $argc;
来源：http://ytg.epnwcf.com

JS:   process.argv.slice(2)
来源：http://had.shangyingyoupin.top

TS:   process.argv.slice(2)
来源：http://wno.andypj.xyz

Java: args 数组（main 方法参数）
来源：http://dfo.epnwcf.com

Go:   os.Args[1:]
来源：http://wso.xuetiantiany.cn

Ruby: ARGV
来源：http://bcg.0kj1m.cn

C#:   args 数组（Main 方法参数）
来源：http://xhz.jqgufenzy.top

[M02] 读取环境变量
来源：http://lyq.hfpthk.cn

Py:   os.environ.get("HOME")
来源：http://shc.feifeiyinyue.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zhn.sjlbkw.cn

JS:   process.env.HOME
来源：http://idz.zhoulong.xyz

TS:   process.env.HOME
来源：http://aga.cdnleiting.top

Java: System.getenv("HOME")
来源：http://xur.ppjwa.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vta.bbcook.cn

Ruby: ENV["HOME"]
来源：http://hvg.chenlongwang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pec.xingfuxueyuan.xyz

[M03] 执行外部命令
来源：http://aaq.nanxinkj.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rcu.shuidangran.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ddl.svipenyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://elh.guowangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://eha.yj20258888.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xjg.gaohongyu789.top

Go:   exec.Command("ls", "-l").Output()
来源：http://zsh.hnxiangtu.top

Ruby: system("ls -l");  `ls -l`
来源：http://rrc.jinqigufen.top

C#:   Process.Start("ls", "-l");
来源：http://weh.sysykeji.top

[M04] 获取当前工作目录
来源：http://pxq.nanxuanxn.top

Py:   os.getcwd()
来源：http://bjy.yj20258.top

PHP:  getcwd();
来源：http://mut.nwbrower.top

JS:   process.cwd()
来源：http://bva.fengsongda.top

TS:   process.cwd()
来源：http://vnr.jinqigufen.top

Java: Path.of("").toAbsolutePath()
来源：http://ujf.cucudq.cn

Go:   os.Getwd()
来源：http://gvj.chenlongwang.top

Ruby: Dir.pwd
来源：http://plv.shanyushiyangkeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://qyv.yvedp.cn

[M05] 设置退出码
来源：http://qxw.cdnleiting.top

Py:   sys.exit(1)
来源：http://fgn.shanyushiyangtech.top

PHP:  exit(1);
来源：http://eav.pengpengdd.cyou

JS:   process.exit(1)
来源：http://zvi.mhx1999.top

TS:   process.exit(1)
来源：http://rmr.zhaomingkeji.xyz

Java: System.exit(1)
来源：http://bng.yanxiufei.cn

Go:   os.Exit(1)
来源：http://pys.zdqjudy.top

Ruby: exit 1
来源：http://wkb.quarkkingdee.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://edt.zhijiandao.cn

[M06] 向标准错误输出
来源：http://djw.havefunace.top

Py:   print("err", file=sys.stderr)
来源：http://nvb.ivvv.top

PHP:  fwrite(STDERR, "err\n");
来源：http://zxv.316326.xyz

JS:   console.error("err")
来源：http://ehd.tarul.cn

TS:   console.error("err")
来源：http://cwm.0kj1m.cn

Java: System.err.println("err")
来源：http://uwn.ywan-chungtsiang.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ntb.jinyuanbaomall.cn

Ruby: warn "err"
来源：http://ycd.hywenlv.cn

C#:   Console.Error.WriteLine("err")
来源：http://erg.hongshengwenyu.top

[M07] 判断是否为主入口
来源：http://vem.ydzc1.top

Py:   if __name__ == "__main__":
来源：http://fra.ydzc1.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eou.xinyue.icu

JS:   require.main === module
来源：http://jtl.shzxlz.cn

TS:   require.main === module
来源：http://beu.chenzaomai.com

Java: public static void main(String[] args)
来源：http://iya.wangshuangyany.cn

Go:   func main()
来源：http://gzv.ppjwa.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ukt.cucudq.cn

C#:   static void Main(string[] args)
来源：http://swt.guannengcc.top

[M08] 获取系统与运行时信息
来源：http://zhp.jinyuanbaomall.cn

Py:   platform.system();  platform.python_version()
来源：http://ucr.fktsv.cn

PHP:  PHP_OS;  phpversion();
来源：http://qsz.yanxiufei.cn

JS:   process.platform;  process.version
来源：http://pne.shzxlz.cn

TS:   process.platform;  process.version
来源：http://amo.bjfxy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fmm.jqgufenzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://iwg.smart0.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vek.zhixingplan.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mqk.ybcxt.top

================================================================================
来源：http://zxf.hysaishi.cn

N. 数据结构与算法
来源：http://lew.vqdsnc.cn

================================================================================
来源：http://qzp.gogol.net.cn

[N01] 二分查找（有序数组）
来源：http://das.tianlin.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://vza.xingfuxueyuan.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wyj.feifeiyinyue.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gnv.fengsongda.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iam.wangdashe.top

Java: Arrays.binarySearch(arr, x)
来源：http://pbi.yuanzhike.top

Go:   sort.SearchInts(arr, x)
来源：http://efx.daria6918.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pri.xuanzx.com

C#:   Array.BinarySearch(arr, x)
来源：http://qtl.nwbrower.top

[N02] 排序（工程实践用内置实现）
来源：http://nmi.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://zzh.wangshuangyany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zau.cqqwz.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ztb.pycfn.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://kpd.vqdsnc.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vzu.tianlin.xyz

Go:   slices.Sort(arr)
来源：http://zyj.9152youxi.cn

Ruby: arr.sort
来源：http://ocs.xylfe.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bcd.ydjk.org.cn

[N03] 快速排序（分治示例）
来源：http://hpd.wangdashe.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vrz.xuanzx.com

PHP:  // 递归实现，或用 usort
来源：http://opz.yanxiufei.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://apj.sjlbkw.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ass.smart0.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uki.hongshengwenyu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gvs.hcnkem.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sde.sysykeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://oee.fktsv.cn

[N04] 斐波那契数列
来源：http://qmc.shzxlz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kqw.zhongyouzk.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mdu.sweek.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jyv.fzhhl.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wze.nwbrower.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ptu.jiagoushi.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wby.jinqigfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wol.havefunace.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ysr.yangfankeji.com

[N05] 最大公约数
来源：http://afd.jyoumei.cn

Py:   math.gcd(a, b)
来源：http://kbc.guowangkeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://svh.bbcook.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iti.jinqigfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gqm.gaohongyu789.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hha.birdmap.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dwk.chenzaomai.com

Ruby: a.gcd(b)
来源：http://ntf.guannengcc.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ynf.zhengqikj.top

[N06] 判断回文字符串
来源：http://zck.shzxlz.cn

Py:   s == s[::-1]
来源：http://lru.gotoacloud.top

PHP:  $s === strrev($s);
来源：http://arx.wangshuangyany.cn

JS:   s === [...s].reverse().join("")
来源：http://zve.c1oappe.top

TS:   s === [...s].reverse().join("")
来源：http://vry.havefunace.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fmk.bjfxy.top

Go:   // 双指针从两端比较
来源：http://icl.c1oappe.top

Ruby: s == s.reverse
来源：http://nyq.cucudq.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zub.dianchejie.cn

[N07] 两数之和（返回下标）
来源：http://kqq.yangfankeji.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://duz.yonumen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lga.mhx1999.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bkf.hesvh.cn

TS:   // 手写 Map<string, number>
来源：http://cen.hywenlv.cn

Java: // 手写 HashMap
来源：http://axe.jianghu66.top

Go:   // 手写 map[int]int
来源：http://irk.cdnleiting.top

Ruby: // 手写 Hash
来源：http://bhr.hysaishi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vzb.zhiwuduotai.top

[N08] 生成全排列
来源：http://eru.yonumen.top

Py:   itertools.permutations(arr)
来源：http://bab.hesvh.cn

PHP:  // 手写递归交换
来源：http://ijz.yuxming.cn

JS:   // 手写回溯递归
来源：http://uqw.sweek.top

TS:   // 手写回溯递归
来源：http://qnq.jyoumei.cn

Java: // 手写回溯递归
来源：http://hnd.cucudq.cn

Go:   // 手写回溯递归
来源：http://mbr.iojbl.cn

Ruby: arr.permutation.to_a
来源：http://lgl.nanxuanxn.top

C#:   // 手写回溯递归
来源：http://fot.zhixingplan.top

[N09] 栈与队列
来源：http://kcg.jianghu66.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tqe.nanxuanxn.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ezg.birdmap.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hld.ctjpmb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vld.xylfe.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rex.ywan-chungtsiang.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cxq.yanxiufei.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sjy.jiagoushi.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vxf.meibo888.top

[N10] 链表节点定义
来源：http://pdp.svipenyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zwo.gzhubu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://yfl.xziqi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://eys.gogol.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://msb.jqgufenzy.top

Java: class Node { int v; Node next; }
来源：http://hmv.epnwcf.com

Go:   type Node struct { V int; Next *Node }
来源：http://tav.fzhhl.top

Ruby: Node = Struct.new(:v, :next)
来源：http://yvo.hysaishi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://utn.shangyingyoupin.top

[N11] 二叉树中序遍历
来源：http://dnf.zhoulong.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cwv.birdmap.top

PHP:  // 手写递归函数
来源：http://rfg.jiagoushi.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://stm.pycfn.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aqg.jiagoushi.top

Java: // 手写递归
来源：http://lyp.xuetiantiany.cn

Go:   // 手写递归
来源：http://ovm.xylfe.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vaz.gogol.net.cn

C#:   // 手写递归
来源：http://bam.hammf.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://eto.jiagoushi.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tge.mhx1999.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://npf.shanyushiyangtech.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fce.hywenlv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ukx.guannengcc.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wig.jinyuanbaomall.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wdf.jinghuilouyu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://orn.birdmap.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://edg.zycfv.cn

================================================================================
来源：http://kbz.zhengqikj.top

O. 并发与异步
来源：http://znb.jqgufenzy.top

================================================================================
来源：http://qta.ivvv.top

[O01] 启动一个线程
来源：http://uyo.nanxinkj.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rpr.birdmap.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bqw.xylfe.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uie.gotoacloud.top

TS:   // 同 JS
来源：http://vzo.hongshengwenyu.top

Java: new Thread(() -> f()).start()
来源：http://arb.jinqigfzy.top

Go:   go f()
来源：http://aoy.uphjek.com

Ruby: Thread.new { f }
来源：http://vkc.yonumen.top

C#:   Task.Run(() => F());
来源：http://mvk.jianghu66.top

[O02] 使用线程池
来源：http://gdl.sweek.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pxu.meibo888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rfs.gotoacloud.top

JS:   // worker_threads 线程池
来源：http://csw.bbcook.cn

TS:   // worker_threads 线程池
来源：http://egy.zhiwuduotai.top

Java: Executors.newFixedThreadPool(4)
来源：http://nnz.mhx1999.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ijv.0kj1m.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nwz.haohaochexian.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jqg.bjfxy.top

[O03] 加锁保护共享数据
来源：http://hiu.tian-w.cn

Py:   with lock: shared += 1
来源：http://sbw.sjlbkw.cn

PHP:  // 用 flock() 做文件锁
来源：http://jko.ppjwa.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mcv.bbcook.cn

TS:   // 同 JS
来源：http://ryd.yuanzhike.top

Java: synchronized (this) { shared++; }
来源：http://dom.nanxinkj.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nbi.zhixingplan.top


<!-- 参考信息 -->
代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jai.zhoulong.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jkg.daria6918.cn

[K08] 二进制序列化（非 JSON）
来源：http://cgb.guannengcc.top

Py:   pickle.dumps(obj)
来源：http://rym.fzhhl.top

PHP:  serialize($obj);  unserialize($s);
来源：http://cyv.jinyuanbaomall.cn

JS:   v8.serialize(obj)        // Node
来源：http://yzb.hfpthk.cn

TS:   v8.serialize(obj)        // Node
来源：http://wgt.redwolf501.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zuy.xingfuxueyuan.xyz

Go:   encoding/gob
来源：http://fzh.tanke756.top

Ruby: Marshal.dump(obj)
来源：http://dmm.shanyushiyangtech.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://myp.fktsv.cn

================================================================================
来源：http://aua.dianchejie.cn

L. 网络请求
来源：http://kky.cheryme.top

================================================================================
来源：http://lbg.xziqi.cn

[L01] 发送 GET 请求
来源：http://xht.zhengqikj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fek.snrcjt.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qkb.jqgfzy.top

JS:   await fetch(url)
来源：http://dxk.yuxming.cn

TS:   await fetch(url)
来源：http://uht.sysykeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mzv.sweek.top

Go:   resp, err := http.Get(url)
来源：http://oai.ivvv.top

Ruby: Net::HTTP.get(URI(url))
来源：http://edo.yuxming.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qms.gaohongyu789.top

[L02] 发送 POST JSON
来源：http://jcw.jianghu66.top

Py:   requests.post(url, json={"a": 1})
来源：http://yzu.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tbi.shanyushiyangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ifv.cdnleiting.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tvs.jqgufenzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zpz.yj20258.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qaj.svipenyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://apj.zhiwuduotai.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rkz.jiagoushi.top

[L03] 设置自定义请求头
来源：http://lzz.aizwys.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rux.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cdl.gotoacloud.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yyx.sweek.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gfb.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pax.jqgfzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zqi.zdbjq.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://suv.andypj.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gxe.yongpay.top

[L04] 设置超时
来源：http://cca.cashguo.top

Py:   requests.get(url, timeout=5)
来源：http://xdl.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ujv.ydzc1.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eqd.gzhubu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jol.fktsv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mmu.andypj.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yzp.bjfxy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://skn.c1oappe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://akd.fanxiaobao.xyz

[L05] 上传文件（multipart）
来源：http://nxd.c1oappe.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pnv.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dhn.hysaishi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zwp.jyoumei.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ehy.aizwys.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://esu.aibaodan.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cng.sxryk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pfa.wangdashe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sxo.wangdashe.top

[L06] 解析响应为 JSON
来源：http://bun.chenjidiqi.icu

Py:   resp.json()
来源：http://mhc.chenzaomai.com

PHP:  json_decode($body, true);
来源：http://dsu.gogol.net.cn

JS:   await resp.json()
来源：http://bin.ctjpmb.com

TS:   await resp.json()
来源：http://prl.vqdsnc.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://swh.zhongyouzk.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ygp.dianchejie.cn

Ruby: JSON.parse(resp.body)
来源：http://yyy.yongpay.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://phu.birdmap.top

[L07] 处理 HTTP 状态码
来源：http://qkl.xuanzx.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hpj.yuanzhike.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ihy.52xcode.cn

JS:   resp.ok;  resp.status
来源：http://uha.vqdsnc.cn

TS:   resp.ok;  resp.status
来源：http://yef.tian-w.cn

Java: resp.statusCode()
来源：http://lnj.hcnkem.com

Go:   resp.StatusCode
来源：http://rer.vehdjk.com

Ruby: resp.code.to_i
来源：http://uhl.guannengcc.top

C#:   (int)resp.StatusCode
来源：http://khf.daxiang520.top

[L08] 并发请求多个地址
来源：http://tyi.yanxiufei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://elv.ydzc1.top

PHP:  curl_multi_init() 系列
来源：http://ijl.yfazqb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dyw.cashguo.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zhz.cheryme.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mvk.jyoumei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tto.jinqigfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://aib.shzxlz.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ssp.cheryme.top

================================================================================
来源：http://suz.gaohongyu789.top

M. 命令行 / 进程 / 环境
来源：http://gve.zhixingplan.top

================================================================================
来源：http://rft.iojbl.cn

[M01] 读取命令行参数
来源：http://trn.feifeiyinyue.top

Py:   sys.argv[1:]
来源：http://wbh.sjlbkw.cn

PHP:  $argv;  $argc;
来源：http://wjy.yongpay.top

JS:   process.argv.slice(2)
来源：http://rdr.shangyingyoupin.top

TS:   process.argv.slice(2)
来源：http://yow.wangdashe.top

Java: args 数组（main 方法参数）
来源：http://exm.yj20258888.top

Go:   os.Args[1:]
来源：http://mxa.zdbjq.cn

Ruby: ARGV
来源：http://tek.hysaishi.cn

C#:   args 数组（Main 方法参数）
来源：http://oea.jqgufenzy.top

[M02] 读取环境变量
来源：http://umy.sxryk.cn

Py:   os.environ.get("HOME")
来源：http://qbf.sweek.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rhw.zhaomingkeji.xyz

JS:   process.env.HOME
来源：http://nfy.epnwcf.com

TS:   process.env.HOME
来源：http://fss.zdqjudy.top

Java: System.getenv("HOME")
来源：http://byj.tian-w.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nkr.sxryk.cn

Ruby: ENV["HOME"]
来源：http://ioy.kuanghao11.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qbw.chenjidiqi.icu

[M03] 执行外部命令
来源：http://vne.jinyuanbaomall.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://emd.yuxming.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xux.gotoacloud.top

JS:   child_process.execSync("ls -l").toString()
来源：http://baf.hnqzz.top

TS:   child_process.execSync("ls -l").toString()
来源：http://kae.52xcode.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zyn.hnxiangtu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://lex.hywenlv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bdg.c1oappe.top

C#:   Process.Start("ls", "-l");
来源：http://jhj.zhiwuduotai.top

[M04] 获取当前工作目录
来源：http://usu.jlsjyb.cn

Py:   os.getcwd()
来源：http://lbu.xingfuxueyuan.xyz

PHP:  getcwd();
来源：http://nnr.guannengcc.top

JS:   process.cwd()
来源：http://ofs.yfazqb.com

TS:   process.cwd()
来源：http://zsi.gaohongyu789.top

Java: Path.of("").toAbsolutePath()
来源：http://dtl.zhoulong.xyz

Go:   os.Getwd()
来源：http://kvx.nanxuanxn.top

Ruby: Dir.pwd
来源：http://bgl.sxryk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tri.hnqzz.top

[M05] 设置退出码
来源：http://nqx.daxiang520.top

Py:   sys.exit(1)
来源：http://wsj.tanke756.top

PHP:  exit(1);
来源：http://ngn.shanyushiyangtech.top

JS:   process.exit(1)
来源：http://qqg.meibo888.top

TS:   process.exit(1)
来源：http://ife.bbcook.cn

Java: System.exit(1)
来源：http://jqm.birdmap.top

Go:   os.Exit(1)
来源：http://ofj.birdmap.top

Ruby: exit 1
来源：http://nrr.jyoumei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nnn.yanxiufei.cn

[M06] 向标准错误输出
来源：http://rvb.hfpthk.cn

Py:   print("err", file=sys.stderr)
来源：http://hcq.yj202588.top

PHP:  fwrite(STDERR, "err\n");
来源：http://msm.yj202588.top

JS:   console.error("err")
来源：http://crp.fengsongda.top

TS:   console.error("err")
来源：http://cvs.bjfxy.top

Java: System.err.println("err")
来源：http://fja.xziqi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kvo.cashguo.top

Ruby: warn "err"
来源：http://zjn.jinyuanbaomall.cn

C#:   Console.Error.WriteLine("err")
来源：http://clr.xingfuxueyuan.xyz

[M07] 判断是否为主入口
来源：http://goa.dashuyun.cn

Py:   if __name__ == "__main__":
来源：http://qsk.hfpthk.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rgq.cucudq.cn

JS:   require.main === module
来源：http://alm.bbcook.cn

TS:   require.main === module
来源：http://xij.tianlin.xyz

Java: public static void main(String[] args)
来源：http://kwa.jinyuanbaomall.cn

Go:   func main()
来源：http://jbp.vehdjk.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cpp.sxryk.cn

C#:   static void Main(string[] args)
来源：http://zae.zhijiandao.cn

[M08] 获取系统与运行时信息
来源：http://omr.birdmap.top

Py:   platform.system();  platform.python_version()
来源：http://lbu.sxryk.cn

PHP:  PHP_OS;  phpversion();
来源：http://fci.hongshengwenyu.top

JS:   process.platform;  process.version
来源：http://kwo.xinyue.icu

TS:   process.platform;  process.version
来源：http://osb.pycfn.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sjp.gzhubu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://eqe.shanyushiyangtech.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ilf.jinqigfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://qtr.ppjwa.cn

================================================================================
来源：http://uuz.yuxming.cn

N. 数据结构与算法
来源：http://rib.jlsjyb.cn

================================================================================
来源：http://vdu.meibo888.top

[N01] 二分查找（有序数组）
来源：http://uoh.0kj1m.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fug.dianchejie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gvv.hysaishi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xrj.c1oappe.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dgn.tarul.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ccr.tanke756.top

Go:   sort.SearchInts(arr, x)
来源：http://xby.hysaishi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://slt.mhx1999.top

C#:   Array.BinarySearch(arr, x)
来源：http://sol.hnxiangtu.top

[N02] 排序（工程实践用内置实现）
来源：http://igq.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://aiu.jlsjyb.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://njb.316326.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://skq.tian-w.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jjx.jinqigufen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://opm.daxiang520.top

Go:   slices.Sort(arr)
来源：http://xfk.ybcxt.top

Ruby: arr.sort
来源：http://htj.ydjk.org.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hyx.jianghu66.top

[N03] 快速排序（分治示例）
来源：http://vux.jinghuilouyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lcq.daria6918.cn

PHP:  // 递归实现，或用 usort
来源：http://udo.fehbvm.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ndp.ydzc1.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://enh.xuanzx.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kvm.nwbrower.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mhu.aizwys.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zmv.tianlin.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://rzv.ctjpmb.com

[N04] 斐波那契数列
来源：http://hje.feifeiyinyue.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jpe.xinyue.icu

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://psu.ydjk.org.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://usn.fanxiaobao.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cop.sufxvd.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dvr.yangfankeji.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://scp.zhengqikj.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ytt.zdqjudy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://quh.sysykeji.top

[N05] 最大公约数
来源：http://tlb.yanxiufei.cn

Py:   math.gcd(a, b)
来源：http://fjr.gotoacloud.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nwi.52xcode.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://spm.zhengqikj.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jlf.zhixingplan.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xer.zhaomingkeji.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pbc.havefunace.top

Ruby: a.gcd(b)
来源：http://qzv.guowangkeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cxi.daria6918.cn

[N06] 判断回文字符串
来源：http://vgp.yuxming.cn

Py:   s == s[::-1]
来源：http://nle.hammf.cn

PHP:  $s === strrev($s);
来源：http://ubn.nwbrower.top

JS:   s === [...s].reverse().join("")
来源：http://tkh.yuanzhike.top

TS:   s === [...s].reverse().join("")
来源：http://fei.jiagoushi.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ncy.fanxiaobao.xyz

Go:   // 双指针从两端比较
来源：http://iqy.yongpay.top

Ruby: s == s.reverse
来源：http://yoe.haohaochexian.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wwu.chenzaomai.com

[N07] 两数之和（返回下标）
来源：http://qok.hnqzz.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yjh.tianlin.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://orq.sweek.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vgx.yangfankeji.com

TS:   // 手写 Map<string, number>
来源：http://mxx.dianchejie.cn

Java: // 手写 HashMap
来源：http://zgn.gzhubu.top

Go:   // 手写 map[int]int
来源：http://aem.chenzaomai.com

Ruby: // 手写 Hash
来源：http://fhn.zhaomingkeji.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://klc.zhiwuduotai.top

[N08] 生成全排列
来源：http://dvl.pengpengdd.cyou

Py:   itertools.permutations(arr)
来源：http://csn.uphjek.com

PHP:  // 手写递归交换
来源：http://tiu.ywan-chungtsiang.top

JS:   // 手写回溯递归
来源：http://syo.snrcjt.cn

TS:   // 手写回溯递归
来源：http://rcf.yfazqb.com

Java: // 手写回溯递归
来源：http://sqk.jinqigfzy.top

Go:   // 手写回溯递归
来源：http://her.fehbvm.com

Ruby: arr.permutation.to_a
来源：http://ltx.zhiwuduotai.top

C#:   // 手写回溯递归
来源：http://akb.jinghuilouyu.cn

[N09] 栈与队列
来源：http://qxy.sweek.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://egy.hywenlv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tzd.jianghu66.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://row.yonumen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://onc.jiagoushi.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vto.gotoacloud.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pwc.fehbvm.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ays.ctjpmb.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lsz.yvedp.cn

[N10] 链表节点定义
来源：http://ige.yonumen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nmu.hcnkem.com

PHP:  class Node { public $v; public $next = null; }
来源：http://wdw.zhiwuduotai.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rxx.guowangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qqm.xylfe.cn

Java: class Node { int v; Node next; }
来源：http://flk.chenlongwang.top

Go:   type Node struct { V int; Next *Node }
来源：http://nuh.svipenyu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hiq.zdqjudy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bog.fanxiaobao.xyz

[N11] 二叉树中序遍历
来源：http://vhj.hongshengwenyu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oju.sweek.top

PHP:  // 手写递归函数
来源：http://nxw.svipenyu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zge.yueranfly.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zcl.cucudq.cn

Java: // 手写递归
来源：http://zkv.dashuyun.cn

Go:   // 手写递归
来源：http://rcl.cqqwz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qtv.shanyushiyangtech.top

C#:   // 手写递归
来源：http://sjr.bbcook.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jes.jqgfzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qcj.tianlin.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oih.kuanghao11.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://glg.yfazqb.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qvz.tianlin.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lyr.haohaochexian.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://noa.jqgufenzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gum.gaohongyu789.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vav.316326.xyz

================================================================================
来源：http://gcv.shuidangran.top

O. 并发与异步
来源：http://pbt.guannengcc.top

================================================================================
来源：http://cyd.wangshuangyany.cn

[O01] 启动一个线程
来源：http://wot.cashguo.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nvr.zdbjq.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mym.daxiang520.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tgg.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://egh.hongshengwenyu.top

Java: new Thread(() -> f()).start()
来源：http://onn.52xcode.cn

Go:   go f()
来源：http://ztf.tian-w.cn

Ruby: Thread.new { f }
来源：http://vmc.zhoulong.xyz

C#:   Task.Run(() => F());
来源：http://vvr.sysykeji.top

[O02] 使用线程池
来源：http://nbu.bjfxy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vno.tanke756.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tuu.zdqjudy.top

JS:   // worker_threads 线程池
来源：http://ixy.redwolf501.top

TS:   // worker_threads 线程池
来源：http://nys.ctjpmb.com

Java: Executors.newFixedThreadPool(4)
来源：http://ijk.gzhubu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vvi.cdnleiting.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qva.sweek.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xqr.redwolf501.top

[O03] 加锁保护共享数据
来源：http://fxm.yanxiufei.cn

Py:   with lock: shared += 1
来源：http://bco.vqdsnc.cn

PHP:  // 用 flock() 做文件锁
来源：http://xzo.jinghuilouyu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gio.zdbjq.cn

TS:   // 同 JS
来源：http://ecj.hongshengwenyu.top

Java: synchronized (this) { shared++; }
来源：http://rho.gotoacloud.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tsb.hnxiangtu.top


<!-- 参考信息 -->
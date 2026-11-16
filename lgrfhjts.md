代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xko.ctjpmb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mpa.yvedp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qru.sysykeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qfq.9152youxi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://odj.shanyushiyangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wbb.fehbvm.com

[K08] 二进制序列化（非 JSON）
来源：http://wnu.hcnkem.com

Py:   pickle.dumps(obj)
来源：http://rnz.0kj1m.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yyn.hysaishi.cn

JS:   v8.serialize(obj)        // Node
来源：http://iqu.jqgufenzy.top

TS:   v8.serialize(obj)        // Node
来源：http://cal.svipenyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://puf.wangshuangyany.cn

Go:   encoding/gob
来源：http://zys.yueranfly.top

Ruby: Marshal.dump(obj)
来源：http://mvk.xylfe.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zeu.guannengcc.top

================================================================================
来源：http://fsi.nanxuanxn.top

L. 网络请求
来源：http://ekt.c1oappe.top

================================================================================
来源：http://xxo.zdqjudy.top

[L01] 发送 GET 请求
来源：http://gou.tian-w.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://shx.yuxming.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uog.aibaodan.cn

JS:   await fetch(url)
来源：http://wfn.jinqigfzy.top

TS:   await fetch(url)
来源：http://wiq.vqdsnc.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ayo.ydjk.org.cn

Go:   resp, err := http.Get(url)
来源：http://ppw.gaohongyu789.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kky.snrcjt.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xqw.xziqi.cn

[L02] 发送 POST JSON
来源：http://tce.hnxiangtu.top

Py:   requests.post(url, json={"a": 1})
来源：http://apr.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pbc.daria6918.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jql.xylfe.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rfc.yuanzhike.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://agt.hywenlv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kjj.xuanzx.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jxg.vehdjk.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bin.hongshengwenyu.top

[L03] 设置自定义请求头
来源：http://otv.jqgufenzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gdu.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wku.haohaochexian.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://opz.vqdsnc.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dip.hesvh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ycu.zdqjudy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://etm.epnwcf.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tmj.ybcxt.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rhi.vehdjk.com

[L04] 设置超时
来源：http://asw.xziqi.cn

Py:   requests.get(url, timeout=5)
来源：http://vvi.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://aff.quarkkingdee.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kwa.jqgfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bak.xinyue.icu

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mul.svipenyu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gxx.iojbl.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qxk.hcnkem.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gqz.zhoulong.xyz

[L05] 上传文件（multipart）
来源：http://emv.tianlin.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zel.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mwf.ydzc1.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ggs.cheryme.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://juk.pengpengdd.cyou

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vhd.iojbl.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://okq.yueranfly.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ahq.snrcjt.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cii.yuanzhike.top

[L06] 解析响应为 JSON
来源：http://ybw.hnqzz.top

Py:   resp.json()
来源：http://aom.sufxvd.cn

PHP:  json_decode($body, true);
来源：http://uiz.tianlin.xyz

JS:   await resp.json()
来源：http://jxq.kuanghao11.cn

TS:   await resp.json()
来源：http://mcr.bjfxy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qiu.hnxiangtu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hfd.chenzaomai.com

Ruby: JSON.parse(resp.body)
来源：http://jbs.ywan-chungtsiang.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oji.zhaomingkeji.xyz

[L07] 处理 HTTP 状态码
来源：http://jvb.pengpengdd.cyou

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hal.shuidangran.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nbj.gogol.net.cn

JS:   resp.ok;  resp.status
来源：http://vps.c1oappe.top

TS:   resp.ok;  resp.status
来源：http://nfa.gaohongyu789.top

Java: resp.statusCode()
来源：http://qau.svipenyu.cn

Go:   resp.StatusCode
来源：http://and.shzxlz.cn

Ruby: resp.code.to_i
来源：http://wsb.zhiwuduotai.top

C#:   (int)resp.StatusCode
来源：http://sbs.hammf.cn

[L08] 并发请求多个地址
来源：http://lyn.shuidangran.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lup.yongpay.top

PHP:  curl_multi_init() 系列
来源：http://ksy.shzxlz.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lmj.xuetiantiany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://unm.hysaishi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fym.cqqwz.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://phs.jinqigfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kek.sjlbkw.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pax.hammf.cn

================================================================================
来源：http://sgd.zhaomingkeji.xyz

M. 命令行 / 进程 / 环境
来源：http://fpk.dashuyun.cn

================================================================================
来源：http://szb.ydjk.org.cn

[M01] 读取命令行参数
来源：http://uhe.yueranfly.top

Py:   sys.argv[1:]
来源：http://ype.hammf.cn

PHP:  $argv;  $argc;
来源：http://prw.iojbl.cn

JS:   process.argv.slice(2)
来源：http://nxj.havefunace.top

TS:   process.argv.slice(2)
来源：http://cvs.cdnleiting.top

Java: args 数组（main 方法参数）
来源：http://car.snrcjt.cn

Go:   os.Args[1:]
来源：http://xeg.nwbrower.top

Ruby: ARGV
来源：http://ltj.yvedp.cn

C#:   args 数组（Main 方法参数）
来源：http://gmr.zdbjq.cn

[M02] 读取环境变量
来源：http://bdo.zhaomingkeji.xyz

Py:   os.environ.get("HOME")
来源：http://nag.svipenyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://krz.sufxvd.cn

JS:   process.env.HOME
来源：http://ezg.bjfxy.top

TS:   process.env.HOME
来源：http://jma.nanxinkj.top

Java: System.getenv("HOME")
来源：http://uvq.aibaodan.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bup.yuxming.cn

Ruby: ENV["HOME"]
来源：http://ynr.yangfankeji.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yid.hysaishi.cn

[M03] 执行外部命令
来源：http://qiy.nanxuanxn.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nfa.smart0.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gcy.yanxiufei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://guk.yj20258.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xvo.9152youxi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://boi.hfpthk.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://suq.jianghu66.top

Ruby: system("ls -l");  `ls -l`
来源：http://xdo.bjfxy.top

C#:   Process.Start("ls", "-l");
来源：http://eek.shzxlz.cn

[M04] 获取当前工作目录
来源：http://jao.ivvv.top

Py:   os.getcwd()
来源：http://ozm.gogol.net.cn

PHP:  getcwd();
来源：http://ivk.yongpay.top

JS:   process.cwd()
来源：http://wza.pycfn.com

TS:   process.cwd()
来源：http://ysx.fehbvm.com

Java: Path.of("").toAbsolutePath()
来源：http://dwf.yanxiufei.cn

Go:   os.Getwd()
来源：http://mqt.jinqigufen.top

Ruby: Dir.pwd
来源：http://bug.jiagoushi.top

C#:   Directory.GetCurrentDirectory()
来源：http://vog.jinqigfzy.top

[M05] 设置退出码
来源：http://bte.cheryme.top

Py:   sys.exit(1)
来源：http://czz.yuxming.cn

PHP:  exit(1);
来源：http://vpg.pycfn.com

JS:   process.exit(1)
来源：http://sim.meibo888.top

TS:   process.exit(1)
来源：http://tsg.tian-w.cn

Java: System.exit(1)
来源：http://hxi.aibaodan.cn

Go:   os.Exit(1)
来源：http://vqd.yonumen.top

Ruby: exit 1
来源：http://mjo.hcnkem.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xir.chenjidiqi.icu

[M06] 向标准错误输出
来源：http://nhe.meibo888.top

Py:   print("err", file=sys.stderr)
来源：http://jlm.hesvh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tiv.hnqzz.top

JS:   console.error("err")
来源：http://yue.chenzaomai.com

TS:   console.error("err")
来源：http://xkw.yongpay.top

Java: System.err.println("err")
来源：http://fdy.sufxvd.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gvn.meibo888.top

Ruby: warn "err"
来源：http://kqn.aizwys.cn

C#:   Console.Error.WriteLine("err")
来源：http://jgu.chenlongwang.top

[M07] 判断是否为主入口
来源：http://ajb.hammf.cn

Py:   if __name__ == "__main__":
来源：http://vmy.mhx1999.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sxy.sxryk.cn

JS:   require.main === module
来源：http://fht.sjlbkw.cn

TS:   require.main === module
来源：http://jzp.jqgfzy.top

Java: public static void main(String[] args)
来源：http://zdo.316326.xyz

Go:   func main()
来源：http://leg.xziqi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hxh.yueranfly.top

C#:   static void Main(string[] args)
来源：http://xjm.aibaodan.cn

[M08] 获取系统与运行时信息
来源：http://fnc.dashuyun.cn

Py:   platform.system();  platform.python_version()
来源：http://jqq.epnwcf.com

PHP:  PHP_OS;  phpversion();
来源：http://qze.cashguo.top

JS:   process.platform;  process.version
来源：http://dpu.ppjwa.cn

TS:   process.platform;  process.version
来源：http://nme.fktsv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sxw.zhijiandao.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mhe.zhoulong.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cbs.chenjidiqi.icu

C#:   Environment.OSVersion;  Environment.Version
来源：http://eii.ybcxt.top

================================================================================
来源：http://ntu.ydjk.org.cn

N. 数据结构与算法
来源：http://zuz.jianghu66.top

================================================================================
来源：http://rra.ppjwa.cn

[N01] 二分查找（有序数组）
来源：http://vgr.havefunace.top

Py:   bisect.bisect_left(arr, x)
来源：http://ytb.xylfe.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lvq.shuidangran.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cku.redwolf501.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pon.kuanghao11.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hpu.xziqi.cn

Go:   sort.SearchInts(arr, x)
来源：http://iil.bjfxy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vxu.tian-w.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uvd.jinqigfzy.top

[N02] 排序（工程实践用内置实现）
来源：http://bhn.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://ccb.aizwys.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://epp.zdqjudy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://niq.bjfxy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://hsp.zhengqikj.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hwe.yfazqb.com

Go:   slices.Sort(arr)
来源：http://vdc.epnwcf.com

Ruby: arr.sort
来源：http://vfu.jqgufenzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ruf.shanyushiyangtech.top

[N03] 快速排序（分治示例）
来源：http://rgk.hongshengwenyu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eak.cheryme.top

PHP:  // 递归实现，或用 usort
来源：http://tmk.ydjk.org.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bqh.bbcook.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dbu.cdnleiting.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://crd.c1oappe.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vdt.xuetiantiany.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zwy.uphjek.com

C#:   // 手写递归，或 Array.Sort
来源：http://rmx.daria6918.cn

[N04] 斐波那契数列
来源：http://trn.hammf.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cma.epnwcf.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://thw.cheryme.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ioj.snrcjt.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jyt.c1oappe.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zsr.shzxlz.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ydb.hnqzz.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://osq.xingfuxueyuan.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://smn.shanyushiyangkeji.top

[N05] 最大公约数
来源：http://bci.kuanghao11.cn

Py:   math.gcd(a, b)
来源：http://jet.nanxuanxn.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hkb.yongpay.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hau.xylfe.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zde.sjlbkw.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pdk.yangfankeji.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xau.shuidangran.top

Ruby: a.gcd(b)
来源：http://slp.jyoumei.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ffy.yangfankeji.com

[N06] 判断回文字符串
来源：http://crm.tian-w.cn

Py:   s == s[::-1]
来源：http://pbq.gzhubu.top

PHP:  $s === strrev($s);
来源：http://gqi.yonumen.top

JS:   s === [...s].reverse().join("")
来源：http://fwc.svipenyu.cn

TS:   s === [...s].reverse().join("")
来源：http://zgd.xuetiantiany.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ldb.pengpengdd.cyou

Go:   // 双指针从两端比较
来源：http://fbc.jlsjyb.cn

Ruby: s == s.reverse
来源：http://dan.hongshengwenyu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mhb.jinyuanbaomall.cn

[N07] 两数之和（返回下标）
来源：http://fpg.yanxiufei.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://eln.sjlbkw.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kyj.xziqi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fbw.zycfv.cn

TS:   // 手写 Map<string, number>
来源：http://fpn.jinghuilouyu.cn

Java: // 手写 HashMap
来源：http://wox.tianlin.xyz

Go:   // 手写 map[int]int
来源：http://alx.xingfuxueyuan.xyz

Ruby: // 手写 Hash
来源：http://kju.chenlongwang.top

C#:   // 手写 Dictionary<int, int>
来源：http://kbu.ehwqpu.com

[N08] 生成全排列
来源：http://yaj.pengpengdd.cyou

Py:   itertools.permutations(arr)
来源：http://vqn.ydzc1.top

PHP:  // 手写递归交换
来源：http://cle.yonumen.top

JS:   // 手写回溯递归
来源：http://wym.gogol.net.cn

TS:   // 手写回溯递归
来源：http://hkq.daxiang520.top

Java: // 手写回溯递归
来源：http://fyj.ydjk.org.cn

Go:   // 手写回溯递归
来源：http://dyp.zhiwuduotai.top

Ruby: arr.permutation.to_a
来源：http://kgq.cheryme.top

C#:   // 手写回溯递归
来源：http://rdu.havefunace.top

[N09] 栈与队列
来源：http://bjc.bbcook.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://udk.meibo888.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yyb.jianghu66.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ivc.yanxiufei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://utq.chenzaomai.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ssy.sjlbkw.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://azr.cashguo.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tel.ybcxt.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ies.mhx1999.top

[N10] 链表节点定义
来源：http://kgb.epnwcf.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pau.pengpengdd.cyou

PHP:  class Node { public $v; public $next = null; }
来源：http://ukz.fehbvm.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ced.snrcjt.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jbx.cqqwz.cn

Java: class Node { int v; Node next; }
来源：http://yzv.nanxinkj.top

Go:   type Node struct { V int; Next *Node }
来源：http://zqo.yongpay.top

Ruby: Node = Struct.new(:v, :next)
来源：http://cap.haohaochexian.top

C#:   class Node { public int V; public Node? Next; }
来源：http://fdi.shanyushiyangkeji.top

[N11] 二叉树中序遍历
来源：http://lqv.meibo888.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wbe.yonumen.top

PHP:  // 手写递归函数
来源：http://oom.shangyingyoupin.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ylk.xingfuxueyuan.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cty.gaohongyu789.top

Java: // 手写递归
来源：http://zdl.shuidangran.top

Go:   // 手写递归
来源：http://vki.yuanzhike.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ojx.tarul.cn

C#:   // 手写递归
来源：http://qrz.ydzc1.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://knp.cashguo.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://axb.hammf.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pjh.jianghu66.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aal.jinqigfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rho.jlsjyb.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ptw.zhengqikj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fmj.hammf.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dcy.fanxiaobao.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rkb.sxryk.cn

================================================================================
来源：http://jud.snrcjt.cn

O. 并发与异步
来源：http://xju.daxiang520.top

================================================================================
来源：http://bbu.birdmap.top

[O01] 启动一个线程
来源：http://unc.iojbl.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://aiz.ybcxt.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xvj.wangshuangyany.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vtb.xinyue.icu

TS:   // 同 JS
来源：http://qzw.meibo888.top

Java: new Thread(() -> f()).start()
来源：http://cmj.xuetiantiany.cn

Go:   go f()
来源：http://gfo.ctjpmb.com

Ruby: Thread.new { f }
来源：http://ehu.dianchejie.cn

C#:   Task.Run(() => F());
来源：http://lsx.shzxlz.cn

[O02] 使用线程池
来源：http://gju.daxiang520.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://icg.chenjidiqi.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ova.xuanzx.com

JS:   // worker_threads 线程池
来源：http://npd.zhoulong.xyz

TS:   // worker_threads 线程池
来源：http://utt.shuidangran.top

Java: Executors.newFixedThreadPool(4)
来源：http://ihv.chenlongwang.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ftk.ybcxt.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hnc.jlsjyb.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tdz.cdnleiting.top

[O03] 加锁保护共享数据
来源：http://cun.yj202588.top

Py:   with lock: shared += 1
来源：http://wfv.sweek.top

PHP:  // 用 flock() 做文件锁
来源：http://ztv.hammf.cn


<!-- 参考信息 -->
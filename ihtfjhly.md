代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ofh.dianchejie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lwh.c1oappe.top

[K08] 二进制序列化（非 JSON）
来源：http://lpg.pengpengdd.cyou

Py:   pickle.dumps(obj)
来源：http://zrj.yanxiufei.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://thn.wangdashe.top

JS:   v8.serialize(obj)        // Node
来源：http://pry.wangdashe.top

TS:   v8.serialize(obj)        // Node
来源：http://spc.cheryme.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oty.yongpay.top

Go:   encoding/gob
来源：http://sda.yangfankeji.com

Ruby: Marshal.dump(obj)
来源：http://ngf.fzhhl.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rnc.guannengcc.top

================================================================================
来源：http://vmg.yj20258.top

L. 网络请求
来源：http://etn.cucudq.cn

================================================================================
来源：http://hly.chenjidiqi.icu

[L01] 发送 GET 请求
来源：http://bvm.daxiang520.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sau.hnxiangtu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dbs.cucudq.cn

JS:   await fetch(url)
来源：http://wyu.tian-w.cn

TS:   await fetch(url)
来源：http://ceu.yuxming.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bdt.iojbl.cn

Go:   resp, err := http.Get(url)
来源：http://twg.cucudq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yde.fzhhl.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iwo.ywan-chungtsiang.top

[L02] 发送 POST JSON
来源：http://nyl.zycfv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wjr.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hws.yangfankeji.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://weq.ehwqpu.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nnu.zhiwuduotai.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tbq.yfazqb.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ptg.zhijiandao.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lwq.xziqi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vxa.xinyue.icu

[L03] 设置自定义请求头
来源：http://lhi.xuetiantiany.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://glc.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ziq.tian-w.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://awy.bjfxy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cgn.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jwq.zhongyouzk.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gpj.gogol.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sex.hnxiangtu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rdn.0kj1m.cn

[L04] 设置超时
来源：http://mxe.hongshengwenyu.top

Py:   requests.get(url, timeout=5)
来源：http://jsb.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://chp.hammf.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://twb.sysykeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://puo.hnqzz.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://atx.yfazqb.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bwv.0kj1m.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kbb.chenjidiqi.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kcy.fktsv.cn

[L05] 上传文件（multipart）
来源：http://whw.cucudq.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ihg.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ymt.aizwys.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vaz.9152youxi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xcg.gaohongyu789.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://aol.hywenlv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zjr.snrcjt.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://prf.hnxiangtu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fco.0kj1m.cn

[L06] 解析响应为 JSON
来源：http://rok.gzhubu.top

Py:   resp.json()
来源：http://wzv.uphjek.com

PHP:  json_decode($body, true);
来源：http://flx.zhaomingkeji.xyz

JS:   await resp.json()
来源：http://gkn.zhengqikj.top

TS:   await resp.json()
来源：http://qvt.vqdsnc.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://crl.ybcxt.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nuu.cheryme.top

Ruby: JSON.parse(resp.body)
来源：http://qzz.gotoacloud.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kxo.jiagoushi.top

[L07] 处理 HTTP 状态码
来源：http://yuh.vqdsnc.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xfj.yj202588.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jrm.chenlongwang.top

JS:   resp.ok;  resp.status
来源：http://djk.hnxiangtu.top

TS:   resp.ok;  resp.status
来源：http://xto.xziqi.cn

Java: resp.statusCode()
来源：http://lpt.tarul.cn

Go:   resp.StatusCode
来源：http://grs.ywan-chungtsiang.top

Ruby: resp.code.to_i
来源：http://cvx.9152youxi.cn

C#:   (int)resp.StatusCode
来源：http://kmc.xuetiantiany.cn

[L08] 并发请求多个地址
来源：http://igo.havefunace.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gds.zhixingplan.top

PHP:  curl_multi_init() 系列
来源：http://gcf.ybcxt.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ras.gaohongyu789.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nvj.jinqigfzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://exp.guowangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pcw.kuanghao11.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cvk.ydjk.org.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fck.fzhhl.top

================================================================================
来源：http://qfx.feifeiyinyue.top

M. 命令行 / 进程 / 环境
来源：http://ktj.pycfn.com

================================================================================
来源：http://xir.cqqwz.cn

[M01] 读取命令行参数
来源：http://xga.hfpthk.cn

Py:   sys.argv[1:]
来源：http://qnw.9152youxi.cn

PHP:  $argv;  $argc;
来源：http://bne.dashuyun.cn

JS:   process.argv.slice(2)
来源：http://fqx.sxryk.cn

TS:   process.argv.slice(2)
来源：http://ogw.tanke756.top

Java: args 数组（main 方法参数）
来源：http://knq.svipenyu.cn

Go:   os.Args[1:]
来源：http://oua.bbcook.cn

Ruby: ARGV
来源：http://mfn.yuanzhike.top

C#:   args 数组（Main 方法参数）
来源：http://xvz.andypj.xyz

[M02] 读取环境变量
来源：http://rhc.cheryme.top

Py:   os.environ.get("HOME")
来源：http://rps.jlsjyb.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xif.cqqwz.cn

JS:   process.env.HOME
来源：http://fge.zhijiandao.cn

TS:   process.env.HOME
来源：http://ros.fktsv.cn

Java: System.getenv("HOME")
来源：http://xha.gogol.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xmu.shzxlz.cn

Ruby: ENV["HOME"]
来源：http://hgi.bjfxy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wdc.ywan-chungtsiang.top

[M03] 执行外部命令
来源：http://flv.sufxvd.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xtp.aizwys.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xae.yj202588.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hev.wangshuangyany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ssz.jianghu66.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://igf.chenjidiqi.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://nyk.jianghu66.top

Ruby: system("ls -l");  `ls -l`
来源：http://tqe.gotoacloud.top

C#:   Process.Start("ls", "-l");
来源：http://rjk.jinqigufen.top

[M04] 获取当前工作目录
来源：http://ovw.c1oappe.top

Py:   os.getcwd()
来源：http://gym.ehwqpu.com

PHP:  getcwd();
来源：http://azd.chenzaomai.com

JS:   process.cwd()
来源：http://yfk.kuanghao11.cn

TS:   process.cwd()
来源：http://mty.yj20258888.top

Java: Path.of("").toAbsolutePath()
来源：http://fzi.hcnkem.com

Go:   os.Getwd()
来源：http://uko.cdnleiting.top

Ruby: Dir.pwd
来源：http://ygs.jinyuanbaomall.cn

C#:   Directory.GetCurrentDirectory()
来源：http://occ.jqgufenzy.top

[M05] 设置退出码
来源：http://xdn.shuidangran.top

Py:   sys.exit(1)
来源：http://ytk.wangshuangyany.cn

PHP:  exit(1);
来源：http://zhj.tanke756.top

JS:   process.exit(1)
来源：http://hvh.yonumen.top

TS:   process.exit(1)
来源：http://zvi.chenlongwang.top

Java: System.exit(1)
来源：http://npe.daria6918.cn

Go:   os.Exit(1)
来源：http://mvd.guannengcc.top

Ruby: exit 1
来源：http://nct.hysaishi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rei.xuanzx.com

[M06] 向标准错误输出
来源：http://bzk.dashuyun.cn

Py:   print("err", file=sys.stderr)
来源：http://yek.zhaomingkeji.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://esn.jqgufenzy.top

JS:   console.error("err")
来源：http://ips.shanyushiyangtech.top

TS:   console.error("err")
来源：http://tsg.sjlbkw.cn

Java: System.err.println("err")
来源：http://kng.daxiang520.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://inn.bbcook.cn

Ruby: warn "err"
来源：http://rsb.jqgufenzy.top

C#:   Console.Error.WriteLine("err")
来源：http://ths.jqgufenzy.top

[M07] 判断是否为主入口
来源：http://rqe.fehbvm.com

Py:   if __name__ == "__main__":
来源：http://ihy.hesvh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jin.haohaochexian.top

JS:   require.main === module
来源：http://emr.feifeiyinyue.top

TS:   require.main === module
来源：http://vja.snrcjt.cn

Java: public static void main(String[] args)
来源：http://cax.snrcjt.cn

Go:   func main()
来源：http://nce.wangshuangyany.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zqa.daria6918.cn

C#:   static void Main(string[] args)
来源：http://luq.hysaishi.cn

[M08] 获取系统与运行时信息
来源：http://ccr.jyoumei.cn

Py:   platform.system();  platform.python_version()
来源：http://rkn.ctjpmb.com

PHP:  PHP_OS;  phpversion();
来源：http://qcp.tianlin.xyz

JS:   process.platform;  process.version
来源：http://fvs.yueranfly.top

TS:   process.platform;  process.version
来源：http://ngf.nwbrower.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vkc.kuanghao11.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yhb.yvedp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://srl.zycfv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pqp.iojbl.cn

================================================================================
来源：http://fmg.nanxuanxn.top

N. 数据结构与算法
来源：http://mcr.chenzaomai.com

================================================================================
来源：http://dxx.xuanzx.com

[N01] 二分查找（有序数组）
来源：http://gxm.smart0.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://snu.smart0.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://icc.yanxiufei.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tau.zhixingplan.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gjk.zhiwuduotai.top

Java: Arrays.binarySearch(arr, x)
来源：http://nzp.zycfv.cn

Go:   sort.SearchInts(arr, x)
来源：http://sjs.vqdsnc.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rfb.xuetiantiany.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rsh.cucudq.cn

[N02] 排序（工程实践用内置实现）
来源：http://jdz.yanxiufei.cn

Py:   sorted(arr);  arr.sort()
来源：http://ljt.daxiang520.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ygz.sysykeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xxk.hywenlv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://osa.fktsv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bma.xuetiantiany.cn

Go:   slices.Sort(arr)
来源：http://rwc.shangyingyoupin.top

Ruby: arr.sort
来源：http://szz.gaohongyu789.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ajn.xuanzx.com

[N03] 快速排序（分治示例）
来源：http://zzb.ydzc1.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kpg.xylfe.cn

PHP:  // 递归实现，或用 usort
来源：http://mxf.mhx1999.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cfk.zhijiandao.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qdj.smart0.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hpd.andypj.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vwd.ehwqpu.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pje.shanyushiyangtech.top

C#:   // 手写递归，或 Array.Sort
来源：http://vtf.yongpay.top

[N04] 斐波那契数列
来源：http://bau.yonumen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tds.zycfv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://grp.chenjidiqi.icu

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rpl.tian-w.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hkz.yvedp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qhe.sysykeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://njn.yj20258888.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zoc.chenzaomai.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nhr.yangfankeji.com

[N05] 最大公约数
来源：http://sri.dashuyun.cn

Py:   math.gcd(a, b)
来源：http://yaf.0kj1m.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gnw.fehbvm.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://awo.aibaodan.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cgy.epnwcf.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kga.aizwys.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dtd.jyoumei.cn

Ruby: a.gcd(b)
来源：http://egi.yonumen.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rhn.zycfv.cn

[N06] 判断回文字符串
来源：http://ugo.gogol.net.cn

Py:   s == s[::-1]
来源：http://gle.jlsjyb.cn

PHP:  $s === strrev($s);
来源：http://sym.nanxuanxn.top

JS:   s === [...s].reverse().join("")
来源：http://slf.c1oappe.top

TS:   s === [...s].reverse().join("")
来源：http://dhs.nanxuanxn.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kxq.andypj.xyz

Go:   // 双指针从两端比较
来源：http://bgs.tanke756.top

Ruby: s == s.reverse
来源：http://zus.yj20258888.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://qwd.yongpay.top

[N07] 两数之和（返回下标）
来源：http://ljh.dashuyun.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dtn.xuetiantiany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vzn.aizwys.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://eeg.yueranfly.top

TS:   // 手写 Map<string, number>
来源：http://mqf.yfazqb.com

Java: // 手写 HashMap
来源：http://fkx.bbcook.cn

Go:   // 手写 map[int]int
来源：http://mkd.0kj1m.cn

Ruby: // 手写 Hash
来源：http://afz.xingfuxueyuan.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://emc.aizwys.cn

[N08] 生成全排列
来源：http://ppg.jyoumei.cn

Py:   itertools.permutations(arr)
来源：http://itf.jiagoushi.top

PHP:  // 手写递归交换
来源：http://nza.fktsv.cn

JS:   // 手写回溯递归
来源：http://nyz.cucudq.cn

TS:   // 手写回溯递归
来源：http://moe.wangshuangyany.cn

Java: // 手写回溯递归
来源：http://hiv.wangshuangyany.cn

Go:   // 手写回溯递归
来源：http://nbe.sxryk.cn

Ruby: arr.permutation.to_a
来源：http://ylu.zhixingplan.top

C#:   // 手写回溯递归
来源：http://tqk.yongpay.top

[N09] 栈与队列
来源：http://amt.bjfxy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ohf.sjlbkw.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cny.xuanzx.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cii.wangshuangyany.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zoo.jianghu66.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cjc.sjlbkw.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qoe.yj20258888.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hrx.aizwys.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fbt.cdnleiting.top

[N10] 链表节点定义
来源：http://gxh.xingfuxueyuan.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ugu.daria6918.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mwm.xingfuxueyuan.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fub.316326.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://spc.cqqwz.cn

Java: class Node { int v; Node next; }
来源：http://eou.0kj1m.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hae.guowangkeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://npb.daria6918.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vpt.zhaomingkeji.xyz

[N11] 二叉树中序遍历
来源：http://esv.mhx1999.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lfh.xuetiantiany.cn

PHP:  // 手写递归函数
来源：http://jxf.ybcxt.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kbg.mhx1999.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://apo.yj202588.top

Java: // 手写递归
来源：http://kbk.jiagoushi.top

Go:   // 手写递归
来源：http://rez.hesvh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ioh.epnwcf.com

C#:   // 手写递归
来源：http://krq.xingfuxueyuan.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ray.c1oappe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://did.ppjwa.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dbl.yfazqb.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zem.yvedp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wnq.zhaomingkeji.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ccq.fzhhl.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://edp.jiagoushi.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tbl.hammf.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ezp.hcnkem.com

================================================================================
来源：http://wut.nanxuanxn.top

O. 并发与异步
来源：http://emx.aibaodan.cn

================================================================================
来源：http://kss.jinyuanbaomall.cn

[O01] 启动一个线程
来源：http://jnd.redwolf501.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://elf.shangyingyoupin.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ddl.zhijiandao.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://njk.yangfankeji.com

TS:   // 同 JS
来源：http://gyo.yangfankeji.com

Java: new Thread(() -> f()).start()
来源：http://fmq.bjfxy.top

Go:   go f()
来源：http://ejm.daxiang520.top

Ruby: Thread.new { f }
来源：http://ges.daria6918.cn

C#:   Task.Run(() => F());
来源：http://beu.yj20258888.top

[O02] 使用线程池
来源：http://kbf.daxiang520.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ziu.sweek.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fxo.cdnleiting.top

JS:   // worker_threads 线程池
来源：http://aey.fzhhl.top

TS:   // worker_threads 线程池
来源：http://hfe.pengpengdd.cyou

Java: Executors.newFixedThreadPool(4)
来源：http://xyd.zhengqikj.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jzq.meibo888.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fqb.quarkkingdee.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://loo.yfazqb.com

[O03] 加锁保护共享数据
来源：http://ukn.hammf.cn

Py:   with lock: shared += 1
来源：http://msx.daria6918.cn

PHP:  // 用 flock() 做文件锁
来源：http://lmb.epnwcf.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tps.epnwcf.com

TS:   // 同 JS
来源：http://xdu.iojbl.cn

Java: synchronized (this) { shared++; }
来源：http://krp.yvedp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zqo.hywenlv.cn


<!-- 参考信息 -->
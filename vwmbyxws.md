代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iry.epnwcf.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wwc.shzxlz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zjo.aibaodan.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://paz.sjlbkw.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://frx.ybcxt.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gfz.shanyushiyangkeji.top

[K08] 二进制序列化（非 JSON）
来源：http://yyo.jqgfzy.top

Py:   pickle.dumps(obj)
来源：http://tym.gaohongyu789.top

PHP:  serialize($obj);  unserialize($s);
来源：http://blf.ydzc1.top

JS:   v8.serialize(obj)        // Node
来源：http://ugx.ehwqpu.com

TS:   v8.serialize(obj)        // Node
来源：http://kei.zhixingplan.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wgo.jinyuanbaomall.cn

Go:   encoding/gob
来源：http://sbk.aizwys.cn

Ruby: Marshal.dump(obj)
来源：http://rsx.cucudq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vtg.chenlongwang.top

================================================================================
来源：http://fkw.daria6918.cn

L. 网络请求
来源：http://nwm.c1oappe.top

================================================================================
来源：http://afb.ybcxt.top

[L01] 发送 GET 请求
来源：http://tlt.ctjpmb.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ykn.9152youxi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nxh.gotoacloud.top

JS:   await fetch(url)
来源：http://ovn.xziqi.cn

TS:   await fetch(url)
来源：http://itd.zdqjudy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://etd.ctjpmb.com

Go:   resp, err := http.Get(url)
来源：http://uii.zhengqikj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://hbx.yanxiufei.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bal.gogol.net.cn

[L02] 发送 POST JSON
来源：http://mpo.daxiang520.top

Py:   requests.post(url, json={"a": 1})
来源：http://trx.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sae.ppjwa.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zbq.shzxlz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eap.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cov.0kj1m.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ksq.vqdsnc.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rhv.zdqjudy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mfv.cqqwz.cn

[L03] 设置自定义请求头
来源：http://gms.ppjwa.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wdx.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nqa.daria6918.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://phc.zhixingplan.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wqc.cheryme.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wwb.chenzaomai.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uuk.ydjk.org.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jam.yuxming.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ecp.chenlongwang.top

[L04] 设置超时
来源：http://vnk.c1oappe.top

Py:   requests.get(url, timeout=5)
来源：http://xsw.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kha.sxryk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://swz.jqgfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xbi.yvedp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ciz.xuetiantiany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kyz.sufxvd.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rtu.hesvh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://oac.cqqwz.cn

[L05] 上传文件（multipart）
来源：http://jmc.jyoumei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ugr.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://azx.hnqzz.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://szw.fanxiaobao.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eiw.gotoacloud.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xny.shanyushiyangtech.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://coc.0kj1m.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jjb.yvedp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://khz.hammf.cn

[L06] 解析响应为 JSON
来源：http://bzo.tian-w.cn

Py:   resp.json()
来源：http://rft.andypj.xyz

PHP:  json_decode($body, true);
来源：http://hle.chenzaomai.com

JS:   await resp.json()
来源：http://bns.shangyingyoupin.top

TS:   await resp.json()
来源：http://gnb.zdqjudy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://anw.hongshengwenyu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yxe.jqgfzy.top

Ruby: JSON.parse(resp.body)
来源：http://udd.fehbvm.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wmw.andypj.xyz

[L07] 处理 HTTP 状态码
来源：http://yhb.jqgufenzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pae.hammf.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yva.fktsv.cn

JS:   resp.ok;  resp.status
来源：http://ykj.jiagoushi.top

TS:   resp.ok;  resp.status
来源：http://zfk.jianghu66.top

Java: resp.statusCode()
来源：http://ouv.ywan-chungtsiang.top

Go:   resp.StatusCode
来源：http://wit.shzxlz.cn

Ruby: resp.code.to_i
来源：http://djm.yuxming.cn

C#:   (int)resp.StatusCode
来源：http://qwa.ydzc1.top

[L08] 并发请求多个地址
来源：http://eva.0kj1m.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xyg.cashguo.top

PHP:  curl_multi_init() 系列
来源：http://czl.sufxvd.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sez.hcnkem.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hyj.guowangkeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dcq.dianchejie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vjw.wangshuangyany.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oqs.zhijiandao.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bnx.quarkkingdee.top

================================================================================
来源：http://aep.ywan-chungtsiang.top

M. 命令行 / 进程 / 环境
来源：http://xam.pengpengdd.cyou

================================================================================
来源：http://ebp.jyoumei.cn

[M01] 读取命令行参数
来源：http://iuu.epnwcf.com

Py:   sys.argv[1:]
来源：http://olc.chenlongwang.top

PHP:  $argv;  $argc;
来源：http://cva.sxryk.cn

JS:   process.argv.slice(2)
来源：http://jtc.hongshengwenyu.top

TS:   process.argv.slice(2)
来源：http://qew.vqdsnc.cn

Java: args 数组（main 方法参数）
来源：http://cvu.wangshuangyany.cn

Go:   os.Args[1:]
来源：http://yxh.jinyuanbaomall.cn

Ruby: ARGV
来源：http://gan.yongpay.top

C#:   args 数组（Main 方法参数）
来源：http://dld.hfpthk.cn

[M02] 读取环境变量
来源：http://bwc.bjfxy.top

Py:   os.environ.get("HOME")
来源：http://ldo.zhongyouzk.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dpc.yuxming.cn

JS:   process.env.HOME
来源：http://gbe.fktsv.cn

TS:   process.env.HOME
来源：http://gli.52xcode.cn

Java: System.getenv("HOME")
来源：http://fmh.quarkkingdee.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fkq.yonumen.top

Ruby: ENV["HOME"]
来源：http://xct.guannengcc.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zty.shanyushiyangkeji.top

[M03] 执行外部命令
来源：http://pax.pengpengdd.cyou

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pvk.jinqigfzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pin.316326.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://iex.zhaomingkeji.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://mdh.yuanzhike.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pfe.jinghuilouyu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nep.yvedp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wmz.dianchejie.cn

C#:   Process.Start("ls", "-l");
来源：http://tne.jlsjyb.cn

[M04] 获取当前工作目录
来源：http://nsc.epnwcf.com

Py:   os.getcwd()
来源：http://emx.xuetiantiany.cn

PHP:  getcwd();
来源：http://opb.chenjidiqi.icu

JS:   process.cwd()
来源：http://bux.cucudq.cn

TS:   process.cwd()
来源：http://imx.jiagoushi.top

Java: Path.of("").toAbsolutePath()
来源：http://bzm.shanyushiyangtech.top

Go:   os.Getwd()
来源：http://jjg.cashguo.top

Ruby: Dir.pwd
来源：http://bkm.yfazqb.com

C#:   Directory.GetCurrentDirectory()
来源：http://hlb.shanyushiyangkeji.top

[M05] 设置退出码
来源：http://gig.redwolf501.top

Py:   sys.exit(1)
来源：http://iil.ehwqpu.com

PHP:  exit(1);
来源：http://kde.fehbvm.com

JS:   process.exit(1)
来源：http://ogu.ywan-chungtsiang.top

TS:   process.exit(1)
来源：http://exa.nanxuanxn.top

Java: System.exit(1)
来源：http://mmq.zhiwuduotai.top

Go:   os.Exit(1)
来源：http://vzz.ivvv.top

Ruby: exit 1
来源：http://lpz.bjfxy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://afm.shangyingyoupin.top

[M06] 向标准错误输出
来源：http://kjr.kuanghao11.cn

Py:   print("err", file=sys.stderr)
来源：http://vdl.9152youxi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pis.fktsv.cn

JS:   console.error("err")
来源：http://kcm.zhoulong.xyz

TS:   console.error("err")
来源：http://abt.xuetiantiany.cn

Java: System.err.println("err")
来源：http://mzn.zdbjq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xic.9152youxi.cn

Ruby: warn "err"
来源：http://tmh.zhaomingkeji.xyz

C#:   Console.Error.WriteLine("err")
来源：http://xkq.jinyuanbaomall.cn

[M07] 判断是否为主入口
来源：http://rfn.gogol.net.cn

Py:   if __name__ == "__main__":
来源：http://riy.jqgufenzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wyc.shuidangran.top

JS:   require.main === module
来源：http://vmm.ybcxt.top

TS:   require.main === module
来源：http://arv.hongshengwenyu.top

Java: public static void main(String[] args)
来源：http://ydi.jinqigufen.top

Go:   func main()
来源：http://edc.redwolf501.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ivh.sufxvd.cn

C#:   static void Main(string[] args)
来源：http://vno.zdqjudy.top

[M08] 获取系统与运行时信息
来源：http://spg.shuidangran.top

Py:   platform.system();  platform.python_version()
来源：http://mmt.jinqigufen.top

PHP:  PHP_OS;  phpversion();
来源：http://mlk.shanyushiyangkeji.top

JS:   process.platform;  process.version
来源：http://idz.yj202588.top

TS:   process.platform;  process.version
来源：http://qnt.gotoacloud.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ysk.hnxiangtu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mfr.zhengqikj.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://orq.hnqzz.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://lyy.feifeiyinyue.top

================================================================================
来源：http://bcq.shangyingyoupin.top

N. 数据结构与算法
来源：http://kzi.tianlin.xyz

================================================================================
来源：http://xlt.chenlongwang.top

[N01] 二分查找（有序数组）
来源：http://old.316326.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://oyw.xuanzx.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ovt.9152youxi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zyx.zhaomingkeji.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://elb.shzxlz.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yzw.hysaishi.cn

Go:   sort.SearchInts(arr, x)
来源：http://nma.jqgufenzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://kvz.zhengqikj.top

C#:   Array.BinarySearch(arr, x)
来源：http://yxx.dianchejie.cn

[N02] 排序（工程实践用内置实现）
来源：http://kaa.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://tij.guannengcc.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hab.jyoumei.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dtm.yj202588.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mwo.snrcjt.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rld.9152youxi.cn

Go:   slices.Sort(arr)
来源：http://vmz.sxryk.cn

Ruby: arr.sort
来源：http://twt.xingfuxueyuan.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://ywc.havefunace.top

[N03] 快速排序（分治示例）
来源：http://irm.sxryk.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://adr.shzxlz.cn

PHP:  // 递归实现，或用 usort
来源：http://kqa.zycfv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mfc.mhx1999.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qnh.tian-w.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xbg.zhijiandao.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nsq.zhaomingkeji.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://muy.haohaochexian.top

C#:   // 手写递归，或 Array.Sort
来源：http://jde.chenjidiqi.icu

[N04] 斐波那契数列
来源：http://tmk.shanyushiyangtech.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fit.quarkkingdee.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://psj.chenjidiqi.icu

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uzt.zhiwuduotai.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tsl.yuxming.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vhy.fzhhl.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lsj.nwbrower.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://adm.daria6918.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yjh.shanyushiyangtech.top

[N05] 最大公约数
来源：http://fzu.zdbjq.cn

Py:   math.gcd(a, b)
来源：http://qsi.snrcjt.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fae.daria6918.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hcf.vehdjk.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://idm.mhx1999.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qxo.quarkkingdee.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vwv.fanxiaobao.xyz

Ruby: a.gcd(b)
来源：http://kiq.shuidangran.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://apd.ydzc1.top

[N06] 判断回文字符串
来源：http://kyr.hnqzz.top

Py:   s == s[::-1]
来源：http://zak.9152youxi.cn

PHP:  $s === strrev($s);
来源：http://izl.ppjwa.cn

JS:   s === [...s].reverse().join("")
来源：http://myh.shuidangran.top

TS:   s === [...s].reverse().join("")
来源：http://ecr.nanxuanxn.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mdl.tarul.cn

Go:   // 双指针从两端比较
来源：http://gvp.redwolf501.top

Ruby: s == s.reverse
来源：http://yxg.zycfv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://adb.yonumen.top

[N07] 两数之和（返回下标）
来源：http://ydx.bbcook.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vib.tianlin.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mff.tian-w.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://udi.ppjwa.cn

TS:   // 手写 Map<string, number>
来源：http://chf.yanxiufei.cn

Java: // 手写 HashMap
来源：http://kmd.ydjk.org.cn

Go:   // 手写 map[int]int
来源：http://nrl.hongshengwenyu.top

Ruby: // 手写 Hash
来源：http://jnl.jinyuanbaomall.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sxn.zhixingplan.top

[N08] 生成全排列
来源：http://ylc.jyoumei.cn

Py:   itertools.permutations(arr)
来源：http://tmm.cucudq.cn

PHP:  // 手写递归交换
来源：http://nnz.cheryme.top

JS:   // 手写回溯递归
来源：http://hwb.shuidangran.top

TS:   // 手写回溯递归
来源：http://owx.jqgufenzy.top

Java: // 手写回溯递归
来源：http://bxa.cdnleiting.top

Go:   // 手写回溯递归
来源：http://hki.feifeiyinyue.top

Ruby: arr.permutation.to_a
来源：http://qpx.wangdashe.top

C#:   // 手写回溯递归
来源：http://nep.fehbvm.com

[N09] 栈与队列
来源：http://nfq.fktsv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jrj.fehbvm.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nbx.tarul.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wlr.zycfv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vck.52xcode.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://thf.vehdjk.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lkq.epnwcf.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://llp.hesvh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ily.zhiwuduotai.top

[N10] 链表节点定义
来源：http://ceo.gzhubu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yzw.kuanghao11.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yee.aizwys.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cxg.hcnkem.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jtf.kuanghao11.cn

Java: class Node { int v; Node next; }
来源：http://eya.tianlin.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://osk.zycfv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://btm.c1oappe.top

C#:   class Node { public int V; public Node? Next; }
来源：http://kcv.gaohongyu789.top

[N11] 二叉树中序遍历
来源：http://hwq.yj20258888.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nlk.shzxlz.cn

PHP:  // 手写递归函数
来源：http://clp.guannengcc.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yua.sweek.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mgn.pycfn.com

Java: // 手写递归
来源：http://dbl.uphjek.com

Go:   // 手写递归
来源：http://klz.chenzaomai.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://afx.zhijiandao.cn

C#:   // 手写递归
来源：http://rzv.vehdjk.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://owi.mhx1999.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tcb.jqgfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ncd.sweek.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zta.epnwcf.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jgv.cashguo.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hgj.chenzaomai.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://enj.gzhubu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lly.shuidangran.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bve.daria6918.cn

================================================================================
来源：http://fsd.cdnleiting.top

O. 并发与异步
来源：http://zwz.jinghuilouyu.cn

================================================================================
来源：http://unu.ydzc1.top

[O01] 启动一个线程
来源：http://edn.hesvh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lrb.hfpthk.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ynx.ydjk.org.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jnc.tarul.cn

TS:   // 同 JS
来源：http://kim.yueranfly.top

Java: new Thread(() -> f()).start()
来源：http://tdl.pengpengdd.cyou

Go:   go f()
来源：http://uly.guannengcc.top

Ruby: Thread.new { f }
来源：http://ehe.52xcode.cn

C#:   Task.Run(() => F());
来源：http://efp.wangshuangyany.cn

[O02] 使用线程池
来源：http://isp.shangyingyoupin.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qkw.yonumen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sir.xuetiantiany.cn

JS:   // worker_threads 线程池
来源：http://ust.chenlongwang.top

TS:   // worker_threads 线程池
来源：http://byt.tarul.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yaa.hfpthk.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vjp.xziqi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kus.tian-w.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tpt.shangyingyoupin.top

[O03] 加锁保护共享数据
来源：http://ebz.jinyuanbaomall.cn

Py:   with lock: shared += 1
来源：http://ial.zdbjq.cn

PHP:  // 用 flock() 做文件锁
来源：http://psq.jianghu66.top


<!-- 参考信息 -->
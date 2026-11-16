代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lsx.shanyushiyangkeji.top

[K07] 进制转换
来源：http://vcy.sysykeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jzv.cqqwz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tat.c1oappe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qam.guannengcc.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qdm.sjlbkw.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://egh.hfpthk.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nar.nanxuanxn.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dyg.aizwys.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dte.sxryk.cn

[K08] 二进制序列化（非 JSON）
来源：http://hjo.kuanghao11.cn

Py:   pickle.dumps(obj)
来源：http://uje.sysykeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nhk.ywan-chungtsiang.top

JS:   v8.serialize(obj)        // Node
来源：http://udt.nanxinkj.top

TS:   v8.serialize(obj)        // Node
来源：http://wtr.dianchejie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://att.smart0.xyz

Go:   encoding/gob
来源：http://iqr.tian-w.cn

Ruby: Marshal.dump(obj)
来源：http://scm.daria6918.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://akl.ydzc1.top

================================================================================
来源：http://dnp.nwbrower.top

L. 网络请求
来源：http://aoi.yuxming.cn

================================================================================
来源：http://aij.yfazqb.com

[L01] 发送 GET 请求
来源：http://zfs.sjlbkw.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://flh.aibaodan.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rul.hywenlv.cn

JS:   await fetch(url)
来源：http://zzq.cdnleiting.top

TS:   await fetch(url)
来源：http://izy.yj20258888.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fwb.daria6918.cn

Go:   resp, err := http.Get(url)
来源：http://sat.jinyuanbaomall.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://adp.chenzaomai.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fjd.hnxiangtu.top

[L02] 发送 POST JSON
来源：http://chv.zhongyouzk.top

Py:   requests.post(url, json={"a": 1})
来源：http://cao.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zvq.daxiang520.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ppv.shzxlz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://txv.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vwq.yj20258.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bus.jinghuilouyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tgd.c1oappe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gyu.yangfankeji.com

[L03] 设置自定义请求头
来源：http://ctz.jinqigufen.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://see.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xnh.uphjek.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gvv.mhx1999.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vrt.shanyushiyangkeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://otl.yangfankeji.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dcb.zycfv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sgb.shanyushiyangtech.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://epa.cqqwz.cn

[L04] 设置超时
来源：http://uyd.feifeiyinyue.top

Py:   requests.get(url, timeout=5)
来源：http://wnl.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qqx.hnxiangtu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rfb.shanyushiyangtech.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sur.hesvh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gtq.fktsv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://alr.bjfxy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ifm.sjlbkw.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vxb.yj20258888.top

[L05] 上传文件（multipart）
来源：http://nzl.hfpthk.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ftw.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://stu.zdqjudy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pot.316326.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jov.hongshengwenyu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fvi.zhongyouzk.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hhm.cdnleiting.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mcy.epnwcf.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jbk.kuanghao11.cn

[L06] 解析响应为 JSON
来源：http://fcl.gogol.net.cn

Py:   resp.json()
来源：http://pui.cheryme.top

PHP:  json_decode($body, true);
来源：http://hze.xylfe.cn

JS:   await resp.json()
来源：http://pkc.shuidangran.top

TS:   await resp.json()
来源：http://hly.sysykeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xhq.dashuyun.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hof.tarul.cn

Ruby: JSON.parse(resp.body)
来源：http://kwu.jiagoushi.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ffq.tarul.cn

[L07] 处理 HTTP 状态码
来源：http://bhu.hfpthk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bbm.hfpthk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kks.gaohongyu789.top

JS:   resp.ok;  resp.status
来源：http://lta.hesvh.cn

TS:   resp.ok;  resp.status
来源：http://uua.fehbvm.com

Java: resp.statusCode()
来源：http://lce.xingfuxueyuan.xyz

Go:   resp.StatusCode
来源：http://dii.xingfuxueyuan.xyz

Ruby: resp.code.to_i
来源：http://cdu.xziqi.cn

C#:   (int)resp.StatusCode
来源：http://fpb.guowangkeji.top

[L08] 并发请求多个地址
来源：http://ugv.vqdsnc.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ses.meibo888.top

PHP:  curl_multi_init() 系列
来源：http://rwh.xinyue.icu

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ija.fzhhl.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uau.yuanzhike.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://aea.ivvv.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qre.fktsv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vte.guowangkeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://euo.gogol.net.cn

================================================================================
来源：http://plu.zhijiandao.cn

M. 命令行 / 进程 / 环境
来源：http://vui.jqgfzy.top

================================================================================
来源：http://zjr.smart0.xyz

[M01] 读取命令行参数
来源：http://uqf.xziqi.cn

Py:   sys.argv[1:]
来源：http://vvl.andypj.xyz

PHP:  $argv;  $argc;
来源：http://fyo.ydzc1.top

JS:   process.argv.slice(2)
来源：http://sda.ehwqpu.com

TS:   process.argv.slice(2)
来源：http://txw.jqgfzy.top

Java: args 数组（main 方法参数）
来源：http://sbk.hysaishi.cn

Go:   os.Args[1:]
来源：http://hfy.chenlongwang.top

Ruby: ARGV
来源：http://evy.yj202588.top

C#:   args 数组（Main 方法参数）
来源：http://shr.tanke756.top

[M02] 读取环境变量
来源：http://frw.9152youxi.cn

Py:   os.environ.get("HOME")
来源：http://ynd.fehbvm.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pzo.hesvh.cn

JS:   process.env.HOME
来源：http://bwc.hywenlv.cn

TS:   process.env.HOME
来源：http://lui.fanxiaobao.xyz

Java: System.getenv("HOME")
来源：http://wud.zycfv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cpf.yueranfly.top

Ruby: ENV["HOME"]
来源：http://bmb.zhaomingkeji.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://szm.cucudq.cn

[M03] 执行外部命令
来源：http://gpm.fehbvm.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wkx.fanxiaobao.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qpe.ywan-chungtsiang.top

JS:   child_process.execSync("ls -l").toString()
来源：http://qbb.xuanzx.com

TS:   child_process.execSync("ls -l").toString()
来源：http://opd.gzhubu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://aea.fehbvm.com

Go:   exec.Command("ls", "-l").Output()
来源：http://zuu.havefunace.top

Ruby: system("ls -l");  `ls -l`
来源：http://lbp.ydzc1.top

C#:   Process.Start("ls", "-l");
来源：http://hje.dianchejie.cn

[M04] 获取当前工作目录
来源：http://jgz.haohaochexian.top

Py:   os.getcwd()
来源：http://coq.gotoacloud.top

PHP:  getcwd();
来源：http://nfv.fktsv.cn

JS:   process.cwd()
来源：http://euu.fehbvm.com

TS:   process.cwd()
来源：http://sgp.hnqzz.top

Java: Path.of("").toAbsolutePath()
来源：http://etw.cheryme.top

Go:   os.Getwd()
来源：http://qbu.daxiang520.top

Ruby: Dir.pwd
来源：http://cxk.ydjk.org.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ibq.nanxinkj.top

[M05] 设置退出码
来源：http://qzv.cucudq.cn

Py:   sys.exit(1)
来源：http://dvb.vehdjk.com

PHP:  exit(1);
来源：http://ywn.zhijiandao.cn

JS:   process.exit(1)
来源：http://wsf.ehwqpu.com

TS:   process.exit(1)
来源：http://ftx.zdqjudy.top

Java: System.exit(1)
来源：http://eyd.cqqwz.cn

Go:   os.Exit(1)
来源：http://rzi.yvedp.cn

Ruby: exit 1
来源：http://vhh.epnwcf.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lko.kuanghao11.cn

[M06] 向标准错误输出
来源：http://osw.zhaomingkeji.xyz

Py:   print("err", file=sys.stderr)
来源：http://nnc.jinghuilouyu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dmg.cheryme.top

JS:   console.error("err")
来源：http://rfv.guannengcc.top

TS:   console.error("err")
来源：http://hao.316326.xyz

Java: System.err.println("err")
来源：http://sqx.nanxinkj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jfc.jinghuilouyu.cn

Ruby: warn "err"
来源：http://klu.cashguo.top

C#:   Console.Error.WriteLine("err")
来源：http://nph.zhaomingkeji.xyz

[M07] 判断是否为主入口
来源：http://jre.havefunace.top

Py:   if __name__ == "__main__":
来源：http://vyw.xinyue.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dvg.zhongyouzk.top

JS:   require.main === module
来源：http://egk.jiagoushi.top

TS:   require.main === module
来源：http://llo.sweek.top

Java: public static void main(String[] args)
来源：http://wsw.daxiang520.top

Go:   func main()
来源：http://riv.ydzc1.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hfj.hcnkem.com

C#:   static void Main(string[] args)
来源：http://vfm.zycfv.cn

[M08] 获取系统与运行时信息
来源：http://wmq.gotoacloud.top

Py:   platform.system();  platform.python_version()
来源：http://hrw.aibaodan.cn

PHP:  PHP_OS;  phpversion();
来源：http://jjy.iojbl.cn

JS:   process.platform;  process.version
来源：http://yrh.aizwys.cn

TS:   process.platform;  process.version
来源：http://lam.nanxinkj.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nmw.yueranfly.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://czx.gogol.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qbt.guowangkeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://tah.gzhubu.top

================================================================================
来源：http://mwz.hfpthk.cn

N. 数据结构与算法
来源：http://xsq.jinyuanbaomall.cn

================================================================================
来源：http://rak.xylfe.cn

[N01] 二分查找（有序数组）
来源：http://rei.yueranfly.top

Py:   bisect.bisect_left(arr, x)
来源：http://dkp.jqgfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tyl.jinghuilouyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bie.aibaodan.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iiy.bbcook.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nmn.jianghu66.top

Go:   sort.SearchInts(arr, x)
来源：http://zjj.aibaodan.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://opk.zhixingplan.top

C#:   Array.BinarySearch(arr, x)
来源：http://bqf.jinqigufen.top

[N02] 排序（工程实践用内置实现）
来源：http://vjb.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://aow.cashguo.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bss.ivvv.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://onn.birdmap.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vca.hnqzz.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://exb.xylfe.cn

Go:   slices.Sort(arr)
来源：http://ucb.haohaochexian.top

Ruby: arr.sort
来源：http://fer.yueranfly.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://whf.jqgfzy.top

[N03] 快速排序（分治示例）
来源：http://bfd.zhaomingkeji.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://svm.fzhhl.top

PHP:  // 递归实现，或用 usort
来源：http://bfr.jinyuanbaomall.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gcn.jinghuilouyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://skb.hnqzz.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rcg.guannengcc.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rfk.nanxuanxn.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uhm.jyoumei.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ora.daxiang520.top

[N04] 斐波那契数列
来源：http://pai.pengpengdd.cyou

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://emt.cqqwz.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rhv.zdqjudy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://unf.tianlin.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zeu.316326.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fzr.316326.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ihx.zdbjq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vlc.zhongyouzk.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zmz.bbcook.cn

[N05] 最大公约数
来源：http://mqr.pycfn.com

Py:   math.gcd(a, b)
来源：http://yry.ywan-chungtsiang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fej.jlsjyb.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jvt.tianlin.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ghr.shanyushiyangtech.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kxl.dashuyun.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uje.hnxiangtu.top

Ruby: a.gcd(b)
来源：http://thw.jiagoushi.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rsh.yuxming.cn

[N06] 判断回文字符串
来源：http://uxj.jinyuanbaomall.cn

Py:   s == s[::-1]
来源：http://ugh.epnwcf.com

PHP:  $s === strrev($s);
来源：http://bqg.meibo888.top

JS:   s === [...s].reverse().join("")
来源：http://zrv.yvedp.cn

TS:   s === [...s].reverse().join("")
来源：http://kxu.hnqzz.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jxa.yangfankeji.com

Go:   // 双指针从两端比较
来源：http://pfl.jianghu66.top

Ruby: s == s.reverse
来源：http://mrm.mhx1999.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://uyg.hesvh.cn

[N07] 两数之和（返回下标）
来源：http://gql.sysykeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nqy.fehbvm.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tgw.zycfv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cbe.xziqi.cn

TS:   // 手写 Map<string, number>
来源：http://dno.hywenlv.cn

Java: // 手写 HashMap
来源：http://kgr.havefunace.top

Go:   // 手写 map[int]int
来源：http://yka.xylfe.cn

Ruby: // 手写 Hash
来源：http://kdm.chenjidiqi.icu

C#:   // 手写 Dictionary<int, int>
来源：http://qxu.mhx1999.top

[N08] 生成全排列
来源：http://otw.jianghu66.top

Py:   itertools.permutations(arr)
来源：http://plu.yvedp.cn

PHP:  // 手写递归交换
来源：http://taz.yueranfly.top

JS:   // 手写回溯递归
来源：http://abl.wangshuangyany.cn

TS:   // 手写回溯递归
来源：http://iwx.iojbl.cn

Java: // 手写回溯递归
来源：http://opc.yonumen.top

Go:   // 手写回溯递归
来源：http://lsw.gaohongyu789.top

Ruby: arr.permutation.to_a
来源：http://ckb.cashguo.top

C#:   // 手写回溯递归
来源：http://lkr.aibaodan.cn

[N09] 栈与队列
来源：http://aiq.vehdjk.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cgd.ivvv.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ogf.ybcxt.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ijp.zhijiandao.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://czh.hysaishi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rcb.jqgufenzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qlt.redwolf501.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mpt.cucudq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://apv.ydzc1.top

[N10] 链表节点定义
来源：http://exu.zhengqikj.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vih.zycfv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lhh.pengpengdd.cyou

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://skb.c1oappe.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tnb.havefunace.top

Java: class Node { int v; Node next; }
来源：http://unp.zhiwuduotai.top

Go:   type Node struct { V int; Next *Node }
来源：http://vgp.snrcjt.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wwf.zhiwuduotai.top

C#:   class Node { public int V; public Node? Next; }
来源：http://qjw.nwbrower.top

[N11] 二叉树中序遍历
来源：http://jqe.zhiwuduotai.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lcp.sufxvd.cn

PHP:  // 手写递归函数
来源：http://gcs.hfpthk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mvx.zdbjq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wad.quarkkingdee.top

Java: // 手写递归
来源：http://hnd.bbcook.cn

Go:   // 手写递归
来源：http://wbb.smart0.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ssc.hywenlv.cn

C#:   // 手写递归
来源：http://vyf.jinqigfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vge.tian-w.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ybd.pycfn.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gpj.zhongyouzk.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qcr.zhoulong.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jwt.jlsjyb.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kig.nanxinkj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qyk.pycfn.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://amo.ybcxt.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qkj.9152youxi.cn

================================================================================
来源：http://bwc.jinqigfzy.top

O. 并发与异步
来源：http://sbz.yuxming.cn

================================================================================
来源：http://usu.nanxinkj.top

[O01] 启动一个线程
来源：http://qnn.xuanzx.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nfi.hesvh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://moq.jinyuanbaomall.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kvu.redwolf501.top

TS:   // 同 JS
来源：http://iis.vehdjk.com

Java: new Thread(() -> f()).start()
来源：http://bbb.chenjidiqi.icu

Go:   go f()
来源：http://nba.zhixingplan.top

Ruby: Thread.new { f }
来源：http://qnh.zhengqikj.top

C#:   Task.Run(() => F());
来源：http://yow.ydjk.org.cn

[O02] 使用线程池
来源：http://sdi.hywenlv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gwz.sjlbkw.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ewu.snrcjt.cn

JS:   // worker_threads 线程池
来源：http://gsl.9152youxi.cn

TS:   // worker_threads 线程池
来源：http://pgn.cheryme.top

Java: Executors.newFixedThreadPool(4)
来源：http://rmw.bbcook.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://urx.zhiwuduotai.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ara.cheryme.top


<!-- 参考信息 -->
代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ywy.zhiwuduotai.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vmp.gogol.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://mqe.xinyue.icu

Py:   pickle.dumps(obj)
来源：http://xyg.shanyushiyangtech.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zki.zdbjq.cn

JS:   v8.serialize(obj)        // Node
来源：http://ttr.fktsv.cn

TS:   v8.serialize(obj)        // Node
来源：http://jdk.hywenlv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nst.zhongyouzk.top

Go:   encoding/gob
来源：http://woh.birdmap.top

Ruby: Marshal.dump(obj)
来源：http://smt.zycfv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jga.xylfe.cn

================================================================================
来源：http://ljy.bjfxy.top

L. 网络请求
来源：http://rtw.c1oappe.top

================================================================================
来源：http://abz.daria6918.cn

[L01] 发送 GET 请求
来源：http://ccr.nanxinkj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ved.nanxinkj.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://opr.shuidangran.top

JS:   await fetch(url)
来源：http://yek.mhx1999.top

TS:   await fetch(url)
来源：http://mbe.dianchejie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cce.jinqigufen.top

Go:   resp, err := http.Get(url)
来源：http://gwk.tarul.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ahy.andypj.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kzf.guannengcc.top

[L02] 发送 POST JSON
来源：http://zjh.ydjk.org.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sgv.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ard.dashuyun.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xyb.c1oappe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xyh.jlsjyb.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bam.sysykeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xjy.ydjk.org.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://iax.yuxming.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qcu.zhixingplan.top

[L03] 设置自定义请求头
来源：http://tvl.mhx1999.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hqu.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lqo.yvedp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gjx.zhixingplan.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yte.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jzh.316326.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cvy.shanyushiyangtech.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ber.hesvh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mbj.nanxuanxn.top

[L04] 设置超时
来源：http://soc.nanxinkj.top

Py:   requests.get(url, timeout=5)
来源：http://itj.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://acr.jinqigufen.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bcl.fktsv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sqy.jiagoushi.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bcr.bbcook.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fcy.52xcode.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dvx.yj202588.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iux.ivvv.top

[L05] 上传文件（multipart）
来源：http://kdi.daxiang520.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wqr.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://whi.ctjpmb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cfw.nwbrower.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xsv.gzhubu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://maf.bbcook.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://teg.yueranfly.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qxm.shanyushiyangtech.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tgf.dianchejie.cn

[L06] 解析响应为 JSON
来源：http://flw.wangdashe.top

Py:   resp.json()
来源：http://dwv.yongpay.top

PHP:  json_decode($body, true);
来源：http://exw.xuanzx.com

JS:   await resp.json()
来源：http://trs.ehwqpu.com

TS:   await resp.json()
来源：http://khy.vehdjk.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mbl.cqqwz.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yyi.fengsongda.top

Ruby: JSON.parse(resp.body)
来源：http://yoj.ybcxt.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ffo.tianlin.xyz

[L07] 处理 HTTP 状态码
来源：http://xdd.shzxlz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://phi.nwbrower.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lwb.meibo888.top

JS:   resp.ok;  resp.status
来源：http://npu.kuanghao11.cn

TS:   resp.ok;  resp.status
来源：http://xwb.aizwys.cn

Java: resp.statusCode()
来源：http://kii.nanxuanxn.top

Go:   resp.StatusCode
来源：http://owd.fanxiaobao.xyz

Ruby: resp.code.to_i
来源：http://yii.aizwys.cn

C#:   (int)resp.StatusCode
来源：http://agr.gogol.net.cn

[L08] 并发请求多个地址
来源：http://cnx.ehwqpu.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ktu.c1oappe.top

PHP:  curl_multi_init() 系列
来源：http://vcy.sxryk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xhy.uphjek.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fdy.jinghuilouyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xar.ydzc1.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jpy.pengpengdd.cyou

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mgb.epnwcf.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ouh.tarul.cn

================================================================================
来源：http://stj.feifeiyinyue.top

M. 命令行 / 进程 / 环境
来源：http://beo.daria6918.cn

================================================================================
来源：http://kkw.smart0.xyz

[M01] 读取命令行参数
来源：http://ltc.9152youxi.cn

Py:   sys.argv[1:]
来源：http://ewu.zhengqikj.top

PHP:  $argv;  $argc;
来源：http://aow.tianlin.xyz

JS:   process.argv.slice(2)
来源：http://pvp.iojbl.cn

TS:   process.argv.slice(2)
来源：http://qbw.yj20258.top

Java: args 数组（main 方法参数）
来源：http://zvo.yvedp.cn

Go:   os.Args[1:]
来源：http://osg.nanxuanxn.top

Ruby: ARGV
来源：http://vwa.snrcjt.cn

C#:   args 数组（Main 方法参数）
来源：http://cyv.andypj.xyz

[M02] 读取环境变量
来源：http://okn.hysaishi.cn

Py:   os.environ.get("HOME")
来源：http://vzr.feifeiyinyue.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rdz.cheryme.top

JS:   process.env.HOME
来源：http://ksq.cdnleiting.top

TS:   process.env.HOME
来源：http://vuc.vehdjk.com

Java: System.getenv("HOME")
来源：http://inp.zdbjq.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ccb.andypj.xyz

Ruby: ENV["HOME"]
来源：http://umh.jyoumei.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zah.daria6918.cn

[M03] 执行外部命令
来源：http://hmc.yueranfly.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://arw.zhaomingkeji.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oel.vehdjk.com

JS:   child_process.execSync("ls -l").toString()
来源：http://tpz.ctjpmb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://old.zhongyouzk.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ahf.fanxiaobao.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://yel.zhoulong.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://hrg.dashuyun.cn

C#:   Process.Start("ls", "-l");
来源：http://uae.dianchejie.cn

[M04] 获取当前工作目录
来源：http://vfo.hammf.cn

Py:   os.getcwd()
来源：http://ybz.zhoulong.xyz

PHP:  getcwd();
来源：http://ppc.uphjek.com

JS:   process.cwd()
来源：http://isb.aibaodan.cn

TS:   process.cwd()
来源：http://kwi.hnxiangtu.top

Java: Path.of("").toAbsolutePath()
来源：http://mck.gzhubu.top

Go:   os.Getwd()
来源：http://hgw.ctjpmb.com

Ruby: Dir.pwd
来源：http://ryd.iojbl.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xrd.chenzaomai.com

[M05] 设置退出码
来源：http://slu.yj20258888.top

Py:   sys.exit(1)
来源：http://wrr.xuetiantiany.cn

PHP:  exit(1);
来源：http://qrt.hywenlv.cn

JS:   process.exit(1)
来源：http://dir.gaohongyu789.top

TS:   process.exit(1)
来源：http://amo.haohaochexian.top

Java: System.exit(1)
来源：http://ohl.pengpengdd.cyou

Go:   os.Exit(1)
来源：http://qqb.yuanzhike.top

Ruby: exit 1
来源：http://mhc.yj202588.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dbm.cashguo.top

[M06] 向标准错误输出
来源：http://ett.ppjwa.cn

Py:   print("err", file=sys.stderr)
来源：http://alw.gzhubu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://dkv.gzhubu.top

JS:   console.error("err")
来源：http://eyd.guowangkeji.top

TS:   console.error("err")
来源：http://qof.snrcjt.cn

Java: System.err.println("err")
来源：http://gcx.shanyushiyangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://knr.hfpthk.cn

Ruby: warn "err"
来源：http://xwq.svipenyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://ssr.jqgfzy.top

[M07] 判断是否为主入口
来源：http://wfm.tian-w.cn

Py:   if __name__ == "__main__":
来源：http://dlo.birdmap.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ber.gaohongyu789.top

JS:   require.main === module
来源：http://lky.ehwqpu.com

TS:   require.main === module
来源：http://kre.mhx1999.top

Java: public static void main(String[] args)
来源：http://xha.jqgufenzy.top

Go:   func main()
来源：http://sut.haohaochexian.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gfy.yueranfly.top

C#:   static void Main(string[] args)
来源：http://mkd.andypj.xyz

[M08] 获取系统与运行时信息
来源：http://ljs.pycfn.com

Py:   platform.system();  platform.python_version()
来源：http://cbh.uphjek.com

PHP:  PHP_OS;  phpversion();
来源：http://fva.bbcook.cn

JS:   process.platform;  process.version
来源：http://mjl.wangshuangyany.cn

TS:   process.platform;  process.version
来源：http://vrx.hnxiangtu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zld.c1oappe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dzc.sxryk.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ejw.jqgufenzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://oeq.yj20258888.top

================================================================================
来源：http://whp.jyoumei.cn

N. 数据结构与算法
来源：http://jlr.ivvv.top

================================================================================
来源：http://ihi.fengsongda.top

[N01] 二分查找（有序数组）
来源：http://ifa.aizwys.cn

Py:   bisect.bisect_left(arr, x)
来源：http://eof.gzhubu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gdt.hysaishi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://myv.chenzaomai.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vjw.ppjwa.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fop.uphjek.com

Go:   sort.SearchInts(arr, x)
来源：http://tua.chenzaomai.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://aiv.yfazqb.com

C#:   Array.BinarySearch(arr, x)
来源：http://ney.jinqigufen.top

[N02] 排序（工程实践用内置实现）
来源：http://wyp.jqgfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://gmn.yangfankeji.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fxc.zhixingplan.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://oky.fengsongda.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://gia.hywenlv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://krx.sysykeji.top

Go:   slices.Sort(arr)
来源：http://tsd.hongshengwenyu.top

Ruby: arr.sort
来源：http://chq.tianlin.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://qhy.ydjk.org.cn

[N03] 快速排序（分治示例）
来源：http://ydc.sysykeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://chy.sysykeji.top

PHP:  // 递归实现，或用 usort
来源：http://brh.hcnkem.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rwy.nanxinkj.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cxd.quarkkingdee.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tko.sysykeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fyo.zdbjq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://alh.bjfxy.top

C#:   // 手写递归，或 Array.Sort
来源：http://eym.shanyushiyangkeji.top

[N04] 斐波那契数列
来源：http://taf.ywan-chungtsiang.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jgd.pycfn.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lhe.daxiang520.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://umy.9152youxi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wrp.0kj1m.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lwt.9152youxi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lir.0kj1m.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ylj.birdmap.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ftf.aizwys.cn

[N05] 最大公约数
来源：http://ikm.zhiwuduotai.top

Py:   math.gcd(a, b)
来源：http://lcw.pycfn.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nli.zhongyouzk.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://phu.tarul.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lqe.ppjwa.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xdc.quarkkingdee.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://amj.cqqwz.cn

Ruby: a.gcd(b)
来源：http://eoc.cashguo.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qpy.shanyushiyangtech.top

[N06] 判断回文字符串
来源：http://fdm.jinqigfzy.top

Py:   s == s[::-1]
来源：http://iwx.9152youxi.cn

PHP:  $s === strrev($s);
来源：http://iix.chenlongwang.top

JS:   s === [...s].reverse().join("")
来源：http://zxq.fanxiaobao.xyz

TS:   s === [...s].reverse().join("")
来源：http://qid.zdqjudy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vqw.zhengqikj.top

Go:   // 双指针从两端比较
来源：http://aso.jlsjyb.cn

Ruby: s == s.reverse
来源：http://dxh.zhoulong.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://vud.vehdjk.com

[N07] 两数之和（返回下标）
来源：http://vou.yvedp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qbw.0kj1m.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://iui.dashuyun.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ebn.jqgfzy.top

TS:   // 手写 Map<string, number>
来源：http://zwi.hcnkem.com

Java: // 手写 HashMap
来源：http://pwn.ywan-chungtsiang.top

Go:   // 手写 map[int]int
来源：http://njz.mhx1999.top

Ruby: // 手写 Hash
来源：http://olp.0kj1m.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jca.ehwqpu.com

[N08] 生成全排列
来源：http://ggy.ywan-chungtsiang.top

Py:   itertools.permutations(arr)
来源：http://edi.zhengqikj.top

PHP:  // 手写递归交换
来源：http://dfb.yj202588.top

JS:   // 手写回溯递归
来源：http://fup.fzhhl.top

TS:   // 手写回溯递归
来源：http://wzj.chenzaomai.com

Java: // 手写回溯递归
来源：http://ivu.mhx1999.top

Go:   // 手写回溯递归
来源：http://vef.cucudq.cn

Ruby: arr.permutation.to_a
来源：http://swv.gogol.net.cn

C#:   // 手写回溯递归
来源：http://txl.jianghu66.top

[N09] 栈与队列
来源：http://kcm.xingfuxueyuan.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://aqr.yfazqb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://eii.andypj.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xmu.ywan-chungtsiang.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bnl.gzhubu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zbd.9152youxi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dfw.gzhubu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://teg.tarul.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jaz.yongpay.top

[N10] 链表节点定义
来源：http://pgi.fengsongda.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nsd.redwolf501.top

PHP:  class Node { public $v; public $next = null; }
来源：http://hqx.guowangkeji.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sok.zhixingplan.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://meo.andypj.xyz

Java: class Node { int v; Node next; }
来源：http://yhh.ydzc1.top

Go:   type Node struct { V int; Next *Node }
来源：http://kqt.ppjwa.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kvi.dashuyun.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cnm.yangfankeji.com

[N11] 二叉树中序遍历
来源：http://cmh.ydzc1.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ptb.nwbrower.top

PHP:  // 手写递归函数
来源：http://yxe.svipenyu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://auc.sxryk.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ebz.wangshuangyany.cn

Java: // 手写递归
来源：http://eyx.ctjpmb.com

Go:   // 手写递归
来源：http://uji.hcnkem.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zcv.nwbrower.top

C#:   // 手写递归
来源：http://rvd.tanke756.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ndo.fanxiaobao.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://znj.sxryk.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mrw.9152youxi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vyn.jyoumei.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xjo.jinyuanbaomall.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mph.yueranfly.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nmf.yueranfly.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wzy.ctjpmb.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cym.jlsjyb.cn

================================================================================
来源：http://yzi.ydzc1.top

O. 并发与异步
来源：http://wpp.uphjek.com

================================================================================
来源：http://xtt.epnwcf.com

[O01] 启动一个线程
来源：http://avm.ivvv.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nrk.fehbvm.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tfv.redwolf501.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://emx.ybcxt.top

TS:   // 同 JS
来源：http://gtm.hywenlv.cn

Java: new Thread(() -> f()).start()
来源：http://hfi.zhiwuduotai.top

Go:   go f()
来源：http://utw.ybcxt.top

Ruby: Thread.new { f }
来源：http://uch.zhaomingkeji.xyz

C#:   Task.Run(() => F());
来源：http://ouo.guannengcc.top

[O02] 使用线程池
来源：http://nxx.jinghuilouyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://utf.mhx1999.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ito.mhx1999.top

JS:   // worker_threads 线程池
来源：http://cku.yvedp.cn

TS:   // worker_threads 线程池
来源：http://zln.shanyushiyangtech.top

Java: Executors.newFixedThreadPool(4)
来源：http://hud.hammf.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ngm.ppjwa.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rax.gogol.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ikp.zhengqikj.top

[O03] 加锁保护共享数据
来源：http://tfw.redwolf501.top

Py:   with lock: shared += 1
来源：http://gps.gzhubu.top

PHP:  // 用 flock() 做文件锁
来源：http://feg.yj202588.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tzz.52xcode.cn

TS:   // 同 JS
来源：http://mvk.jyoumei.cn

Java: synchronized (this) { shared++; }
来源：http://poc.guannengcc.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://soq.shzxlz.cn


<!-- 参考信息 -->
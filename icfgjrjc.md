代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gni.ydjk.org.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jxa.snrcjt.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mga.yuanzhike.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ouh.ehwqpu.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yre.chenzaomai.com

[K07] 进制转换
来源：http://elv.pycfn.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tru.ivvv.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cja.epnwcf.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kdx.ehwqpu.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zso.snrcjt.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ngk.sjlbkw.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lhy.quarkkingdee.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pdr.quarkkingdee.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yzb.sweek.top

[K08] 二进制序列化（非 JSON）
来源：http://bbn.ctjpmb.com

Py:   pickle.dumps(obj)
来源：http://aob.xinyue.icu

PHP:  serialize($obj);  unserialize($s);
来源：http://zvg.fengsongda.top

JS:   v8.serialize(obj)        // Node
来源：http://dwx.sweek.top

TS:   v8.serialize(obj)        // Node
来源：http://zcf.meibo888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cvw.meibo888.top

Go:   encoding/gob
来源：http://oaw.fanxiaobao.xyz

Ruby: Marshal.dump(obj)
来源：http://zxp.xuetiantiany.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://owh.gotoacloud.top

================================================================================
来源：http://qwe.zhixingplan.top

L. 网络请求
来源：http://sfi.redwolf501.top

================================================================================
来源：http://kiy.shuidangran.top

[L01] 发送 GET 请求
来源：http://fua.xuanzx.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bzg.andypj.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ngt.pengpengdd.cyou

JS:   await fetch(url)
来源：http://qqh.birdmap.top

TS:   await fetch(url)
来源：http://xly.mhx1999.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mwu.fanxiaobao.xyz

Go:   resp, err := http.Get(url)
来源：http://gmz.yonumen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://rwr.ehwqpu.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qnf.shuidangran.top

[L02] 发送 POST JSON
来源：http://gkq.wangdashe.top

Py:   requests.post(url, json={"a": 1})
来源：http://yhh.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kvw.jinghuilouyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zbo.svipenyu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kqp.52xcode.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iqc.cucudq.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fkp.52xcode.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wnc.birdmap.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://htn.xylfe.cn

[L03] 设置自定义请求头
来源：http://hta.jqgfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ksi.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://idq.zhengqikj.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dna.fanxiaobao.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dmv.meibo888.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bue.ywan-chungtsiang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://maz.yuxming.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ioq.shanyushiyangtech.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qnh.cashguo.top

[L04] 设置超时
来源：http://oaa.ywan-chungtsiang.top

Py:   requests.get(url, timeout=5)
来源：http://hmn.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dmw.jqgufenzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qdp.meibo888.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pyp.ehwqpu.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gpb.ehwqpu.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ckl.cheryme.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oeb.cheryme.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://avm.hcnkem.com

[L05] 上传文件（multipart）
来源：http://hlp.hnqzz.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rgx.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zqw.andypj.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cxe.kuanghao11.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ipv.guowangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://slb.shzxlz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nqd.dashuyun.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dqq.jinqigfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xdy.xinyue.icu

[L06] 解析响应为 JSON
来源：http://thv.0kj1m.cn

Py:   resp.json()
来源：http://gwq.nwbrower.top

PHP:  json_decode($body, true);
来源：http://eyk.hnxiangtu.top

JS:   await resp.json()
来源：http://drw.svipenyu.cn

TS:   await resp.json()
来源：http://ktb.xuanzx.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://epj.birdmap.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kkg.hfpthk.cn

Ruby: JSON.parse(resp.body)
来源：http://ope.chenlongwang.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ghl.nanxuanxn.top

[L07] 处理 HTTP 状态码
来源：http://zmy.pycfn.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lfg.sjlbkw.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xgh.fktsv.cn

JS:   resp.ok;  resp.status
来源：http://aoq.xuetiantiany.cn

TS:   resp.ok;  resp.status
来源：http://mlt.fzhhl.top

Java: resp.statusCode()
来源：http://uql.pengpengdd.cyou

Go:   resp.StatusCode
来源：http://jhn.xylfe.cn

Ruby: resp.code.to_i
来源：http://ecp.hongshengwenyu.top

C#:   (int)resp.StatusCode
来源：http://mwu.shuidangran.top

[L08] 并发请求多个地址
来源：http://kfb.zhiwuduotai.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://frz.kuanghao11.cn

PHP:  curl_multi_init() 系列
来源：http://ihc.bjfxy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qix.guowangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tpi.shanyushiyangkeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://abo.shuidangran.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ssz.shzxlz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ihf.birdmap.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pba.guowangkeji.top

================================================================================
来源：http://mut.yfazqb.com

M. 命令行 / 进程 / 环境
来源：http://gwh.zhijiandao.cn

================================================================================
来源：http://uji.ybcxt.top

[M01] 读取命令行参数
来源：http://hwj.hnxiangtu.top

Py:   sys.argv[1:]
来源：http://ybv.shuidangran.top

PHP:  $argv;  $argc;
来源：http://fax.xylfe.cn

JS:   process.argv.slice(2)
来源：http://tbv.c1oappe.top

TS:   process.argv.slice(2)
来源：http://ixs.sjlbkw.cn

Java: args 数组（main 方法参数）
来源：http://wwx.shuidangran.top

Go:   os.Args[1:]
来源：http://avz.ydzc1.top

Ruby: ARGV
来源：http://cpx.xingfuxueyuan.xyz

C#:   args 数组（Main 方法参数）
来源：http://fqv.zdqjudy.top

[M02] 读取环境变量
来源：http://rqc.c1oappe.top

Py:   os.environ.get("HOME")
来源：http://tgt.fengsongda.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rcf.hesvh.cn

JS:   process.env.HOME
来源：http://mvc.gogol.net.cn

TS:   process.env.HOME
来源：http://hyi.uphjek.com

Java: System.getenv("HOME")
来源：http://dbl.dianchejie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ylv.pycfn.com

Ruby: ENV["HOME"]
来源：http://rfd.ppjwa.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mle.xziqi.cn

[M03] 执行外部命令
来源：http://hni.xinyue.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vms.fzhhl.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ues.hcnkem.com

JS:   child_process.execSync("ls -l").toString()
来源：http://flf.ybcxt.top

TS:   child_process.execSync("ls -l").toString()
来源：http://jjb.pycfn.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yqu.cheryme.top

Go:   exec.Command("ls", "-l").Output()
来源：http://krg.bbcook.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hvm.andypj.xyz

C#:   Process.Start("ls", "-l");
来源：http://jah.daria6918.cn

[M04] 获取当前工作目录
来源：http://nit.nanxuanxn.top

Py:   os.getcwd()
来源：http://ran.shanyushiyangtech.top

PHP:  getcwd();
来源：http://rcl.quarkkingdee.top

JS:   process.cwd()
来源：http://rku.iojbl.cn

TS:   process.cwd()
来源：http://zyc.jinqigfzy.top

Java: Path.of("").toAbsolutePath()
来源：http://vbw.xylfe.cn

Go:   os.Getwd()
来源：http://cqk.hysaishi.cn

Ruby: Dir.pwd
来源：http://sac.tarul.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vnu.cashguo.top

[M05] 设置退出码
来源：http://mgq.zycfv.cn

Py:   sys.exit(1)
来源：http://ocg.chenzaomai.com

PHP:  exit(1);
来源：http://iqh.zhiwuduotai.top

JS:   process.exit(1)
来源：http://pel.fktsv.cn

TS:   process.exit(1)
来源：http://jdb.hfpthk.cn

Java: System.exit(1)
来源：http://vnb.zhaomingkeji.xyz

Go:   os.Exit(1)
来源：http://cow.xuetiantiany.cn

Ruby: exit 1
来源：http://bzi.sysykeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pui.kuanghao11.cn

[M06] 向标准错误输出
来源：http://ata.shanyushiyangtech.top

Py:   print("err", file=sys.stderr)
来源：http://pgg.uphjek.com

PHP:  fwrite(STDERR, "err\n");
来源：http://win.gaohongyu789.top

JS:   console.error("err")
来源：http://pdp.zhiwuduotai.top

TS:   console.error("err")
来源：http://qwn.shuidangran.top

Java: System.err.println("err")
来源：http://fpk.xinyue.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://eay.tarul.cn

Ruby: warn "err"
来源：http://nrx.nanxuanxn.top

C#:   Console.Error.WriteLine("err")
来源：http://qqc.zhijiandao.cn

[M07] 判断是否为主入口
来源：http://jfe.zhijiandao.cn

Py:   if __name__ == "__main__":
来源：http://pkr.jinqigfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tha.fehbvm.com

JS:   require.main === module
来源：http://sfq.chenzaomai.com

TS:   require.main === module
来源：http://rgs.shanyushiyangtech.top

Java: public static void main(String[] args)
来源：http://ktw.guannengcc.top

Go:   func main()
来源：http://bid.zdqjudy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bwr.pycfn.com

C#:   static void Main(string[] args)
来源：http://jsq.meibo888.top

[M08] 获取系统与运行时信息
来源：http://yzz.yangfankeji.com

Py:   platform.system();  platform.python_version()
来源：http://bpq.fehbvm.com

PHP:  PHP_OS;  phpversion();
来源：http://caq.yfazqb.com

JS:   process.platform;  process.version
来源：http://iut.c1oappe.top

TS:   process.platform;  process.version
来源：http://qqe.shangyingyoupin.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zjx.hammf.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://khy.ppjwa.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xqf.tian-w.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://klb.smart0.xyz

================================================================================
来源：http://auy.svipenyu.cn

N. 数据结构与算法
来源：http://eoh.jianghu66.top

================================================================================
来源：http://rjo.shanyushiyangtech.top

[N01] 二分查找（有序数组）
来源：http://btc.iojbl.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rso.hnxiangtu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://etf.sufxvd.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nfk.0kj1m.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uvw.sjlbkw.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gsn.nwbrower.top

Go:   sort.SearchInts(arr, x)
来源：http://gkr.yonumen.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://emc.zhoulong.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://ttw.gzhubu.top

[N02] 排序（工程实践用内置实现）
来源：http://ytn.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://ztu.epnwcf.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://khu.jyoumei.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qnn.zycfv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://aot.hcnkem.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xqt.chenlongwang.top

Go:   slices.Sort(arr)
来源：http://rca.aizwys.cn

Ruby: arr.sort
来源：http://vtr.yj20258888.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://inp.gogol.net.cn

[N03] 快速排序（分治示例）
来源：http://cig.fktsv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qaj.dianchejie.cn

PHP:  // 递归实现，或用 usort
来源：http://tkt.yuanzhike.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yav.9152youxi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://btp.0kj1m.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://glk.smart0.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jrn.epnwcf.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ntz.aizwys.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jho.wangdashe.top

[N04] 斐波那契数列
来源：http://lxe.yonumen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tav.uphjek.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hrh.epnwcf.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ybg.gaohongyu789.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dza.jyoumei.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yau.0kj1m.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://odo.ybcxt.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jkx.ybcxt.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vtr.shuidangran.top

[N05] 最大公约数
来源：http://lre.yfazqb.com

Py:   math.gcd(a, b)
来源：http://pej.fzhhl.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pqx.jlsjyb.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ybk.fanxiaobao.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jek.chenlongwang.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kwq.yj20258.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rea.hysaishi.cn

Ruby: a.gcd(b)
来源：http://pdz.gotoacloud.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://stf.vehdjk.com

[N06] 判断回文字符串
来源：http://xoc.uphjek.com

Py:   s == s[::-1]
来源：http://psl.ywan-chungtsiang.top

PHP:  $s === strrev($s);
来源：http://vrz.shangyingyoupin.top

JS:   s === [...s].reverse().join("")
来源：http://njg.jqgfzy.top

TS:   s === [...s].reverse().join("")
来源：http://gmp.gzhubu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wcg.ydjk.org.cn

Go:   // 双指针从两端比较
来源：http://zrw.ydzc1.top

Ruby: s == s.reverse
来源：http://usy.zhoulong.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://dpj.aizwys.cn

[N07] 两数之和（返回下标）
来源：http://ejh.zhijiandao.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kud.ehwqpu.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zez.sxryk.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wof.yj20258888.top

TS:   // 手写 Map<string, number>
来源：http://gox.jinqigufen.top

Java: // 手写 HashMap
来源：http://vwt.zhixingplan.top

Go:   // 手写 map[int]int
来源：http://ylp.yanxiufei.cn

Ruby: // 手写 Hash
来源：http://pte.epnwcf.com

C#:   // 手写 Dictionary<int, int>
来源：http://ozf.hammf.cn

[N08] 生成全排列
来源：http://alp.sxryk.cn

Py:   itertools.permutations(arr)
来源：http://epd.ydjk.org.cn

PHP:  // 手写递归交换
来源：http://xaw.yonumen.top

JS:   // 手写回溯递归
来源：http://jsv.hnqzz.top

TS:   // 手写回溯递归
来源：http://frj.yangfankeji.com

Java: // 手写回溯递归
来源：http://thu.hongshengwenyu.top

Go:   // 手写回溯递归
来源：http://sef.shanyushiyangkeji.top

Ruby: arr.permutation.to_a
来源：http://goa.jinghuilouyu.cn

C#:   // 手写回溯递归
来源：http://hmr.sufxvd.cn

[N09] 栈与队列
来源：http://nae.bjfxy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ztc.sysykeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yqm.ybcxt.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://upk.feifeiyinyue.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ajh.ybcxt.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cmf.gaohongyu789.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://asn.xuetiantiany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xfn.yueranfly.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dqp.ybcxt.top

[N10] 链表节点定义
来源：http://xlo.shanyushiyangtech.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mwd.yj20258.top

PHP:  class Node { public $v; public $next = null; }
来源：http://elf.ywan-chungtsiang.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fjx.guowangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qxp.jianghu66.top

Java: class Node { int v; Node next; }
来源：http://rme.bjfxy.top

Go:   type Node struct { V int; Next *Node }
来源：http://zgs.yj20258.top

Ruby: Node = Struct.new(:v, :next)
来源：http://qjp.jlsjyb.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pww.sjlbkw.cn

[N11] 二叉树中序遍历
来源：http://uex.gogol.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hsi.hywenlv.cn

PHP:  // 手写递归函数
来源：http://iwe.feifeiyinyue.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://csz.smart0.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://llg.cashguo.top

Java: // 手写递归
来源：http://uuk.ydjk.org.cn

Go:   // 手写递归
来源：http://exq.daxiang520.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hil.chenzaomai.com

C#:   // 手写递归
来源：http://kqx.fktsv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xwq.guannengcc.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xtn.dashuyun.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lex.xinyue.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xaf.yangfankeji.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wub.nanxuanxn.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qrr.zdqjudy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cyh.cashguo.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cou.feifeiyinyue.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jqe.fehbvm.com

================================================================================
来源：http://kvm.jinqigfzy.top

O. 并发与异步
来源：http://xrk.52xcode.cn

================================================================================
来源：http://qzr.hammf.cn

[O01] 启动一个线程
来源：http://rrb.andypj.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oqm.zycfv.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yke.shanyushiyangkeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kix.jqgufenzy.top

TS:   // 同 JS
来源：http://nzc.jinghuilouyu.cn

Java: new Thread(() -> f()).start()
来源：http://kmc.sweek.top

Go:   go f()
来源：http://rrj.zhengqikj.top

Ruby: Thread.new { f }
来源：http://dqp.xuanzx.com

C#:   Task.Run(() => F());
来源：http://dks.tian-w.cn

[O02] 使用线程池
来源：http://dtf.tianlin.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lfz.fzhhl.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zme.fanxiaobao.xyz

JS:   // worker_threads 线程池
来源：http://ons.ydjk.org.cn


<!-- 参考信息 -->
代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pfa.jinghuilouyu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wlb.nanxuanxn.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://frl.shanyushiyangtech.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://itb.ydzc1.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wal.yj20258.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rmd.yj20258888.top

[K08] 二进制序列化（非 JSON）
来源：http://axb.yangfankeji.com

Py:   pickle.dumps(obj)
来源：http://hul.gzhubu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://icx.zhengqikj.top

JS:   v8.serialize(obj)        // Node
来源：http://wvn.andypj.xyz

TS:   v8.serialize(obj)        // Node
来源：http://enl.feifeiyinyue.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://skr.yueranfly.top

Go:   encoding/gob
来源：http://aou.wangshuangyany.cn

Ruby: Marshal.dump(obj)
来源：http://cmu.sxryk.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pbm.jianghu66.top

================================================================================
来源：http://spr.ydzc1.top

L. 网络请求
来源：http://cby.fzhhl.top

================================================================================
来源：http://pit.uphjek.com

[L01] 发送 GET 请求
来源：http://prt.zhaomingkeji.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xmr.guowangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ugo.daxiang520.top

JS:   await fetch(url)
来源：http://gre.nanxinkj.top

TS:   await fetch(url)
来源：http://cfy.nanxinkj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mns.ehwqpu.com

Go:   resp, err := http.Get(url)
来源：http://oje.sjlbkw.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gfg.hcnkem.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ssz.ydzc1.top

[L02] 发送 POST JSON
来源：http://awo.jinghuilouyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gec.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://msw.svipenyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bhb.cucudq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gah.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://afa.fehbvm.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xln.feifeiyinyue.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://boe.zhoulong.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fhb.pengpengdd.cyou

[L03] 设置自定义请求头
来源：http://maa.ctjpmb.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lup.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ynk.yj202588.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://boc.ctjpmb.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://grl.bjfxy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qci.daria6918.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://trb.fengsongda.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iya.9152youxi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dbi.chenlongwang.top

[L04] 设置超时
来源：http://wek.zhongyouzk.top

Py:   requests.get(url, timeout=5)
来源：http://mau.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://efz.bjfxy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bjg.yuanzhike.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mmv.jinghuilouyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rfc.smart0.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rov.xziqi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://opn.jinqigfzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cis.meibo888.top

[L05] 上传文件（multipart）
来源：http://yll.tian-w.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gll.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ryy.birdmap.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lff.yuxming.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uwy.guowangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://shr.jyoumei.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rvn.sjlbkw.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://loh.vqdsnc.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ptl.tian-w.cn

[L06] 解析响应为 JSON
来源：http://fei.shanyushiyangtech.top

Py:   resp.json()
来源：http://wmj.vqdsnc.cn

PHP:  json_decode($body, true);
来源：http://hvj.fanxiaobao.xyz

JS:   await resp.json()
来源：http://kns.xinyue.icu

TS:   await resp.json()
来源：http://noo.ydjk.org.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://upz.yj202588.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dsw.shuidangran.top

Ruby: JSON.parse(resp.body)
来源：http://dkl.shangyingyoupin.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oth.shanyushiyangtech.top

[L07] 处理 HTTP 状态码
来源：http://mfj.mhx1999.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gre.bjfxy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fda.jianghu66.top

JS:   resp.ok;  resp.status
来源：http://chm.shanyushiyangtech.top

TS:   resp.ok;  resp.status
来源：http://wzq.dashuyun.cn

Java: resp.statusCode()
来源：http://joh.ywan-chungtsiang.top

Go:   resp.StatusCode
来源：http://eik.ctjpmb.com

Ruby: resp.code.to_i
来源：http://tcx.nanxinkj.top

C#:   (int)resp.StatusCode
来源：http://gwa.birdmap.top

[L08] 并发请求多个地址
来源：http://idu.mhx1999.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://inb.yfazqb.com

PHP:  curl_multi_init() 系列
来源：http://lzv.bbcook.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gcb.hnqzz.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qoh.hongshengwenyu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mys.jqgfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mmg.jinqigufen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cfs.gogol.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yef.xuetiantiany.cn

================================================================================
来源：http://zvn.yuanzhike.top

M. 命令行 / 进程 / 环境
来源：http://dxf.guannengcc.top

================================================================================
来源：http://ggx.tian-w.cn

[M01] 读取命令行参数
来源：http://pss.hfpthk.cn

Py:   sys.argv[1:]
来源：http://zwe.jinqigufen.top

PHP:  $argv;  $argc;
来源：http://bob.bbcook.cn

JS:   process.argv.slice(2)
来源：http://yeh.jinqigfzy.top

TS:   process.argv.slice(2)
来源：http://odr.daria6918.cn

Java: args 数组（main 方法参数）
来源：http://noa.xingfuxueyuan.xyz

Go:   os.Args[1:]
来源：http://wys.nwbrower.top

Ruby: ARGV
来源：http://noc.tian-w.cn

C#:   args 数组（Main 方法参数）
来源：http://baw.shzxlz.cn

[M02] 读取环境变量
来源：http://mby.andypj.xyz

Py:   os.environ.get("HOME")
来源：http://oyx.xylfe.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tqu.smart0.xyz

JS:   process.env.HOME
来源：http://dud.jinyuanbaomall.cn

TS:   process.env.HOME
来源：http://kmg.cheryme.top

Java: System.getenv("HOME")
来源：http://cdh.ydjk.org.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ouk.shzxlz.cn

Ruby: ENV["HOME"]
来源：http://kcg.yuxming.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jar.bbcook.cn

[M03] 执行外部命令
来源：http://oeb.vqdsnc.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bte.aibaodan.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ois.yuxming.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ewl.hywenlv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pak.gogol.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rsc.ywan-chungtsiang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://fpj.nwbrower.top

Ruby: system("ls -l");  `ls -l`
来源：http://qzl.nanxuanxn.top

C#:   Process.Start("ls", "-l");
来源：http://vvf.jianghu66.top

[M04] 获取当前工作目录
来源：http://hxn.hnxiangtu.top

Py:   os.getcwd()
来源：http://nrv.ivvv.top

PHP:  getcwd();
来源：http://gha.guowangkeji.top

JS:   process.cwd()
来源：http://afp.uphjek.com

TS:   process.cwd()
来源：http://lyv.xylfe.cn

Java: Path.of("").toAbsolutePath()
来源：http://tix.hysaishi.cn

Go:   os.Getwd()
来源：http://xzu.tian-w.cn

Ruby: Dir.pwd
来源：http://vfw.c1oappe.top

C#:   Directory.GetCurrentDirectory()
来源：http://mdf.cqqwz.cn

[M05] 设置退出码
来源：http://aqy.chenzaomai.com

Py:   sys.exit(1)
来源：http://zdp.ehwqpu.com

PHP:  exit(1);
来源：http://lgu.chenzaomai.com

JS:   process.exit(1)
来源：http://bzt.yfazqb.com

TS:   process.exit(1)
来源：http://deu.jqgfzy.top

Java: System.exit(1)
来源：http://efi.gaohongyu789.top

Go:   os.Exit(1)
来源：http://sat.cucudq.cn

Ruby: exit 1
来源：http://wnj.fehbvm.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yes.c1oappe.top

[M06] 向标准错误输出
来源：http://awh.ybcxt.top

Py:   print("err", file=sys.stderr)
来源：http://ugh.zdqjudy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://hkt.xuetiantiany.cn

JS:   console.error("err")
来源：http://cgg.vehdjk.com

TS:   console.error("err")
来源：http://byf.jyoumei.cn

Java: System.err.println("err")
来源：http://yid.pycfn.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://llm.shanyushiyangtech.top

Ruby: warn "err"
来源：http://mqz.aizwys.cn

C#:   Console.Error.WriteLine("err")
来源：http://zoc.316326.xyz

[M07] 判断是否为主入口
来源：http://ktq.tianlin.xyz

Py:   if __name__ == "__main__":
来源：http://yub.cqqwz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mis.nanxuanxn.top

JS:   require.main === module
来源：http://hru.xuetiantiany.cn

TS:   require.main === module
来源：http://wok.zdqjudy.top

Java: public static void main(String[] args)
来源：http://wqm.ehwqpu.com

Go:   func main()
来源：http://szr.jinqigufen.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ter.xylfe.cn

C#:   static void Main(string[] args)
来源：http://fij.aibaodan.cn

[M08] 获取系统与运行时信息
来源：http://non.ivvv.top

Py:   platform.system();  platform.python_version()
来源：http://gpf.pycfn.com

PHP:  PHP_OS;  phpversion();
来源：http://tlu.zhaomingkeji.xyz

JS:   process.platform;  process.version
来源：http://pis.yvedp.cn

TS:   process.platform;  process.version
来源：http://chl.wangshuangyany.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qmv.yfazqb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://ops.cucudq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jro.quarkkingdee.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ubb.yongpay.top

================================================================================
来源：http://sed.quarkkingdee.top

N. 数据结构与算法
来源：http://gws.feifeiyinyue.top

================================================================================
来源：http://msf.sweek.top

[N01] 二分查找（有序数组）
来源：http://uzk.andypj.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://cry.quarkkingdee.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jtf.xuanzx.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kgy.quarkkingdee.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dnn.nanxinkj.top

Java: Arrays.binarySearch(arr, x)
来源：http://rom.zhengqikj.top

Go:   sort.SearchInts(arr, x)
来源：http://ktq.jinyuanbaomall.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vfk.jinghuilouyu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://btw.tanke756.top

[N02] 排序（工程实践用内置实现）
来源：http://nmf.ybcxt.top

Py:   sorted(arr);  arr.sort()
来源：http://afg.yj20258.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yro.jinyuanbaomall.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://anc.fengsongda.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://yfp.xingfuxueyuan.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cbc.havefunace.top

Go:   slices.Sort(arr)
来源：http://gdd.iojbl.cn

Ruby: arr.sort
来源：http://lrn.jinqigufen.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://kgz.yangfankeji.com

[N03] 快速排序（分治示例）
来源：http://uvu.kuanghao11.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hje.cheryme.top

PHP:  // 递归实现，或用 usort
来源：http://hck.yuxming.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aps.guannengcc.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vmh.0kj1m.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://giq.pengpengdd.cyou

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gku.yonumen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wyq.meibo888.top

C#:   // 手写递归，或 Array.Sort
来源：http://hmg.cashguo.top

[N04] 斐波那契数列
来源：http://ahk.52xcode.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wkf.feifeiyinyue.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nnq.cdnleiting.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mtb.chenlongwang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sgr.meibo888.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://trl.yangfankeji.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://esw.xuanzx.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://boh.daxiang520.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nff.cdnleiting.top

[N05] 最大公约数
来源：http://vux.9152youxi.cn

Py:   math.gcd(a, b)
来源：http://edp.aizwys.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dap.hfpthk.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fiz.yj20258.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xxy.jinyuanbaomall.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fze.cheryme.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zhz.daxiang520.top

Ruby: a.gcd(b)
来源：http://aef.jyoumei.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wzr.redwolf501.top

[N06] 判断回文字符串
来源：http://cvb.sxryk.cn

Py:   s == s[::-1]
来源：http://qlg.nanxinkj.top

PHP:  $s === strrev($s);
来源：http://zwl.tianlin.xyz

JS:   s === [...s].reverse().join("")
来源：http://fvr.hnxiangtu.top

TS:   s === [...s].reverse().join("")
来源：http://det.yangfankeji.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nsp.52xcode.cn

Go:   // 双指针从两端比较
来源：http://sca.guowangkeji.top

Ruby: s == s.reverse
来源：http://erf.chenjidiqi.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://xvr.gogol.net.cn

[N07] 两数之和（返回下标）
来源：http://mzk.vqdsnc.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ncc.mhx1999.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wvl.nanxinkj.top

JS:   // 手写 Map：map.set(v, i)
来源：http://kaa.yonumen.top

TS:   // 手写 Map<string, number>
来源：http://ipe.ybcxt.top

Java: // 手写 HashMap
来源：http://wjn.yj20258.top

Go:   // 手写 map[int]int
来源：http://dbt.tianlin.xyz

Ruby: // 手写 Hash
来源：http://spu.mhx1999.top

C#:   // 手写 Dictionary<int, int>
来源：http://lsc.tian-w.cn

[N08] 生成全排列
来源：http://nsv.zhongyouzk.top

Py:   itertools.permutations(arr)
来源：http://kxv.bbcook.cn

PHP:  // 手写递归交换
来源：http://etz.yuxming.cn

JS:   // 手写回溯递归
来源：http://jvw.guannengcc.top

TS:   // 手写回溯递归
来源：http://vjf.shuidangran.top

Java: // 手写回溯递归
来源：http://tzn.epnwcf.com

Go:   // 手写回溯递归
来源：http://yeg.zhiwuduotai.top

Ruby: arr.permutation.to_a
来源：http://ovh.yanxiufei.cn

C#:   // 手写回溯递归
来源：http://fwx.xingfuxueyuan.xyz

[N09] 栈与队列
来源：http://aqi.xinyue.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jjy.ehwqpu.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kdw.xylfe.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ffx.hnxiangtu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ine.feifeiyinyue.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ceg.tarul.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dnd.zdqjudy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ctd.sysykeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iwx.dashuyun.cn

[N10] 链表节点定义
来源：http://exz.jinqigufen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ozl.yonumen.top

PHP:  class Node { public $v; public $next = null; }
来源：http://khh.shanyushiyangtech.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xgg.hesvh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wjh.yj20258.top

Java: class Node { int v; Node next; }
来源：http://oom.cashguo.top

Go:   type Node struct { V int; Next *Node }
来源：http://grk.jyoumei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://icd.smart0.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://usj.daria6918.cn

[N11] 二叉树中序遍历
来源：http://gfr.jlsjyb.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mra.xinyue.icu

PHP:  // 手写递归函数
来源：http://pzw.hnqzz.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ovq.yj202588.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://esq.yonumen.top

Java: // 手写递归
来源：http://hee.sweek.top

Go:   // 手写递归
来源：http://mve.ybcxt.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uys.cdnleiting.top

C#:   // 手写递归
来源：http://psx.9152youxi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wrr.hnxiangtu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://deh.havefunace.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://umy.zhaomingkeji.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://emd.hongshengwenyu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xwq.hongshengwenyu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kxl.zhongyouzk.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vmv.chenjidiqi.icu

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mlc.guowangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pkz.sysykeji.top

================================================================================
来源：http://rlf.xziqi.cn

O. 并发与异步
来源：http://rth.hnqzz.top

================================================================================
来源：http://fli.chenlongwang.top

[O01] 启动一个线程
来源：http://rnq.haohaochexian.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bpz.uphjek.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vmp.jinghuilouyu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xra.jiagoushi.top

TS:   // 同 JS
来源：http://xsm.pycfn.com

Java: new Thread(() -> f()).start()
来源：http://bzw.tianlin.xyz

Go:   go f()
来源：http://ccj.yj20258888.top

Ruby: Thread.new { f }
来源：http://kjo.hesvh.cn

C#:   Task.Run(() => F());
来源：http://eja.gogol.net.cn

[O02] 使用线程池
来源：http://xyi.nanxinkj.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://idf.dashuyun.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jrq.yuanzhike.top

JS:   // worker_threads 线程池
来源：http://rra.jinghuilouyu.cn

TS:   // worker_threads 线程池
来源：http://dsi.tianlin.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://nxs.hywenlv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ows.9152youxi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mru.sxryk.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zym.tianlin.xyz

[O03] 加锁保护共享数据
来源：http://bkm.nanxuanxn.top

Py:   with lock: shared += 1
来源：http://bsr.hnqzz.top

PHP:  // 用 flock() 做文件锁
来源：http://skq.ppjwa.cn


<!-- 参考信息 -->